# Future Technical Reading

**Purpose:** Excellent books for your architect + AI red teamer role that don't fit the 44-week plan. Read these after plan completion or when a specific need arises.

**Why these were deferred:** The 44-week plan already has heavy reading. Adding more books would recreate the overload problem. These are "right profile, wrong time" — each one becomes more valuable after you've completed the relevant track.

-----

## Tier 1: Read First After Plan Completion

These directly extend what you learned. High impact for your role.

| Book | Author | Pages | ~Cost | Extends |
|------|--------|-------|-------|---------|
| Learning Domain-Driven Design | Vlad Khononov | ~290 | ~$50 | Track 8 (Architecture) |
| Designing Data-Intensive Applications | Martin Kleppmann | ~550 | ~$45 | Track 8 (Architecture) |
| Threat Modeling: Designing for Security | Adam Shostack | ~300 | ~$40 | Track 10 (AI/ML Security) |

### Learning Domain-Driven Design (Khononov)

**What it adds:** Strategic DDD — bounded contexts, subdomains, context mapping, EventStorming. Your plan covers tactical DDD (entities, value objects, repos) through Three Dots Labs + Cosmic Python. Khononov adds the architect-level "where to draw boundaries" thinking.

**When to read:** After Track 8. If DDD resonates during Week 14, consider reading this earlier.

**Why it was deferred:** Adding 290 pages to Track 8 Phase 2 would undo the overload fixes. The tactical DDD in the plan is sufficient for directing Claude Code. Strategic DDD becomes important when designing larger systems.

### Designing Data-Intensive Applications (Kleppmann)

**What it adds:** How production data systems actually work — databases, replication, partitioning, batch/stream processing, distributed systems. Widely considered one of the best software architecture books ever written.

**When to read:** After Track 8. This deepens your understanding of the systems you'll eventually attack (databases behind RAG apps, streaming pipelines in ML systems, distributed architectures).

**Why it was deferred:** 550 pages of dense material. Not directly relevant to the AI red teaming goal, but invaluable for understanding production system architecture at a deeper level.

### Threat Modeling: Designing for Security (Shostack)

**What it adds:** Structured methodology for identifying threats in system designs. STRIDE model, attack trees, data flow diagrams. This is how architects think about security before code is written.

**When to read:** After Track 10. Your AI red team assessments (Week 28) would benefit from formal threat modeling methodology, but the plan already has enough content for that week.

**Why it was deferred:** The plan teaches threat identification through practical experience (HTB labs, OWASP, MITRE ATLAS). Shostack adds the formal methodology — valuable for professional engagements but not needed during initial learning.

-----

## Tier 2: Read When a Specific Need Arises

Valuable but situational. Pick these up when you encounter the relevant problem at work.

| Book | Author | Pages | ~Cost | When to Read |
|------|--------|-------|-------|-------------|
| Software Architecture: The Hard Parts | Richards, Ford, et al. | ~400 | ~$50 | When you face distributed system trade-offs at work |
| Building Microservices | Sam Newman | ~600 | ~$50 | When microservices become relevant at your job |
| Concurrency in Go | Katherine Cox-Buday | ~250 | ~$40 | When Go concurrency needs deepening beyond Track 8/11 |
| The Alignment Problem | Brian Christian | ~350 | ~$18 | When you want broader AI safety context beyond red teaming |

### Software Architecture: The Hard Parts (Richards, Ford, Dehghani, Sadalage)

**What it adds:** Sequel to Fundamentals of Software Architecture (already in your plan). Focuses on trade-off analysis for breaking apart monoliths, data decomposition, distributed workflows. Advanced distributed architecture patterns.

**When to read:** When you're directing Claude Code to build or refactor distributed systems at work. The fundamentals book (in your plan) covers enough for the 44 weeks.

### Building Microservices (Sam Newman)

**What it adds:** Comprehensive guide to microservice architecture — service decomposition, communication patterns, testing, deployment, security. Richards & Ford covers microservices as one style among many; Newman goes deep on just microservices.

**When to read:** Only if your work involves microservice architectures. Many teams don't need microservices, and Newman himself warns against premature adoption.

### Concurrency in Go (Cox-Buday)

**What it adds:** Deep dive into Go concurrency — goroutines, channels, select, context, patterns (fan-out/fan-in, pipelines, rate limiting). Track 8 Week 12 and Track 11 cover concurrency, but Cox-Buday goes deeper.

