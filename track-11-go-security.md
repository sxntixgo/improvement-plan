# Track 11: Go Security Tools (Black Hat Go)

**Duration:** 4 weeks | **Hours/week:** 18 | **Priority:** HIGH
**Goal:** Build offensive security tools in Go

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why Right After Track 8?

You just spent 12 weeks mastering Go foundations and software architecture. Your Go skills are at their peak. This is the ideal time to apply them to security:

- **Black Hat Go** teaches offensive security tool building in Go
- Go's goroutines are perfect for concurrent security scanning
- Clean architecture patterns from Track 8 apply directly to tool design
- You'll produce 4 portfolio-ready security tools in 4 weeks
- No context-switching — 16+ continuous weeks of Go mastery (Tracks 8 + 11)

**Note:** Go for AI Security (LLM testing tools in Go) comes later as a capstone in Track 10, after you've learned AI/ML security concepts.

-----

## Resources

|Resource                    |Cost         |Focus                  |
|----------------------------|-------------|-----------------------|
|Black Hat Go                |Already owned|Offensive security tools|
|100 Go Mistakes (Harsanyi)  |Already bought (Track 8)|Reference throughout|

-----

## Phase Overview

|Week|Focus                      |Key Output                          |
|----|---------------------------|------------------------------------|
|21  |TCP/UDP clients and servers|Concurrent port scanner             |
|22  |HTTP clients, scraping     |Web reconnaissance tool             |
|23  |DNS, SMB, databases        |DNS enumeration tool                |
|24  |Packet processing, plugins |Custom security scanner (capstone)  |

-----

**Primary Resource:** Black Hat Go (Steele et al.) - Already owned

### Week 21: TCP/UDP Networking

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

### Week 22: HTTP Clients & Scraping

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|HTTP client patterns, custom transports|
|Wed-Thu|4|Web scraping, form submission|
|Fri|2|Proxy awareness, TLS configuration|
|Weekend|6|Project: Web reconnaissance tool|

### Week 23: DNS, SMB, and Databases

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|DNS enumeration, subdomain discovery|
|Wed-Thu|4|SMB client, database interaction|
|Fri|2|Practice: Combine tools into recon pipeline|
|Weekend|6|Project: DNS enumeration tool with concurrent lookups|

### Week 24: Packet Processing & Plugins (Capstone)

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Raw packet capture and injection|
|Wed-Thu|4|Plugin architecture with Go plugins|
|Fri|2|Build extensible scanner framework|
|Weekend|6|Capstone: Custom security scanner with plugin support|

**Capstone Project:**
Build an extensible Go security scanner that combines techniques from Weeks 21-23:
- Plugin architecture for different scan types
- Concurrent scanning with goroutine worker pools
- Clean architecture (from Track 8)
- Structured JSON output
- Docker multi-stage build
- CLAUDE.md for the project

-----

## Projects & Outputs

|Project                    |Week |Output                          |Share             |
|---------------------------|-----|--------------------------------|------------------|
|Concurrent port scanner    |21   |CLI tool with goroutines        |GitHub            |
|Web reconnaissance tool    |22   |HTTP recon tool                 |GitHub            |
|DNS enumeration tool       |23   |Concurrent DNS scanner          |GitHub            |
|Custom security scanner    |24   |Plugin-based scanner framework  |GitHub + Blog post|

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

-----

## What's Next?

After this track, you'll learn Python (Track 9) and AI/ML Security (Track 10). At the end of Track 10, you'll come back to Go to build **AI security tools in Go** — combining your Go mastery with your new AI red teaming skills. That capstone produces a unique portfolio piece: an LLM security testing CLI tool built with goroutines.

-----

## Checkpoint

After completing this track, you should be able to:

- [ ] Build offensive security tools in Go (Black Hat Go patterns)
- [ ] Use Go's concurrency model for parallel security scanning
- [ ] Build TCP/UDP, HTTP, and DNS security tools
- [ ] Create distributable security tool binaries
- [ ] Apply clean architecture to security tool projects
- [ ] Review Go security code for common vulnerabilities
