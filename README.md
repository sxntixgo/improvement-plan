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

-----

## Leadership Reading List (Bedtime Reading)

**Purpose:** Non-technical books for mental break and building discipline/leadership mindset

**Books you already own, organized by learning phase:**

### Phase 1: Foundation (Weeks 1-10)
**Goal:** Build systems, establish standards, create habits

|Book                            |Why Read Now                                  |Priority|
|--------------------------------|----------------------------------------------|--------|
|**The Score Takes Care of Itself** (Walsh)|Building your 66-week system, standards of performance|⭐⭐⭐|
|**Atomic Habits** (Clear)       |Establishing daily learning habits            |⭐⭐⭐|
|**High Output Management** (Grove)|Managing your learning as a high-output system|⭐⭐   |

**Start with:** The Score Takes Care of Itself (perfect for Week 1!)

### Phase 2: Long-Term Discipline (Weeks 11-20)
**Goal:** Stay disciplined through longer tracks (Python Core)

|Book                    |Why Read Now                                    |Priority|
|------------------------|------------------------------------------------|--------|
|**Legacy** (All Blacks) |Long-term excellence, "sweep the sheds" mindset |⭐⭐⭐|
|**Leaders Eat Last** (Sinek)|Service mindset, taking care of yourself       |⭐⭐   |
|**High Performance**    |Sustaining high performance over time           |⭐⭐   |

**Best for this phase:** Legacy (discipline + humility for the long journey)

### Phase 3: Pushing Through (Weeks 21-30)
**Goal:** AI/ML Security + Python Advanced (harder material)

|Book                         |Why Read Now                                |Priority|
|-----------------------------|---------------------------------------------|--------|
|**The Captains Class** (Walker)|Leadership from any position, perseverance |⭐⭐⭐|
|**Start With Why** (Sinek)   |Remember your purpose when it gets hard     |⭐⭐   |
|**Elon Musk**                |Pushing boundaries, learning hard things    |⭐⭐   |

**Best for this phase:** The Captains Class (championship teams = long-term commitment)

### Phase 4: Mastery (Weeks 31-46)
**Goal:** Go Deep Dive (becoming expert)

|Book                                 |Why Read Now                          |Priority|
|-------------------------------------|--------------------------------------|--------|
|**Paradigma Guardiola**              |Mastery, systems thinking (Spanish)   |⭐⭐⭐|
|**Marcelo Bielsa: Los 11 Caminos al Gol**|Tactics, depth, mastery (Spanish)|⭐⭐   |
|**Creativity Inc** (Catmull)         |Building something excellent          |⭐⭐   |

**Best for this phase:** Paradigma Guardiola (systems mastery like your Go mastery)

### Phase 5: Finishing Strong (Weeks 47-66)
**Goal:** JavaScript/TypeScript (final 20 weeks)

|Book                              |Why Read Now                             |Priority|
|----------------------------------|-----------------------------------------|--------|
|**Revolución Scaloni**            |Underdog story, finishing strong         |⭐⭐⭐|
|**Measure What Matters** (Doerr)  |OKRs, measuring progress to completion   |⭐⭐   |
|**The Snowball** (Buffett bio)    |Long-term thinking, compounding knowledge|⭐⭐   |

**Best for this phase:** Revolución Scaloni (Argentina's journey = your journey)

### Anytime Reads (No Specific Phase)

|Book                              |Why                                      |
|----------------------------------|-----------------------------------------|
|**Six Thinking Hats** (de Bono)   |Problem-solving frameworks (short)       |
|**The 21 Irrefutable Laws**       |General leadership principles            |
|**The Southwest Airlines Way**    |Culture, consistency                     |
|**The Firm**                      |Business strategy                        |
|**The Founders Dilemma**          |Startup lessons                          |
|**The Startup Game**              |Entrepreneurship                         |
|**Get Scalable**                  |Scaling systems                          |
|**The Design of Extraordinary Things**|Design thinking                     |

### Save for Later (After 66 Weeks)
|Book                        |Why Wait                                |
|----------------------------|----------------------------------------|
|**This Time Is Different**  |Economics/finance, heavy reading        |

-----

## Recommended Reading Pace

**Typical bedtime reading:** 20-30 pages per night = finish 250-page book in ~2 weeks

**Suggested schedule:**
- **Weeks 1-2:** The Score Takes Care of Itself (~250 pages)
- **Weeks 3-5:** Atomic Habits (~300 pages)
- **Weeks 6-8:** High Output Management (~250 pages)
- **Weeks 9-11:** Legacy (~200 pages)
- **Weeks 12-14:** Leaders Eat Last (~350 pages)
- **Continue pattern through 66 weeks...**

**Note on longer books:**
- **The Snowball** (~900 pages) - Plan 4-6 weeks at bedtime pace
- **This Time Is Different** (~400 pages) - Plan 3-4 weeks

**You own ~25 books = can easily cover 1-2 per month throughout your journey**

-----

## Why This Reading List Works

**Mental Break:**
- No coding/technical content before bed
- Inspires without stressing
- Better sleep vs reading technical docs

**Leadership Development:**
- Build discipline for 66-week journey
- Learn from sports (your interest)
- Develop leadership mindset for senior roles

**Phase Alignment:**
- Books match what you're going through
- "The Score Takes Care of Itself" perfect for Week 1 (building systems)
- "Legacy" perfect for Weeks 11+ (long-term excellence)
- "Revolución Scaloni" perfect for final stretch (underdog finishing strong)

**Spanish Books:**
- Paradigma Guardiola, Revolución Scaloni, Bielsa book
- Great if Spanish is your language
- Sports leadership from your culture

-----
