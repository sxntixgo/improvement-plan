# Consolidated Learning Plan - Overview

**Security Engineer → AI Red Teaming Transition**
**Available Time: 18 hours/week**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

**Mode: Sequential (one track at a time)**
**Updated: February 7, 2026**

-----

## What This Plan Builds On

This plan is not starting from zero. Two significant strengths shape the structure:

- **Go is your work language.** You write Go daily on the job. The plan front-loads Go as the vehicle for learning software architecture, then layers security tooling on top. Go gets 19 total weeks (crash course + foundations/architecture + security tools) because it directly serves your career.
- **You already build with Claude Code.** Track 3 is designed for an advanced user, not a beginner walkthrough. It focuses on workflow automation, multi-file refactoring, and integrating Claude Code into your development process at scale.

The restructured plan teaches architecture in Go first (Track 8), then transfers that knowledge to Python (Track 9) and beyond. This means Python Core can be compressed without losing depth, and Go security tooling (Track 11) becomes a unique differentiator for AI red teaming.

-----

## Priority Order & Timeline

|Track|Name                                      |Weeks |Duration |File                                       |
|-----|------------------------------------------|------|---------|-------------------------------------------|
|1    |Reading Skills                            |1     |1 week   |[track-01-reading-skills.md](track-01-reading-skills.md)|
|2    |Note-Taking (Obsidian)                    |2-3   |2 weeks  |[track-02-note-taking.md](track-02-note-taking.md)|
|3    |Claude Code Advanced                      |4     |1 week   |[track-03-claude-code.md](track-03-claude-code.md)|
|4    |Git Mastery                               |5     |1 week   |[track-04-git-mastery.md](track-04-git-mastery.md)|
|5    |Go Crash Course                           |6     |1 week   |[track-05-go-crash-course.md](track-05-go-crash-course.md)|
|6    |Docker Essentials                         |7     |1 week   |[track-06-docker-essentials.md](track-06-docker-essentials.md)|
|7    |LLM Security Primer                       |8     |1 week   |[track-07-llm-security-primer.md](track-07-llm-security-primer.md)|
|8    |Go Foundations + Software Architecture    |9-20  |12 weeks |[track-08-go-foundations-architecture.md](track-08-go-foundations-architecture.md)|
|11   |Go Security Tools (Black Hat Go)          |21-24 |4 weeks  |[track-11-go-security.md](track-11-go-security.md)|
|     |**Break**                                 |      |1 week   |                                           |
|9    |Python Core + TDD                         |25-32 |8 weeks  |[track-09-python-core.md](track-09-python-core.md)|
|10   |AI/ML Security + Go for AI Security       |33-42 |10 weeks |[track-10-ai-ml-security.md](track-10-ai-ml-security.md)|
|     |**Break**                                 |      |1 week   |                                           |
|12   |Python Advanced                           |43-48 |6 weeks  |[track-12-python-advanced.md](track-12-python-advanced.md)|
|13   |JavaScript/TypeScript                     |49-62 |14 weeks |[track-13-javascript.md](track-13-javascript.md)|
|     |**Break**                                 |after 56|1 week |                                           |

**Total Duration:** 62 learning weeks + 3 break weeks = **65 weeks (~15 months)**

### Language Allocation

|Language          |Tracks                              |Total Weeks|
|------------------|------------------------------------|-----------|
|Go                |5 (crash) + 8 (foundations/arch) + 11 (Black Hat Go) + 10 capstone (2 wks)|19 weeks|
|Python            |9 (core + TDD) + 12 (advanced)     |14 weeks   |
|JavaScript/TypeScript|13                               |14 weeks   |

-----

## Weekly Habits

|Habit      |When                     |Output                                   |
|-----------|-------------------------|-----------------------------------------|
|Blog update|End of each week         |Progress, learnings, reflections         |
|Book review|After finishing each book|Published review on blog                 |
|Code push  |As you build             |Public GitHub repos for relevant projects|

-----

## Key Changes from Previous Plan

