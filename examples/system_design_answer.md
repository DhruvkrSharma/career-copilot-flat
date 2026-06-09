# ML System Design Answer Examples

## Question 1: Design a Real-Time Image Moderation System

### Context
> "Design a system that automatically detects and flags inappropriate content (violence, nudity, hate symbols) in user-uploaded images for a social media platform processing 10M images/day."

### Strong Answer

**Requirements Clarification:**
- Latency: < 500ms per image (user upload flow)
- Throughput: ~115 images/second average
- Accuracy: > 95% precision (minimize false positives to avoid over-censorship)
- Categories: Violence, nudity, hate symbols, spam text
- Actions: Auto-block (high confidence), flag for review (medium), pass (low)

**High-Level Architecture:**
```
User Upload → API Gateway → Image Queue (Kafka)
                                    ↓
                            Preprocessing Service
                            (resize, normalize)
                                    ↓
                            Model Serving (Triton)
                            ┌───────┼───────┐
                            │       │       │
                         NSFW    Violence  OCR+Hate
                         Model   Model     Pipeline
                            │       │       │
                            └───────┼───────┘
                                    ↓
                            Decision Aggregator
                            ┌───────┼───────┐
                         Auto-Block  Flag   Pass
                                    ↓
                            Results DB + Notification
```

**Model Choices:**
- NSFW: Fine-tuned EfficientNet-B3 (good accuracy/speed tradeoff)
- Violence: CLIP-based zero-shot + fine-tuned classifier ensemble
- OCR: PaddleOCR → text classifier for hate speech
- Why ensemble: Different content types need specialized models

**Key Design Decisions:**
1. **Async processing via Kafka** — Decouples upload from moderation, handles spikes
2. **Triton Inference Server** — GPU batching, model versioning, A/B testing
3. **Three-tier decision** — Auto-block/flag/pass reduces human review load by 80%
4. **Confidence thresholds** — High confidence (>0.95) auto-action, medium (0.7-0.95) human review

**Scaling:**
- Horizontal scaling of model serving pods
- GPU batching (batch size 32) for throughput
- Redis cache for duplicate image detection (perceptual hashing)
- Regional deployment for latency

**Monitoring:**
- Precision/recall tracking per category (daily)
- Latency P50/P95/P99 dashboards
- Drift detection on input distribution
- Human reviewer feedback loop for model retraining

**Why This Answer is Strong:**
- Clarified requirements first
- Drew clear architecture
- Justified model choices with tradeoffs
- Addressed scaling and monitoring
- Mentioned feedback loops

---

## Question 2: Design a Recommendation System

### Context
> "Design a movie recommendation system for a streaming platform with 50M users and 100K movies."

### Strong Answer Structure

**1. Problem Decomposition:**
- Cold start (new users, new movies)
- Real-time personalization
- Diversity (not just similar items)
- Freshness (promote new content)

**2. Two-Stage Architecture:**
```
Stage 1: Candidate Generation (fast, broad)
  - Collaborative filtering (user-item matrix, ALS)
  - Content-based (movie embeddings from metadata)
  - Popularity-based (for cold start)
  → Output: 500 candidates

Stage 2: Ranking (slow, precise)
  - Deep learning ranker (Wide & Deep / DeepFM)
  - Features: user history, movie features, context (time, device)
  - → Output: Top 20 ranked recommendations
```

**3. Feature Engineering:**
- User: watch history, ratings, demographics, session behavior
- Item: genre, actors, director, release year, embeddings from poster/trailer
- Context: time of day, device, day of week
- Cross: user-genre affinity, recency-weighted interactions

**4. Handling Cold Start:**
- New users: Content-based + popularity + onboarding quiz
- New movies: Content features + similar movie embeddings + boost factor

**5. Evaluation:**
- Offline: NDCG@20, MAP@20, Coverage, Diversity
- Online: CTR, Watch time, Completion rate
- A/B testing framework for model comparison

**6. Serving:**
- Pre-compute recommendations (batch, daily)
- Real-time re-ranking based on session context
- Feature store (Feast) for consistent features across training/serving

---

## System Design Answer Checklist

| Step | Must Include |
|------|-------------|
| Requirements | Clarify scale, latency, accuracy needs |
| Architecture | High-level diagram with clear data flow |
| Model Selection | Specific models with justification |
| Data Pipeline | How data flows from raw to features to predictions |
| Scaling | How to handle 10x traffic |
| Monitoring | What metrics to track, how to detect issues |
| Tradeoffs | At least 2 tradeoffs discussed |
| Iteration | How to improve over time (A/B testing, feedback loops) |

## Common Mistakes

1. **Jumping to model architecture** without clarifying requirements
2. **No scale discussion** — Works for 100 users but not 10M
3. **No monitoring** — Deploy and forget
4. **Single model** — No ensemble or multi-stage thinking
5. **No offline/online evaluation** distinction
6. **Ignoring cold start** — Only works for existing users
