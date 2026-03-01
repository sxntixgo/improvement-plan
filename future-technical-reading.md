# Future Technical Reading

**Purpose:** Excellent books for your architect + AI red teamer role that don't fit the 44-week plan. Read these after plan completion or when a specific need arises.

**Why these were deferred:** The 44-week plan already has heavy reading. Adding more books would recreate the overload problem. These are "right profile, wrong time" — each one becomes more valuable after you've completed the relevant track.

-----

## Tier 1: Read First After Plan Completion

These directly extend what you learned. High impact for your role.

| Book | Author | Pages | ~Cost | Extends |
|------|--------|-------|-------|---------|
| Adversarial AI Attacks, Mitigations, and Defense Strategies | John Sotiropoulos | ~586 | ~$50 | Track 10 (AI/ML Security) |
| Build a Large Language Model From Scratch | Sebastian Raschka | ~368 | ~$45 | Track 10 (AI/ML Security) |
| Learning Domain-Driven Design | Vlad Khononov | ~290 | ~$50 | Track 8 (Architecture) |
| Designing Data-Intensive Applications | Martin Kleppmann | ~550 | ~$45 | Track 8 (Architecture) |
| Threat Modeling: Designing for Security | Adam Shostack | ~300 | ~$40 | Track 10 (AI/ML Security) |

### Adversarial AI Attacks, Mitigations, and Defense Strategies (Sotiropoulos)

**What it adds:** Comprehensive offense + defense + threat modeling for AI systems. Covers LLMs, computer vision, NLP, and supply chain attacks. Author is **OWASP LLM Top 10 co-lead** — this is the practitioner's manual for AI red teaming.

**When to read:** First after Track 10. This is the single most relevant post-plan book for your AI red teamer role. It deepens everything you learned in Track 10 with a structured offensive/defensive methodology from someone who literally defines the industry standards.

**Why it was deferred:** 586 pages on top of Track 10's already heavy AI security content. Your plan covers the same ground through Huyen + Dursey + hands-on labs. Sotiropoulos adds the OWASP-aligned methodology and broader attack surface coverage.

### Build a Large Language Model From Scratch (Raschka)

**What it adds:** "Know your target" — understand LLM internals from tokenization to attention mechanisms to fine-tuning. Better red teaming comes from understanding how models actually work under the hood. Raschka is a respected ML researcher and the book is hands-on with code.

**When to read:** After Track 10. When you want to move from "test the API surface" to "understand why these attacks work at the model level." This foundation makes your AI red team assessments significantly deeper.

**Why it was deferred:** 368 pages of model internals. Track 10 focuses on attacking AI systems from the outside (which is the immediate job need). Model internals become important when you want to understand *why* attacks succeed, not just *that* they succeed.

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
| Security Engineering, 3rd ed | Ross Anderson | ~1000+ | **FREE** | Reference — read chapters as security questions arise |
| Software Architecture: The Hard Parts | Richards, Ford, et al. | ~400 | ~$50 | When you face distributed system trade-offs at work |
| Building Microservices | Sam Newman | ~600 | ~$50 | When microservices become relevant at your job |
| Concurrency in Go | Katherine Cox-Buday | ~250 | ~$40 | When Go concurrency needs deepening beyond Track 8/11 |
| Hacking APIs | Corey Ball | ~368 | ~$35 | When you need API pentesting fundamentals for AI system testing |
| The Alignment Problem | Brian Christian | ~350 | ~$18 | When you want broader AI safety context beyond red teaming |

### Security Engineering, 3rd ed (Ross Anderson)

**What it adds:** The foundational security architecture reference — covers threat modeling, access control, cryptography, system design, economics of security, and much more. Written by one of the most respected security researchers in the world. The 3rd edition is available **FREE online** from Cambridge University Press.

**When to read:** Use as a reference book. Don't read cover-to-cover (1000+ pages). Instead, read specific chapters when security architecture questions arise at work — e.g., the threat modeling chapter before an assessment, the cryptography chapter when reviewing AI model encryption.

### Software Architecture: The Hard Parts (Richards, Ford, Dehghani, Sadalage)

**What it adds:** Sequel to Fundamentals of Software Architecture (already in your plan). Focuses on trade-off analysis for breaking apart monoliths, data decomposition, distributed workflows. Advanced distributed architecture patterns.

**When to read:** When you're directing Claude Code to build or refactor distributed systems at work. The fundamentals book (in your plan) covers enough for the 44 weeks.

### Building Microservices (Sam Newman)

**What it adds:** Comprehensive guide to microservice architecture — service decomposition, communication patterns, testing, deployment, security. Richards & Ford covers microservices as one style among many; Newman goes deep on just microservices.

**When to read:** Only if your work involves microservice architectures. Many teams don't need microservices, and Newman himself warns against premature adoption.

### Concurrency in Go (Cox-Buday)

**What it adds:** Deep dive into Go concurrency — goroutines, channels, select, context, patterns (fan-out/fan-in, pipelines, rate limiting). Track 8 Week 12 and Track 11 cover concurrency, but Cox-Buday goes deeper.

