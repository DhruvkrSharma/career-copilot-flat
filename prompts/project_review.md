# Project Review Prompt

## Instructions

Evaluate an AI/ML project for portfolio quality, interview value, and recruiter impact.

## Input Required

- Project Name
- Problem Statement
- Architecture / Approach
- Dataset used
- Training details
- Deployment status
- Repository link (if available)

## Evaluation Process

Score using `rubrics/project_evaluation_rubric.md` (100 points total).

### Review Areas

1. **Problem Definition** (10 pts)
   - Is the problem clear and real-world?
   - Who benefits from this solution?

2. **Technical Complexity** (20 pts)
   - Is this beyond tutorial-level?
   - Custom implementations or novel approaches?

3. **Model Performance** (15 pts)
   - Are evaluation metrics reported?
   - Baseline comparisons?
   - Error analysis?

4. **Software Engineering** (15 pts)
   - Code quality and structure?
   - Testing? Version control?

5. **Deployment** (10 pts)
   - Is it accessible / demo-able?
   - Docker, web app, API?

6. **Documentation** (10 pts)
   - README quality?
   - Architecture diagrams?

7. **Innovation** (10 pts)
   - What makes this unique?
   - Not a common tutorial project?

8. **Scalability** (5 pts)
   - Performance optimized?
   - Handles real-world load?

9. **Business Impact** (5 pts)
   - Real-world applicability?
   - Clear value proposition?

## Output Format

```
Project Score: __/100

Problem:      __/10
Complexity:   __/20
Performance:  __/15
Engineering:  __/15
Deployment:   __/10
Documentation:__/10
Innovation:   __/10
Scalability:  __/5
Impact:       __/5

✅ Strengths:
- ...

❌ Weaknesses:
- ...

📈 Resume Value: [High/Medium/Low]
🎤 Interview Value: [High/Medium/Low]
💼 Portfolio Value: [High/Medium/Low]

🔧 Improvement Roadmap:
1. [Quick Win] ...
2. [Medium Effort] ...
3. [High Impact] ...
```
