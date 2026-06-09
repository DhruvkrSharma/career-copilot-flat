# Strong AI Project Signals

> **Last Updated:** June 2026

Projects score highest when they include:

## Problem

Clear real-world problem statement.
- Why does this matter?
- Who benefits?
- What is the current gap?
- How is this different from a tutorial project?

## Dataset

Source documented.
- Size mentioned
- Preprocessing steps described
- Train/val/test split documented
- Data quality considerations addressed
- Data versioning used (DVC, Git LFS)
- For LLM projects: corpus description, chunking strategy, embedding model choice

## Architecture

Model architecture explained.
- Why this architecture was chosen
- Comparison with alternatives considered
- Diagram or description of the pipeline
- For agentic projects: agent architecture diagram (supervisor vs swarm vs hierarchical), tool registry, memory design

## Training

Training process documented.
- Hyperparameters listed
- Training curves shown
- Hardware/compute mentioned
- Training duration noted
- Data augmentation techniques used
- For LLM fine-tuning: base model, method (LoRA/QLoRA/DPO/GRPO), dataset size, training loss curves

## Evaluation

Metrics included:
- Accuracy
- Precision
- Recall
- F1 Score
- mAP (for detection)
- IoU (for segmentation)
- BLEU/ROUGE (for NLP)
- Perplexity (for language models)
- AUC-ROC (for classification)
- Confusion matrix
- RAGAS scores (for RAG — faithfulness, relevance, context precision)
- LLM-as-judge evaluations (for GenAI)
- Agent task completion rate (for agentic systems)
- Cost per query / Cost per task (for production systems)
- Latency benchmarks (p50, p95, p99)

## Deployment

Evidence of deployment:
- Web App (Streamlit, Gradio, Flask, FastAPI, Next.js)
- API (REST, gRPC, WebSocket)
- Mobile App
- Docker containerization
- Cloud deployment (AWS, GCP, Azure)
- Edge deployment
- Live demo link or video walkthrough
- CI/CD pipeline (GitHub Actions, Jenkins)

## Scalability

Performance considerations:
- Latency benchmarks (p50, p95, p99)
- Inference speed (tokens/sec for LLMs, FPS for CV)
- Model optimization (quantization, pruning, distillation, speculative decoding)
- Batch processing capabilities
- Concurrent request handling
- Cost optimization (model routing, caching, token management)

## Observability (🆕 2026)

Production monitoring:
- Logging and tracing (LangSmith, LangFuse, Helicone)
- Drift detection (data drift, concept drift)
- Error tracking and alerting
- Token usage and cost monitoring
- User feedback collection

## Documentation

Quality indicators:
- Comprehensive README
- Screenshots / Demo GIFs / Video walkthrough
- Architecture diagram (Mermaid, draw.io, Excalidraw)
- Installation instructions (with Docker support)
- Usage examples
- API documentation (Swagger/OpenAPI)
- Contributing guidelines
- License
- Badges (CI status, coverage, Python version)

---

# Weak Project Signals

These indicate low-quality or non-differentiating projects:

- **Tutorial clones** — Following a YouTube tutorial without modification
- **No metrics** — No evaluation results reported
- **No deployment** — Code only runs in a notebook
- **No documentation** — Empty or minimal README
- **No explanation of design choices** — No justification for architecture/approach
- **No reproducibility** — Missing requirements.txt, no instructions to run
- **Toy datasets** — Using MNIST/CIFAR without meaningful extension
- **No error analysis** — No discussion of failure cases
- **No version control hygiene** — Single "initial commit", no meaningful history
- **Hardcoded paths** — Code that only works on the author's machine
- **API wrapper only** — Just calling OpenAI API with a basic prompt, no architecture (🆕 2026)
- **No evaluation pipeline** — For GenAI projects, no systematic evaluation beyond "it looks good" (🆕 2026)
- **No cost awareness** — For LLM projects, no mention of token costs or optimization (🆕 2026)
- **Single-turn only** — Chatbot with no memory, context, or multi-turn capability (🆕 2026)

---

# Project Tier Classification

| Tier | Characteristics |
|------|----------------|
| **S-Tier** | Novel problem, custom dataset, deployed with monitoring, documented, with evaluation pipeline, cost-optimized, and live demo |
| **A-Tier** | Clear problem, good architecture, metrics, deployment, some evaluation beyond accuracy |
| **B-Tier** | Standard problem, decent implementation, basic metrics, Docker/cloud deployment |
| **C-Tier** | Tutorial-level, minimal customization, notebook-only, no deployment |
| **D-Tier** | Incomplete, no documentation, no metrics, broken code |

---

# 2026 Project Archetypes (What Recruiters Want to See)

## 🔥 S-Tier Project Archetypes

### 1. Multi-Agent System with Tool Use
- Multiple specialized agents coordinating on a complex task
- Tool registry with external API integrations (search, code execution, database)
- Memory system (short-term + long-term)
- Error recovery and self-correction
- Human-in-the-loop checkpoints for critical actions
- Evaluation with golden trajectories
- **Why hot:** #1 in-demand skill in 2026

### 2. Production Agentic RAG Pipeline
- Agentic RAG (query planning, multi-step retrieval)
- Hybrid retrieval (dense + sparse + re-ranking)
- Evaluation pipeline (RAGAS, faithfulness, relevance)
- Hallucination detection
- Deployed with monitoring (LangSmith/LangFuse)
- Cost tracking per query
- **Why hot:** Direct job relevance, shows production maturity

### 3. Fine-Tuned Domain LLM with Evaluation
- Domain-specific fine-tuning (LoRA/QLoRA/DPO)
- Custom evaluation dataset
- Comparison against base model
- Deployed as API with monitoring
- Cost analysis (fine-tuned vs prompted)
- **Why hot:** Shows GenAI depth beyond API calls

### 4. Real-Time Multi-Modal Pipeline
- Combines vision + language (+ audio)
- Real-time processing with latency benchmarks
- Edge or cloud deployment
- Practical use case (document understanding, visual Q&A, video analysis)
- **Why hot:** Multi-modal is booming

### 5. ML Monitoring & Observability Platform
- Drift detection (data + model)
- Automated retraining triggers
- Dashboard with metrics visualization
- Alerting system
- A/B testing framework
- **Why hot:** MLOps is still severely under-supplied

## ⚠️ Overused Projects to Avoid (or Heavily Differentiate)

| Overused Project | How to Differentiate |
|-----------------|---------------------|
| Basic chatbot (just OpenAI API) | Add RAG, evaluation, multi-agent, memory, deployment |
| MNIST/CIFAR classifier | Use custom dataset, deploy on edge, add explainability |
| Sentiment analysis | Use domain-specific data, fine-tune, deploy as API with monitoring |
| Basic object detection | Custom dataset, real-time inference, edge deployment, metrics dashboard |
| Simple RAG Q&A | Add agentic retrieval, evaluation pipeline, hybrid search, cost tracking |
