# Track 8: Go Foundations + Software Architecture

**Duration:** 12 weeks | **Hours/week:** 18 | **Priority:** HIGH
**Goal:** Go language mastery and software architecture patterns for your daily work

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why Go First?

Go is your daily work language. Learning software architecture in Go means:

- **Immediate impact** at work — apply patterns the same week you learn them
- **Architecture transfers** — once you learn clean architecture in Go, applying it in Python or TypeScript is straightforward
- **Compound growth** — 12 weeks of structured Go learning while writing Go at work daily = accelerated mastery
- **Interview readiness** — you can discuss architecture decisions in your strongest language

You already have a crash course foundation from Track 5 (Week 6). Now you go deep.

-----

## Phase Overview

|Phase|Weeks|Focus                    |Key Resource                            |
|-----|-----|-------------------------|----------------------------------------|
|1    |9-12 |Go Web App (Learn by Doing)|Let's Go (Edwards)                    |
|2    |13-16|Go Software Architecture |Architecture resources + projects        |
|3    |17-20|Go JSON API + Production |Let's Go Further (Edwards) + 100 Go Mistakes|

-----

## Resources

|Resource                      |Cost         |Phase|Project-Driven?              |
|------------------------------|-------------|-----|-----------------------------|
|Let's Go (Alex Edwards)       |~$40         |1    |Yes (builds full web app)    |
|Let's Go Further (Alex Edwards)|~$40        |3    |Yes (builds full JSON API)   |
|Learning Go, 1st ed (Bodner)  |Already owned|1-3  |Reference for fundamentals   |
|100 Go Mistakes (Harsanyi)    |Already owned|1-3  |Reference throughout         |
|Go by Example                 |Free         |1    |Yes (exercises)              |
|Exercism Go Track             |Free         |1    |Yes (mentored)              |
|Effective Go                  |Free         |1-2  |Reference                    |