**When to read:** When you're directing Claude Code to build concurrent Go tools and need to review complex concurrency patterns. Track 8 + Black Hat Go may be sufficient.

### The Alignment Problem (Brian Christian)

**What it adds:** Broader AI safety context — how AI systems learn values, fairness in ML, reward hacking, interpretability. Not a security book, but gives context for why AI red teaming matters beyond just prompt injection.

**When to read:** When you want to articulate the "why" of AI red teaming to stakeholders, or when you're curious about the broader AI safety landscape.

-----

## Dropped from Plan (Track 12 & 13)

These books were in the original 65-week plan but dropped when restructuring for the architect role. They're here for reference if your needs change.

### Track 12: Python Advanced (DROPPED)

| Book | ~Cost | Status | When It Would Matter |
|------|-------|--------|---------------------|
| Black Hat Python (Seitz & Arnold) | ~$35 | Not owned | If you decide to write Python security tools yourself instead of using Go |
| Fluent Python (Ramalho) | ~$50 | Not owned | If you need deep Python internals (decorators, metaclasses, data model) for reviewing complex AI codebases |
| Using Asyncio in Python (Fowler) | ~$50 | Not owned | If you need to review or debug async Python in production AI systems |

**Why dropped:** You're building security tools in Go (your work language), not Python. Claude Code handles async Python. You understand concurrency concepts from Go (Track 8). The architect doesn't need to write advanced Python — they need to review it, which Track 9 covers.

### Track 13: JavaScript/TypeScript (DROPPED)

| Book | ~Cost | Status | When It Would Matter |
|------|-------|--------|---------------------|
| Programming TypeScript (Cherny) | ~$40 | Not owned | If your work shifts to web/frontend or TypeScript-based AI tools |
| Zero To Mastery Node.js | ~$40 | Not owned | If you need to understand Node.js backends (some AI apps use them) |

**Why dropped:** Not relevant to AI red teaming goal. You own 4 JS/TS books as reference if you ever need them:
- Eloquent JavaScript (Haverbeke) — already owned
- Web Development with Node and Express (Brown) — already owned
- Node.js: The Comprehensive Guide (Springer) — already owned
- You Don't Know JS, 1st ed (Simpson) — already owned

**Total dropped:** 5 books, ~$215 saved. None of these are needed for the architect + AI red teamer path.

-----

## Not Recommended (Considered and Skipped)

| Book | Why Skip |
|------|----------|
| The Pragmatic Programmer (Hunt & Thomas) | Aimed at working programmers, not architects. Overlaps with Ousterhout + Richards & Ford for your role. |
| Clean Architecture (Uncle Bob) | Ousterhout + Richards & Ford cover this ground better and more modernly. Clean Architecture is more prescriptive and less nuanced. |
| Domain-Driven Design (Eric Evans, "Blue Book") | 500+ pages, dense, academic. Khononov (Tier 1) covers the same ground in 290 pages with modern context. Read Evans only if you become a DDD specialist. |

-----

## Cost Summary

| Tier | Books | Total Cost |
|------|-------|-----------|
| Tier 1 | 3 books | ~$135 |
| Tier 2 | 4 books | ~$158 |
| **All** | **7 books** | **~$293** |

No urgency to buy any of these. Purchase when you're ready to read them — after Week 44.

-----

## How This Relates to Your Plan

```
44-Week Plan (active learning)
├── Track 8: Architecture via Go     → Tier 1: Khononov, Kleppmann extend this
├── Track 10: AI/ML Security         → Tier 1: Shostack extends this
├── Track 9: Python Core             → Dropped books: Black Hat Python, Fluent Python, Asyncio
└── Track 11: Go Security + Capstone → Tier 2: Cox-Buday extends this

Dropped Tracks (Track 12 & 13)
├── Python Advanced: 3 books — read only if role shifts to writing Python
└── JS/TS: 2 books + 3 owned as reference — read only if role shifts to web/frontend

Leadership Reading List (bedtime reading, parallel to plan)
└── 27 books, all owned, separate from technical reading

Future Technical Reading (THIS LIST — after plan completion)
├── Tier 1: 3 books, read first
└── Tier 2: 4 books, read when needed
```
