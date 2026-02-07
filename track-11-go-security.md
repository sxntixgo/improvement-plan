# Track 11: Go Security Tools + Go for AI Security

**Duration:** 6 weeks | **Hours/week:** 18 | **Priority:** HIGH
**Goal:** Build security tools in Go and apply Go to AI red teaming

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why Now?

You have deep Go foundations from Track 8 (Weeks 9-20) and AI/ML security knowledge from Track 10 (Weeks 29-36). Now you combine them:

- **Black Hat Go** teaches offensive security tool building in Go
- **Go for AI Security** applies Go's concurrency model to LLM security testing
- You've been writing Go at work for 30+ weeks — this track pushes you into expert territory
- Go's goroutines are perfect for concurrent security scanning

-----

## Phase Overview

|Phase|Weeks|Focus                    |Key Resource                 |
|-----|-----|-------------------------|-----------------------------|
|1    |37-40|Security Tools (Black Hat Go)|Black Hat Go - Already owned|
|2    |41-42|Go for AI Security       |Hands-on projects            |

-----

## Resources

|Resource                    |Cost         |Focus                  |
|----------------------------|-------------|-----------------------|
|Black Hat Go                |Already owned|Offensive security tools|
|100 Go Mistakes (Harsanyi)  |Already bought (Track 8)|Reference throughout|

-----

## Phase 1: Security Tools with Black Hat Go (Weeks 37-40)

**Primary Resource:** Black Hat Go (Steele et al.) - Already owned

### Week 37: TCP/UDP Networking

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|TCP client/server, port scanning|
|Wed-Thu|4|UDP, raw sockets|
|Fri|2|Practice: Build concurrent port scanner with goroutines|
|Weekend|6|Project: Multi-threaded port scanner with service detection|

**Key Concepts:**
- net.Dial, net.Listen for TCP connections
- Concurrent scanning with goroutines + semaphore pattern
- Banner grabbing and service detection
- Timeout handling with context

### Week 38: HTTP Clients & Scraping

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|HTTP client patterns, custom transports|
|Wed-Thu|4|Web scraping, form submission|
|Fri|2|Proxy awareness, TLS configuration|
|Weekend|6|Project: Web reconnaissance tool|

### Week 39: DNS, SMB, and Databases

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|DNS enumeration, subdomain discovery|
|Wed-Thu|4|SMB client, database interaction|
|Fri|2|Practice: Combine tools into recon pipeline|
|Weekend|6|Project: DNS enumeration tool with concurrent lookups|

### Week 40: Packet Processing & Plugins

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Raw packet capture and injection|
|Wed-Thu|4|Plugin architecture with Go plugins|
|Fri|2|Build extensible scanner framework|
|Weekend|6|Project: Custom security scanner with plugin support|

-----

## Phase 2: Go for AI Security (Weeks 41-42)

**Why This Phase:**
No one else is building AI security tools in Go. Most AI red teamers only use Python. Your Go skills give you a unique edge:
- Go's concurrency model is ideal for parallel prompt injection testing
- Go binaries are easy to distribute (no Python environment needed)
- Go's performance handles high-volume API testing efficiently
- gRPC security testing is natural in Go (gRPC is a Go-native technology)

### Week 41: Go-Based LLM Security Testing Tools

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Build concurrent prompt injection tester|
|Wed-Thu|4|Go HTTP client for LLM API interaction (OpenAI, Anthropic APIs)|
|Fri|2|gRPC security testing patterns|
|Weekend|6|Project: LLM API fuzzer with goroutines|

**Concurrent Prompt Injection Tester:**
```go
type TestCase struct {
    Name     string
    Prompt   string
    Expected string // "blocked", "leaked", "safe"
}

type Result struct {
    TestCase TestCase
    Response string
    Status   string // "pass", "fail", "error"
    Duration time.Duration
}

func RunTests(ctx context.Context, cases []TestCase, workers int) []Result {
    // Fan-out: distribute test cases to worker goroutines
    // Fan-in: collect results through channel
    // Context: cancel all workers on timeout
}
```

