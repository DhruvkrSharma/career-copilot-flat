# Career Diagnose — Quick Triage Prompt

## Instructions

Perform a **rapid diagnostic** (5-minute triage) of career readiness. This is the lightweight version of `career full-review`.

## Input Required

- Resume (text or file)
- Target role
- GitHub URL (optional)

## Quick Checklist

Run through this checklist and assign a traffic light to each:

```
CAREER QUICK DIAGNOSTIC
═══════════════════════

Resume
  □ Exists and is 1 page?                    🟢 🟡 🔴
  □ Has 3+ projects with metrics?             🟢 🟡 🔴
  □ Uses action verbs (not "responsible for")? 🟢 🟡 🔴
  □ Includes GitHub + LinkedIn links?          🟢 🟡 🔴
  □ Skills section matches target role?        🟢 🟡 🔴

GitHub
  □ Has 4+ pinned repos with READMEs?          🟢 🟡 🔴
  □ Active in last 3 months?                   🟢 🟡 🔴
  □ At least 1 deployed project?               🟢 🟡 🔴

Projects
  □ At least 1 project beyond tutorial-level?  🟢 🟡 🔴
  □ At least 1 project with evaluation metrics?🟢 🟡 🔴
  □ At least 1 project with deployment?        🟢 🟡 🔴

Interview Readiness
  □ Can explain top 2 projects in STAR format?  🟢 🟡 🔴
  □ Familiar with DSA fundamentals?             🟢 🟡 🔴
  □ Knows ML theory basics?                     🟢 🟡 🔴

Market Fit
  □ Has at least 1 GenAI/LLM project?           🟢 🟡 🔴
  □ Has deployment/MLOps experience?             🟢 🟡 🔴
```

## Traffic Light Scoring

- 🟢 **Green** (2 pts) — Meets standard, no action needed
- 🟡 **Yellow** (1 pt) — Partially meets, minor fix needed
- 🔴 **Red** (0 pts) — Missing or failing, urgent fix needed

**Max Score: 32 points**

## Output Format

```
QUICK DIAGNOSTIC RESULT
═══════════════════════

Diagnostic Score: __/32

Resume:     🟢🟢🟡🔴🟢  __/10
GitHub:     🟢🟡🔴       __/6
Projects:   🟢🟢🟡       __/6
Interview:  🟡🟢🟢       __/6
Market Fit: 🔴🟡         __/4

Overall Status: [🟢 Ready | 🟡 Gaps to Fix | 🔴 Not Ready]

🔥 Top 3 Urgent Fixes:
1. [Highest impact fix]
2. [Second priority]
3. [Third priority]

⏱️ Estimated time to fix: [X days/weeks]

💡 Run `career full-review` for detailed scoring and 30/90 day plan.
```

## When to Use

- First-time assessment (before deep review)
- Weekly check-in on progress
- Quick pre-application readiness check
