# Career Full Review — Orchestration Prompt

## Instructions

Execute a **complete career package evaluation** producing a unified Career Score /100.

This is the flagship command. It orchestrates all individual rubrics and prompts into a single cohesive assessment.

## Input Required

- Resume (text or file)
- GitHub profile content (see Data Acquisition below)
- List of top 3–5 projects (with descriptions)
- Target role(s)
- LinkedIn profile content (optional — see Data Acquisition below)
- Experience level (Intern / Junior / Mid / Senior)

## Data Acquisition — How to Get Profile Data

> **Critical:** This skill cannot fetch live web content. All data must come from the user. Be explicit about what you need and don't hallucinate content you haven't been given.

### GitHub
Ask the user to provide ONE of the following:
1. **Paste their GitHub profile page content** — bio, pinned repos, contribution graph description
2. **Paste README files** from their top 3–5 repositories
3. **Describe their GitHub** — pinned repos, languages used, stars, documentation quality

If the user hasn't provided GitHub data, **ask for it explicitly** before scoring this section. Do not guess or infer. If the user declines, score GitHub as "Not Assessed" and adjust the Career Score weights accordingly.

### LinkedIn
Ask the user to provide ONE of the following:
1. **Paste their LinkedIn profile content** — headline, about section, experience, skills
2. **Screenshot** of their profile (if supported by the tool)
3. **Describe their LinkedIn** — headline, summary, endorsements, connections estimate

If not provided, mark LinkedIn as "Not Assessed" and use the weights without LinkedIn.

## Orchestration Sequence

### Step 1: Resume Analysis
- Load `rubrics/ai_resume_rubric.md` for scoring criteria (with calibration anchors)
- Load `prompts/ats_review.md` for ATS evaluation
- Load `prompts/keyword_analysis.md` for keyword gap analysis
- Load `knowledge/resume_best_practices.md` for quality benchmarks and canonical rewrite rules
- Load `knowledge/ai_ml_keywords.md` for role-specific keywords
- Reference `examples/good_resume_example.md` for before/after demonstrations
- **Output: ATS Score /100**

### Step 2: GitHub Analysis (requires user-provided data)
- Load `rubrics/github_rubric.md` for scoring criteria
- Load `prompts/github_review.md` for evaluation process
- Reference `examples/weak_github_example.md` for comparison
- **Precondition:** User must have provided GitHub profile content. If not, ask.
- **Output: GitHub Score /100 (or "Not Assessed")**

### Step 3: Project Portfolio Analysis
- Load `rubrics/project_evaluation_rubric.md` for scoring criteria
- Load `prompts/project_review.md` for evaluation process
- Load `knowledge/project_patterns.md` for strong/weak signal detection
- Reference `examples/strong_project_example.md` for benchmarks
- Score each project individually, then compute weighted average
- **Output: Project Score /100**

### Step 4: Interview Readiness Assessment
- Load `rubrics/interview_rubric.md` for scoring criteria
- Load `prompts/interview.md` for question bank
- Load `knowledge/interview_knowledge.md` for topic coverage
- Reference `examples/interview_answer_example.md` for STAR benchmarks
- Assess based on resume evidence + project depth + stated skills
- **Output: Interview Score /100**

### Step 5: Market Fit Assessment
- Load `knowledge/market_intelligence.md` for market demands
- Load `knowledge/ai_ml_keywords.md` for role alignment
- Cross-reference candidate's skills vs market demand
- ⚠️ **Staleness caveat:** Market data has a shelf life. Note the "Last Updated" date from market_intelligence.md. If it's >6 months old, caveat salary and trend claims with "as of [date] — verify against current postings."
- **Output: Market Fit Score /100**

### Step 6: LinkedIn Assessment (if data provided)
- Load `rubrics/linkedin_rubric.md` for scoring criteria
- Load `prompts/linkedin_review.md` for evaluation process
- **Precondition:** User must have provided LinkedIn content. If not, ask. If declined, skip.
- **Output: LinkedIn Score /100 (or "Not Assessed")**

### Step 7: Personalization (if available)
- Load `knowledge/my_profile.md` for candidate context
- Compare current state vs goals
- Identify specific gaps relative to target companies and roles

## Score Calculation

```
Career Score = weighted average of:
  ATS Score        × 0.25
  Project Score    × 0.25
  GitHub Score     × 0.15
  Interview Score  × 0.20
  Market Fit Score × 0.15

If LinkedIn provided:
  Career Score = weighted average of:
    ATS Score        × 0.20
    Project Score    × 0.20
    GitHub Score     × 0.15
    Interview Score  × 0.15
    Market Fit Score × 0.15
    LinkedIn Score   × 0.15

If GitHub or LinkedIn is "Not Assessed":
  Redistribute their weight proportionally across assessed categories.
  State which categories were not assessed and why.
```

## Output Format

```
CAREER READINESS REPORT

Career Score: __/100  [Elite|Strong|Adequate|Weak|Rebuild]

  ATS Score        __/100
  Project Score    __/100
  GitHub Score     __/100 (or "Not Assessed")
  Interview Score  __/100
  Market Fit Score __/100
  LinkedIn Score   __/100 (or "Not Assessed")

TOP STRENGTHS
1. ...
2. ...
3. ...

CRITICAL GAPS
1. ...
2. ...
3. ...

30-DAY ACTION PLAN
Week 1: ...
Week 2: ...
Week 3: ...
Week 4: ...

90-DAY ROADMAP
Month 1: ...
Month 2: ...
Month 3: ...

TARGET READINESS
Role: [Target Role]
Current Level: [Not Ready / Almost Ready / Ready]
Estimated time to ready: [X weeks/months]
```

## Rules for Scoring

1. **Never inflate scores** — Use the calibration anchors in each rubric. A 60 means 60.
2. **Evidence-based only** — Score only what you can see or verify.
3. **Ask for missing info** — Don't guess. If GitHub data isn't provided, ask. If the user declines, mark as "Not Assessed."
4. **Cross-reference** — If resume claims "deployed" but no deployment evidence exists (no link, no GitHub, no demo), flag the discrepancy.
5. **Flag unverifiable claims** — If metrics seem implausible (e.g., "99.99% accuracy on a novel task"), note it as a potential interview risk.
6. **Actionable plans only** — Every weakness must have a concrete fix in the 30/90 day plan.
7. **Prioritize by impact** — 30-day plan should focus on highest-ROI improvements first.
8. **Resume rewrite rules** — When suggesting resume improvements, follow the canonical rewrite rules in `knowledge/resume_best_practices.md` § "Rewrite Rules — Canonical Reference".
9. **Caveat stale data** — If quoting salaries, model names, or market trends from knowledge files, check the "Last Updated" date and caveat if it's old.
