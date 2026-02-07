# Track 12: Python Advanced

**Duration:** 6 weeks | **Total:** ~108 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** MEDIUM
**Goal:** AST manipulation, linting, and async patterns

-----

## Why After Go Security?

These are advanced topics that build on your core Python skills but aren't required for ML/AI work:

- AST manipulation for building security tools
- Custom linting rules for code analysis
- Async patterns for high-performance scanners

You can do effective AI red teaming without these, but they're valuable for:

- Building custom static analysis tools
- Creating high-performance security scanners
- Deep code analysis capabilities

**Why compressed to 6 weeks (from 8):**
You already understand concurrency deeply from Go (goroutines, channels, fan-out/fan-in). Python's asyncio will feel familiar — you're learning syntax, not concepts.

-----

## Phase Overview

|Phase|Weeks|Focus             |Key Resource                          |
|-----|-----|------------------|--------------------------------------|
|1    |43-45|Code Quality / AST|DeepSource AST tutorial + Ruff - FREE |
|2    |46-48|Async Python      |Beazley workshops + Fowler book - ~$50|

-----

## Books

|Book                            |Cost|Phase    |Project-Driven?       |
|--------------------------------|----|---------|----------------------|
|Using Asyncio in Python (Fowler)|~$50|2        |Yes (examples)        |
|Fluent Python, 2nd ed (Ramalho) |~$50|Reference|No (reference)        |
|Black Hat Python, 2nd ed        |~$35|Security |Yes (security tools)  |

**Total Book Cost:** ~$50-135 (Fowler required, others optional)

-----

## Video Resources

|Resource                                |Cost|Focus                   |
|----------------------------------------|----|------------------------|
|David Beazley Python Workshops (YouTube)|Free|Async, advanced patterns|
|ArjanCodes (YouTube)                    |Free|Clean code, patterns    |

-----

## Phase 1: Code Quality / AST (Weeks 43-45)

**Resources:**

- DeepSource AST tutorial - FREE
- Ruff documentation - FREE
- Semgrep documentation - FREE

|Week|Focus                                    |
|----|-----------------------------------------|
|43  |Python AST basics, ast module            |
|44  |Writing custom lint rules with AST + Semgrep rule authoring|
|45  |Integration with CI/CD + capstone project|

**Project:** Custom linter rule (Semgrep or AST-based)

-----

## Phase 2: Async Python (Weeks 46-48)

**Resources:**

- David Beazley workshops (YouTube) - FREE
- Using Asyncio in Python (Fowler) - ~$50

|Week|Focus                                         |
|----|----------------------------------------------|
|46  |asyncio fundamentals, event loop, async/await |
|47  |Concurrent HTTP requests, aiohttp, tasks      |
|48  |Building async tools, error handling, capstone |

**Your Go Advantage:**
You already understand concurrent programming from Go. Here's how concepts map:

| Go | Python asyncio |
|----|----------------|
| goroutines | coroutines (async def) |
| channels | asyncio.Queue |
| select | asyncio.wait / gather |
| sync.WaitGroup | asyncio.gather |
| context.Context | asyncio.timeout / TaskGroup |
| errgroup | asyncio.TaskGroup (Python 3.11+) |

**Comparison Exercise (Week 48):**
Build the same concurrent security scanner in both Python (asyncio) and Go (goroutines). Compare:
- Lines of code
- Performance (throughput, latency)
- Error handling patterns
- Readability
- Blog post: "Python asyncio vs Go goroutines for Security Scanning"

**Project:** Async Security Scanner Orchestrator

-----

## Projects & Outputs

|Project                        |Output                            |Share    |
|-------------------------------|----------------------------------|---------|
|Custom linter rule             |Semgrep or AST-based              |GitHub   |
|Async Security Scanner         |Orchestrator tool                 |GitHub   |
|AST deep dive                  |How Python AST works              |Blog post|
|Go vs Python scanner comparison|Same tool in both languages        |Blog post|

-----

## Claude Code Integration

**AST Analysis:**
```
EXPLAIN: "Show me how to parse this Python file's AST and find
all function calls that use eval() or exec(). I want to build
a security linter."

CREATE: "Write an AST visitor that detects SQL injection patterns
in Python code. Flag any string concatenation used in database queries."
```

**Async Patterns:**
```
EXPLAIN: "I understand Go's goroutine + channel pattern for
fan-out/fan-in. Show me the equivalent in Python asyncio.
Side-by-side comparison."

REFACTOR: "Convert this synchronous Python HTTP client to use
aiohttp with proper connection pooling and error handling."
```

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
- Compare Python async patterns to Go concurrency (and choose the right tool)
