# Books & Resources Optimization Guide

**Updated:** February 15, 2026
**Status:** Aligned with architect-focused plan (44 weeks)

-----

## TL;DR

**Total budget: ~$245** for 6 remaining books across 44 weeks. The plan prioritizes:
- **Books for understanding architecture** — read to understand, not to type along
- **Free resources first** — most tracks use free online books, courses, and workshops
- **No paid courses or subscriptions needed** — HTB Academy ($20/month x 2) is the only subscription, and it's already budgeted in Track 10

-----

## What You Already Own

|Book                                          |Track                                |
|----------------------------------------------|-------------------------------------|
|How to Read a Book (Adler & Van Doren)        |Track 1: Reading Skills              |
|Speed Reading (Knight)                        |Track 1: Reading Skills              |
|How to Take Smart Notes (Ahrens)              |Track 2: Note-Taking                 |
|Building a Second Brain (Forte)               |Track 2: Note-Taking                 |
|Pro Git (Chacon & Straub)                     |Track 4: Git Mastery                 |
|Developer's Playbook for LLM Security (Wilson)|Track 7: LLM Security Primer         |
|Test-Driven Development with Python (Percival)|Track 9: Python Core + TDD           |
|Black Hat Go (Steele et al.)                  |Track 11: Go Security Tools          |
|Node.js: The Comprehensive Guide (Springer)   |Reference (not in active plan)       |
|Web Development with Node and Express (Brown) |Reference (not in active plan)       |
|Eloquent JavaScript (Haverbeke)               |Reference (not in active plan)       |
|100 Go Mistakes (Harsanyi)                    |Track 8: Software Architecture       |
|Learning Go, 1st ed (Bodner)                  |Track 8: Software Architecture       |
|Red Teaming AI (Dursey)                       |Track 10: AI/ML Security             |

**14 books already owned** covering Tracks 1, 2, 4, 7, 8, 9, 10, and 11.
**3 JS/TS books** set aside as reference — not in the active 44-week plan.

-----

## Books to Purchase

|Book                                      |Cost |Track                                  |When to Buy         |
|------------------------------------------|-----|---------------------------------------|---------------------|
|Let's Go (Edwards)                        |~$40 |Track 8: Software Architecture         |Before Week 9        |
|Let's Go Further (Edwards)                |~$40 |Track 8: Software Architecture         |Before Week 9        |
|A Philosophy of Software Design (Ousterhout)|~$25|Track 8: Software Architecture         |Before Week 13       |
|Fundamentals of Software Architecture (Richards & Ford)|~$50|Track 8: Software Architecture|Before Week 13       |
|Python Testing with pytest, 2nd ed (Okken)|~$40 |Track 9: Python Core + TDD            |Before Week 30       |
|AI Engineering (Huyen)                    |~$50 |Track 10: AI/ML Security              |Before Week 21       |

**Total: ~$245**

-----

## What Was Dropped (and Why)

|Book/Course                    |Original Cost|Why Dropped                                           |
|-------------------------------|-------------|------------------------------------------------------|
|Using Asyncio in Python (Fowler)|~$50        |Track 12 dropped entirely. You understand concurrency from Go.|
|Fluent Python (Ramalho)        |~$50         |Reference book — not needed for architect role; use online docs|
|Black Hat Python               |~$35         |You're building security tools in Go (your work language), not Python|
|Programming TypeScript         |~$40         |Track 13 dropped entirely                             |
|NVIDIA Adversarial ML course   |$90          |HTB Academy covers adversarial techniques with better hands-on labs|
|TestDriven.io subscription     |~$30/month   |Percival book (free online) is sufficient for TDD concepts|
|Real Python subscription       |~$60/year    |Not needed — you direct Claude Code, you don't write Python|
|Zero To Mastery Node.js        |~$40         |Track 13 dropped entirely                             |
|TCM Security Python courses    |Subscription |HTB Academy AI Red Teamer path is more relevant to your goals|

**Total saved: ~$395 in books and courses that don't add value for an architect role**

-----

## Track-by-Track Resource Strategy

