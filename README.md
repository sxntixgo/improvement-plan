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

|Track|Name                  |Weeks|Duration|File                         |
|-----|----------------------|-----|--------|-----------------------------|
|1    |Reading Skills        |1    |1 week  |<track-01-reading-skills.md> |
|2    |Note-Taking (Obsidian)|2-3  |2 weeks |<track-02-note-taking.md>    |
|3    |Claude Code           |4    |1 week  |<track-03-claude-code.md>    |
|4    |Python Core           |5-14 |10 weeks|<track-04-python-core.md>    |
|5    |AI/ML Security        |15-22|8 weeks |<track-05-ai-ml-security.md> |
|6    |JavaScript/Node.js    |23-42|20 weeks|<track-06-javascript.md>     |
|7    |Python Advanced       |43-50|8 weeks |<track-07-python-advanced.md>|
|8    |Go/Golang             |51-62|12 weeks|<track-08-golang.md>         |

**Total Duration:** 62 weeks (~15 months)

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
                    Python Core (TDD, pytest, architecture)
                              ↓
                    AI/ML Security ← requires Python testing skills
                              ↓
                    JavaScript/Node.js
                              ↓
                    Python Advanced (AST, async) ← nice-to-have, not blocking
                              ↓
                    Go/Golang
```

**Why Python is split:**

- **Python Core** (Track 4): TDD + pytest + architecture — essential for reviewing ML code
- **Python Advanced** (Track 7): AST + async — useful but not required for AI red teaming

-----

## Books Already Owned

|Book                                          |Track         |
|----------------------------------------------|--------------|
|How to Read a Book (Adler & Van Doren)        |Reading Skills|
|Speed Reading (Knight)                        |Reading Skills|
|How to Take Smart Notes (Ahrens)              |Note-Taking   |
|Building a Second Brain (Forte)               |Note-Taking   |
|Developer's Playbook for LLM Security (Wilson)|AI/ML         |
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
