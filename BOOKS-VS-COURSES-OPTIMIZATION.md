# Books & Resources Optimization Guide

**Updated:** February 7, 2026
**Status:** Aligned with restructured plan (Go-first, 65 weeks)

-----

## TL;DR

**Total budget: ~$230** for 5 remaining books across 65 weeks. The plan prioritizes:
- **Books for Go** — your work language deserves deep reference material
- **Free resources first** — most tracks use free online books, courses, and workshops
- **No paid courses or subscriptions needed** — HTB Academy ($20/month × 2) is the only subscription, and it's already budgeted in Track 10

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
|Node.js: The Comprehensive Guide (Springer)   |Track 13: JavaScript/TypeScript      |
|Web Development with Node and Express (Brown) |Track 13: JavaScript/TypeScript      |
|Eloquent JavaScript (Haverbeke)               |Track 13: JavaScript/TypeScript      |
|100 Go Mistakes (Harsanyi)                    |Track 8: Go Foundations + Architecture|

**12 books already owned** covering Tracks 1, 2, 4, 7, 8, 9, 11, and 13.

-----

## Books to Purchase

|Book                                      |Cost |Track                                  |When to Buy         |
|------------------------------------------|-----|---------------------------------------|---------------------|
|Learning Go, 2nd ed (Bodner)              |~$50 |Track 8: Go Foundations + Architecture |Before Week 9        |
|Let's Go (Edwards)                        |~$40 |Track 8: Go Foundations + Architecture |Before Week 9        |
|Python Testing with pytest, 2nd ed (Okken)|~$40 |Track 9: Python Core + TDD            |Before Week 25       |
|AI Engineering (Huyen)                    |~$50 |Track 10: AI/ML Security              |Before Week 33       |
|Red Teaming AI (Dursey)                   |~$50 |Track 10: AI/ML Security              |July 2026 (on release)|

**Total: ~$230**

-----

## What Was Dropped (and Why)

|Book/Course                    |Original Cost|Why Dropped                                           |
|-------------------------------|-------------|------------------------------------------------------|
|Using Asyncio in Python (Fowler)|~$50        |David Beazley's free workshops + Go concurrency knowledge make this unnecessary|
|Fluent Python (Ramalho)        |~$50         |Reference book — not needed for a 6-week track; use online docs|
|Black Hat Python               |~$35         |You're building security tools in Go (your work language), not Python|
|Programming TypeScript         |~$40         |JS/TS track compressed to 14 weeks; YDKJS + online docs sufficient|
|NVIDIA Adversarial ML course   |$90          |HTB Academy covers adversarial techniques with better hands-on labs|
|TestDriven.io subscription     |~$30/month   |Percival book (free online) is sufficient for TDD with Django|
|Real Python subscription       |~$60/year    |Beazley workshops (free) cover async Python effectively|
|Zero To Mastery Node.js        |~$40         |You own 4 JS/TS books already — no need to add a course|
|TCM Security Python courses    |Subscription |HTB Academy AI Red Teamer path is more relevant to your goals|

**Total saved: ~$395 in books and courses that don't add value over free alternatives**

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

### Track 8: Go Foundations + Architecture (Weeks 9-20)
**Books to buy:** $90 (Bodner + Edwards) — 100 Go Mistakes already owned

This is the biggest book investment because Go is your work language and this is a 12-week track:
- **Learning Go (Bodner):** Primary Go language reference — practical, idiomatic
- **100 Go Mistakes (Harsanyi):** Already owned — code review companion, reference throughout career
- **Let's Go (Edwards):** Web development in Go — project-driven, builds real app

**Why books over courses for Go:**
- Limited quality Go courses for your level (you already use Go daily)
- These books are project-driven with hands-on exercises
- Black Hat Go (owned) adds security context in Track 11
- No course covers Go + software architecture together

### Track 9: Python Core + TDD (Weeks 25-32)
**Books to buy:** $40 (Okken)

- **Percival TDD book:** Free online at obeythetestinggoat.com (owned physical copy too)
- **Okken pytest:** $40 — best pytest reference, essential for TDD workflow
- **Cosmic Python:** Free online at cosmicpython.com — architecture patterns in Python
- **Video:** ArjanCodes YouTube (free) for clean code patterns

### Track 10: AI/ML Security (Weeks 33-42)
**Books to buy:** $100 (Huyen + Dursey)

- **AI Engineering (Huyen):** $50 — essential for understanding production AI systems you'll be attacking. Covers RAG architecture, prompt engineering, evaluation, and inference — all directly relevant to red teaming
- **Red Teaming AI (Dursey):** $50 — releases July 2026, the first dedicated AI red teaming book. Buy on release
- **HTB Academy:** ~$20/month × 2 months — hands-on labs (budgeted separately)
- **Free:** Fast.ai, Hugging Face NLP course, OWASP LLM Top 10, HackAPrompt, Crucible CTF

**Why Huyen is essential (not optional):**
The previous optimization guide recommended skipping Huyen. That was wrong. Huyen's chapters on RAG (Ch 6), prompt engineering (Ch 5), evaluation (Ch 3-4), and production architecture (Ch 7, 9, 10) map directly to attack surfaces you need to understand. HTB Academy teaches exploitation; Huyen teaches the systems you're exploiting.

### Track 11: Go Security Tools (Weeks 21-24)
**Books to buy:** $0

- **Black Hat Go:** Already owned — THE resource for Go security tools
- No other books needed for this 4-week track

### Track 12: Python Advanced (Weeks 43-48)
**Books to buy:** $0

- **David Beazley workshops:** Free on YouTube — covers async Python deeply
- **Python asyncio documentation:** Free online
- **DeepSource AST tutorial + Ruff docs:** Free online

**Why no Fowler book:**
You already understand concurrency from Go (goroutines, channels, fan-out/fan-in). Python's asyncio is syntax, not a new concept. Beazley's free workshops are enough.

### Track 13: JavaScript/TypeScript (Weeks 49-62)
**Books to buy:** $0

- **Eloquent JavaScript:** Already owned
- **Node.js Comprehensive Guide (Springer):** Already owned
- **Web Dev with Node/Express (Brown):** Already owned
- **Free:** You Don't Know JS Yet (free on GitHub), The Odin Project, JavaScript30, TypeScript Handbook

You own 3 JS/TS books. YDKJS is free online — no purchase needed.

-----

## Budget Summary

|Category       |Cost  |Details                                        |
|---------------|------|-----------------------------------------------|
|Go books       |$90   |Bodner ($50) + Edwards ($40) — Harsanyi owned  |
|Python book    |$40   |Okken pytest                                   |
|AI/ML books    |$100  |Huyen ($50) + Dursey ($50)                     |
|HTB Academy    |~$40  |$20/month × 2 months (Track 10)                |
|**Total**      |**~$270**|                                            |

**Books you already own:** 12 (worth ~$400+)
**Free online resources used:** 15+ (Fast.ai, Hugging Face, Cosmic Python, Percival, Beazley, Odin Project, etc.)

-----

## Key Principle

**Books for depth, free resources for breadth.**

- Go books ($90 remaining) → your work language, worth the investment
- AI/ML books ($100) → understand the systems you'll attack
- pytest book ($40) → essential TDD reference
- Everything else → free online resources are sufficient

The plan avoids paid subscriptions (Real Python, TestDriven.io, ZTM) in favor of high-quality free alternatives and the books you already own.