**When to read:** When you're directing Claude Code to build concurrent Go tools and need to review complex concurrency patterns. Track 8 + Black Hat Go may be sufficient.

### Hacking APIs (Corey Ball)

**What it adds:** API pentesting methodology — reconnaissance, authentication attacks, authorization flaws, injection, rate limiting bypass. Most AI systems expose REST/GraphQL APIs, so API security is directly relevant to AI red teaming.

**When to read:** Only if your API pentesting fundamentals need strengthening. Skip if you're already comfortable with API security from your security engineering background.

### The Alignment Problem (Brian Christian)

**What it adds:** Broader AI safety context — how AI systems learn values, fairness in ML, reward hacking, interpretability. Not a security book, but gives context for why AI red teaming matters beyond just prompt injection.

**When to read:** When you want to articulate the "why" of AI red teaming to stakeholders, or when you're curious about the broader AI safety landscape.

-----

## Tier 3: Software Engineering Craft

Broader software engineering books that deepen your architect skills. Read after Tier 1 and Tier 2, or when a specific need arises at work. Two are free.

| Book | Author | Pages | ~Cost | Focus |
|------|--------|-------|-------|-------|
| Machine Learning Design Patterns | Lakshmanan, Robinson, Munn (Google) | ~400 | ~$35 | How ML systems are architecturally designed — "know your target" |
| Building Secure and Reliable Systems | Adkins et al. (Google) | ~555 | **FREE** | Security + reliability intersection — your exact career overlap |
| Software Engineering at Google | Winters, Manshreck, Wright | ~602 | **FREE** | Engineering at scale — code review, testing philosophy, dependency management |
| API Design Patterns | JJ Geewax (Google) | ~480 | ~$35 | REST/gRPC design vocabulary for directing Claude Code |
| Unit Testing Principles, Practices, and Patterns | Vladimir Khorikov | ~304 | ~$40 | What makes tests *good* — judging AI-generated test quality |
| Team Topologies | Matthew Skelton, Manuel Pais | ~240 | ~$30 | Org design determines system architecture (Conway's Law applied deliberately) |
| Accelerate | Forsgren, Humble, Kim | ~269 | ~$30 | Research-backed evidence for which engineering practices actually work (DORA metrics) |
| Refactoring, 2nd ed | Martin Fowler | ~448 | ~$45 | 70+ named refactoring patterns — the vocabulary of code transformation |
| Understanding Distributed Systems | Roberto Vitillo | ~344 | ~$40 | Practical companion to Kleppmann's DDIA — faster path to distributed systems knowledge |

### Machine Learning Design Patterns (Lakshmanan, Robinson, Munn)

**What it adds:** 30 design patterns for ML systems — data representation, model training, serving, reproducibility, fairness. Written by three Google Cloud ML engineers. Understanding how ML systems are *designed* is prerequisite knowledge for understanding how they can *fail* or be *attacked*.

**When to read:** After Track 10. This is the architectural complement to your AI security knowledge. You'll attack ML systems more effectively when you understand their design patterns.

### Building Secure and Reliable Systems (Adkins et al.)

**What it adds:** The intersection of security engineering and reliability engineering, from Google's security and SRE teams. Covers secure-by-default design, least privilege in infrastructure, recovery planning. **FREE online** from Google.

**When to read:** After Track 8 or 10. This validates and extends your security instincts into systems design. Pairs well with Shostack's Threat Modeling (Tier 1).

### Software Engineering at Google (Winters, Manshreck, Wright)

**What it adds:** How Google manages a 250M-line codebase — code review culture, testing philosophy, dependency management, large-scale changes. When you direct an AI to write code, the chapters on evaluating and accepting code are directly applicable. **FREE online** at abseil.io.

**When to read:** When you want the engineering-culture-at-scale perspective. The code review and testing strategy chapters are immediately useful for your Claude Code workflow.

### API Design Patterns (Geewax)

**What it adds:** Naming conventions, resource design, pagination, filtering, authentication, long-running operations. Covers REST, gRPC, and general patterns. As an architect directing code generation, having principled API design vocabulary lets you specify API contracts precisely.

**When to read:** When you're directing Claude Code to build APIs and want to give more precise specifications.

### Unit Testing Principles, Practices, and Patterns (Khorikov)

**What it adds:** The four pillars of a good unit test, when mocks help vs. hurt, integration testing strategy, testing anti-patterns. 4.57 Goodreads rating — the highest-rated testing book published in recent years. Complements Percival (TDD mechanics) and Okken (pytest) by adding the "philosophy of what makes tests valuable" layer.

**When to read:** After Track 9 Phase 1A (TDD with Percival). When you need to evaluate whether Claude Code's tests are *good*, not just passing.

### Team Topologies (Skelton, Pais)

**What it adds:** Four fundamental team types and three interaction modes. Conway's Law applied deliberately — your team structure determines your system architecture. The language of "stream-aligned teams," "platform teams," and "cognitive load" has become industry standard.

**When to read:** When you start thinking about how team boundaries affect the systems you're designing or attacking.

### Accelerate (Forsgren, Humble, Kim)

**What it adds:** Research-backed evidence for which engineering practices improve outcomes. Introduces the DORA metrics (deployment frequency, lead time, change failure rate, MTTR) that are now industry standard. Every architect should know this framework.

**When to read:** When you want the empirical justification for modern software delivery practices.

### Refactoring, 2nd ed (Fowler)

**What it adds:** 70+ named refactoring patterns with motivation, mechanics, and examples. The vocabulary of code transformation — "Extract Method," "Replace Conditional with Polymorphism," etc. Ousterhout (in your plan) covers the *why* of design; Fowler covers the *how* of transforming code to get there.

**When to read:** Use as a reference book. When you need to tell Claude Code "apply Extract Class here," this is where that vocabulary comes from.

### Understanding Distributed Systems (Vitillo)

**What it adds:** A more practical, concise companion to Kleppmann's DDIA. Covers network stack, consistency models, scalability, reliability, and resiliency. Where DDIA goes deep into theory, Vitillo focuses on actionable knowledge. Read before or alongside Kleppmann.

**When to read:** When you want distributed systems knowledge without committing to Kleppmann's 550 dense pages first.

-----

## Watch List: Forthcoming Books

| Book | Author | Pages | Expected | Why Watch |
|------|--------|-------|----------|-----------|
| Practical AI Security | Daniel Farlow | ~392 | April 2026 | 30+ hands-on Python demos for AI security testing. O'Reilly. Worth pre-ordering when available. |

**Note:** Your Kindle edition of Red Teaming AI (Dursey) will get a No Starch Press print edition in July 2026 — no need to repurchase unless you want the physical book.

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
| Head First Design Patterns (Eric Freeman) | Java/OOP-centric — teaches Gang of Four patterns via inheritance and classes. Go favors composition and interfaces, not traditional OOP. Ousterhout covers design principles, Richards & Ford covers architecture patterns, and Let's Go/Let's Go Further teach idiomatic Go patterns. As an architect directing Claude Code, you need to know *when* to apply patterns (already covered), not how to implement them by hand in Java. |
| Domain-Driven Design (Eric Evans, "Blue Book") | 500+ pages, dense, academic. Khononov (Tier 1) covers the same ground in 290 pages with modern context. Read Evans only if you become a DDD specialist. |
| StatQuest Illustrated Guides (Starmer) — ML, Neural Networks, Statistics | Beginner-level illustrated introductions. Your plan already covers the same ground deeper via Fast.ai (Week 21), Hugging Face NLP (Week 22), and AI Engineering Ch 2. Raschka (Tier 1) goes far deeper on model internals. Watch the free YouTube videos instead if you need a concept refresher. |
| Software Engineering for Data Scientists (Nelson) | Aimed at junior data scientists who've never used Git or written tests. You're a Security Engineer — this is well below your baseline. Your plan covers SE fundamentals deeper in your actual languages (Go, Python). |

-----

## Cost Summary

| Tier | Books | Total Cost |
|------|-------|-----------|
| Tier 1 | 5 books | ~$230 |
| Tier 2 | 6 books | ~$193 (includes 1 FREE) |
| Tier 3 | 9 books | ~$255 (includes 2 FREE) |
| Watch List | 1 book | TBD (forthcoming) |
| **All** | **21 books** | **~$678** |

No urgency to buy any of these. Purchase when you're ready to read them — after Week 44. Three books are free online (Anderson, Google SRE, SWE at Google).

-----

## How This Relates to Your Plan

```
44-Week Plan (active learning)
├── Track 8: Architecture via Go     → Tier 1: Khononov, Kleppmann extend this
│                                      Tier 3: API Patterns, Refactoring, Distributed Systems, Team Topologies
├── Track 10: AI/ML Security         → Tier 1: Sotiropoulos, Raschka, Shostack extend this
│                                      Tier 3: ML Design Patterns, Secure & Reliable Systems
├── Track 9: Python Core             → Tier 3: Unit Testing Principles extends this
│                                      Dropped: Black Hat Python, Fluent Python, Asyncio
└── Track 11: Go Security + Capstone → Tier 2: Cox-Buday, Hacking APIs extend this

Dropped Tracks (Track 12 & 13)
├── Python Advanced: 3 books — read only if role shifts to writing Python
└── JS/TS: 2 books + 4 owned as reference — read only if role shifts to web/frontend

Leadership Reading List (bedtime reading, parallel to plan)
└── 27 books, all owned, separate from technical reading

Future Technical Reading (THIS LIST — after plan completion)
├── Tier 1: 5 books, read first (AI security + architecture deep dives)
├── Tier 2: 6 books, read when needed (includes 1 FREE reference)
├── Tier 3: 9 books, software engineering craft (includes 2 FREE)
└── Watch List: 1 forthcoming book (Practical AI Security, April 2026)
```