1. **Go is front-loaded as the work language.** Track 8 is 12 weeks of Go + software architecture, taught together.
2. **Software architecture is learned in Go, not just Python.** Design patterns, clean architecture, and project structure are all practiced in Go first.
3. **Python Core compressed from 10 to 8 weeks.** Architecture concepts already learned in Go transfer directly; Python track focuses on Python-specific idioms, TDD, and pytest.
4. **Go Security (Track 11) placed right after Go Foundations (Track 8).** 16+ continuous weeks of Go mastery with no context-switching. Black Hat Go builds directly on Track 8 architecture skills. Go for AI Security (2 weeks) is a capstone in Track 10, after learning AI security concepts.
5. **Python Advanced compressed from 8 to 6 weeks.** Go concurrency knowledge (goroutines, channels) transfers to Python asyncio, reducing ramp-up time.
6. **JS/TS compressed from 20 to 14 weeks.** Focused on what matters for web security context.
7. **Claude Code track updated for advanced users.** Assumes existing experience; focuses on power-user workflows and automation.
8. **Go Crash Course includes self-assessment.** Skip material you already know from daily work; spend time only on gaps.
9. **Go total allocation up from 13 to 19 weeks.** Reflects Go's central role in your current job and future security tooling.
10. **Python total: 14 weeks (down from 18).** Still substantial, but architecture learning already done in Go.
11. **JS/TS: 14 weeks (down from 20).** Compressed but complete.

-----

## Track Logic

```
Reading → Note-Taking → Claude Code Advanced
                              ↓
                    Git Mastery ← Foundation for all development
                              ↓
                    Go Crash Course ← For immediate work needs
                              ↓
                    Docker Essentials ← Infrastructure for all projects
                              ↓
                    LLM Security Primer (Wilson book) ← Security context
                              ↓
                    Go Foundations + Software Architecture ← Work language + architecture
                              ↓
                    Go Security Tools (Black Hat Go) ← 16+ weeks continuous Go mastery
                              ↓
                    Python Core + TDD ← Architecture transfers from Go
                              ↓
                    AI/ML Security + Go for AI Security ← requires Python; Go capstone at end
                              ↓
                    Python Advanced (AST, async) ← Go concurrency knowledge transfers
                              ↓
                    JavaScript/TypeScript ← Web security context (compressed)
```

**Why Go is front-loaded (Tracks 5, 8, 11):**
- You write Go at work every day. Learning architecture in Go means immediate application on the job.
- Go Crash Course (Track 5) fills gaps in your existing knowledge with a self-assessment gate.
- Go Foundations + Software Architecture (Track 8) is the longest single track at 12 weeks because it carries dual purpose: deep Go mastery and software design principles.
- Go Security Tools (Track 11) is placed **immediately after Track 8** to maintain momentum — 16+ continuous weeks of Go with no context-switching.
- Go for AI Security (Track 10 capstone, Weeks 41-42) comes after AI/ML Security so you can build Go-based AI security tools, a rare and valuable skill set.

**Why architecture is taught in Go, then transferred:**
- Learning architecture in your strongest language reduces cognitive load.
- Python Core (Track 9) can then focus on Python-specific patterns (TDD, pytest, Pythonic idioms) instead of re-teaching design principles.
- This compression is why Python Core drops from 10 to 8 weeks without losing effectiveness.

**Why Git and Docker early:**
- **Git** is foundational for ALL development work (code management, collaboration).
- **Docker** enables containerized dev environments, ML deployment, security labs.
- Both learned early = available for all future tracks.

**Why Python is split:**
- **Python Core + TDD** (Track 9): pytest, TDD workflow, Pythonic patterns. Architecture transfers from Go.
- **Python Advanced** (Track 12): AST manipulation, async/await. Go concurrency knowledge (goroutines, channels, select) maps directly to asyncio concepts.

-----

## Books Already Owned

|Book                                          |Track                                   |
|----------------------------------------------|----------------------------------------|
|How to Read a Book (Adler & Van Doren)        |Track 1: Reading Skills                 |
|Speed Reading (Knight)                        |Track 1: Reading Skills                 |
|How to Take Smart Notes (Ahrens)              |Track 2: Note-Taking                    |
|Building a Second Brain (Forte)               |Track 2: Note-Taking                    |
|Pro Git (Chacon & Straub)                     |Track 4: Git Mastery                    |
|Developer's Playbook for LLM Security (Wilson)|Track 7: LLM Security Primer            |
|Test-Driven Development with Python (Percival)|Track 9: Python Core + TDD              |
|Black Hat Go (Steele et al.)                  |Track 11: Go Security Tools             |
|Node.js: The Comprehensive Guide (Springer)   |Track 13: JavaScript/TypeScript         |
|Web Development with Node and Express (Brown) |Track 13: JavaScript/TypeScript         |
|You Don't Know JS 1st edition (Simpson)       |Track 13: JavaScript/TypeScript         |
|Eloquent JavaScript (Haverbeke)               |Track 13: JavaScript/TypeScript         |
|100 Go Mistakes (Harsanyi)                    |Track 8: Go Foundations + Architecture  |

