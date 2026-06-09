# 🚀 Career Copilot — AI/ML Career Operating System

A comprehensive Claude Skill for AI/ML career optimization. ATS analysis, resume optimization, keyword research, GitHub review, LinkedIn review, project evaluation, interview preparation, market fit analysis, and career readiness scoring.

## 📋 What This Does

Career Copilot is a complete **career operating system** for AI/ML engineers. Instead of evaluating just your resume, it evaluates your entire candidate package:

- **Resume** — ATS compatibility, keyword density, bullet quality
- **GitHub** — Profile presentation, code quality, documentation
- **LinkedIn** — Recruiter visibility, professional brand, network
- **Projects** — Technical depth, deployment, documentation, metrics
- **Interview Readiness** — STAR answers, technical fluency, system design
- **Market Fit** — Alignment with 2025 hiring trends and in-demand skills

## 🎯 Commands

| Command | Description |
|---------|-------------|
| `career diagnose` | Quick 5-minute triage with traffic-light scoring |
| `career keywords` | Keyword gap analysis for target roles |
| `career optimize` | Resume optimization for ATS and recruiters |
| `career github` | GitHub profile review and scoring |
| `career linkedin` | LinkedIn profile review and scoring |
| `career projects` | Project portfolio evaluation |
| `career interview` | Technical + behavioral interview simulation |
| `career full-review` | **Complete career package evaluation** → Career Score /100 |

## 📁 Folder Structure

```
career-copilot/
├── SKILL.md                              # Entry point — commands, persona, file routing
│
├── knowledge/
│   ├── ai_ml_keywords.md                 # Keywords by role (AI, ML, CV, GenAI, MLOps, SWE)
│   ├── project_patterns.md               # Strong vs weak project signals
│   ├── interview_knowledge.md            # Interview topics (DSA, ML, DL, CV, GenAI, Behavioral)
│   ├── resume_best_practices.md          # Resume writing rules and ATS optimization
│   ├── market_intelligence.md            # 2025 hiring trends, salaries, hot skills
│   └── my_profile.md                     # Personal profile template (fill in your details)
│
├── rubrics/
│   ├── ai_resume_rubric.md               # 100-point resume scoring (7 categories)
│   ├── github_rubric.md                  # 100-point GitHub scoring (7 categories)
│   ├── interview_rubric.md               # 100-point interview scoring (6 categories)
│   ├── project_evaluation_rubric.md      # 100-point project scoring (9 categories)
│   └── linkedin_rubric.md                # 100-point LinkedIn scoring (7 categories)
│
├── prompts/
│   ├── career_full_review.md             # Orchestration prompt (flagship command)
│   ├── career_diagnose.md                # Quick triage diagnostic
│   ├── ats_review.md                     # ATS compatibility analysis
│   ├── keyword_analysis.md               # Keyword gap analysis
│   ├── resume_rewrite.md                 # Resume bullet rewriting
│   ├── github_review.md                  # GitHub profile evaluation
│   ├── linkedin_review.md                # LinkedIn profile evaluation
│   ├── project_review.md                 # Project portfolio evaluation
│   └── interview.md                      # Interview simulation
│
└── examples/
    ├── good_resume_example.md            # Weak vs strong resume bullets
    ├── strong_project_example.md         # S-tier project benchmark
    ├── interview_answer_example.md       # STAR method demonstrations
    ├── weak_github_example.md            # Bad vs good GitHub profiles
    ├── linkedin_example.md               # Weak vs strong LinkedIn profiles
    └── system_design_answer.md           # ML system design answers
```

## 🔧 Installation

### For Claude Code (Skills)
```bash
mkdir -p ~/.claude/skills/
cp -r career-copilot/ ~/.claude/skills/career-copilot/
```

### Personalization
Edit `knowledge/my_profile.md` with your actual details to enable personalized scoring.

## 📊 Full Review Output

Running `career full-review` produces:

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

🏆 Top Strengths
⚠️ Critical Gaps
📋 30-Day Action Plan
📋 90-Day Roadmap
🎯 Target Readiness
```

## 🎓 Target Roles

Optimized for:
- AI Engineer
- Machine Learning Engineer
- Computer Vision Engineer
- Data Scientist
- MLOps Engineer
- Software Engineer
- GenAI Engineer

## 📈 What Makes This Different

Unlike simple resume review tools, Career Copilot:

1. **Evaluates the full package** — Resume + GitHub + LinkedIn + Projects + Interview readiness
2. **Uses structured rubrics** — 100-point scoring with transparent criteria
3. **Market-aware** — Knows what recruiters are looking for in 2025
4. **Personalized** — Fill in your profile for tailored recommendations
5. **Actionable** — Every weakness comes with a concrete fix and timeline

## 📝 License

MIT
