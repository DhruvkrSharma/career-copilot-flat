# Common Interview Areas

> **Last Updated:** June 2026

## Software Engineering

### Data Structures & Algorithms
- Arrays, Strings, Linked Lists
- Stacks, Queues, Heaps
- Trees, Graphs, Tries
- Hash Maps, Sets
- Dynamic Programming
- Greedy Algorithms
- Sliding Window, Two Pointers
- BFS, DFS, Topological Sort
- Binary Search variations
- Monotonic Stack / Queue

### Object-Oriented Programming
- SOLID Principles
- Design Patterns (Factory, Observer, Strategy, Singleton, Builder)
- Inheritance vs Composition
- Abstraction, Encapsulation, Polymorphism

### System Design
- Load Balancing
- Caching (Redis, Memcached)
- Database Sharding
- Message Queues (Kafka, RabbitMQ, SQS)
- Microservices vs Monolith
- CAP Theorem
- Rate Limiting
- API Gateway
- Event-Driven Architecture
- Observability (Metrics, Logs, Traces)

### Databases
- SQL (JOINs, Indexing, Normalization)
- NoSQL (MongoDB, DynamoDB, Cassandra)
- ACID Properties
- Query Optimization
- ORMs
- Vector Databases (Pinecone, ChromaDB, Qdrant, Weaviate)
- Time-Series Databases

### Operating Systems
- Processes vs Threads
- Concurrency, Deadlocks
- Memory Management
- File Systems
- Scheduling Algorithms

### Networks
- TCP/IP, HTTP/HTTPS, HTTP/2, HTTP/3
- REST vs GraphQL vs gRPC
- WebSockets, Server-Sent Events (SSE)
- DNS, CDN
- SSL/TLS

---

## Machine Learning

### Fundamentals
- Bias vs Variance tradeoff
- Overfitting and Underfitting
- Regularization (L1, L2, Dropout)
- Cross Validation (K-Fold, Stratified)
- Train/Val/Test split strategy
- Data Leakage
- Class Imbalance Strategies

### Evaluation Metrics
- Accuracy, Precision, Recall, F1
- AUC-ROC, AUC-PR
- Confusion Matrix
- Log Loss
- Mean Squared Error, RMSE, MAE
- R² Score
- Calibration Curves

### Algorithms
- Linear/Logistic Regression
- Decision Trees, Random Forests
- Gradient Boosting (XGBoost, LightGBM, CatBoost)
- SVM
- KNN
- K-Means, DBSCAN
- PCA, t-SNE, UMAP
- Bayesian Methods
- Gaussian Processes

### Feature Engineering
- One-Hot Encoding
- Label Encoding
- Feature Scaling (StandardScaler, MinMaxScaler)
- Feature Selection (Mutual Information, Recursive Feature Elimination)
- Handling Missing Data
- Handling Imbalanced Data (SMOTE, class weights, focal loss)
- Target Encoding
- Feature Stores (Feast, Tecton)

---

## Deep Learning

### Architectures
- CNN (Convolutional Neural Networks)
- RNN (Recurrent Neural Networks)
- LSTM, GRU
- Transformers
- Attention Mechanisms (Self, Cross, Multi-Head, Flash Attention)
- Autoencoders (VAE, DAE)
- GANs (Generative Adversarial Networks)
- Diffusion Models
- State Space Models (Mamba, S4)
- Mixture of Experts (MoE)

### Training
- Backpropagation
- Gradient Descent variants (SGD, Adam, AdamW)
- Learning Rate Scheduling (Cosine Annealing, Warm-up)
- Batch Normalization, Layer Normalization, RMSNorm
- Weight Initialization (Xavier, He, Kaiming)
- Mixed Precision Training (FP16, BF16)
- Gradient Clipping
- Gradient Accumulation
- Distributed Training (FSDP, DeepSpeed, Megatron-LM)

### Transfer Learning
- Pre-trained Models
- Fine-tuning strategies
- Feature Extraction
- Domain Adaptation
- Knowledge Distillation

---

## Computer Vision

### Tasks
- Image Classification
- Object Detection (YOLO v8/v9/v11, Faster R-CNN, DETR, RT-DETR)
- Semantic Segmentation (U-Net, DeepLab)
- Instance Segmentation (Mask R-CNN)
- Panoptic Segmentation
- Pose Estimation
- OCR (Optical Character Recognition)
- Image Generation (Stable Diffusion, FLUX)
- Document AI / Document Understanding
- Visual Grounding

### Tools & Libraries
- OpenCV
- Albumentations
- PIL/Pillow
- torchvision
- Supervision (Roboflow)
- Ultralytics

### Key Concepts
- Convolution, Pooling, Stride, Padding
- Anchor Boxes, NMS
- IoU (Intersection over Union)
- mAP (Mean Average Precision)
- Data Augmentation
- Vision Transformers (ViT, DINOv2, SigLIP)
- Foundation Models for Vision (SAM 2, Florence-2, Grounding DINO)

---

## GenAI / LLMs

