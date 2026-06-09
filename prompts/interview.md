# Interview Simulation Prompt

## Instructions

Simulate a technical and behavioral interview for an AI/ML role.

## Input Required

- Target role (e.g., "AI Engineer", "ML Engineer", "CV Engineer")
- Experience level (Intern, Junior, Mid, Senior)
- Focus areas (optional: DSA, ML Theory, System Design, Behavioral)
- Resume / project details (for personalized questions)

## Interview Structure

### Round 1: Introduction (5 min)
- "Tell me about yourself"
- "Walk me through your most impactful project"

### Round 2: Technical Deep Dive (20 min)

Based on target role, ask from `knowledge/interview_knowledge.md`:

**For ML/AI roles:**
- Explain bias-variance tradeoff with a real example
- How would you handle class imbalance in production?
- Compare CNN vs ViT for image classification
- Design an ML pipeline for [specific problem]

**For CV roles:**
- Explain how YOLO works at a high level
- What is Non-Maximum Suppression?
- How would you improve a detection model's mAP?
- Explain transfer learning in the context of CV

**For GenAI roles:**
- Explain how RAG works end-to-end
- What are the tradeoffs of fine-tuning vs RAG?
- How do you evaluate LLM outputs?
- Design a customer support chatbot architecture

### Round 3: Coding / Problem Solving (15 min)
- DSA problem appropriate for level
- ML-specific coding (implement a metric, write a data pipeline)

### Round 4: System Design (15 min, Mid+ only)
- Design a real-time recommendation system
- Design an image moderation pipeline
- Design a document Q&A system

### Round 5: Behavioral (10 min)
- Tell me about a time you failed
- Describe a conflict with a teammate
- How do you prioritize when everything is urgent?

## Evaluation

After each answer, provide:

```
Answer Quality: __/10

✅ What was good:
- ...

❌ What was missing:
- ...

💡 Ideal Answer Should Include:
- ...

📝 Sample Strong Answer:
"..."
```

## Final Output

```
Interview Readiness Score: __/100

Technical: __/25
Domain: __/20
Projects: __/20
Communication: __/15
Behavioral: __/10
Problem Solving: __/10

Ready for: [Intern / Junior / Mid / Senior] level interviews

Top 3 Areas to Improve:
1. ...
2. ...
3. ...

Recommended Preparation:
- ...
```
