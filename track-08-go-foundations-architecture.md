# Track 8: Software Architecture (via Go)

**Duration:** 12 weeks | **Hours/week:** 18 | **Priority:** HIGH
**Goal:** Deep understanding of software architecture patterns to direct Claude Code effectively

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why This Track Matters for an Architect

You don't write code — Claude Code does. But you need to **think in systems** to give Claude Code good direction. This track teaches you:

- **What good architecture looks like** — so you can specify it in CLAUDE.md and prompts
- **Why dependencies should point inward** — so you can catch violations in code review
- **How testing layers work** — so you can tell Claude Code what tests to write
- **What production-ready means** — so you can define "done" precisely

Go is the vehicle because it's your work language. The architecture patterns transfer to every language.

-----

## How to Study as an Architect

**Your approach is different from a hands-on coder:**

1. **Read the Edwards books for understanding, not typing along.** Follow the project mentally. Understand WHY each architectural decision is made. You don't need to type every line — you need to understand the structure.

2. **Direct Claude Code to build the projects.** After reading a chapter, give Claude Code architectural instructions to build what you read about. Review what it produces.

3. **Focus on the architecture, not the syntax.** When studying clean architecture or DDD, your goal is to explain these patterns to Claude Code precisely. Can you describe hex architecture well enough that Claude Code implements it correctly?

4. **Use 100 Go Mistakes as a code review guide.** When Claude Code produces Go code, use Harsanyi's book to review it. This is exactly what you'll do at work.

-----

## Phase Overview

|Phase|Weeks|Focus                    |Key Resource                            |
|-----|-----|-------------------------|----------------------------------------|
|1    |9-12 |Go Web App Architecture  |Let's Go (Edwards) — read for understanding|
|2    |13-16|Software Architecture Patterns|Architecture resources + Claude Code projects|
|3    |17-20|Production API Architecture|Let's Go Further (Edwards) — read for understanding|

-----

## Resources

### Go Books

|Resource                      |Cost         |Phase|How to Use                        |
|------------------------------|-------------|-----|----------------------------------|
|Let's Go (Alex Edwards)       |~$40         |1    |Read for architecture understanding|
|Let's Go Further (Alex Edwards)|~$40        |3    |Read for production patterns      |
|Learning Go, 1st ed (Bodner)  |Already owned|1-3  |Reference for Go concepts         |
|100 Go Mistakes (Harsanyi)    |Already owned|1-3  |Code review checklist             |
|Go by Example                 |Free         |1    |Quick reference                   |
|Effective Go                  |Free         |1-2  |Idiomatic patterns                |

### Architecture Books (Language-Agnostic)

|Resource                                       |Cost  |Phase|How to Use                        |
|-----------------------------------------------|------|-----|----------------------------------|
|A Philosophy of Software Design (Ousterhout)    |~$25  |2    |Design principles — complexity, deep modules, interfaces|
|Fundamentals of Software Architecture (Richards & Ford)|~$50|2  |Architecture styles, trade-offs, the architect role|

**Why these two books matter for you:**
- **Ousterhout** teaches you to think about complexity, module design, and interface design. Short (~180 pages). Every concept directly applies to reviewing Claude Code's output — is this module deep or shallow? Is this interface hiding complexity or leaking it?
- **Richards & Ford** is specifically about being an architect. It covers architecture styles (layered, microservices, event-driven), trade-off analysis, and how architects communicate decisions. This is your actual job.

### Architecture Resources (Free)