**Key Features:**
- Fan-out/fan-in pattern for parallel testing
- Rate limiting to avoid API throttling
- Structured logging of all attempts
- JSON/CSV report generation
- Configurable test case library (YAML/JSON input)

### Week 42: Capstone — Go AI Red Team Tool

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Design and build complete AI red team CLI tool|
|Wed-Thu|4|Add reporting, configuration, Docker packaging|
|Fri|2|Write comprehensive tests|
|Weekend|6|Polish, document, blog post|

**Capstone: Go AI Red Team CLI Tool**

Combines everything from this track into a single portfolio piece:

**Features:**
- Concurrent LLM endpoint testing (goroutines)
- Multiple attack pattern libraries (prompt injection, jailbreak, exfiltration)
- Configurable via YAML
- Structured JSON reports with severity ratings
- Rate limiting and retry logic
- Docker multi-stage build
- Clean architecture (from Track 8)

**Tech Stack:**
- cobra for CLI framework
- slog for structured logging
- testify for testing
- net/http for API interaction
- goroutines + channels for concurrency
- CLAUDE.md for project configuration

**Deliverable:**
- GitHub repo with full codebase
- Blog post: "Building an AI Red Team Tool in Go"
- Docker image published
- Unique portfolio piece (AI security + Go = rare combination)

-----

## Projects & Outputs

|Project                    |Week |Output                          |Share             |
|---------------------------|-----|--------------------------------|------------------|
|Concurrent port scanner    |37   |CLI tool with goroutines        |GitHub            |
|Web reconnaissance tool    |38   |HTTP recon tool                 |GitHub            |
|DNS enumeration tool       |39   |Concurrent DNS scanner          |GitHub            |
|Custom security scanner    |40   |Plugin-based scanner framework  |GitHub + Blog post|
|LLM API fuzzer             |41   |Concurrent prompt injection tester|GitHub           |
|Go AI Red Team CLI Tool    |42   |Complete AI security tool       |GitHub + Blog post|

-----

## Claude Code Integration

**Security Tool Development:**
```
CREATE: "Build a Go concurrent port scanner using the fan-out/fan-in
pattern. Use a semaphore to limit concurrent connections to 100.
Include service detection via banner grabbing."

REVIEW: "Review this Go security tool for:
- Proper error handling in concurrent code
- Resource cleanup (deferred Close calls)
- Race conditions
- Input validation"
```

**AI Security Tool Development:**
```
CREATE: "Build a Go CLI tool that tests LLM API endpoints for prompt
injection vulnerabilities. Use goroutines for parallel testing.
Accept test cases from a YAML config file."

TEST: "Generate table-driven tests for this LLM testing function.
Include: timeout cases, rate limit cases, malformed response cases."
```

-----

## Go Code Review Checklist (Security Focus)

**Reference:** 100 Go Mistakes and How to Avoid Them (Harsanyi)

- [ ] Error handling (not ignoring errors)?
- [ ] Race conditions (proper mutex / channel usage)?
- [ ] Resource leaks (defer for cleanup)?
- [ ] Goroutine leaks (context cancellation)?
- [ ] Input validation on all external data?
- [ ] Crypto: using crypto/rand not math/rand?
- [ ] SQL injection (parameterized queries)?
- [ ] Command injection (proper escaping)?
- [ ] TLS verification not disabled?
- [ ] Rate limiting on API calls?

-----

## Checkpoint

After completing this track, you should be able to:

- [ ] Build offensive security tools in Go (Black Hat Go patterns)
- [ ] Use Go's concurrency model for parallel security scanning
- [ ] Build Go tools that test LLM APIs for vulnerabilities
- [ ] Create distributable security tool binaries
- [ ] Apply clean architecture to security tool projects
- [ ] Review Go security code for common vulnerabilities
- [ ] Combine Go expertise with AI red teaming knowledge (unique skill)
