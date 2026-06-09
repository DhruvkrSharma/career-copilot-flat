# Keyword Analysis Prompt

## Instructions

Perform a keyword gap analysis between a candidate's resume and their target role. The goal is to identify relevant terms that are missing — not to hit density targets or match percentages.

**Important framing:** This analysis helps the candidate use the right terminology so recruiters can find them when searching the ATS. It is NOT about gaming a keyword-counting algorithm. See `prompts/ats_review.md` for the evidence-based ATS model.

## Input Required

- Resume text
- Target role (e.g., "AI Engineer", "Computer Vision Engineer")
- Target job description (if available — significantly improves relevance)

## Analysis Steps

### 1. Extract Resume Terms

- Technical skills mentioned (tools, frameworks, languages)
- Methodologies and techniques
- Domain-specific terms
- Metrics and evidence of outcomes

### 2. Extract Target Terms

- **From job description (if provided):** Extract technical terms, tools, skills, methodologies, and qualifications. Note the JD's exact phrasing — recruiters often search using their own JD's language.
- **From role keyword bank:** Reference `knowledge/ai_ml_keywords.md` for the target role's expected skills.

### 3. Gap Analysis

| Category | What to check |
|----------|--------------|
| ✅ **Present** | Terms in the resume that are relevant to the target role/JD |
| ❌ **Missing & Important** | Terms from the JD or core role skills that are absent from the resume and that the candidate could plausibly add |
| ⚠️ **Missing but Aspirational** | Terms the candidate doesn't have experience with — these shouldn't be added dishonestly |
| 🔇 **Present but Irrelevant** | Terms in the resume that aren't relevant to this specific role — candidates may want to cut these to save space |

### 4. Priority Ranking

Rank missing terms by relevance:

1. **High priority** — Appears in the JD or is a core skill for this role. Missing these means a recruiter searching for them won't find you.
2. **Medium priority** — Relevant to the role but not explicitly in the JD. Having these makes the candidate more competitive.
3. **Stretch / aspirational** — Skills the candidate is learning or hasn't used yet. These should NOT be added to the resume unless the candidate can defend them in an interview.

### 5. Plausibility Check

For each suggested addition, consider:
- Can the candidate truthfully claim this skill?
- Will they be able to discuss it in an interview?
- Is there evidence in their projects/experience to support it?

If not, mark it as aspirational rather than "add this now."

## Output Format

```
Keyword Analysis for [Target Role]

Relevant Terms Present: __ terms found
Important Terms Missing: __ terms to consider adding
Irrelevant Terms: __ terms that could be removed to save space

HIGH PRIORITY (recruiters will likely search for these):
- [term] — in JD / core role skill. Suggested placement: [Skills section / specific bullet]
- ...

MEDIUM PRIORITY (strengthens candidacy):
- [term] — relevant to role. Add if you have genuine experience
- ...

ASPIRATIONAL (don't add unless truthful):
- [term] — in-demand but candidate may not have experience yet
- ...

COULD REMOVE (save space for more relevant terms):
- [term] — not relevant to this target role
- ...

Suggested Bullet Improvements:
- [Existing bullet] → add "[missing term]" if the candidate actually used it
- ...
```
