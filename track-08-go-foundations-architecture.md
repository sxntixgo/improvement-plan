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

|Phase|Weeks|Focus                    |Key Resource                       |
|-----|-----|-------------------------|-----------------------------------|
|1    |9-12 |Go Language Mastery      |Learning Go, 2nd ed (Bodner)       |
|2    |13-16|Go Software Architecture |Architecture resources + projects   |
|3    |17-20|Go Web Dev + Production  |Let's Go (Edwards) + 100 Go Mistakes|

-----

## Resources

|Resource                    |Cost         |Phase|Project-Driven?              |
|----------------------------|-------------|-----|-----------------------------|
|Learning Go, 2nd ed (Bodner)|~$50         |1    |Yes (structured intro)       |
|100 Go Mistakes (Harsanyi)  |~$40         |1-3  |Yes (reference throughout)   |
|Let's Go (Alex Edwards)     |~$40         |3    |Yes (builds full web app)    |
|Go by Example               |Free         |1    |Yes (exercises)              |
|Exercism Go Track           |Free         |1    |Yes (mentored)              |
|Effective Go                |Free         |1-2  |Reference                    |

**Architecture Resources (Free):**
- [Go Project Layout](https://github.com/golang-standards/project-layout) - Standard project structure
- [Kat Zien - How Do You Structure Your Go Apps](https://www.youtube.com/watch?v=oL6JBUk6tj0) - GopherCon talk
- [Three Dots Labs - Go with The Domain](https://threedots.tech/post/ddd-lite-in-go-introduction/) - DDD in Go series
- [Three Dots Labs - Wild Workouts](https://github.com/ThreeDotsLabs/wild-workouts-go-ddd-example) - Full DDD example app
- [ardanlabs/service](https://github.com/ardanlabs/service) - Production Go service template
- [Go Time Podcast - Architecture episodes](https://changelog.com/gotime) - Listen during commute

-----

## Phase 1: Go Language Mastery (Weeks 9-12)

**Primary Resource:** Learning Go, 2nd ed (Bodner)

### Week 9: Types, Declarations, Control Flow

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Chapters 1-3: Types, composite types, blocks/control flow|
|Wed-Thu|4|Chapters 4-5: Functions, closures, defer|
|Fri|2|Practice: Exercism Go Track (first 10 exercises)|
|Weekend|6|Build: Refactor a real work function using new patterns|

**CLAUDE.md Integration:**
```
REVIEW: "Review this Go function from my work codebase.
Flag any anti-patterns from '100 Go Mistakes' and suggest
idiomatic Go alternatives."
```

**Key Concepts:**
- Value types vs reference types (when does Go copy?)
- Slices: capacity, length, and when they share memory
- Maps: zero values, nil maps vs empty maps
- Multiple return values, named returns (and when to avoid them)

### Week 10: Structs, Interfaces, Generics

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Chapters 6-7: Pointers, structs, methods|
|Wed-Thu|4|Chapters 8-9: Interfaces, generics|
|Fri|2|Practice: Exercism (interfaces exercises)|
|Weekend|6|Build: Interface-driven refactor of work code|

**Key Concepts:**
- Pointer receivers vs value receivers (when to use each)
- Interface satisfaction is implicit — design implications
- Accept interfaces, return structs
- Small interfaces (io.Reader, io.Writer, fmt.Stringer)
- Generics: type constraints, when to use vs interfaces

**Architecture Preview:**
Interfaces are the foundation of Go architecture. Understanding them deeply now pays off in Phase 2.

### Week 11: Concurrency Deep Dive

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Chapters 12-13: Goroutines, channels, select|
|Wed-Thu|4|Sync package: WaitGroup, Mutex, Once, errgroup|
|Fri|2|Concurrency patterns: fan-out/fan-in, pipeline, worker pool|
|Weekend|6|Build: Concurrent file processor for work|

**Key Concepts:**
- Goroutine lifecycle and leaks
- Buffered vs unbuffered channels
- Channel direction (send-only, receive-only)
- Context for cancellation and timeouts
- sync.WaitGroup, sync.Mutex, sync.Once
- errgroup for concurrent error handling
- Race detector: `go test -race`

**100 Go Mistakes Reference (use throughout):**
- Mistake #61: Propagating inappropriate context
- Mistake #66: Using mutexes inaccurately
- Mistake #69: Forgetting about goroutine leaks

### Week 12: Error Handling, Testing, Modules

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Chapters 10-11: Errors, modules, packages|
|Wed-Thu|4|Chapter 15: Testing — table-driven, subtests, testify|
|Fri|2|Practice: Write tests for your work code|
|Weekend|6|Build: Well-tested CLI tool with proper error handling|

**Key Concepts:**
- Custom error types with `errors.Is` and `errors.As`
- Error wrapping: `fmt.Errorf("context: %w", err)`
- Sentinel errors vs error types vs opaque errors
- Table-driven tests (Go's signature testing pattern)
- Test helpers, subtests, test fixtures
- Benchmarks and fuzzing
- Module management and go.mod

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

## Phase 3: Go Web Development + Production (Weeks 17-20)

**Primary Resource:** Let's Go (Alex Edwards) - ~$40
**Reference:** 100 Go Mistakes (Harsanyi) — use throughout

### Week 17: HTTP Basics, Routing, Handlers

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go: Chapters 1-4 (Foundation setup)|
|Wed-Thu|4|Routing patterns, ServeMux, path parameters|
|Fri|2|Practice: Apply clean architecture to Let's Go project|
|Weekend|6|Build: HTTP server with proper project structure|

### Week 18: Templates, Middleware, Database

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go: Chapters 5-8 (Templates, middleware)|
|Wed-Thu|4|Database integration with repository pattern|
|Fri|2|Middleware: logging, recovery, CORS, auth|
|Weekend|6|Build: Web app with database, applying Week 14 DDD patterns|

### Week 19: Authentication, Sessions, Security

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Let's Go: Chapters 9-12 (Auth, sessions)|
|Wed-Thu|4|Security: CSRF, XSS prevention, secure headers|
|Fri|2|100 Go Mistakes: Security-related chapters|
|Weekend|6|Build: Secure web app with auth|

### Week 20: Production Readiness + Capstone

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Production: graceful shutdown, health checks, config management|
|Wed-Thu|4|Observability: structured logging (slog), metrics, tracing|
|Fri|2|Docker: multi-stage builds for Go apps|
|Weekend|6|Capstone: Production-ready Go service (GitHub portfolio piece)|

**Capstone Project: Production Go Service**
Build a production-ready Go service that demonstrates:
- Clean architecture / hex architecture
- Domain-driven design patterns
- RESTful API with middleware
- Database integration with repository pattern
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
|Concurrent file processor         |11   |CLI tool with goroutines         |GitHub            |
|Well-tested CLI tool              |12   |CLI with proper error handling   |GitHub            |
|Clean architecture Go project     |13   |Restructured project             |GitHub            |
|DDD domain model                  |14   |Domain-driven Go service         |GitHub            |
|REST API with clean architecture  |15-16|Full API with test suite          |GitHub            |
|Production-ready Go service       |17-20|Capstone: full web service        |GitHub + Blog post|

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