**Architecture Resources (Free):**
- [Go Project Layout](https://github.com/golang-standards/project-layout) - Standard project structure
- [Kat Zien - How Do You Structure Your Go Apps](https://www.youtube.com/watch?v=oL6JBUk6tj0) - GopherCon talk
- [Three Dots Labs - Go with The Domain](https://threedots.tech/post/ddd-lite-in-go-introduction/) - DDD in Go series
- [Three Dots Labs - Wild Workouts](https://github.com/ThreeDotsLabs/wild-workouts-go-ddd-example) - Full DDD example app
- [ardanlabs/service](https://github.com/ardanlabs/service) - Production Go service template
- [Go Time Podcast - Architecture episodes](https://changelog.com/gotime) - Listen during commute

-----

## Phase 1: Go Web App — Learn by Doing (Weeks 9-12)

**Primary Resource:** Let's Go (Alex Edwards) — build a complete web application
**Reference:** Learning Go, 1st ed (Bodner) — look up fundamentals as needed

You learn Go by building a real web app from Chapter 1. When you hit a concept you don't understand (interfaces, goroutines, error handling), look it up in Bodner. This is faster than reading theory first.

### Week 9: Project Setup + Routing + Templates

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go Ch 1-3: Project structure, routing, HTML templates|
|Wed-Thu|4|Let's Go Ch 4: Configuration, error handling, logging|
|Fri|2|Supplement: Go by Example (types, functions, error handling)|
|Weekend|6|Extend: Add a new page/route to the app. Exercism (first 5 exercises)|

**Reference Bodner when you need:**
- Types, slices, maps (Chapters 1-3)
- Functions, closures, defer (Chapters 4-5)

### Week 10: Database + Middleware + Sessions

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go Ch 5-7: MySQL, middleware, RESTful routing|
|Wed-Thu|4|Let's Go Ch 8-9: Sessions, server-side validation|
|Fri|2|Supplement: Exercism (interfaces exercises)|
|Weekend|6|Extend: Add a new database model + CRUD to the app|

**Key Concepts (learned through the project):**
- Structs, methods, interfaces — Edwards teaches these through the app
- Pointer receivers vs value receivers
- Interface satisfaction is implicit
- Accept interfaces, return structs
- Dependency injection via struct fields

**Reference Bodner when you need:**
- Pointers, structs, methods (Chapters 6-7)
- Interfaces (Chapter 8)

### Week 11: HTTPS + Testing + Authentication

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go Ch 10-11: HTTPS, testing handlers/middleware|
|Wed-Thu|4|Let's Go Ch 12-13: Authentication, embedding, file serving|
|Fri|2|Practice: Write tests for your work code using patterns from the book|
|Weekend|6|Extend: Add authentication to a work project|

**Key Concepts (learned through the project):**
- Table-driven tests (Go's signature testing pattern)
- Test helpers, subtests, httptest package
- Mocking with interfaces
- HTTPS/TLS configuration

**100 Go Mistakes Reference (use throughout):**
- Mistake #2: Unnecessary nested code
- Mistake #45: Returning a nil receiver
- Mistake #78: Not using httptest

### Week 12: Concurrency + Polish + Deploy

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Bodner Ch 12-13: Goroutines, channels, select (focused study)|
|Wed-Thu|4|Concurrency patterns: fan-out/fan-in, pipeline, worker pool|
|Fri|2|Practice: Add concurrency to your Let's Go app (background tasks)|
|Weekend|6|Capstone: Deploy the app, write tests, clean up code|

**Key Concepts:**
- Goroutine lifecycle and leaks
- Buffered vs unbuffered channels
- Context for cancellation and timeouts
- sync.WaitGroup, errgroup
- Race detector: `go test -race`

**100 Go Mistakes Reference:**
- Mistake #61: Propagating inappropriate context
- Mistake #66: Using mutexes inaccurately
- Mistake #69: Forgetting about goroutine leaks

**Why concurrency last in Phase 1:**
Edwards doesn't cover concurrency deeply. Use Week 12 to read Bodner's concurrency chapters — by now you have enough Go context from 3 weeks of building to understand goroutines and channels properly.

-----

## Phase 2: Go Software Architecture (Weeks 13-16)

**Why Architecture Matters:**
You're not just writing functions — you're building systems. Clean architecture makes code testable, maintainable, and easy to change. Learning this in Go (your work language) means you can apply it immediately.

### Week 13: Clean Architecture + Project Structure

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Clean Architecture principles in Go|
|Wed-Thu|4|Hex Architecture / Ports & Adapters|
|Fri|2|Study: ardanlabs/service project structure|
|Weekend|6|Build: Restructure a personal project with clean architecture|

**Core Concepts:**
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

**Hands-On:**
1. Study [Kat Zien's GopherCon talk](https://www.youtube.com/watch?v=oL6JBUk6tj0) on structuring Go apps
2. Clone and study [ardanlabs/service](https://github.com/ardanlabs/service)
3. Restructure a personal Go project following clean architecture

**Claude Code Integration:**
```
REVIEW: "Review this Go project structure for clean architecture
violations. Check that dependencies point inward and domain
has no external imports."

REFACTOR: "Refactor this Go code to use hex architecture.
Extract interfaces for the repository layer and move them
to the domain package."
```

### Week 14: Domain-Driven Design in Go

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|DDD Lite in Go: entities, value objects, aggregates|
|Wed-Thu|4|Repository pattern, service layer in Go|
|Fri|2|Study: Three Dots Labs Wild Workouts example|
|Weekend|6|Build: Domain model for a real-world problem|

**Core Concepts:**
- **Entities:** Types with identity (User, Order)
  ```go
  type User struct {
      ID        uuid.UUID
      Email     string
      CreatedAt time.Time
  }
  ```
- **Value Objects:** Immutable types defined by their values
  ```go
  type Money struct {
      Amount   int64
      Currency string
  }
  ```
- **Repository Interface (domain package):**
  ```go
  type UserRepository interface {
      FindByID(ctx context.Context, id uuid.UUID) (*User, error)
      Save(ctx context.Context, user *User) error
      Delete(ctx context.Context, id uuid.UUID) error
  }
  ```
- **Service Layer:**
  ```go
  type UserService struct {
      repo UserRepository  // depends on interface, not implementation
      log  *slog.Logger
  }

  func NewUserService(repo UserRepository, log *slog.Logger) *UserService {
      return &UserService{repo: repo, log: log}
  }
  ```

**Resources:**
- [Three Dots Labs: DDD Lite in Go](https://threedots.tech/post/ddd-lite-in-go-introduction/)
- [Three Dots Labs: Wild Workouts](https://github.com/ThreeDotsLabs/wild-workouts-go-ddd-example)

### Week 15: Dependency Injection + API Design

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Dependency injection in Go (without frameworks)|
|Wed-Thu|4|RESTful API design patterns in Go|
|Fri|2|Middleware patterns and chains|
|Weekend|6|Build: REST API with clean architecture + DI|

**Core Concepts:**
- **Constructor Injection (Go's approach):**
  ```go
  // No DI framework needed — just constructors
  func main() {
      db := postgres.NewConnection(cfg.DatabaseURL)
      userRepo := postgres.NewUserRepository(db)
      userService := service.NewUserService(userRepo, logger)
      userHandler := handler.NewUserHandler(userService)

      mux := http.NewServeMux()
      mux.HandleFunc("GET /users/{id}", userHandler.GetByID)
      mux.HandleFunc("POST /users", userHandler.Create)
  }
  ```
- **Middleware Pattern:**
  ```go
  func LoggingMiddleware(next http.Handler) http.Handler {
      return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
          start := time.Now()
          next.ServeHTTP(w, r)
          slog.Info("request", "method", r.Method, "path", r.URL.Path,
              "duration", time.Since(start))
      })
  }
  ```
- **Context Propagation:** Pass context through layers for cancellation/timeouts
- **Error Handling in APIs:** Domain errors → HTTP status codes mapping

### Week 16: Testing Architecture + Integration Tests

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Testing strategies: unit, integration, end-to-end|
|Wed-Thu|4|Testcontainers for integration tests|
|Fri|2|Mocking with interfaces (no mocking frameworks needed)|
|Weekend|6|Build: Full test suite for Week 15 API project|

**Core Concepts:**
- **Test Pyramid in Go:**
  - Unit tests: Test domain logic (pure functions, no dependencies)
  - Integration tests: Test repository implementations with real DB
  - End-to-end: Test HTTP handlers with httptest
- **Interface-Based Mocking:**
  ```go
  // In tests — implement the interface directly
  type mockUserRepo struct {
      users map[uuid.UUID]*domain.User
  }

  func (m *mockUserRepo) FindByID(ctx context.Context, id uuid.UUID) (*domain.User, error) {
      user, ok := m.users[id]
      if !ok {
          return nil, domain.ErrUserNotFound
      }
      return user, nil
  }
  ```
- **Testcontainers for Real DB Tests:**
  ```go
  func TestUserRepository_Integration(t *testing.T) {
      ctx := context.Background()
      pgContainer, _ := postgres.RunContainer(ctx)
      defer pgContainer.Terminate(ctx)
      // ... run tests against real PostgreSQL
  }
  ```
- **httptest for Handler Tests:**
  ```go
  func TestGetUser(t *testing.T) {
      req := httptest.NewRequest("GET", "/users/123", nil)
      w := httptest.NewRecorder()
      handler.GetByID(w, req)
      assert.Equal(t, http.StatusOK, w.Code)
  }
  ```

-----

## Phase 3: Go JSON API + Production (Weeks 17-20)

**Primary Resource:** Let's Go Further (Alex Edwards) — build a complete JSON API
**Reference:** 100 Go Mistakes (Harsanyi) — use throughout

Let's Go Further picks up where Let's Go left off. You build a full JSON API from scratch with production-grade features. Apply the architecture patterns from Phase 2 as you build.

### Week 17: JSON API Foundations

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go Further: API setup, JSON encoding/decoding, routing|
|Wed-Thu|4|Database migrations, SQL queries, CRUD endpoints|
|Fri|2|Apply: Clean architecture structure from Phase 2 to the project|
|Weekend|6|Build: Extend the API with a new resource, apply DDD patterns|

### Week 18: Filtering, Sorting, Pagination + Validation

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go Further: Query string parsing, filtering, sorting|
|Wed-Thu|4|Input validation, error handling patterns|
|Fri|2|100 Go Mistakes: API-related chapters|
|Weekend|6|Build: Add full CRUD with validation to a work-related API|

### Week 19: Authentication, Permissions, Rate Limiting

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go Further: User registration, activation emails|
|Wed-Thu|4|Authentication tokens, permission-based authorization|
|Fri|2|Rate limiting, IP-based throttling, CORS|
|Weekend|6|Build: Add auth + permissions to your Phase 2 API project|

### Week 20: Production Deployment + Capstone

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go Further: Graceful shutdown, metrics, build versioning|
|Wed-Thu|4|Observability: structured logging (slog), health checks|
|Fri|2|Docker: multi-stage builds for Go apps|
|Weekend|6|Capstone: Production-ready Go API (GitHub portfolio piece)|

**Capstone Project: Production Go API**
By Week 20, you've built two complete Go projects (web app + JSON API). Polish the API as your capstone:
- Clean architecture / hex architecture (Phase 2 patterns)
- JSON API with authentication, permissions, rate limiting
- Database with migrations
- Comprehensive test suite (unit + integration)
- Docker multi-stage build
- Structured logging and health checks
- CLAUDE.md for the project

-----

## Go Code Review Checklist

**Reference:** 100 Go Mistakes and How to Avoid Them (Harsanyi) — use throughout

**Architecture:**
- [ ] Dependencies point inward (domain has no external imports)?
- [ ] Interfaces defined where they're consumed?
- [ ] Constructor injection for dependencies?
- [ ] Clear separation of domain, service, handler layers?

**Code Quality:**
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
- [ ] Memory safety (bounds checking)?

**Testing:**
- [ ] Table-driven tests?
- [ ] Interface-based mocking (no mock frameworks)?
- [ ] Integration tests with testcontainers?
- [ ] Race detector enabled (`-race` flag)?

-----

## Projects & Outputs

|Project                           |Week |Output                           |Share             |
|----------------------------------|-----|---------------------------------|------------------|
|Let's Go web app                  |9-11 |Complete web app (templates, DB, auth)|GitHub        |
|Concurrency deep dive             |12   |Add goroutines to Let's Go app   |GitHub            |
|Clean architecture Go project     |13   |Restructured project             |GitHub            |
|DDD domain model                  |14   |Domain-driven Go service         |GitHub            |
|REST API with clean architecture  |15-16|Full API with test suite          |GitHub            |
|Let's Go Further JSON API         |17-19|Production API (auth, rate limiting)|GitHub          |
|Production-ready Go API (capstone)|20   |Polished API portfolio piece      |GitHub + Blog post|

-----

## Claude Code Integration

Use Claude Code as your Go architecture companion throughout this track:

**Architecture Reviews:**
```
REVIEW: "Review this Go project for clean architecture violations.
Check dependency direction, interface placement, and layer separation."
```

**Pattern Application:**
```
REFACTOR: "Refactor this Go handler to use the repository pattern.
Extract the database logic into a separate repository implementation
that satisfies this interface: [paste interface]"
```

**Test Generation:**
```
TEST: "Generate table-driven tests for this Go function.
Include edge cases: nil inputs, empty slices, context cancellation."
```

**Code Quality:**
```
REVIEW: "Check this Go code against '100 Go Mistakes' patterns.
Focus on: error handling, concurrency, and interface design."
```

**CLAUDE.md for Each Project:**
Create a CLAUDE.md at the start of each project with build/test commands, architecture decisions, and code style preferences.

-----

## Checkpoint

Before moving to Track 9: Python Core, you should be able to:

- [ ] Write idiomatic Go with proper error handling
- [ ] Design systems using clean / hex architecture
- [ ] Apply DDD patterns (entities, value objects, repositories)
- [ ] Use dependency injection without frameworks
- [ ] Build REST APIs with middleware
- [ ] Write comprehensive tests (unit, integration, e2e)
- [ ] Use goroutines, channels, and sync primitives correctly
- [ ] Structure Go projects for production
- [ ] Review Go code for architecture and quality issues
- [ ] Create effective CLAUDE.md files for Go projects
