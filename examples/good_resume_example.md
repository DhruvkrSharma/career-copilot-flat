# Good Resume Examples — Weak vs Strong

## Example 1: Face Recognition Project

### ❌ Weak
> Created a face recognition attendance system.

### ✅ Strong
> Built a real-time face recognition attendance system using OpenCV and KNN, achieving 96% recognition accuracy across 500+ facial samples while reducing manual attendance processing time by 90%.

### Why Strong:
- Action verb: "Built"
- Technology: OpenCV, KNN
- Metric: 96% accuracy
- Scale: 500+ samples
- Impact: 90% time reduction

---

## Example 2: Object Detection

### ❌ Weak
> Worked on object detection using YOLO.

### ✅ Strong
> Engineered a real-time object detection pipeline using YOLOv8 and FastAPI, achieving 92% mAP@0.5 on a custom 10K-image dataset with inference latency under 30ms per frame.

### Why Strong:
- Specific model version (YOLOv8)
- Deployment tech (FastAPI)
- Metric: 92% mAP@0.5
- Dataset scale: 10K images
- Performance: 30ms latency

---

## Example 3: NLP / GenAI

### ❌ Weak
> Helped with building a chatbot using LangChain.

### ✅ Strong
> Architected a RAG-based customer support chatbot using LangChain, ChromaDB, and GPT-4, reducing average ticket resolution time by 45% across 10K+ monthly queries.

### Why Strong:
- Action verb: "Architected"
- Full tech stack listed
- Business metric: 45% reduction
- Scale: 10K+ queries/month

---

## Example 4: Data Pipeline

### ❌ Weak
> Responsible for data preprocessing tasks.

### ✅ Strong
> Designed and automated a data preprocessing pipeline using Apache Airflow and Pandas, processing 2M+ records daily with 99.5% data quality accuracy, reducing manual effort by 80%.

### Why Strong:
- Not "responsible for" — uses "Designed and automated"
- Specific tools
- Scale: 2M+ records
- Quality metric: 99.5%
- Impact: 80% effort reduction

---

## Example 5: Model Optimization

### ❌ Weak
> Optimized a machine learning model.

### ✅ Strong
> Reduced inference latency of a production ResNet-50 model by 60% through TensorRT optimization and INT8 quantization, enabling deployment on edge devices with < 50ms response time.

### Why Strong:
- Specific model (ResNet-50)
- Specific technique (TensorRT, INT8)
- Metric: 60% reduction
- Context: edge deployment
- Performance: < 50ms

---

## Pattern Summary

| Element | Weak | Strong |
|---------|------|--------|
| Verb | "Worked on", "Helped" | "Built", "Engineered", "Architected" |
| Tech | Vague or missing | Specific tools and versions |
| Metrics | None | Accuracy, latency, scale, impact |
| Impact | Not mentioned | Quantified business/technical impact |
| Scale | Not mentioned | Dataset size, users, throughput |

---

## ATS Optimization Examples — Keyword Preservation

### ❌ BAD Optimization (Drops ATS Score)

**Original bullet:**
> Built a face recognition attendance system using OpenCV and KNN, achieving 96% accuracy on 500+ samples.

**Bad rewrite:**
> Orchestrated an advanced biometric verification solution leveraging cutting-edge computer vision algorithms, delivering superior recognition performance across hundreds of facial samples.

**Why BAD:**
- Dropped keywords: "OpenCV", "KNN", "96%", "500+"
- Replaced exact tools with vague descriptions
- ATS searching for "OpenCV" or "KNN" will NOT find this resume
- Score DECREASED despite sounding "fancier"

### ✅ GOOD Optimization (Boosts ATS Score)

**Original bullet:**
> Built a face recognition attendance system using OpenCV and KNN, achieving 96% accuracy on 500+ samples.

**Good rewrite:**
> Engineered a real-time face recognition attendance system using OpenCV, KNN, and Python, achieving 96% validation accuracy across 500+ facial samples while reducing manual attendance processing time by 90%.

**Why GOOD:**
- ALL original keywords preserved: OpenCV, KNN, 96%, 500+
- Keywords ADDED: "Python", "real-time", "validation accuracy"
- Metric ADDED: "90% processing time reduction"
- Action verb upgraded: "Built" → "Engineered"
- ATS score INCREASED

### ❌ BAD: Skills-Only Keyword Placement

```
Skills: PyTorch, Docker, FastAPI, RAG, LangChain

Projects:
• Built a chatbot that answers questions from documents
• Made an image classifier with good accuracy
```

**Problem:** Keywords only in Skills section. Project bullets have zero keyword matches. ATS scores this LOW.

### ✅ GOOD: Multi-Placement Keywords

```
Skills: PyTorch, Docker, FastAPI, RAG, LangChain

Projects:
• Architected a RAG-based document Q&A chatbot using LangChain and ChromaDB, deployed via FastAPI and Docker, serving 10K+ queries/month
• Built a PyTorch image classification model achieving 94% accuracy on a custom 15K-image dataset, with REST API via FastAPI
```

**Why GOOD:** Every keyword from Skills also appears in context inside bullets. ATS ranks this MUCH higher.