### Core Concepts
- Large Language Models (LLMs)
- Tokenization (BPE, SentencePiece, Tiktoken)
- Attention is All You Need (Transformer Architecture)
- Prompt Engineering (Zero-Shot, Few-Shot, Chain-of-Thought, Tree-of-Thought)
- In-Context Learning
- Structured Outputs / JSON Mode
- Reasoning Models (o-series, DeepSeek-R1, Claude thinking)
- Long Context Windows (1M+ tokens)
- Mixture of Experts (MoE) Architecture

### RAG (Retrieval Augmented Generation)
- Document Chunking (recursive, semantic, agentic)
- Embedding Models (OpenAI, Cohere, BGE, Jina)
- Vector Databases (Pinecone, ChromaDB, Weaviate, Qdrant, FAISS, Milvus)
- Retrieval Strategies (dense, sparse, hybrid, re-ranking)
- Re-ranking (Cohere Rerank, ColBERT, cross-encoders)
- Agentic RAG (query planning, multi-step retrieval)
- GraphRAG (knowledge graph + retrieval)
- Evaluation (RAGAS, DeepEval, Braintrust)
- Hallucination Detection & Mitigation

### Fine-Tuning
- LoRA, QLoRA
- PEFT (Parameter Efficient Fine-Tuning)
- RLHF (Reinforcement Learning from Human Feedback)
- DPO (Direct Preference Optimization)
- GRPO (Group Relative Policy Optimization)
- Instruction Tuning
- Synthetic Data Generation for Fine-Tuning
- Evaluation of Fine-Tuned Models

### Agentic AI (🔥 CRITICAL for 2026 interviews)
- Function Calling / Tool Use
- Multi-Agent Systems (Supervisor, Swarm, Hierarchical)
- Planning & Reasoning (ReAct, Plan-and-Execute)
- Memory Systems (Short-term, Long-term, Episodic)
- Model Context Protocol (MCP)
- Agent-to-Agent Protocol (A2A)
- Error Recovery & Self-Correction
- Human-in-the-Loop (HITL) Checkpoints
- Agent Evaluation (Golden Trajectories, Step-Level Accuracy)
- Cost Management (Model Routing, Token Optimization)

### Key Interview Questions — Agentic AI
- "How would you design a multi-agent system for X? When supervisor vs swarm?"
- "How do you prevent an agent from getting stuck in an infinite loop?"
- "How would you evaluate the performance of an autonomous agent?"
- "Design an LLM gateway with model routing, rate limiting, and cost tracking."
- "How do you handle state management across long-running agent sessions?"
- "What guardrails would you implement for an agent that can write and execute code?"

---

## MLOps / LLMOps

### Core Practices
- Docker containerization
- Kubernetes orchestration
- MLflow / W&B experiment tracking
- CI/CD for ML pipelines (GitHub Actions, Jenkins)
- Model versioning & registry
- Model monitoring & observability
- Data versioning (DVC)
- Feature stores (Feast, Tecton)
- GPU cluster management
- Cost optimization for inference

### LLMOps (🆕 2026)
- Prompt versioning & management
- LLM observability (LangSmith, LangFuse, Helicone)
- Token usage tracking & cost allocation
- Model routing (big model for hard queries, small for easy)
- Caching strategies for LLM responses
- Guardrails deployment
- A/B testing LLM responses
- Evaluation pipelines (automated, LLM-as-judge)

### Monitoring
- Data Drift detection (Evidently AI, Great Expectations)
- Model Drift detection
- Performance monitoring (latency, throughput, error rate)
- Alerting systems (Prometheus, Grafana, PagerDuty)
- A/B testing in production
- Shadow deployment / Canary releases

---

## AI Safety & Responsible AI (Growing in 2026)

### Key Topics
- Prompt Injection Defense (direct, indirect)
- Jailbreak Prevention
- Red Teaming LLMs
- Guardrails Implementation (NeMo Guardrails, Guardrails AI, LLM Guard)
- Content Filtering & Moderation
- Bias Detection & Mitigation
- Fairness Metrics
- Explainability (SHAP, LIME, Grad-CAM)
- Human-in-the-Loop Design
- AI Governance & Compliance (EU AI Act, NIST AI RMF)
- Data Privacy in AI (Federated Learning, Differential Privacy)

---

## Behavioral Questions

### Key Themes
- **Leadership** — Leading a team or initiative
- **Teamwork** — Collaborating effectively
- **Conflict Resolution** — Handling disagreements
- **Ownership** — Taking responsibility and driving outcomes
- **Failure** — Learning from mistakes (what you'd do differently)
- **Ambiguity** — Working with unclear requirements
- **Impact** — Demonstrating measurable outcomes
- **Growth** — Continuous learning and improvement
- **Customer Focus** — Understanding user needs

### STAR Method
- **Situation** — Context and background
- **Task** — Your specific responsibility
- **Action** — What you did (focus on YOUR actions, use "I" not "we")
- **Result** — Quantified outcome and learnings

### 2026-Specific Behavioral Themes
- **AI Ethics** — "Tell me about a time you had to make a trade-off between model performance and fairness."
- **Production Ownership** — "Describe a time when an AI system you built failed in production. How did you diagnose and fix it?"
- **Cost Awareness** — "How did you optimize costs for an AI system?"
- **Cross-functional** — "How did you explain a complex AI concept to a non-technical stakeholder?"
