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
|12   |JavaScript/Node.js    |47-66 |20 weeks|<track-12-javascript.md>        |

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
                    JavaScript/Node.js ← Web security context
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
- JavaScript is valuable but less urgent for AI red teaming role

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

## Source Conversations

|Topic                     |Link                                                       |
|--------------------------|-----------------------------------------------------------|
|Note-Taking / Obsidian    |https://claude.ai/chat/449c1db6-8e29-42dc-96f4-2cdeaa3422c1|
|JavaScript Mastery Plan   |https://claude.ai/chat/1d05e1a4-d947-481a-b05c-d6ac49ff9fad|
|Python Improvement Plan   |https://claude.ai/chat/7fab6ef6-5e5c-419a-9386-2176b62f1cbb|
|AI Red Teaming/ML Security|https://claude.ai/chat/e6025024-ecd2-4088-9a0a-728267736d8b|
|Go/Golang Learning        |https://claude.ai/chat/087a2c91-7cb9-403e-a749-163dae635363|
|Consolidated Plan v2      |https://claude.ai/chat/7a1879d4-720d-4189-841f-27a2ec7cc70a|

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
