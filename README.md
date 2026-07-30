# Consolidated Learning Plan - Overview

**Security Engineer → AI Red Teaming Transition**
**Available Time: 18 hours/week**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

**Mode: Sequential (one track at a time)**
**Updated: March 12, 2026**

-----

## What This Plan Builds On

This plan is designed for an **architect who directs Claude Code**, not a hands-on coder. Two facts shape everything:

- **You don't write code — Claude Code does.** You architect systems, review output, and give Claude Code precise directions. Every track focuses on understanding patterns and making architectural decisions, not typing syntax. Track 3 is the most important foundation week because Claude Code is your primary tool.
- **Go is your work language, but Claude Code writes it.** You need to understand Go architecture deeply enough to review what Claude Code produces, catch design mistakes, and give effective direction. You don't need to memorize syntax — you need to think in systems.

The plan prioritizes **software architecture first, then AI/ML security** — the two things that matter for your role. Python and JavaScript tracks come later to round out your skills.

-----

## Priority Order & Timeline

### Part I: Foundation (Weeks 1-8) — 8 weeks

Core skills and tooling that every other track depends on.

|Track|Name                                      |Weeks |Duration |File                                       |
|-----|------------------------------------------|------|---------|-------------------------------------------|
|1    |Reading Skills                            |1     |1 week   |[track-01-reading-skills.md](track-01-reading-skills.md)|
|2    |Note-Taking (Obsidian)                    |2-3   |2 weeks  |[track-02-note-taking.md](track-02-note-taking.md)|
|3    |Claude Code Advanced                      |4     |1 week   |[track-03-claude-code.md](track-03-claude-code.md)|
|4    |Git Mastery                               |5     |1 week   |[track-04-git-mastery.md](track-04-git-mastery.md)|
|5    |Go Crash Course                           |6     |1 week   |[track-05-go-crash-course.md](track-05-go-crash-course.md)|
|6    |Docker Essentials                         |7     |1 week   |[track-06-docker-essentials.md](track-06-docker-essentials.md)|
|7    |LLM Security Primer                       |8     |1 week   |[track-07-llm-security-primer.md](track-07-llm-security-primer.md)|

### Part II: Architecture (Weeks 9-20) — 12 weeks

Deep software architecture knowledge. Learn to think in systems so you can direct Claude Code effectively and review its output.

|Track|Name                                      |Weeks |Duration |File                                       |
|-----|------------------------------------------|------|---------|-------------------------------------------|
|8    |Software Architecture (via Go)            |9-20  |12 weeks |[track-08-go-foundations-architecture.md](track-08-go-foundations-architecture.md)|

### Part III: AI/ML Security (Weeks 21-28) — 8 weeks

Your career goal. Prompt injection, RAG poisoning, model attacks, red team methodology.

|Track|Name                                      |Weeks |Duration |File                                       |
|-----|------------------------------------------|------|---------|-------------------------------------------|
|10   |AI/ML Security                            |21-28 |8 weeks  |[track-10-ai-ml-security.md](track-10-ai-ml-security.md)|

### Break (Week 29) — 1 week

### Part IV: Python + Go Security (Weeks 30-43) — 14 weeks

Deepen Python understanding post-AI/ML, then combine Go + AI security into a unique capstone.

|Track|Name                                      |Weeks |Duration |File                                       |
|-----|------------------------------------------|------|---------|-------------------------------------------|
|9    |Python Core + TDD                         |30-37 |8 weeks  |[track-09-python-core.md](track-09-python-core.md)|
|11   |Go Security Tools + AI Capstone           |38-43 |6 weeks  |[track-11-go-security.md](track-11-go-security.md)|

**Total plan: 43 learning weeks + 1 break = 44 weeks (~10 months)**

The plan ends at Track 11. There is no optional phase.

**Previously dropped:** Python Advanced (AST, async) and JavaScript/TypeScript were once staged as an optional Part V. They were cut because neither is required for the AI red teaming goal — the architect reviews Python rather than writing advanced Python, and JS/TS is not on the critical path. See [future-technical-reading.md](future-technical-reading.md) for the rationale and for what to read instead if your needs change. The archived track files live in [archive/](archive/).

-----

### Why This Order

**Foundation → Architecture → AI/ML → Python → Go Security**

1. **Foundation first (Tracks 1-7):** Reading, note-taking, tooling, and security context. Everything else builds on these.
2. **Architecture (Track 8):** You need to think in systems to direct Claude Code effectively. Clean architecture, DDD, and testing patterns are the language of good engineering direction.
3. **AI/ML immediately after (Track 10):** This is your career goal. You don't need Python syntax to understand RAG architecture, prompt injection, or model vulnerabilities — Claude Code writes the code while you focus on concepts and attack surfaces.
4. **Python after AI/ML (Track 9):** Deepens your understanding of the tools you've already used. Now you understand why pytest works the way it does, how Python architecture differs from Go, and can give Claude Code more precise Python direction.
5. **Go Security Tools (Track 11):** Combines everything — Go architecture knowledge + AI security concepts + security tool patterns. The capstone produces an AI Red Team CLI tool in Go. This is where the plan ends.

-----

## The Architect Mindset

Every track in this plan follows the same pattern:

1. **Understand the concept** — Read, study, watch. Know WHY a pattern exists.
2. **Direct Claude Code to build it** — Give precise architectural instructions. Use CLAUDE.md files.
3. **Review the output** — Check architecture, not syntax. Does the structure follow clean architecture? Are dependencies pointing inward? Is the testing strategy right?
4. **Iterate** — Give Claude Code better direction based on what you see.

