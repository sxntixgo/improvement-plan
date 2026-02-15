# Consolidated Learning Plan - Overview

**Security Engineer → AI Red Teaming Transition**
**Available Time: 18 hours/week**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

**Mode: Sequential (one track at a time)**
**Updated: February 15, 2026**

-----

## What This Plan Builds On

This plan is designed for an **architect who directs Claude Code**, not a hands-on coder. Two facts shape everything:

- **You don't write code — Claude Code does.** You architect systems, review output, and give Claude Code precise directions. Every track focuses on understanding patterns and making architectural decisions, not typing syntax. Track 3 is the most important foundation week because Claude Code is your primary tool.
- **Go is your work language, but Claude Code writes it.** You need to understand Go architecture deeply enough to review what Claude Code produces, catch design mistakes, and give effective direction. You don't need to memorize syntax — you need to think in systems.

The restructured plan prioritizes **software architecture first, then AI/ML security** — the two things that matter for your role. Python and JavaScript tracks are either repositioned or dropped because Claude Code handles the implementation.

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
|8    |Software Architecture (via Go)            |9-20  |12 weeks |[track-08-go-foundations-architecture.md](track-08-go-foundations-architecture.md)|
|10   |AI/ML Security                            |21-28 |8 weeks  |[track-10-ai-ml-security.md](track-10-ai-ml-security.md)|
|     |**Break**                                 |      |1 week   |                                           |
|9    |Python Core + TDD                         |30-37 |8 weeks  |[track-09-python-core.md](track-09-python-core.md)|
|11   |Go Security Tools + AI Capstone           |38-43 |6 weeks  |[track-11-go-security.md](track-11-go-security.md)|

**Total Duration:** 43 learning weeks + 1 break week = **44 weeks (~10 months)**

### Why This Order

**Architecture → AI/ML → Python → Go Security Tools**

1. **Architecture first (Track 8):** You need to think in systems to direct Claude Code effectively. Clean architecture, DDD, and testing patterns are the language of good engineering direction.
2. **AI/ML immediately after (Track 10):** This is your career goal. You don't need Python syntax to understand RAG architecture, prompt injection, or model vulnerabilities — Claude Code writes the code while you focus on concepts and attack surfaces.
3. **Python after AI/ML (Track 9):** Deepens your understanding of the tools you've already used. Now you understand why pytest works the way it does, how Python architecture differs from Go, and can give Claude Code more precise Python direction.
4. **Go Security Tools last (Track 11):** Combines everything — Go architecture knowledge + AI security concepts + understanding of how security tools work. The capstone produces an AI Red Team CLI tool in Go.

### What Was Dropped

|Track|Why Dropped|
|-----|-----------|
|Track 12: Python Advanced (AST, async)|Not needed for an architect. Claude Code handles async Python. You understand concurrency concepts from Go.|
|Track 13: JavaScript/TypeScript|Not relevant to your AI red teaming goal. You own 3 JS books if you ever need them later.|

**Savings:** 20 weeks of coding-focused tracks that don't serve your architect + AI red teaming path.

-----

## The Architect Mindset

Every track in this plan follows the same pattern:

1. **Understand the concept** — Read, study, watch. Know WHY a pattern exists.
2. **Direct Claude Code to build it** — Give precise architectural instructions. Use CLAUDE.md files.
3. **Review the output** — Check architecture, not syntax. Does the structure follow clean architecture? Are dependencies pointing inward? Is the testing strategy right?
4. **Iterate** — Give Claude Code better direction based on what you see.

This is fundamentally different from "learn to code." You're learning to **think like a senior architect** who happens to use AI as their implementation tool.

-----

## Weekly Habits

|Habit      |When                     |Output                                   |
|-----------|-------------------------|-----------------------------------------|
|Blog update|End of each week         |Progress, learnings, reflections         |
|Book review|After finishing each book|Published review on blog                 |
|Code push  |As you build             |Public GitHub repos for relevant projects|

-----

## Track Logic

```
Reading → Note-Taking → Claude Code Advanced (YOUR PRIMARY TOOL)
                              ↓
                    Git Mastery ← Foundation for all development
                              ↓
                    Go Crash Course ← Understand your work language
                              ↓
                    Docker Essentials ← Infrastructure for all projects
                              ↓
                    LLM Security Primer (Wilson book) ← Security context
                              ↓
                    Software Architecture via Go ← Think in systems
                              ↓
                    AI/ML Security ← YOUR CAREER GOAL (moved up!)
                              ↓
                    Python Core + TDD ← Deepen understanding post-AI/ML
                              ↓
                    Go Security Tools + AI Capstone ← Combine everything
```

**Why AI/ML moved up (from Week 33 to Week 21):**
You don't write code — Claude Code does. That means you don't need to master Python syntax before studying AI/ML security. You need to understand:
- How foundation models work (to attack them)
- How RAG and agents are architected (to find vulnerabilities)
- How production AI systems are built (to identify attack surfaces)

Claude Code writes the Python for HTB labs, LangChain apps, and exploit scripts. You focus on the architecture and the attack.

**Why Python comes AFTER AI/ML:**
- You've already used Python tools during AI/ML (via Claude Code)
- Now you understand WHY you need Python knowledge
- Track 9 deepens your ability to review Python code and direct Claude Code better
- Architecture patterns from Go (Track 8) transfer to Python

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
|Node.js: The Comprehensive Guide (Springer)   |Reference (not in active plan)          |
|Web Development with Node and Express (Brown) |Reference (not in active plan)          |
|Eloquent JavaScript (Haverbeke)               |Reference (not in active plan)          |
|100 Go Mistakes (Harsanyi)                    |Track 8: Software Architecture          |
|Learning Go, 1st ed (Bodner)                  |Track 8: Software Architecture          |
|Red Teaming AI (Dursey)                       |Track 10: AI/ML Security                |

-----

## Books to Purchase

|Book                                      |Cost |Track                                    |
|------------------------------------------|-----|-----------------------------------------|
|Let's Go (Edwards)                        |~$40 |Track 8: Software Architecture           |
|Let's Go Further (Edwards)                |~$40 |Track 8: Software Architecture           |
|Python Testing with pytest, 2nd ed (Okken)|~$40 |Track 9: Python Core + TDD              |
|AI Engineering (Huyen)                    |~$50 |Track 10: AI/ML Security                |

**Total: ~$170**

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
|Go Time          |Go ecosystem      |

### Newsletters

|Newsletter            |Focus                |
|----------------------|---------------------|
|TLDR Sec              |Security news digest |
|The Pragmatic Engineer|Engineering career   |
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

-----

## Leadership Reading List (Bedtime Reading)

**28 leadership/business books** - organized for bedtime reading throughout your 44-week journey.

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
|Architecture|9-20|Legacy, Captains Class, Leaders Eat Last, A Philosophy of Software Design|
|AI/ML|21-28|Start With Why, Paradigma Guardiola, Creativity Inc|
|Python + Capstone|30-43|Elon Musk, Measure What Matters, Revolución Scaloni|

**Reading Pace:** 20-30 pages/night = 1 book every 2-4 weeks = 15-20 books over 44 weeks

**Full details, checklists, and reading order:** See [leadership-reading-list.md](leadership-reading-list.md)

-----
