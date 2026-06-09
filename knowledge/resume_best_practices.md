# Resume Best Practices

> **Last Updated:** June 2026
> ⚠️ Salary figures, model names, and "hot skills" in this file reflect conditions at the time of writing. Verify against current job postings before quoting to candidates. See `knowledge/market_intelligence.md` for the same caveat.

## General Rules

- Maximum **1 page** for students and early-career (0–3 years).
- Maximum **2 pages** for experienced professionals (3+ years).
- Use a clean, ATS-friendly format (no tables, graphics, columns, or fancy templates).
- Use a standard font: Arial, Calibri, Garamond, or Inter (10–12pt).
- Use consistent formatting throughout.
- Save as PDF with selectable text (unless asked for .docx). Never submit image-PDFs.
- Use reverse chronological order within each section.
- Include a **targeted summary** (2–3 lines) at the top tailored to the specific role — not a generic objective statement.

## Section Priority (for AI/ML roles)

### For GenAI / Agentic AI roles:
1. **Contact Information** — Name, Email, Phone, LinkedIn, GitHub, Portfolio
2. **Summary** — 2–3 lines targeting the specific role, mentioning key skills
3. **Skills** — Languages, Frameworks, LLMs, Tools, Platforms (grouped by category)
4. **Projects** — 3–5 impactful projects with metrics (lead with agentic/GenAI projects)
5. **Experience** — Internships, Research, Work Experience
6. **Education** — Degree, University, GPA (if > 3.5), Relevant Coursework
7. **Certifications / Achievements** — Hackathons, Publications, Awards

### For Traditional ML / CV / Data Science roles:
1. **Contact Information** — Name, Email, Phone, LinkedIn, GitHub, Portfolio
2. **Education** — Degree, University, GPA (if > 3.5), Relevant Coursework
3. **Skills** — Languages, Frameworks, Tools, Platforms
4. **Projects** — 3–5 impactful projects with metrics
5. **Experience** — Internships, Research, Work Experience
6. **Certifications** — Relevant certifications only
7. **Achievements** — Hackathons, Publications, Awards

## Skills Section Formatting

Group skills by category. This makes both ATS search and recruiter scanning effective:

```
Languages: Python, C++, SQL, TypeScript
ML/DL Frameworks: PyTorch, TensorFlow, Scikit-learn, Hugging Face Transformers
GenAI / LLM: LangChain, LangGraph, LlamaIndex, OpenAI API, Gemini API
Vector Databases: ChromaDB, Pinecone, Qdrant, FAISS
MLOps & Infra: Docker, Kubernetes, MLflow, GitHub Actions, AWS SageMaker
Tools: Git, Weights & Biases, LangSmith, Streamlit, FastAPI
```

**Rules:**
- Include both **tool name and version** where relevant: "YOLOv8", not just "YOLO"
- Add a **GenAI / LLM** category if targeting GenAI roles
- Don't list more than 25–30 skills total — list only what you can defend in an interview
- Include both acronyms AND full forms for ambiguous terms: "Retrieval Augmented Generation (RAG)"

## Writing Bullet Points

### Formula

```
Action Verb + What You Did + Technology Used + Quantified Impact
```

### Strong Examples

✅ Built a CNN-based fruit classification model achieving **94% validation accuracy** on 15 classes using TensorFlow and Keras.

✅ Deployed a real-time object detection API using **YOLOv8 and FastAPI**, processing **30 FPS** on edge devices with Docker containerization.

✅ Reduced model inference latency by **40%** through TensorRT optimization and INT8 quantization, cutting cost per request by **60%**.

✅ Architected a multi-agent RAG system using **LangGraph and ChromaDB**, improving answer relevance by **35%** measured via RAGAS faithfulness scoring.

✅ Fine-tuned **Llama 4 Scout** using LoRA on a 50K-sample domain dataset, achieving **15% task accuracy improvement** over the base model at **3x lower inference cost**.

### Weak Examples

❌ Responsible for machine learning tasks.

❌ Worked on a deep learning project.

❌ Helped with data preprocessing.

❌ Used Python and TensorFlow. *(too passive — say "Built X using Y")*

❌ Built a chatbot using OpenAI API. *(too vague — no architecture, no metrics, no scale)*

## Action Verbs to Use

| Category | Verbs |
|----------|-------|
| **Building** | Architected, Built, Designed, Developed, Engineered, Implemented |
| **Improving** | Enhanced, Optimized, Reduced, Streamlined, Accelerated |
| **Leading** | Led, Directed, Managed, Coordinated, Spearheaded |
| **Research** | Analyzed, Evaluated, Investigated, Published, Researched |
| **Deploying** | Deployed, Launched, Released, Shipped, Containerized |
| **AI-Specific** | Fine-tuned, Trained, Orchestrated, Automated, Integrated |

## Action Verbs to AVOID

- Responsible for
- Worked on
- Helped with
- Assisted
- Participated in
- Was involved in
- Tasked with

## ATS & Resume Optimization — What Actually Matters

