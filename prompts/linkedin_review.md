# LinkedIn Review Prompt

## Instructions

Evaluate a LinkedIn profile for recruiter visibility, professional branding, and AI/ML career optimization.

## Input Required

- LinkedIn profile URL or screenshots
- Target role (for keyword alignment)
- Current experience level

## Evaluation Process

Score using `rubrics/linkedin_rubric.md` (100 points total).

### Review Areas

1. **Headline Analysis**
   - Does it contain role-specific keywords?
   - Is it more than "Student at X"?
   - Does it communicate value?

2. **About Section**
   - Is there a compelling narrative?
   - Are technical keywords present naturally?
   - Does it mention top achievements?
   - Is there a call to action?

3. **Experience Section**
   - Impact-driven bullets (Action + Metric)?
   - Relevant to target role?
   - Media attachments (screenshots, links)?

4. **Featured Section**
   - Top projects pinned?
   - Blog posts or articles?
   - Visual media (thumbnails, screenshots)?

5. **Skills & Endorsements**
   - Top 3 skills match target role?
   - Adequate endorsements?

6. **Activity & Content**
   - Posting frequency?
   - Technical content quality?
   - Community engagement?

7. **Network & Recommendations**
   - 500+ connections?
   - Written recommendations?

## Output Format

```
LinkedIn Profile Score: __/100

Headline:       __/15
About:          __/15
Experience:     __/20
Featured:       __/15
Skills:         __/10
Activity:       __/15
Network:        __/10

✅ Strengths:
- ...

❌ Issues:
- ...

✍️ Rewritten Headline Suggestions:
1. "[Suggested headline 1]"
2. "[Suggested headline 2]"
3. "[Suggested headline 3]"

✍️ About Section Draft:
"[Suggested About section based on their profile]"

🔧 Improvement Plan:
1. [Quick win — do today] ...
2. [This week] ...
3. [This month] ...

🚩 Red Flags Found:
- ...
```
