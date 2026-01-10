# Track 8: Python Core

**Duration:** 10 weeks | **Total:** ~180 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** HIGH
**Goal:** TDD and architecture skills needed for ML/AI work

-----

## Why Before ML?

These skills are essential for AI red teaming:

- Testing ML pipelines and model outputs
- Reviewing AI-generated code
- Building reliable security tools
- Understanding codebases you'll be attacking

-----

## Phase Overview

|Phase|Weeks|Focus                |Key Resource                                                 |
|-----|-----|---------------------|-------------------------------------------------------------|
|1A   |9-12 |TDD Methodology      |Test-Driven Development with Python, 3rd ed (Percival) - FREE|
|1B   |13-14|pytest Mastery       |Python Testing with pytest, 2nd ed (Okken) - ~$40            |
|2    |15-18|Architecture Patterns|Architecture Patterns with Python - FREE                     |

-----

## Books

|Book                                                  |Cost       |Phase|Project-Driven?                 |
|------------------------------------------------------|-----------|-----|--------------------------------|
|Test-Driven Development with Python, 3rd ed (Percival)|FREE online|1A   |✅ Yes (Django TDD project)      |
|Python Testing with pytest, 2nd ed (Okken)            |~$40       |1B   |✅ Yes (exercises)               |
|Architecture Patterns with Python (Cosmic Python)     |FREE online|2    |✅ Yes (builds allocation system)|

**Total Book Cost:** ~$40

-----

## Video Resources

|Resource                   |Cost        |Focus               |
|---------------------------|------------|--------------------|
|ArjanCodes (YouTube)       |Free        |Clean code, patterns|
|TCM Security Python courses|Subscription|Security tooling    |

-----

## Phase 1A: TDD Methodology (Weeks 9-12)

**Resource:** Test-Driven Development with Python, 3rd ed (Percival) - FREE at obeythetestinggoat.com

|Week|Chapters|Focus                                 |
|----|--------|--------------------------------------|
|9   |1-4     |Red-Green-Refactor, first Django tests|
|10  |5-8     |Forms, input validation, database     |
|11  |9-12    |Refactoring, deployment               |
|12  |13-16   |Advanced testing patterns             |

**Book Structure:**
- **Part I (Ch 1-8):** The Basics of TDD and Django
- **Part II (Ch 9-12):** Going to Production
- **Part III (Ch 13-16):** Forms and Validation
- **Part IV (Ch 17-27):** Advanced Topics in Testing (optional for later)

**This track covers Parts I-III** (Chapters 1-16), which provide core TDD skills.

**Part IV (Chapters 17-27)** covers advanced topics like spiking, mocking, outside-in development, and CI - these are optional and can be studied later if needed.

**Project:** Build a security tool with TDD (port scanner, log parser)

-----

## Phase 1B: pytest Mastery (Weeks 13-14)

**Resource:** Python Testing with pytest, 2nd ed (Okken) - ~$40

|Week|Chapters|Focus                    |
|----|--------|-------------------------|
|13  |1-6     |Fixtures, parametrization|
|14  |7-12    |Plugins, CI integration  |

-----

## Phase 2: Architecture Patterns (Weeks 15-18)

**Resource:** Architecture Patterns with Python (Cosmic Python) - FREE at cosmicpython.com

|Week|Chapters|Focus                              |
|----|--------|-----------------------------------|
|15  |1-3     |Domain modeling, repository pattern|
|16  |4-6     |Service layer, unit of work        |
|17  |7-9     |Aggregates, events                 |
|18  |10-12   |CQRS, event-driven architecture    |

**Project:** Security Findings Aggregator (Semgrep, Dependabot integration)

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

## Checkpoint

Before moving to AI/ML Security, you should be able to:

- Write tests before code (TDD red-green-refactor)
- Use pytest fixtures and parametrization
- Structure code with repository pattern and service layers
- Review Python code for quality and security issues