> **Key insight:** Mainstream ATS (Greenhouse, Lever, Workday) are databases and workflow tools, not auto-rejection keyword-counters. The real risks are parsing failures and missing the terms recruiters search for. See `prompts/ats_review.md` for the full model.

### High-Impact (Fix These First)
- **No tables, columns, graphics, text boxes, or images** — These break ATS parsers and cause content to be garbled or lost entirely. This is the #1 real risk.
- **Use standard section headers** — "Education", "Experience", "Skills", "Projects". Not "My Journey" or "What I Know". Parsers are trained on standard headers.
- **PDF with selectable text** — Image-PDFs, .pages files, and scanned documents can't be parsed at all.
- **No special characters** — Unicode symbols, smart quotes, emojis, and box-drawing characters can choke parsers.
- **Consistent date formatting** — Parsers use dates to structure your experience timeline. "Jan 2024 – Mar 2025" throughout, not mixed formats.

### Medium-Impact (Do These Next)
- **Include terms recruiters will search for** — Use the same terminology as the job description. If the JD says "Deployed", write "Deployed". This isn't about density — it's about being findable when a recruiter searches.
- **Include both acronym and full form** for ambiguous terms — "Natural Language Processing (NLP)" — because you don't know which form the recruiter will search.
- **Standard bullet points** (•, -, *), not custom symbols.
- **Don't use headers/footers for critical information** — Some parsers skip these entirely.

### Low-Impact / Myths to Avoid
- ❌ **"Keyword density" targets** — There is no evidence that repeating a keyword 2–3 times ranks you higher. Write naturally. If a skill is important, it will appear in your Skills section and in a relevant bullet — that's sufficient.
- ❌ **"≥60% JD keyword match"** — ATS doesn't compute match percentages and reject below a threshold. Recruiters search manually.
- ❌ **"Keywords must appear in multiple sections"** — There's no evidence ATS scores "multi-placement." Use keywords where they naturally belong. Skills section for the list, bullets for context.

## Rewrite Rules — Canonical Reference

> **This is the single authoritative source** for rules governing resume rewrites. Other files (`prompts/resume_rewrite.md`, `prompts/ats_review.md`, `prompts/career_full_review.md`) reference this section rather than duplicating it.

When rewriting or optimizing a resume:

1. **Don't remove relevant content** — If the original resume contains a term that's relevant to the target role, the rewritten version should retain it unless there's a good reason to cut it (e.g., it's inaccurate or irrelevant). Replacing "TensorFlow" with "deep learning framework" loses specificity for no benefit.
2. **Preserve technology names exactly** — Don't change "YOLOv8" to "YOLO" or "FastAPI" to "API framework". Specific names are more useful to both ATS search and human readers.
3. **Keep metrics** — If a bullet has "94% accuracy", the rewritten version should keep it. Cut vague claims, not specific ones.
4. **Use the JD's own language** — If the job description says "Deployed", write "Deployed" — not a synonym the recruiter won't search for.
5. **Improve, don't just rearrange** — A rewrite should make bullets more specific, more impactful, and more evidence-based. If the rewrite just shuffles words, it's not an improvement.
6. **Flag unverifiable claims** — If the user claims "99.9% accuracy" with no context, note that this may be questioned in an interview. Don't score it as a strength without evidence.
7. **Verify the rewrite improved things** — After rewriting, compare the before/after. Did relevant terms survive? Did content get more specific or more vague? Did parsing safety change?

## Showing Production Readiness

Companies want engineers who ship, not just prototype. Signal production readiness:
- ✅ "Deployed via Docker on AWS ECS, serving 500 req/sec"
- ✅ "Monitored with LangSmith, tracking latency and error rate"
- ❌ "Ran in Jupyter notebook locally"

## Include Cost & Evaluation Context Where Truthful

If you genuinely optimized costs or built evaluation systems, mention it:
- "Reduced LLM API costs by 45% through model routing"
- "Evaluated RAG pipeline with RAGAS (faithfulness: 0.89)"

Don't fabricate these — interviewers will ask for details.

## Links to Include

- **GitHub** — Active profile with pinned projects, README, and CI badges
- **LinkedIn** — Updated and matching resume content
- **Portfolio / Blog** — Deployed projects, technical writing
- **Live Demo Links** — Deployed project URLs
- **Hugging Face** — If you have published models or datasets

## Common Mistakes

1. **No evidence of impact** — Every bullet should show what changed because of your work.
2. **Too many skills** — List only skills you can defend in an interview (max 25–30).
3. **Irrelevant experience** — Focus on ML/AI/SWE relevant work.
4. **Typos/grammar** — Proofread meticulously.
5. **Inconsistent tense** — Past tense for completed, present for ongoing.
6. **Too long** — Ruthlessly cut non-essential content.
7. **Generic objective** — Replace with a targeted summary specific to the role.
8. **Listing duties instead of achievements** — Show impact, not tasks.
9. **Unverifiable superlatives** — "Best-in-class model" or "cutting-edge solution" without evidence damages credibility.
10. **Outdated tool names** — Keep skills current. If you list a tool you used years ago, make sure it's still relevant.
