# Consolidated Learning Plan - Overview

**Security Engineer → AI Red Teaming Transition**
**Available Time: 18 hours/week**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

**Mode: Sequential (one track at a time)**
**Updated: January 8, 2026**

-----

## Priority Order & Timeline

|Track|Name                  |Weeks |Duration|File                            |
|-----|----------------------|------|--------|--------------------------------|
|1    |Reading Skills        |1     |1 week  |<track-01-reading-skills.md>    |
|2    |Note-Taking (Obsidian)|2-3   |2 weeks |<track-02-note-taking.md>       |
|3    |Claude Code           |4     |1 week  |<track-03-claude-code.md>       |
|4    |Git Mastery           |5     |1 week  |<track-04-git-mastery.md>       |
|5    |Go Crash Course       |6     |1 week  |<track-05-go-crash-course.md>   |
|6    |Docker Essentials     |7     |1 week  |<track-06-docker-essentials.md> |
|7    |LLM Security Primer   |8     |1 week  |<track-07-llm-security-primer.md>|
|8    |Python Core           |9-18  |10 weeks|<track-08-python-core.md>       |
|9    |AI/ML Security        |19-26 |8 weeks |<track-09-ai-ml-security.md>    |
|10   |Python Advanced       |27-34 |8 weeks |<track-10-python-advanced.md>   |
|11   |Go Deep Dive          |35-46 |12 weeks|<track-11-golang.md>            |
|12   |JavaScript/TypeScript |47-66 |20 weeks|<track-12-javascript.md>        |

**Total Duration:** 66 weeks (~15 months)

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
Reading → Note-Taking → Claude Code
                              ↓
                    Git Mastery ← Foundation for all development
                              ↓
                    Go Crash Course ← For immediate work needs
                              ↓
                    Docker Essentials ← Infrastructure for all projects
                              ↓
                    LLM Security Primer (Wilson book) ← Security context
                              ↓
                    Python Core (TDD, pytest, architecture)
                              ↓
                    AI/ML Security (HTB Academy + hands-on) ← requires Python
                              ↓
                    Python Advanced (AST, async) ← asyncio for concurrent attacks
                              ↓
                    Go Deep Dive ← Build on crash course (only 28 weeks later)
                              ↓
                    JavaScript/TypeScript ← Web security context
```

**Why Git and Docker early:**
- **Git** is foundational for ALL development work (code management, collaboration)
- **Docker** enables containerized dev environments, ML deployment, security labs
- Both learned early = available for all future tracks (Python, ML, security testing)
- Concentrated 18-hour weeks for better retention vs scattered learning

**Why Docker comes after Go (Week 7):**
- Go needed immediately for work (Week 6)
- Docker learned once = used throughout Python (Weeks 9-18), ML (Weeks 19-26), and all projects
- Week 7 is perfect timing: after immediate work tools, before Python projects begin

**Why Python is split:**
- **Python Core** (Track 8): TDD + pytest + architecture — essential for reviewing ML code
- **Python Advanced** (Track 10): AST + async — asyncio immediately useful for concurrent attack tools

**Why Go comes before JavaScript:**
- You use Go daily at work starting Week 6
- Go Deep Dive (Week 35) reinforces crash course while skills are still fresh (29-week gap vs 41-week gap)
- JavaScript/TypeScript is valuable but less urgent for AI red teaming role
- TypeScript used in modern LLM tools (LangChain, Vercel AI SDK)

-----

## Books Already Owned

|Book                                          |Track         |
|----------------------------------------------|--------------|
|How to Read a Book (Adler & Van Doren)        |Reading Skills|
|Speed Reading (Knight)                        |Reading Skills|
|How to Take Smart Notes (Ahrens)              |Note-Taking   |
|Building a Second Brain (Forte)               |Note-Taking   |
|Pro Git (Chacon & Straub)                     |Git Mastery   |
|Developer's Playbook for LLM Security (Wilson)|AI/ML         |
|Test-Driven Development with Python (Percival)|Python Core   |
|Node.js: The Comprehensive Guide (Springer)   |JavaScript    |
|Web Development with Node and Express (Brown) |JavaScript    |
|You Don't Know JS 1st edition (Simpson)       |JavaScript    |
|Eloquent JavaScript (Haverbeke)               |JavaScript    |
|Black Hat Go (Steele et al.)                  |Go            |

-----

## Books to Purchase

|Book                                      |Cost|Track          |
|------------------------------------------|----|---------------|
|Python Testing with pytest, 2nd ed (Okken)|~$40|Python Core    |
|AI Engineering (Huyen)                    |~$50|AI/ML          |
|Using Asyncio in Python (Fowler)          |~$50|Python Advanced|
|Learning Go, 2nd ed (Bodner)              |~$50|Go             |
|100 Go Mistakes (Harsanyi)                |~$40|Go             |
|Let's Go (Alex Edwards)                   |~$40|Go             |

**Total: ~$270**

**Optional:**

|Book                            |Cost|When                                |
|--------------------------------|----|------------------------------------|
|How AI Works (Kneusel)          |~$30|Read before Track 5 (downtime)      |
|Python Tools for Data Scientists|~$30|Only if you need NumPy/Pandas for ML|

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

|Book                             |Why                                |When          |
|---------------------------------|-----------------------------------|--------------|
|How AI Works (Kneusel)           |Conceptual AI primer, no heavy math|Before Track 5|
|AI Snake Oil (Narayanan & Kapoor)|Critical thinking about AI claims  |Anytime       |

-----

## Leadership Reading List (Bedtime Reading)

**27 leadership/business books you already own** - organized for bedtime reading throughout your 66-week journey.

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
|Foundation|1-10|Score Takes Care of Itself, Atomic Habits, High Output Management|
|Discipline|11-25|Legacy, Captains Class, Leaders Eat Last, Start With Why|
|Mastery|26-40|Bielsa, Paradigma Guardiola, Creativity Inc, Elon Musk|
|Finishing|41-66|Revolución Scaloni, Measure What Matters, The Snowball|

**Reading Pace:** 20-30 pages/night = 1 book every 2-4 weeks = 20-25 books over 66 weeks

**Your Strength:** 7 sports leadership books

**Full details, checklists, and reading order:** See [leadership-reading-list.md](leadership-reading-list.md)

-----
