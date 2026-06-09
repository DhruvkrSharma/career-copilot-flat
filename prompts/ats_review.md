# ATS Review Prompt

## Instructions

Analyze the provided resume for ATS (Applicant Tracking System) compatibility.

## Input Required

- Resume text (paste or upload)
- Target job title (e.g., "AI Engineer", "ML Engineer")
- Target job description (optional, for keyword matching)

## Evaluation Steps

1. **Format Check**
   - Standard section headers?
   - No tables, graphics, or columns?
   - Clean bullet points?
   - Proper font and sizing assumptions?
   - PDF-friendly?

2. **Keyword Analysis**
   - Extract keywords from resume
   - Compare against target role keywords (from `knowledge/ai_ml_keywords.md`)
   - Compare against job description keywords (if provided)
   - Calculate keyword match percentage

3. **Section Completeness**
   - Contact info complete? (Name, Email, Phone, LinkedIn, GitHub)
   - Education present?
   - Skills section present and organized?
   - Projects/Experience with metrics?

4. **Content Quality**
   - Action verbs used? (refer to `knowledge/resume_best_practices.md`)
   - Metrics and quantification present?
   - Weak phrases detected? ("responsible for", "worked on", etc.)

## Output Format

```
ATS Compatibility Score: __/100

Format Score: __/25
Keyword Score: __/25
Section Score: __/25
Content Score: __/25

✅ Strengths:
- ...

❌ Issues Found:
- ...

🔧 Recommended Fixes:
1. ...
2. ...
3. ...

Missing Keywords:
- ...
```
