# Career Full Review — Orchestration Prompt

## Instructions

Execute a **complete career package evaluation** producing a unified Career Score /100.

This is the flagship command. It orchestrates all individual rubrics and prompts into a single cohesive assessment.

## Input Required

- Resume (text or file)
- GitHub username or profile URL
- List of top 3–5 projects (with descriptions)
- Target role(s)
- LinkedIn profile URL (optional)
- Experience level (Intern / Junior / Mid / Senior)

## Orchestration Sequence

### Step 1: Resume Analysis
- Load `rubrics/ai_resume_rubric.md` for scoring criteria
- Load `prompts/ats_review.md` for ATS evaluation
- Load `prompts/keyword_analysis.md` for keyword gap analysis
- Load `knowledge/resume_best_practices.md` for quality benchmarks
- Load `knowledge/ai_ml_keywords.md` for role-specific keywords
- Reference `examples/good_resume_example.md` for before/after demonstrations
- **Output: ATS Score /100**

### Step 2: GitHub Analysis
- Load `rubrics/github_rubric.md` for scoring criteria
- Load `prompts/github_review.md` for evaluation process
- Reference `examples/weak_github_example.md` for comparison
- **Output: GitHub Score /100**

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
- Load `knowledge/market_intelligence.md` for current market demands
- Load `knowledge/ai_ml_keywords.md` for role alignment
- Cross-reference candidate's skills vs market hotlist
- Evaluate target role alignment
- Assess competitiveness for target companies
- **Output: Market Fit Score /100**

### Step 6: LinkedIn Assessment (if provided)
- Load `rubrics/linkedin_rubric.md` for scoring criteria
- Load `prompts/linkedin_review.md` for evaluation process
- **Output: LinkedIn Score /100**

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
```

## Output Format

```
═══════════════════════════════════════════
         CAREER READINESS REPORT
═══════════════════════════════════════════

Career Score: __/100  [Elite|Strong|Good|Average|Weak]

┌─────────────────────────────────────────┐
│  ATS Score        ██████████░░  __/100  │
│  Project Score    ████████░░░░  __/100  │
│  GitHub Score     ██████░░░░░░  __/100  │
│  Interview Score  ████████████  __/100  │
│  Market Fit Score ██████████░░  __/100  │
│  LinkedIn Score   ████████░░░░  __/100  │
└─────────────────────────────────────────┘

🏆 TOP STRENGTHS
1. ...
2. ...
3. ...

⚠️ CRITICAL GAPS
1. ...
2. ...
3. ...

📋 30-DAY ACTION PLAN
Week 1: ...
Week 2: ...
Week 3: ...
Week 4: ...

📋 90-DAY ROADMAP
Month 1: ...
Month 2: ...
Month 3: ...

🎯 TARGET READINESS
Role: [Target Role]
Current Level: [Not Ready / Almost Ready / Ready]
Estimated time to ready: [X weeks/months]
```

## Rules for Scoring

1. **Never inflate scores** — Be honest. A 60 means 60.
2. **Evidence-based only** — Score only what you can see/verify.
3. **Ask for missing info** — Don't guess. If GitHub URL isn't provided, ask.
4. **Cross-reference** — If resume claims "deployed" but GitHub shows no deployment code, flag the discrepancy.
5. **Actionable plans only** — Every weakness must have a concrete fix in the 30/90 day plan.
6. **Prioritize by impact** — 30-day plan should focus on highest-ROI improvements first.