-----

## Books to Purchase

|Book                                      |Cost |Track                                    |
|------------------------------------------|-----|-----------------------------------------|
|Learning Go, 2nd ed (Bodner)              |~$50 |Track 8: Go Foundations + Architecture   |
|Let's Go (Edwards)                        |~$40 |Track 8: Go Foundations + Architecture   |
|Python Testing with pytest, 2nd ed (Okken)|~$40 |Track 9: Python Core + TDD              |
|AI Engineering (Huyen)                    |~$50 |Track 10: AI/ML Security                |
|Red Teaming AI (Dursey)                   |~$50 |Track 10: AI/ML Security (releases July 2026)|

**Total: ~$230**

-----

## Downtime Reading List

Passive content for commutes, lunch breaks, or when you need a break from active learning.

### Blogs

|Blog                 |Focus                 |URL                     |
|---------------------|----------------------|------------------------|
|Anthropic Research   |AI safety, alignment  |anthropic.com/research  |
|Simon Willison       |LLMs, Python, security|simonwillison.net       |
|Lil'Log (Lilian Weng)|ML/AI deep dives      |lilianweng.github.io    |
|Trail of Bits        |Security research     |blog.trailofbits.com    |
|PortSwigger Research |Web security          |portswigger.net/research|
|Nicholas Carlini     |Adversarial ML        |nicholas.carlini.com    |

### Podcasts

|Podcast          |Focus             |
|-----------------|------------------|
|Darknet Diaries  |Security stories  |
|Latent Space     |AI/ML engineering |
|Risky Business   |Security news     |
|Talk Python to Me|Python ecosystem  |
|Go Time          |Go ecosystem      |
|Syntax           |JavaScript/web dev|

### Newsletters

|Newsletter            |Focus                |
|----------------------|---------------------|
|TLDR Sec              |Security news digest |
|The Pragmatic Engineer|Engineering career   |
|Python Weekly         |Python news          |
|JavaScript Weekly     |JS news              |
|Golang Weekly         |Go news              |
|Import AI             |AI research summaries|

### YouTube Channels

|Channel      |Focus                 |
|-------------|----------------------|
|LiveOverflow |Security research     |
|John Hammond |CTF/security          |
|ArjanCodes   |Python patterns       |
|Fireship     |Quick tech explainers |
|3Blue1Brown  |Math/ML visualizations|
|Computerphile|CS concepts           |

### Papers (When Ready)

|Paper                         |Why                      |
|------------------------------|-------------------------|
|Attention Is All You Need     |Transformer foundation   |
|OWASP LLM Top 10              |LLM vulnerabilities      |
|Constitutional AI (Anthropic) |Anthropic's approach     |
|Universal Adversarial Triggers|Prompt injection research|

### Books (Light Reading)

|Book                             |Why                                |When           |
|---------------------------------|-----------------------------------|---------------|
|How AI Works (Kneusel)           |Conceptual AI primer, no heavy math|Before Track 7 |
|AI Snake Oil (Narayanan & Kapoor)|Critical thinking about AI claims  |Anytime        |

-----

## Leadership Reading List (Bedtime Reading)

**27 leadership/business books you already own** - organized for bedtime reading throughout your 65-week journey.

**See detailed reading list with checklists:** [leadership-reading-list.md](leadership-reading-list.md)

### Quick Summary

**Books Currently Reading:**
- [x] The Southwest Airlines Way
- [x] The Captains Class
- [x] Marcelo Bielsa: Los 11 Caminos al Gol

**Next Book to Start:**
- [ ] **The Score Takes Care of Itself** (Bill Walsh) - Perfect for Week 1!

### Reading by Phase

|Phase|Weeks|Priority Books|
|-----|-----|--------------|
|Foundation|1-8|Score Takes Care of Itself, Atomic Habits, High Output Management|
|Deep Work|9-28|Legacy, Captains Class, Leaders Eat Last, Start With Why|
|Mastery|29-48|Bielsa, Paradigma Guardiola, Creativity Inc, Elon Musk|
|Finishing|49-65|Revolución Scaloni, Measure What Matters, The Snowball|

**Reading Pace:** 20-30 pages/night = 1 book every 2-4 weeks = 20-25 books over 65 weeks

**Your Strength:** 7 sports leadership books

**Full details, checklists, and reading order:** See [leadership-reading-list.md](leadership-reading-list.md)

-----
