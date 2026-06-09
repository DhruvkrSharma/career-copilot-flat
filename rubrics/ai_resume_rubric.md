# AI/ML Resume Scoring Rubric

**Total Score: 100 points**

> **Scoring guidance:** Use the calibration anchors under each category to assign scores. When uncertain, pick the lower score and explain what would earn the higher one. Avoid false precision — a 3-point range is more honest than an exact number.

---

## 1. ATS Compatibility / Parseability (20 points)

> This gates everything. A beautifully-written resume scores zero if the ATS parser garbles it.

| Criteria | Points | Description |
|----------|--------|-------------|
| No ATS-breaking formatting | 6 | No tables, graphics, columns, text boxes, Unicode symbols, or emojis |
| Standard section headers | 4 | Uses recognizable headers (Education, Experience, Skills, Projects) |
| Selectable text, safe file format | 4 | PDF with copyable text or .docx. Not image-PDF |
| Relevant terms present | 3 | Core skills for the target role are findable by a recruiter searching the ATS |
| Acronym + full form for key terms | 3 | Ambiguous terms include both: "Natural Language Processing (NLP)" |

**Calibration anchors:**
| Score | What it looks like |
|-------|--------------------|
| 18–20 | Clean single-column PDF, standard headers, all relevant skills present, no formatting risks |
| 14–17 | Mostly clean but minor issues (e.g., one creative header, missing a key acronym expansion) |
| 8–13 | Some formatting risks (light use of columns or tables) OR several relevant skills missing |
| 0–7 | Tables, graphics, image-PDF, or unrecognizable section headers. Parser will fail |

---

## 2. Technical Skills Section (15 points)

| Criteria | Points | Description |
|----------|--------|-------------|
| Relevance | 5 | Skills match target AI/ML roles |
| Organization | 3 | Grouped by category (Languages, Frameworks, Tools) |
| Depth vs Breadth | 4 | Balance between range and demonstrated depth |
| Currency | 3 | Includes current industry-standard tools |

**Calibration anchors:**
| Score | What it looks like |
|-------|--------------------|
| 13–15 | Skills well-organized by category, all relevant to target role, current tools, defensible in interview |
| 9–12 | Reasonable skills but poorly organized, or some outdated/irrelevant entries |
| 5–8 | Skills present but mostly irrelevant to target role, or unorganized wall of text |
| 0–4 | No skills section, or skills that suggest a different career entirely |

---

## 3. Project Quality (25 points)

| Criteria | Points | Description |
|----------|--------|-------------|
| Number of projects | 3 | 3–5 relevant projects |
| Problem statements | 4 | Clear real-world problems being solved |
| Technical complexity | 5 | Advanced techniques, not tutorial-level |
| Evidence of results | 5 | Concrete outcomes (metrics, deployments, user impact). Note: metrics are scored as-stated; flag implausible claims but don't verify |
| Deployment evidence | 4 | Projects deployed or accessible |
| Tech stack clarity | 4 | Technologies clearly mentioned in context |

**Calibration anchors:**
| Score | What it looks like |
|-------|--------------------|
| 21–25 | 4+ projects with clear problems, specific tech stacks, concrete results, at least 1 deployed. Non-tutorial |
| 15–20 | 3+ projects with some metrics and tech detail, but limited deployment or originality |
| 8–14 | Projects exist but are tutorial-level, lack metrics, or have vague descriptions |
| 0–7 | No projects section, or only 1 trivially-described project |

---

## 4. Experience Section (15 points)

| Criteria | Points | Description |
|----------|--------|-------------|
| Impact-driven bullets | 5 | Action Verb + Task + Outcome format |
| Relevance | 4 | AI/ML/SWE relevant experience |
| Progression | 3 | Shows growth in responsibility |
| Evidence of results | 3 | Outcomes described (metrics where available, context when not) |

**Calibration anchors:**
| Score | What it looks like |
|-------|--------------------|
| 13–15 | Strong action verbs, clear outcomes, relevant roles, shows growth |
| 9–12 | Decent experience but weak bullets (duties instead of achievements) or limited relevance |
| 5–8 | Experience present but mostly irrelevant, or all bullets are task descriptions |
| 0–4 | No experience section, or only unrelated work (e.g., retail with no technical framing) |

---

## 5. Education (10 points)

| Criteria | Points | Description |
|----------|--------|-------------|
| Degree relevance | 4 | CS, AI, Math, Statistics, or related |
| GPA (if applicable) | 2 | > 3.5 or equivalent |
| Relevant coursework | 2 | ML, DL, CV, NLP, Statistics listed |
| Academic achievements | 2 | Publications, thesis, honors |

**Calibration anchors:**
| Score | What it looks like |
|-------|--------------------|
| 8–10 | Relevant degree, strong GPA, coursework listed, academic achievements |
| 5–7 | Relevant degree but no GPA/coursework listed, or GPA below 3.5 |
| 2–4 | Unrelated degree but some relevant coursework or self-study evidence |
| 0–1 | No education section or completely unrelated field with no bridge |

---

## 6. Communication Quality (10 points)

| Criteria | Points | Description |
|----------|--------|-------------|
| Clarity | 3 | Easy to read and understand |
| Conciseness | 3 | No filler words or vague statements |
| Grammar & spelling | 2 | Error-free |
| Consistent formatting | 2 | Uniform style throughout |

**Calibration anchors:**
| Score | What it looks like |
|-------|--------------------|
| 8–10 | Clear, concise, error-free, consistent. Could hand to a recruiter right now |
| 5–7 | Readable but some filler, minor inconsistencies, or 1–2 errors |
| 2–4 | Noticeable grammar issues, inconsistent formatting, or verbose/vague throughout |
| 0–1 | Hard to read, many errors, no consistent style |

---

## 7. Differentiators (5 points)

| Criteria | Points | Description |
|----------|--------|-------------|
| Unique projects | 1 | Not common tutorial projects |
| Open source contributions | 1 | Evidence of community involvement |
| Certifications | 1 | Relevant, recognized certifications |
| Hackathons / Competitions | 1 | Kaggle, hackathon placements |
| Publications / Blog | 1 | Technical writing or research |

---

## Score Interpretation

| Score | Rating | Meaning |
|-------|--------|---------|
| 85–100 | Elite | Resume is strong. Ready for top-tier applications. Minor polish only. |
| 70–84 | Strong | Solid foundation. A few specific improvements would elevate it. |
| 55–69 | Adequate | Gets the point across but has clear gaps. Needs targeted work. |
| 40–54 | Weak | Significant issues in multiple categories. Needs substantial revision. |
| Below 40 | Rebuild | Fundamental problems (parsing, missing sections, no projects). Start over with guidance. |

## Honesty & Plausibility Check

When scoring, apply these checks:
- **Metrics are scored as-stated** — If a user claims "96% accuracy," score the bullet for having a metric. You cannot verify the number.
- **Flag implausible claims** — If something seems too good ("99.99% accuracy on a novel task") or vague ("improved performance significantly"), note it as a potential interview risk rather than a strength.
- **Cross-reference where possible** — If resume says "deployed" but no deployment evidence exists (no link, no GitHub, no demo), flag the discrepancy.
- **Don't penalize absence of proof, but don't reward unverified superlatives** — A bullet with "94% accuracy" is better than "great accuracy," but worse than "94% accuracy (validation set, 5-fold CV, confusion matrix in repo)."
