# Resume Rewrite Prompt

## Instructions

Rewrite resume bullet points to maximize impact, clarity, and recruiter engagement.

**Guiding principle:** A rewrite should make the resume more specific, more evidence-based, and more readable — for the human recruiter who will read it after the ATS parser succeeds. Don't optimize for a mythical keyword-counting robot.

## Input Required

- Original resume bullets (or full resume)
- Target role
- Target job description (if available — improves relevance)
- Target company (optional)

## Rewrite Rules

Follow the canonical rewrite rules from `knowledge/resume_best_practices.md` § "Rewrite Rules — Canonical Reference". Key points:

1. Don't remove relevant content — preserve specific tools, metrics, and terminology
2. Preserve technology names exactly — "YOLOv8" stays "YOLOv8"
3. Keep metrics — cut vague claims, not specific ones
4. Use the JD's own language where natural
5. Improve specificity and impact, don't just reshuffle words
6. Flag unverifiable or implausible claims

Use the bullet formula from `knowledge/resume_best_practices.md`:
```
Action Verb + What You Did + Technology Used + Quantified Impact
```

## Process

### Step 1: Assess Current State

Before rewriting, take stock of what's already there:
- What relevant terms and technologies are present?
- What metrics and outcomes are stated?
- What's working well that should be kept?
- What's weak (vague language, missing context, passive voice)?

### Step 2: Identify Weak Bullets

- Missing action verbs (starts with "Responsible for", "Worked on")
- No evidence of impact (no metrics, no outcomes, no context)
- Vague language without specificity
- Missing technology mentions
- Too long or too short

### Step 3: Rewrite Each Bullet

- Start with a strong action verb
- Include specific technologies used
- Add evidence of impact (metrics where available, outcomes when not)
- Keep under 2 lines
- Retain all relevant terms from the original — see canonical rules
- Use the JD's terminology where it naturally fits
- Don't replace specific tool names with generic descriptions

### Step 4: Optimize Section Order

- Lead with the most impressive/relevant bullets
- Group related achievements
- Vary action verbs across bullets

### Step 5: Post-Rewrite Sanity Check

After rewriting, verify:
1. **Relevant terms preserved** — Did any specific technologies, tools, or metrics from the original get lost? If so, restore them.
2. **Content improved** — Are the rewritten bullets more specific and impactful, or did they just get wordier?
3. **Parsing safety** — Did the rewrite introduce any format issues (special characters, overly complex structure)?
4. **Plausibility** — Are there any claims that seem implausible or that the candidate would struggle to defend in an interview? Flag these.

## Output Format

For each bullet:

```
ORIGINAL:
[original text]

REWRITTEN:
[improved text]

WHAT CHANGED:
- [specific improvement and why]
```

Final output:

```
Bullets Rewritten: __/__

Summary of Changes:
- Added evidence of impact to __ bullets
- Replaced __ weak/passive verbs
- Added __ missing technology mentions
- Flagged __ claims that may need verification

Plausibility Flags (if any):
- [bullet] — [concern]

Overall Assessment: [Stronger / Marginally Improved / Neutral — explain]
```
