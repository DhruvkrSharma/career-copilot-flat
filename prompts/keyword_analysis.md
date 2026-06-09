# Keyword Analysis Prompt

## Instructions

Perform a comprehensive keyword gap analysis between a candidate's resume and their target AI/ML role.

## Input Required

- Resume text
- Target role (e.g., "AI Engineer", "Computer Vision Engineer")
- Target job description (optional)

## Analysis Steps

1. **Extract Resume Keywords**
   - Technical skills mentioned
   - Tools and frameworks
   - Methodologies
   - Soft skills

2. **Load Target Keywords**
   - Reference `knowledge/ai_ml_keywords.md` for the target role
   - Extract keywords from job description (if provided)

3. **Gap Analysis**
   - Keywords present in resume ✅
   - Keywords missing from resume ❌
   - Keywords in resume but not needed ⚠️ (noise)

4. **Priority Ranking**
   - Must-have keywords (critical gaps)
   - Nice-to-have keywords (improvement opportunities)
   - Bonus keywords (differentiators)

## Output Format

```
Keyword Analysis for [Target Role]

Match Rate: __% (__/__ keywords matched)

✅ Present Keywords:
- ...

❌ Critical Missing Keywords:
- ...

⚠️ Nice-to-Have Missing:
- ...

📊 Priority Actions:
1. Add [keyword] — appears in 80%+ of job descriptions
2. Add [keyword] — demonstrates [skill area]
3. ...

💡 Suggested Resume Bullets Using Missing Keywords:
- "Built [project] using [missing keyword], achieving [metric]"
- ...
```
