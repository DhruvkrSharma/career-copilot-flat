# ATS Review Prompt

## Instructions

Analyze the provided resume for ATS (Applicant Tracking System) compatibility.

**What ATS actually is:** Most mainstream ATS (Greenhouse, Lever, Workday, iCIMS) are primarily databases and recruiter-workflow tools — not auto-rejection engines that filter on keyword counts. They parse and store resumes so recruiters can search, rank, and manage candidates. The real risks are:
1. **Parsing failure** — Bad formatting (tables, columns, graphics, image-PDFs) causes the ATS to garble or lose content entirely. This is the #1 real risk.
2. **Recruiter search misses** — Recruiters keyword-search within the ATS. If your resume lacks the terms they search for, you won't surface. This is about presence, not density.
3. **Readability by humans** — The recruiter reads what the ATS parsed. If parsing mangled your content, you're out regardless of keywords.

**What ATS is NOT:** A magic keyword-counting robot that rejects resumes below a "match percentage." Don't keyword-stuff. Don't game density. Write for the human who will read you after the parser succeeds.

## Input Required

- Resume text (paste or upload)
- Target job title (e.g., "AI Engineer", "ML Engineer")
- Target job description (if provided — improves keyword relevance assessment)

## Evaluation Steps

### 1. Parseability & Format (30 points)

This is the highest-risk category. A perfectly-written resume scores zero if the ATS can't parse it.

| Check | Points | What to verify |
|-------|--------|---------------|
| No ATS-breaking elements | 8 | No tables, graphics, multi-column layouts, text boxes, headers/footers with critical info, images, icons, or logos |
| Standard section headers | 6 | Uses recognizable headers: "Education", "Experience", "Skills", "Projects" — not creative variants like "What I Know" or "My Journey" |
| Selectable text | 4 | PDF with selectable/copyable text, or .docx. NOT image-PDF, NOT .pages, NOT scanned document |
| Clean bullet points | 4 | Standard bullet characters (•, -, *), not custom symbols, emojis, or box-drawing characters |
| No parser-hostile characters | 4 | No Unicode symbols, smart quotes, ligatures, or non-ASCII characters that parsers choke on |
| Consistent date format | 4 | Uniform date format throughout (e.g., "Jan 2024 – Mar 2025") — parsers use dates to structure experience |

### 2. Keyword Relevance (25 points)

The goal is **presence of relevant terms** so recruiters find you when searching. This is NOT about density or repetition.

| Check | Points | What to verify |
|-------|--------|---------------|
| Role-relevant skills present | 10 | Resume contains the core skills a recruiter would search for in this role. Reference `knowledge/ai_ml_keywords.md` for the target role. Are the obvious terms present? |
| JD alignment (if JD provided) | 8 | Key requirements from the job description are reflected in the resume. Use the JD's terminology — recruiters often search using their own JD's language |
| Acronym + full form for ambiguous terms | 4 | Terms that have common acronyms should include both forms at least once: "Natural Language Processing (NLP)" — because a recruiter might search either form |
| No irrelevant keyword clutter | 3 | Skills listed are defensible in an interview. Listing 50 buzzwords you can't discuss hurts you with the human, even if it looks good to a search |

### 3. Section Completeness (20 points)

| Check | Points | What to verify |
|-------|--------|---------------|
| Contact info complete | 4 | Name, Email, Phone, LinkedIn URL, GitHub URL — all present and parseable |
| Education present | 4 | Degree, University, Graduation date. GPA if strong (>3.5). Relevant coursework if space allows |
| Skills section organized | 4 | Grouped by category (Languages, Frameworks, Tools, Platforms) — not a wall of text. This is what recruiters scan first |
| Projects with evidence of impact | 4 | 3–5 projects, each with at least 1 concrete result (metric, outcome, or deployment evidence) |
| Experience section | 4 | Role, Company, Duration, Impact bullets. If no professional experience, acknowledge it honestly |

### 4. Content Quality (25 points)

| Check | Points | What to verify |
|-------|--------|---------------|
| Strong action verbs | 5 | Bullets start with action verbs. Refer to `knowledge/resume_best_practices.md`. No instances of "Responsible for", "Worked on", "Helped with" |
| Evidence of impact | 6 | Bullets show what was achieved, not just what was done. Metrics where available, but outcomes/context even without numbers |
| Technology in context | 5 | Technologies mentioned WITH context ("Built X using TensorFlow") rather than just listed. This helps both ATS search and recruiter understanding |
| No weak/vague language | 5 | No filler phrases: "responsible for", "worked on", "helped with", "various", "etc." |
| Concise and readable | 4 | Bullets are 1–2 lines max. No walls of text. Easy to scan in 15 seconds |

## Output Format

```
ATS Compatibility Assessment: [Strong / Adequate / Needs Work / At Risk]

Parseability:  __/30  [this is what actually breaks things]
Keywords:      __/25
Completeness:  __/20
Content:       __/25
Total:         __/100

CRITICAL PARSING RISKS (fix these first):
- ...

Keyword Gaps (terms a recruiter would likely search for):
- ...

Content Improvements:
- ...
```

**Scoring guidance:** Use band descriptors below, not pseudo-precise point allocations. When uncertain between two scores for a sub-item, pick the lower one and explain what would earn the higher score.

| Band | Score | Meaning |
|------|-------|---------|
| Strong | 85–100 | Parses cleanly, relevant terms present, strong content. Ready to submit. |
| Adequate | 70–84 | No parsing risks, most terms present, some content improvements possible. Submittable with minor edits. |
| Needs Work | 50–69 | Some parsing risks OR significant keyword gaps OR weak content. Revise before submitting. |
| At Risk | Below 50 | Parsing will likely fail OR major sections missing. Requires significant rework. |

## Comparative Re-Verification Mode

When this prompt is used AFTER a resume rewrite (as a post-optimization check):

1. **Parsing check** — Confirm the rewrite didn't introduce format issues.
2. **Keyword diff** — List terms that were preserved, added, or dropped. Dropped terms should be flagged for review — they may or may not matter depending on relevance.
3. **Content comparison** — Did the rewrite improve clarity, specificity, and impact? Or did it just reshuffle words?
4. **Verdict** — Has the resume improved overall for both ATS parseability and human readability?

```
RE-VERIFICATION:
Parsing: [Clean / Issues introduced]
Keywords: [Added: __, Dropped: __ (review these), Preserved: __]
Content: [Improved / Neutral / Degraded]
Overall: [Improved / Neutral / Regressed — explain why]
```
