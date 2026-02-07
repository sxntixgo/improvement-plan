# Track 10: Python Advanced

**Duration:** 8 weeks | **Total:** ~144 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** MEDIUM
**Goal:** AST manipulation, linting, and async patterns

-----

## Why After AI/ML Security?

These are advanced topics that build on your core Python skills but aren't required for ML/AI work:

- AST manipulation for building security tools
- Custom linting rules for code analysis
- Async patterns for high-performance scanners

You can do effective AI red teaming without these, but they're valuable for:

- Building custom static analysis tools
- Creating high-performance security scanners
- Deep code analysis capabilities

-----

## Phase Overview

|Phase|Weeks|Focus             |Key Resource                          |
|-----|-----|------------------|--------------------------------------|
|3    |27-30|Code Quality / AST|DeepSource AST tutorial + Ruff - FREE |
|4    |31-34|Async Python      |Beazley workshops + Fowler book - ~$50|

-----

## Books

|Book                            |Cost|Phase    |Project-Driven?       |
|--------------------------------|----|---------|----------------------|
|Using Asyncio in Python (Fowler)|~$50|4        |✅ Yes (examples)      |
|Fluent Python, 2nd ed (Ramalho) |~$50|Reference|❌ No (reference)      |
|Black Hat Python, 2nd ed        |~$35|Security |✅ Yes (security tools)|

**Total Book Cost:** ~$50-135 (Fowler required, others optional)

-----

## Video Resources

|Resource                                |Cost|Focus                   |
|----------------------------------------|----|------------------------|
|David Beazley Python Workshops (YouTube)|Free|Async, advanced patterns|
|ArjanCodes (YouTube)                    |Free|Clean code, patterns    |

-----

## Phase 3: Code Quality / AST (Weeks 27-30)

**Resources:**

- DeepSource AST tutorial - FREE
- Ruff documentation - FREE
- Semgrep documentation - FREE

|Week|Focus                             |
|----|----------------------------------|
|27  |Python AST basics, ast module     |
|28  |Writing custom lint rules with AST|
|29  |Semgrep rule authoring            |
|30  |Integration with CI/CD            |

**Project:** Custom linter rule (Semgrep or AST-based)

-----

## Phase 4: Async Python (Weeks 31-34)

**Resources:**

- David Beazley workshops (YouTube) - FREE
- Using Asyncio in Python (Fowler) - ~$50

|Week|Focus                               |
|----|------------------------------------|
|31  |asyncio fundamentals, event loop    |
|32  |async/await patterns, tasks         |
|33  |Concurrent HTTP requests, aiohttp   |
|34  |Building async tools, error handling|

**Project:** Async Security Scanner Orchestrator

-----

## Projects & Outputs

|Project               |Output              |Share    |
|----------------------|--------------------|---------|
|Custom linter rule    |Semgrep or AST-based|GitHub   |
|Async Security Scanner|Orchestrator tool   |GitHub   |
|AST deep dive         |How Python AST works|Blog post|

-----

## Code Review Checklist (Python Advanced)

- [ ] AST transformations preserve semantics?
- [ ] Lint rules have clear error messages?
- [ ] Async: proper awaiting, no blocking calls in async context?
- [ ] Async: exception handling in tasks?
- [ ] Async: proper cleanup with async context managers?
- [ ] Async: avoiding task starvation?

-----

## Checkpoint

After completing this track, you should be able to:

- Parse and analyze Python code with AST
- Write custom Semgrep rules
- Build async tools with proper error handling
- Create high-performance concurrent scanners