- [Go Project Layout](https://github.com/golang-standards/project-layout) - Standard project structure
- [Kat Zien - How Do You Structure Your Go Apps](https://www.youtube.com/watch?v=oL6JBUk6tj0) - GopherCon talk
- [Three Dots Labs - Go with The Domain](https://threedots.tech/post/ddd-lite-in-go-introduction/) - DDD in Go series
- [Three Dots Labs - Wild Workouts](https://github.com/ThreeDotsLabs/wild-workouts-go-ddd-example) - Full DDD example app
- [ardanlabs/service](https://github.com/ardanlabs/service) - Production Go service template
- [Go Time Podcast - Architecture episodes](https://changelog.com/gotime) - Listen during commute
- [martinfowler.com](https://martinfowler.com) - Architecture patterns and articles (microservices, event sourcing, CQRS)

-----

## Phase 1: Go Web App Architecture (Weeks 9-12)

**Primary Resource:** Let's Go (Alex Edwards) — read for architectural understanding
**Reference:** Learning Go, 1st ed (Bodner) — look up concepts as needed

**Your approach:** Read Edwards chapter by chapter. Understand the project structure, routing patterns, middleware chain, and database layer. Then direct Claude Code to build the same app, giving it architectural specifications. Review what Claude Code produces.

### Week 9: Project Structure + Routing + Templates

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Let's Go Ch 1-3: Understand project structure, routing, HTML templates|
|Wed-Thu|4|Read Let's Go Ch 4: Configuration, error handling, logging patterns|
|Fri|2|Review: Go by Example for quick syntax reference|
|Weekend|6|Direct Claude Code: Build the app structure from Ch 1-4. Review the output.|

**Architect Focus:**
- How does Edwards structure the project? (cmd/, internal/, ui/)
- Why does he use dependency injection for the application struct?
- How does the error handling flow from handler → user?

**Claude Code Direction Example:**
```
"Create a Go web application with this structure:
- cmd/web/main.go for the entry point
- internal/models/ for database models
- ui/html/ for templates
- Use dependency injection: application struct holds dependencies
- Configure structured logging with slog
- Follow Let's Go (Alex Edwards) project layout"
```

### Week 10: Database Layer + Middleware Architecture

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Let's Go Ch 5-7: MySQL layer, middleware pattern, RESTful routing|
|Wed-Thu|4|Read Let's Go Ch 8-9: Sessions, server-side validation|
|Fri|2|Study: How middleware chains work in Go|
|Weekend|6|Direct Claude Code: Add database layer + middleware to the app. Review.|

**Architect Focus:**
- How does the repository pattern emerge from Edwards' database layer?
- How does middleware chaining work? (func(http.Handler) http.Handler)
- Where does validation logic belong — handler or service layer?
- How does dependency injection via struct fields enable testability?

**Key Patterns to Understand:**
- Structs, methods, interfaces — how they enable clean architecture
- Pointer receivers vs value receivers — when to use each
- Interface satisfaction is implicit — "accept interfaces, return structs"
- Dependency injection via struct fields — Go's approach (no frameworks)

### Week 11: Testing Architecture + Security Patterns

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Let's Go Ch 10-11: Testing handlers, testing middleware|
|Wed-Thu|4|Read Let's Go Ch 12-13: Authentication, embedding, file serving|
|Fri|2|Study: Go testing patterns (table-driven, httptest)|
|Weekend|6|Direct Claude Code: Add tests + authentication. Review test quality.|

**Architect Focus:**
- Table-driven tests — Go's signature testing pattern
- How does httptest enable handler testing without a running server?
- Interface-based mocking — no framework needed
- Test organization: what goes in *_test.go files?

**Code Review Practice:**
When Claude Code writes tests, review them using 100 Go Mistakes:
- Mistake #78: Not using httptest
- Mistake #2: Unnecessary nested code
- Mistake #45: Returning a nil receiver

### Week 12: Concurrency Architecture

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Bodner Ch 12-13: Goroutines, channels, select (focused study)|
|Wed-Thu|4|Study: Concurrency patterns — fan-out/fan-in, pipeline, worker pool|
|Fri|2|Read: How concurrency applies to web apps (background tasks, graceful shutdown)|
|Weekend|6|Direct Claude Code: Add concurrency to the web app. Review for race conditions.|

**Architect Focus:**
- When to use goroutines vs when NOT to
- Buffered vs unbuffered channels — architectural implications
- Context for cancellation and timeouts — how it flows through layers
- Race detector: tell Claude Code to run `go test -race`

**100 Go Mistakes Reference (for reviewing Claude Code output):**
- Mistake #61: Propagating inappropriate context
- Mistake #66: Using mutexes inaccurately
- Mistake #69: Forgetting about goroutine leaks

-----

## Phase 2: Software Architecture Patterns (Weeks 13-16)

**Why This Phase is Critical for You:**
This is where you learn the vocabulary and patterns to give Claude Code precise architectural direction. After this phase, you can say "use hex architecture with ports and adapters" and Claude Code will know exactly what to build — and you'll know how to verify it did it right.

**Two architecture books anchor this phase:**
- **A Philosophy of Software Design (Ousterhout):** Read during Week 13 (~180 pages). Teaches you to evaluate complexity, module depth, and interface design — the lens you use to review everything Claude Code produces.
- **Fundamentals of Software Architecture (Richards & Ford):** Read during Weeks 14-16 (~400 pages, skim sections you already grasp). Teaches architecture styles, trade-off analysis, and how architects think — this is literally your role.

### Week 13: Design Principles + Clean Architecture

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read: Ousterhout Ch 1-8 (complexity, deep modules, information hiding)|
|Wed-Thu|4|Study: Clean Architecture + Hex Architecture in Go|
|Fri|2|Study: [ardanlabs/service](https://github.com/ardanlabs/service) project structure|
|Weekend|6|Read: Ousterhout Ch 9-18 + Direct Claude Code: Restructure a project. Review.|

**Ousterhout Key Concepts (your new review lens):**
- **Complexity:** The root cause of all software problems. Design it out, don't manage it.
- **Deep vs Shallow Modules:** Deep modules have simple interfaces but powerful functionality. Shallow modules leak complexity. When Claude Code creates a module, ask: is this deep or shallow?
- **Information Hiding:** Each module should hide its internal complexity. If Claude Code exposes implementation details through interfaces, that's a red flag.
- **Interface Design:** Interfaces should be obvious and hard to misuse. Good interfaces reduce cognitive load.
- **Strategic vs Tactical Programming:** You're the strategic thinker. Claude Code is the tactical executor.

**Clean Architecture Concepts (applied through Go):**
- **Dependency Rule:** Dependencies point inward (domain has no external dependencies)
- **Layers in Go:**
  ```
  project/
  ├── cmd/                    # Entry points (main packages)
  │   └── api/
  │       └── main.go
  ├── internal/               # Private application code
  │   ├── domain/             # Business logic, entities, interfaces
  │   │   ├── user.go         # Domain types
  │   │   └── repository.go   # Repository interfaces
  │   ├── service/            # Use cases / application logic
  │   │   └── user_service.go
  │   ├── handler/            # HTTP handlers (adapters)
  │   │   └── user_handler.go
  │   └── storage/            # Database implementations (adapters)
  │       └── postgres/
  │           └── user_repo.go
  ├── pkg/                    # Shared libraries (if needed)
  ├── go.mod
  └── CLAUDE.md
  ```
- **Interface Placement:** Define interfaces where they're used (consumer side), not where they're implemented
- **Hex Architecture:** Ports (interfaces) + Adapters (implementations)

**How to Verify Claude Code's Output (using Ousterhout's lens):**
```
"Review this Go project structure. Check that:
1. Domain package has zero external imports
2. Interfaces are defined in the domain package
3. Dependencies point inward (handler → service → domain)
4. Modules are 'deep' — simple interfaces, rich functionality
5. No information leaking across layer boundaries"
```

### Week 14: DDD + Architecture Styles

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Study: DDD Lite in Go — entities, value objects, aggregates|
|Wed-Thu|4|Read: Richards & Ford Part I — architecture styles (layered, microservices, event-driven)|
|Fri|2|Study: [Three Dots Labs Wild Workouts](https://github.com/ThreeDotsLabs/wild-workouts-go-ddd-example)|
|Weekend|6|Direct Claude Code: Build a domain model for a real-world problem. Review.|

**DDD Core Concepts:**
- **Entities:** Types with identity (User, Order)
- **Value Objects:** Immutable types defined by their values (Money, Email)
- **Repository Interface** (domain package — no implementation details)
- **Service Layer:** Orchestrates domain operations, depends on interfaces

**Richards & Ford Key Concepts (Part I):**
- **Architecture Styles:** Layered, microkernel, microservices, event-driven, space-based — when to use each
- **Architecture Characteristics ("-ilities"):** Scalability, maintainability, testability, deployability — how to evaluate trade-offs
- **Architecture Decisions:** How to make and document them (ADRs)

**Resources:**
- [Three Dots Labs: DDD Lite in Go](https://threedots.tech/post/ddd-lite-in-go-introduction/)
- [Three Dots Labs: Wild Workouts](https://github.com/ThreeDotsLabs/wild-workouts-go-ddd-example)

### Week 15: DI + API Design + Architect Thinking

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Study: Dependency injection in Go (without frameworks)|
|Wed-Thu|4|Read: Richards & Ford Part II — soft skills of architecture (trade-off analysis, communication)|
|Fri|2|Study: Middleware patterns and chains|
|Weekend|6|Direct Claude Code: Build REST API with clean architecture + DI. Review.|

**Go-Specific Concepts:**
- **Constructor Injection** (Go's approach — no DI framework needed)
- **Middleware Pattern** (func(http.Handler) http.Handler)
- **Context Propagation** through layers for cancellation/timeouts
- **Error Handling in APIs:** Domain errors → HTTP status codes mapping

**Richards & Ford Key Concepts (Part II):**
- **Trade-Off Analysis:** Every architecture decision involves trade-offs. There's no "best" architecture — only "best for this context."
- **Architecture Decision Records (ADRs):** Document WHY you chose an architecture, not just what. Useful for CLAUDE.md files.
- **Communicating Architecture:** How to explain architectural decisions to teams. Directly relevant to directing Claude Code.
- **The Architect's Role:** An architect doesn't write all the code — they make sure the system hangs together. This is exactly your role with Claude Code.

**Architect Direction Example (informed by both books):**
```
"Build a Go REST API with:
- Constructor injection for all dependencies (no globals)
- Middleware chain: logging → auth → rate limiting → handler
- Domain errors mapped to HTTP status codes
- Context propagation for cancellation
- Follow hex architecture from Week 13
- Keep modules deep (Ousterhout): simple interfaces, rich implementations
- Document the architecture decision for layered vs microservices"
```

### Week 16: Testing Architecture

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Study: Testing strategies — unit, integration, end-to-end|
|Wed-Thu|4|Study: Testcontainers for integration tests|
|Fri|2|Study: Interface-based mocking (no mocking frameworks)|
|Weekend|6|Direct Claude Code: Write full test suite for Week 15 API. Review test quality.|

**Core Concepts:**
- **Test Pyramid:** Unit tests (domain) → Integration tests (repository) → E2E (handlers)
- **Interface-Based Mocking:** Implement the interface in tests, no mock framework
- **Testcontainers:** Real database in tests (PostgreSQL in Docker)
- **httptest:** Test HTTP handlers without a running server

**How to Review Claude Code's Tests:**
- Are tests testing behavior, not implementation?
- Is the test pyramid balanced (many unit, fewer integration, fewer e2e)?
- Are mocks implementing the same interface the production code uses?
- Is the race detector enabled?

-----

## Phase 3: Production API Architecture (Weeks 17-20)

**Primary Resource:** Let's Go Further (Alex Edwards) — read for production patterns
**Reference:** 100 Go Mistakes (Harsanyi) — code review guide

Read Let's Go Further for production-grade patterns. Direct Claude Code to build, then review against 100 Go Mistakes.

### Week 17: JSON API Architecture

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Let's Go Further: API setup, JSON encoding/decoding, routing|
|Wed-Thu|4|Read: Database migrations, SQL queries, CRUD endpoints|
|Fri|2|Apply: Clean architecture from Phase 2 to this project|
|Weekend|6|Direct Claude Code: Build JSON API with clean architecture. Review.|

### Week 18: Data Flow + Validation Architecture

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Let's Go Further: Query string parsing, filtering, sorting|
|Wed-Thu|4|Read: Input validation, error handling patterns|
|Fri|2|Review: 100 Go Mistakes API-related chapters|
|Weekend|6|Direct Claude Code: Add filtering, sorting, validation. Review patterns.|

### Week 19: Auth + Security Architecture

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Let's Go Further: User registration, activation emails|
|Wed-Thu|4|Read: Authentication tokens, permission-based authorization|
|Fri|2|Read: Rate limiting, IP-based throttling, CORS|
|Weekend|6|Direct Claude Code: Add auth + permissions + rate limiting. Review.|

### Week 20: Production Architecture + Capstone

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Let's Go Further: Graceful shutdown, metrics, build versioning|
|Wed-Thu|4|Study: Observability — structured logging (slog), health checks|
|Fri|2|Study: Docker multi-stage builds for Go apps|
|Weekend|6|Capstone: Direct Claude Code to produce production-ready Go API. Full review.|

**Capstone Review Checklist:**
By Week 20, Claude Code should have built two complete Go projects. Review the API capstone for:
- [ ] Clean architecture / hex architecture
- [ ] JSON API with authentication, permissions, rate limiting
- [ ] Database with migrations
- [ ] Comprehensive test suite (unit + integration)
- [ ] Docker multi-stage build
- [ ] Structured logging and health checks
- [ ] CLAUDE.md for the project
- [ ] No violations from 100 Go Mistakes

-----

## Architecture Review Checklist

Use this checklist every time you review Claude Code's Go output:

**Architecture:**
- [ ] Dependencies point inward (domain has no external imports)?
- [ ] Interfaces defined where they're consumed?
- [ ] Constructor injection for dependencies?
- [ ] Clear separation of domain, service, handler layers?

**Code Quality (via 100 Go Mistakes):**
- [ ] Error handling (not ignoring errors)?
- [ ] Error wrapping with context?
- [ ] Race conditions (proper mutex usage)?
- [ ] Resource leaks (defer for cleanup)?
- [ ] Context propagation through layers?

**Security:**
- [ ] Input validation?
- [ ] Crypto: using crypto/rand not math/rand?
- [ ] SQL injection (parameterized queries)?
- [ ] Command injection (proper escaping)?

**Testing:**
- [ ] Table-driven tests?
- [ ] Interface-based mocking (no mock frameworks)?
- [ ] Integration tests with testcontainers?
- [ ] Race detector enabled (`-race` flag)?

-----

## Projects & Outputs

|Project                           |Week |Output                           |Share             |
|----------------------------------|-----|---------------------------------|------------------|
|Let's Go web app (Claude Code)    |9-11 |Complete web app reviewed by you |GitHub            |
|Concurrency deep dive             |12   |Concurrent Go app reviewed       |GitHub            |
|Clean architecture project        |13   |Restructured project             |GitHub            |
|DDD domain model                  |14   |Domain-driven Go service         |GitHub            |
|REST API with clean architecture  |15-16|Full API with test suite         |GitHub            |
|Let's Go Further JSON API         |17-19|Production API reviewed by you   |GitHub            |
|Production-ready Go API (capstone)|20   |Polished API portfolio piece     |GitHub + Blog post|

-----

## Claude Code Integration

Use Claude Code as your implementation partner throughout this track:

**Architectural Direction:**
```
"Build a Go web application following hex architecture.
Structure: cmd/ for entry, internal/domain/ for business logic,
internal/handler/ for HTTP, internal/storage/ for database.
Interfaces in domain package. Constructor injection. No globals."
```

**Architecture Reviews:**
```
"Review this Go project for clean architecture violations.
Check dependency direction, interface placement, and layer separation."
```

**Code Quality (using 100 Go Mistakes):**
```
"Check this Go code against '100 Go Mistakes' patterns.
Focus on: error handling, concurrency, and interface design."
```

**Test Generation:**
```
"Generate table-driven tests for this Go function.
Include edge cases: nil inputs, empty slices, context cancellation.
Use interface-based mocking, not a mock framework."
```

**CLAUDE.md for Each Project:**
Create a CLAUDE.md at the start of each project with architecture decisions, build/test commands, and code style preferences.

-----

## Checkpoint

Before moving to Track 10: AI/ML Security, you should be able to:

- [ ] Explain clean / hex architecture to Claude Code precisely
- [ ] Evaluate module depth (Ousterhout) — is this deep or shallow?
- [ ] Identify information leaking across boundaries
- [ ] Choose between architecture styles and explain trade-offs (Richards & Ford)
- [ ] Review Go project structure for dependency rule violations
- [ ] Describe DDD patterns (entities, value objects, repositories)
- [ ] Specify dependency injection requirements for Claude Code
- [ ] Define REST API architecture with middleware
- [ ] Review test suites for proper test pyramid balance
- [ ] Identify concurrency issues in Claude Code's output
- [ ] Evaluate Go code against 100 Go Mistakes checklist
- [ ] Create effective CLAUDE.md files with architecture decisions documented
- [ ] Give Claude Code architectural direction that produces production-ready code
