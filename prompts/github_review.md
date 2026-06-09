# GitHub Review Prompt

## Instructions

Evaluate a GitHub profile for recruiter readiness and technical credibility.

## Input Required

- GitHub username or profile URL
- Target role (for context)

## Evaluation Process

Score using `rubrics/github_rubric.md` (100 points total).

### Review Areas

1. **Profile Setup**
   - Photo, bio, pinned repos, links

2. **Repository Audit** (top 5–6 repos)
   - README completeness
   - Code structure and organization
   - Documentation quality
   - Dependencies managed
   - License present

3. **Technical Assessment**
   - Complexity of projects
   - Technology diversity
   - AI/ML specific work
   - Testing presence

4. **Activity Analysis**
   - Contribution graph density
   - Recency of commits
   - Commit message quality

5. **Engineering Practices**
   - Branching, PRs, issues
   - CI/CD pipelines
   - Code quality tools

6. **Community Signal**
   - Open source contributions
   - Stars, forks, followers

## Output Format

```
GitHub Profile Score: __/100

Profile: __/10
Repos: __/25
Technical: __/20
Activity: __/15
Engineering: __/15
Community: __/10
Presentation: __/5

🏆 Top Repositories:
1. [repo] — [why it's strong]
2. [repo] — [why it's strong]

⚠️ Repos Needing Work:
1. [repo] — [what to fix]

🔧 Improvement Plan:
1. ...
2. ...
3. ...

🚩 Red Flags:
- ...
```
