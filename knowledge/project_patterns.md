# Strong AI Project Signals

Projects score highest when they include:

## Problem

Clear real-world problem statement.
- Why does this matter?
- Who benefits?
- What is the current gap?

## Dataset

Source documented.
- Size mentioned
- Preprocessing steps described
- Train/val/test split documented
- Data quality considerations addressed

## Architecture

Model architecture explained.
- Why this architecture was chosen
- Comparison with alternatives considered
- Diagram or description of the pipeline

## Training

Training process documented.
- Hyperparameters listed
- Training curves shown
- Hardware/compute mentioned
- Training duration noted
- Data augmentation techniques used

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

## Deployment

Evidence of deployment:
- Web App (Streamlit, Gradio, Flask, FastAPI)
- API (REST, gRPC)
- Mobile App
- Docker containerization
- Cloud deployment (AWS, GCP, Azure)
- Edge deployment

## Scalability

Performance considerations:
- Latency benchmarks
- Inference speed
- Model optimization (quantization, pruning, distillation)
- Batch processing capabilities
- Concurrent request handling

## Documentation

Quality indicators:
- Comprehensive README
- Screenshots / Demo GIFs
- Architecture diagram
- Installation instructions
- Usage examples
- API documentation
- Contributing guidelines
- License

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

---

# Project Tier Classification

| Tier | Characteristics |
|------|----------------|
| **S-Tier** | Novel problem, custom dataset, deployed, documented, with metrics |
| **A-Tier** | Clear problem, good architecture, metrics, some deployment |
| **B-Tier** | Standard problem, decent implementation, basic metrics |
| **C-Tier** | Tutorial-level, minimal customization, no deployment |
| **D-Tier** | Incomplete, no documentation, no metrics, broken code |
