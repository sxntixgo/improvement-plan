# Track 9: Python Core

**Duration:** 8 weeks | **Total:** ~144 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** MEDIUM
**Goal:** Deepen Python understanding for better AI security tool direction and code review

-----

## Why After AI/ML Security?

You just completed Track 10 (AI/ML Security) where Claude Code wrote Python for HTB labs, LangChain apps, and exploit scripts. Now you understand:

- **Why Python matters** — you've seen it used for real AI security work
- **What Python code looks like** — you've reviewed Claude Code's Python output for 8 weeks
- **Where your gaps are** — you know which Python concepts you need to understand better

This track deepens your ability to:
- Review Python code Claude Code produces (catch bugs, security issues)
- Give Claude Code more precise Python architectural direction
- Understand testing concepts to direct better test strategies
- Map Go architecture patterns to their Pythonic equivalents

**Your advantage:** You've already used Python tools (via Claude Code) during AI/ML security. Architecture patterns from Go (Track 8) transfer directly. You're deepening understanding, not starting from scratch.

-----

## Phase Overview

|Phase|Weeks|Focus                |Key Resource                                                 |
|-----|-----|---------------------|-------------------------------------------------------------|
|1A   |30-33|TDD Methodology      |Test-Driven Development with Python, 3rd ed (Percival) - FREE|
|1B   |34-35|pytest Mastery       |Python Testing with pytest, 2nd ed (Okken) - ~$40            |
|2    |36-37|Architecture in Python|Architecture Patterns with Python - FREE (accelerated)       |

-----

## Books

|Book                                                  |Cost       |Phase|Project-Driven?                 |
|------------------------------------------------------|-----------|-----|--------------------------------|
|Test-Driven Development with Python, 3rd ed (Percival)|FREE online|1A   |Yes (Django TDD project)        |
|Python Testing with pytest, 2nd ed (Okken)            |~$40       |1B   |Yes (exercises)                 |
|Architecture Patterns with Python (Cosmic Python)     |FREE online|2    |Yes (builds allocation system)  |

**Total Book Cost:** ~$40

-----

## Video Resources

|Resource                   |Cost        |Focus               |
|---------------------------|------------|--------------------|
|ArjanCodes (YouTube)       |Free        |Clean code, patterns|

-----

## Phase 1A: TDD Methodology (Weeks 30-33)

**Resource:** Test-Driven Development with Python, 3rd ed (Percival) - FREE at obeythetestinggoat.com

**Your approach as architect:** Read Percival to understand TDD philosophy and testing strategy. You already understand testing architecture from Go (Track 8). Focus on how TDD methodology guides architectural decisions — not on typing Django code.

|Week|Chapters|Focus                                 |
|----|--------|--------------------------------------|
|30  |1-4     |Red-Green-Refactor, first Django tests|
|31  |5-8     |Forms, input validation, database     |
|32  |9-12    |Refactoring, deployment               |
|33  |13-16   |Advanced testing patterns             |

**Book Structure:**
- **Part I (Ch 1-8):** The Basics of TDD and Django
- **Part II (Ch 9-12):** Going to Production
- **Part III (Ch 13-16):** Forms and Validation
- **Part IV (Ch 17-27):** Advanced Topics in Testing (optional for later)

**This track covers Parts I-III** (Chapters 1-16), which provide core TDD skills.

**Part IV (Chapters 17-27)** covers advanced topics like spiking, mocking, outside-in development, and CI - these are optional and can be studied later if needed.

**Project:** Build a security tool with TDD (port scanner, log parser)

-----

## Phase 1B: pytest Mastery (Weeks 34-35)

**Resource:** Python Testing with pytest, 2nd ed (Okken) - ~$40

|Week|Chapters|Focus                    |
|----|--------|-------------------------|
|34  |1-6     |Fixtures, parametrization|
|35  |7-12    |Plugins, CI integration  |

-----

## Phase 2: Architecture Patterns in Python (Weeks 36-37)

**Resource:** Architecture Patterns with Python (Cosmic Python) - FREE at cosmicpython.com

**Why only 2 weeks (instead of 4):**
You already learned architecture in Go (Track 8) and have used Python tools during AI/ML (Track 10). This phase focuses on the **Pythonic equivalents** of patterns you already know, not learning architecture from scratch.

|Week|Chapters|Focus                                     |
|----|--------|------------------------------------------|
|36  |1-6     |Domain modeling, repository, service layer — the Pythonic way|
|37  |7-12    |Events, CQRS — advanced patterns (skim what you know, deep dive on new concepts)|

**Key Mappings from Go → Python:**
- Go interfaces → Python Protocols / ABCs
- Go constructor injection → Python `__init__` injection
- Go `internal/` package → Python `_private` modules
- Go table-driven tests → pytest parametrize
- Go `context.Context` → Python contextvars / dependency injection
- Go error wrapping → Python exception chaining (`raise ... from`)

**Project:** Security Findings Aggregator (Semgrep, Dependabot integration) — apply architecture patterns

-----

## Projects & Outputs

|Project                     |Output                         |Share    |
|----------------------------|-------------------------------|---------|
|Security tool with TDD      |Port scanner or log parser     |GitHub   |
|Security Findings Aggregator|Semgrep/Dependabot integration |GitHub   |
|TDD learnings               |Key insights from Percival book|Blog post|

-----

## Code Review Checklist (Python Core)

- [ ] Type hints present and correct?
- [ ] Error handling appropriate (not bare `except:`)?
- [ ] Resource cleanup (context managers, finally blocks)?
- [ ] Security: input validation, no hardcoded secrets, safe deserialization?
- [ ] Tests included? Meaningful or just coverage padding?
- [ ] Dependencies reasonable?
- [ ] Pythonic idioms vs. Java-in-Python?

-----

## Claude Code Integration

Use Claude Code as a **continuous accelerator** throughout Python Core:

**Learning Python as a Go Developer:**
```
EXPLAIN: "I'm a Go developer learning Python. Explain how Python's
error handling (try/except) compares to Go's (err != nil) pattern.
Show equivalent code side by side."

REVIEW: "Review this Python code from a Go developer's perspective.
Flag any 'Go-isms' I'm bringing over that aren't Pythonic."
```

**TDD with Claude Code:**
```
TEST: "Generate pytest test cases for this function using
table-driven tests (similar to Go's table-driven test pattern).
Include edge cases and error conditions."

CREATE: "Write a Python function that [requirement] using TDD.
Start with the test, then implement. Use pytest fixtures."
```

**Architecture with Claude Code:**
```
EXPLAIN: "Compare Go's interface pattern (implicit satisfaction)
with Python's Protocol/ABC pattern. When should I use each?"

REFACTOR: "Refactor this Python code to use the repository pattern.
I'm familiar with this from Go — show me the Pythonic equivalent."
```

**CLAUDE.md for Python Projects:**
Create a CLAUDE.md for each Python project:
```markdown
# Python Project

# Build & Test
- `pytest` to run all tests
- `pytest --cov` for coverage
- `ruff check .` for linting
- `mypy .` for type checking

# Code Style
- Type hints on all public functions
- pytest fixtures over setUp/tearDown
- Repository pattern for data access
```

-----

## Checkpoint

Before moving to Track 11: Go Security Tools + AI Capstone, you should be able to:

- Explain TDD methodology (red-green-refactor) to Claude Code
- Direct Claude Code to use pytest fixtures and parametrization
- Review Python architecture for repository pattern and service layer violations
- Review Python code for quality and security issues
- Map Go architecture patterns to Pythonic equivalents
- Give Claude Code more precise Python direction than before Track 10