This is fundamentally different from "learn to code." You're learning to **think like a senior architect** who happens to use AI as their implementation tool.

-----

## Track Logic

```
Part I: Foundation
  Reading → Note-Taking → Claude Code Advanced (YOUR PRIMARY TOOL)
                                ↓
                      Git Mastery ← Foundation for all development
                                ↓
                      Go Crash Course ← Understand your work language
                                ↓
                      Docker Essentials ← Infrastructure for all projects
                                ↓
                      LLM Security Primer (Wilson book) ← Security context

Part II: Architecture
                                ↓
                      Software Architecture via Go ← Think in systems

Part III: AI/ML Security
                                ↓
                      AI/ML Security ← YOUR CAREER GOAL

Part IV: Python + Go Security
                                ↓
                      Python Core + TDD ← Deepen understanding post-AI/ML
                                ↓
                      Go Security Tools + AI Capstone ← Combine everything
                                ↓
                             DONE (Week 43)
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

## Weekly Habits

|Habit      |When                     |Output                                   |
|-----------|-------------------------|-----------------------------------------|
|Blog update|End of each week         |Progress, learnings, reflections         |
|Book review|After finishing each book|Published review on blog                 |
|Code push  |As you build             |Public GitHub repos for relevant projects|

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
|Python Testing with pytest (Okken)            |Track 9: Python Core + TDD              |
|Architecture Patterns with Python (Percival & Gregory)|Track 9: Python Core + TDD       |
|100 Go Mistakes (Harsanyi)                    |Track 8 + 11: Architecture + Go Security|
|Learning Go (Bodner)                          |Track 8: Software Architecture          |
|Let's Go (Edwards)                            |Track 8: Software Architecture          |
|Let's Go Further (Edwards)                    |Track 8: Software Architecture          |
|A Philosophy of Software Design (Ousterhout)  |Track 8: Software Architecture          |
|Fundamentals of Software Architecture (Richards & Ford)|Track 8: Software Architecture |
|AI Engineering (Huyen)                        |Track 10: AI/ML Security                |
|Red Teaming AI (Dursey)                       |Track 10: AI/ML Security                |
|Black Hat Go (Steele et al.)                  |Track 11: Go Security Tools             |

**Owned but not used by this plan** (kept as reference if your needs change — see [future-technical-reading.md](future-technical-reading.md)):

|Book                                          |Note                                    |
|----------------------------------------------|----------------------------------------|
|Eloquent JavaScript (Haverbeke)               |JS/TS not on the critical path          |
|Web Development with Node and Express (Brown) |JS/TS not on the critical path          |
|You Don't Know JS (Simpson)                   |JS/TS not on the critical path          |
|Node.js: The Comprehensive Guide (Springer)   |JS/TS not on the critical path          |
|JavaScript and jQuery (Duckett)               |JS/TS not on the critical path          |

-----

## Remaining Costs

**All books in this plan are owned. No book purchases remain.**

The only outstanding cost is one subscription:

|Item                     |Cost         |Track                   |Needed By|
|-------------------------|-------------|------------------------|---------|
|HTB Academy AI Red Teamer|~$20/mo × 2  |Track 10: AI/ML Security|Week 23  |

**Total remaining: ~$40**

Everything else in the plan runs on free resources — Go by Example, Effective Go, Three Dots Labs, martinfowler.com, C4 Model, Architecture Katas, Garak, OWASP LLM Top 10, HackAPrompt, and the Python books (Percival and Cosmic Python are free online).

-----

## Chapter Selection Summary

Every book has explicit READ/SKIP chapter guidance in its track file. Here's the overview:

|Book|Track|Chapters Read|
|----|-----|-------------|
|Speed Reading (Knight)|1|9 of 15|
|How to Read a Book (Adler)|1|14 of 21|
|How to Take Smart Notes (Ahrens)|2|9 of 14|
|Building a Second Brain (Forte)|2|7 of 10|
|LLM Security (Wilson)|7|8 of 12|
|Philosophy of Software Design (Ousterhout)|8|12 of 18|
|Fundamentals of Software Architecture (Richards & Ford)|8|~12 of 24|
|TDD with Python (Percival)|9|10 of 27|
|pytest (Okken)|9|8 of 12|
|Architecture Patterns with Python (Percival & Gregory)|9|7 of 13|
|AI Engineering (Huyen)|10|6 of 10|
|Red Teaming AI (Dursey)|10|10 of 11|
|Black Hat Go (Steele et al.)|11|6 of 14|

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

**28 leadership/business books** - organized for bedtime reading throughout your journey.

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
|Part I: Foundation|1-8|Score Takes Care of Itself, Atomic Habits, High Output Management|
|Part II: Architecture|9-20|Legacy, Captains Class, Leaders Eat Last, Start With Why|
|Part III: AI/ML|21-28|Start With Why, Paradigma Guardiola, Creativity Inc|
|Part IV: Python + Capstone|30-43|Elon Musk, Measure What Matters, Revolución Scaloni|

**Reading Pace:** 20-30 pages/night = 1 book every 2-4 weeks

**Full details, checklists, and reading order:** See [leadership-reading-list.md](leadership-reading-list.md)

**After plan completion:** See [future-technical-reading.md](future-technical-reading.md) for 7 technical books that extend this plan (Khononov DDD, Kleppmann DDIA, Shostack Threat Modeling, and more)

-----