### Tracks 1-7: Foundation (Weeks 1-8)
**Books to buy:** $0 — all owned or free online
- Track 1: How to Read a Book + Speed Reading (owned)
- Track 2: Smart Notes + Second Brain (owned)
- Track 3: Claude Code documentation (free)
- Track 4: Pro Git (owned + free online)
- Track 5: Tour of Go, Go by Example, Effective Go (all free online)
- Track 6: Docker documentation (free)
- Track 7: Wilson LLM Security book (owned)

### Track 8: Software Architecture (Weeks 9-20)
**Books to buy:** $155 (Let's Go + Let's Go Further + Ousterhout + Richards & Ford) — Bodner 1st ed + Harsanyi already owned

Read for architectural understanding, not typing along:
- **Learning Go, 1st ed (Bodner):** Already owned — reference for Go concepts
- **100 Go Mistakes (Harsanyi):** Already owned — code review checklist for Claude Code output
- **Let's Go (Edwards):** Read for web app architecture — project structure, middleware, testing patterns
- **Let's Go Further (Edwards):** Read for production API architecture — auth, rate limiting, deployment
- **A Philosophy of Software Design (Ousterhout):** Week 13 — design principles, complexity, deep modules. Your lens for reviewing Claude Code output. (~180 pages, one full week)
- **Fundamentals of Software Architecture (Richards & Ford):** Week 15 — architecture styles, trade-off analysis, the architect role. This IS your job description. (~400 pages, skim selectively)

### Track 10: AI/ML Security (Weeks 21-28)
**Books to buy:** $50 (Huyen) — Dursey already owned

- **AI Engineering (Huyen):** $50 — essential for understanding production AI systems you'll attack
- **Red Teaming AI (Dursey):** Already owned — AI red teaming methodology
- **HTB Academy:** ~$20/month x 2 months — hands-on labs (budgeted separately)
- **Free courses:** Fast.ai, Hugging Face NLP course, OWASP LLM Top 10, MITRE ATLAS, HackAPrompt, Crucible CTF
- **Free tools:** Garak (NVIDIA — LLM vulnerability scanner), PyRIT (Microsoft — programmable red team framework)
- **Free frameworks:** NIST AI RMF, NIST Gen AI Profile, Google SAIF, AI Incident Database

### Track 9: Python Core + TDD (Weeks 30-37)
**Books to buy:** $40 (Okken)

- **Percival TDD book:** Free online at obeythetestinggoat.com (owned physical copy too)
- **Okken pytest:** $40 — understand testing concepts to direct Claude Code
- **Cosmic Python:** Free online at cosmicpython.com — Python architecture patterns

### Track 11: Go Security Tools + AI Capstone (Weeks 38-43)
**Books to buy:** $0

- **Black Hat Go:** Already owned — security tool architecture concepts
- **100 Go Mistakes:** Already owned — code review reference

-----

## Budget Summary

|Category       |Cost  |Details                                        |
|---------------|------|-----------------------------------------------|
|Go books       |$80   |Let's Go ($40) + Let's Go Further ($40) — Bodner + Harsanyi owned|
|Architecture   |$75   |Ousterhout ($25) + Richards & Ford ($50)        |
|Python book    |$40   |Okken pytest                                   |
|AI/ML books    |$50   |Huyen ($50) — Dursey already owned             |
|HTB Academy    |~$40  |$20/month x 2 months (Track 10)                |
|**Total**      |**~$285**|                                            |

**Books you already own:** 14 (worth ~$500+)
**Free online resources used:** 15+ (Fast.ai, Hugging Face, Cosmic Python, Percival, Odin Project, etc.)

-----

## Key Principle

**Books for architectural understanding, free resources for breadth.**

- Go books ($80) → read for Go-specific architecture patterns, review Claude Code output
- Architecture books ($75) → language-agnostic design principles and architect role
- AI/ML book ($50) → understand the systems you'll attack
- pytest book ($40) → understand testing concepts to direct Claude Code
- Everything else → free online resources are sufficient

As an architect who directs Claude Code, you don't need to memorize syntax. You need to understand systems deeply enough to give precise direction and review output effectively.
