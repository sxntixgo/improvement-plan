# Track 11: Go Security Tools + AI Security Capstone

**Duration:** 6 weeks | **Hours/week:** 18 | **Priority:** HIGH
**Goal:** Build offensive security tools in Go + combine Go + AI security into a unique capstone

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why This Track Last?

This track combines everything you've learned:

- **Track 8:** Software architecture, clean architecture, DDD, testing patterns (in Go)
- **Track 10:** AI/ML security — prompt injection, RAG poisoning, model attacks
- **Track 9:** Python understanding — you now know both ecosystems

Now you direct Claude Code to build Go security tools using your architecture knowledge and your AI security knowledge. The capstone produces an AI Red Team CLI tool in Go — a unique portfolio piece that almost no one else has.

**Your architect approach:** Read Black Hat Go for security tool concepts and architecture. Direct Claude Code to build the tools. Review output for architecture quality and security correctness.

-----

## Resources

|Resource                    |Cost         |Focus                  |
|----------------------------|-------------|-----------------------|
|Black Hat Go                |Already owned|Offensive security tools|
|100 Go Mistakes (Harsanyi)  |Already owned|Code review reference (not read cover-to-cover)|

**Black Hat Go (Steele et al.) — You're reading 6 of 14 chapters.** Skipping Go basics (already know Go), server-side, niche protocols, and topics outside AI red teaming.

|Chapter|Title                                             |What to Do                                              |
|-------|--------------------------------------------------|---------------------------------------------------------|
|1      |Go Fundamentals and Concepts                      |SKIP — You already know Go from Tracks 4 and 8           |
|2      |TCP and Go: Scanners and Proxies                  |⭐ READ (Week 38) — Core networking patterns for security tools|
|3      |HTTP Clients: Remote Interaction with Tools        |⭐ READ (Week 39) — HTTP client patterns for recon and API testing|
|4      |HTTP Servers: Routing and Middleware               |SKIP — You're building offensive tools, not web servers   |
|5      |Exploiting DNS: Recon and More                    |⭐ READ (Week 40) — DNS enumeration, subdomain discovery  |
|6      |SMB and NTLM: A Peek Down the Rabbit Hole         |SKIP — Niche Windows protocol, not relevant to AI red teaming|
|7      |Databases and Filesystems: Pilfering and Abusing   |SKIP — Traditional pentest technique, not AI security     |
|8      |Packet Processing: Living on the Wire              |⭐ READ (Week 41) — Raw packet capture, network analysis   |
|9      |Exploit Code: Writing and Porting                  |⭐ READ (Week 40) — Exploit writing patterns transfer to AI tool building|
|10     |Extendable Tools: Using Go Plugins and Lua         |⭐ READ (Week 41) — Plugin architecture for extensible scanner|
|11     |Cryptography: Implementing and Attacking           |SKIP — Crypto implementation details, not needed for AI tools|
|12     |Windows: System Interaction and Analysis           |SKIP — Platform-specific, not relevant                    |
|13     |Steganography: Hiding Data                         |SKIP — Niche technique, not relevant to AI red teaming    |
|14     |Command and Control: Building a RAT                |SKIP — Building RATs is not your career path              |

-----

## Phase Overview

|Week|Focus                      |Black Hat Go Chapters|Key Output                          |
|----|---------------------------|---------------------|------------------------------------|
|38  |TCP/UDP networking         |Ch 2                 |Concurrent port scanner             |
|39  |HTTP clients, scraping     |Ch 3                 |Web reconnaissance tool             |
|40  |DNS recon + exploit patterns|Ch 5, 9             |DNS enumeration tool                |
|41  |Packet processing, plugins |Ch 8, 10             |Custom security scanner (capstone)  |
|42  |Go-based LLM Security Tools|—                    |Concurrent prompt injection tester  |
|43  |**AI Red Team CLI Tool**   |—                    |**Complete AI security tool in Go** |

-----

## Phase 1: Go Security Tools (Weeks 38-41)

**Primary Resource:** Black Hat Go (Steele et al.) — Already owned (selected chapters, see above)

### Week 38: TCP/UDP Networking (Black Hat Go Ch 2)

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Ch 2: TCP client/server, port scanning concepts|
|Wed-Thu|4|Read Ch 2 cont'd: UDP, raw sockets patterns|
|Fri|2|Study: Fan-out/fan-in pattern for concurrent scanning|
|Weekend|6|Direct Claude Code: Build concurrent port scanner. Review architecture.|

**Architect Focus:**
- How does the fan-out/fan-in pattern apply to network scanning?
- What's the right concurrency limit (semaphore pattern)?
- How should errors propagate in concurrent code?

**Claude Code Direction:**
```
"Build a Go concurrent port scanner with:
- Fan-out/fan-in pattern using goroutines
- Semaphore to limit concurrent connections to 100
- Banner grabbing for service detection
- Context for timeout/cancellation
- Structured JSON output
- Clean architecture: domain/ for scan types, scanner/ for implementation"
```

### Week 39: HTTP Clients & Scraping (Black Hat Go Ch 3)

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Ch 3: HTTP client patterns, custom transports|
|Wed-Thu|4|Read Ch 3 cont'd: Web scraping, form submission|
|Fri|2|Study: Proxy awareness, TLS configuration|
|Weekend|6|Direct Claude Code: Build web reconnaissance tool. Review.|

### Week 40: DNS Recon + Exploit Patterns (Black Hat Go Ch 5, 9)

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Ch 5: DNS enumeration, subdomain discovery|
|Wed-Thu|4|Read Ch 9: Exploit code patterns — writing and porting exploits in Go|
|Fri|2|Study: How to combine tools into a recon pipeline|
|Weekend|6|Direct Claude Code: Build DNS enumeration tool. Review.|

### Week 41: Packet Processing & Plugins (Black Hat Go Ch 8, 10)

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Read Ch 8: Raw packet capture and injection|
|Wed-Thu|4|Read Ch 10: Plugin architecture with Go plugins and Lua|
|Fri|2|Design: Extensible scanner framework architecture|
|Weekend|6|Direct Claude Code: Build extensible security scanner. Review.|

**Security Scanner Architecture (direct Claude Code):**
```
"Build an extensible Go security scanner with:
- Plugin architecture for different scan types
- Concurrent scanning with goroutine worker pools
- Clean architecture (domain/, scanner/, plugin/, report/)
- Structured JSON output
- Docker multi-stage build
- CLAUDE.md for the project"
```

-----

## Phase 2: AI Security Capstone (Weeks 42-43)

**Why Now:**
You have deep Go architecture knowledge (Track 8) + AI/ML security expertise (Track 10) + Go security tool patterns (Phase 1). This is where you combine them to build something unique.

Most AI red teamers only use Python. Your Go skills give you a unique edge:
- Go's concurrency model is ideal for parallel prompt injection testing
- Go binaries are easy to distribute (no Python environment needed)
- Go's performance handles high-volume API testing efficiently
- Clean architecture makes the tool maintainable and extensible

### Week 42: Go-Based LLM Security Testing Tools

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Design + direct Claude Code: Concurrent prompt injection tester|
|Wed-Thu|4|Design: Go HTTP client for LLM API interaction (OpenAI, Anthropic APIs)|
|Fri|2|Study: gRPC security testing patterns|
|Weekend|6|Direct Claude Code: LLM API fuzzer with goroutines. Review.|

**Architect Design (before directing Claude Code):**
```
Concurrent Prompt Injection Tester:
- TestCase struct: Name, Prompt, Expected result
- Result struct: TestCase, Response, Status, Duration
- RunTests: fan-out/fan-in with configurable worker count
- Rate limiter to avoid API throttling
- JSON/CSV report generation
- YAML input for test case libraries
```

### Week 43: Capstone — Go AI Red Team CLI Tool

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Design complete AI red team CLI architecture|
|Wed-Thu|4|Direct Claude Code: Build the tool. Review architecture.|
|Fri|2|Direct Claude Code: Add reporting, configuration, Docker packaging|
|Weekend|6|Direct Claude Code: Tests, polish, documentation. Blog post.|

**Capstone: Go AI Red Team CLI Tool**

Combines Go mastery + AI security knowledge into a single portfolio piece:

**Features (specify to Claude Code):**
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
- net/http for API interaction
- goroutines + channels for concurrency
- CLAUDE.md for project configuration

**Architecture Review Checklist (final review):**
- [ ] Clean architecture / hex architecture
- [ ] Domain layer has no external dependencies
- [ ] Interfaces defined at consumer side
- [ ] Constructor injection throughout
- [ ] Comprehensive test suite
- [ ] Docker multi-stage build
- [ ] Structured logging and error handling
- [ ] No violations from 100 Go Mistakes
- [ ] CLAUDE.md complete

**Deliverable:**
- GitHub repo with full codebase
- Blog post: "Building an AI Red Team Tool in Go"
- Docker image published
- Unique portfolio piece (AI security + Go = rare combination)

-----

## Projects & Outputs

|Project                    |Week |Output                          |Share             |
|---------------------------|-----|--------------------------------|------------------|
|Concurrent port scanner    |38   |CLI tool with goroutines        |GitHub            |
|Web reconnaissance tool    |39   |HTTP recon tool                 |GitHub            |
|DNS enumeration tool       |40   |Concurrent DNS scanner          |GitHub            |
|Custom security scanner    |41   |Plugin-based scanner framework  |GitHub + Blog post|
|LLM API fuzzer             |42   |Concurrent prompt injection tester|GitHub           |
|**Go AI Red Team CLI Tool**|43   |**Complete AI security tool**   |**GitHub + Blog** |

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

## Claude Code Integration

**Security Tool Direction:**
```
"Build a Go concurrent port scanner using the fan-out/fan-in
pattern. Use a semaphore to limit concurrent connections to 100.
Include service detection via banner grabbing.
Follow clean architecture: domain/ for types, scanner/ for logic."
```

**AI Red Team Tool Direction:**
```
"Build a Go CLI tool for AI red teaming with:
- cobra CLI framework
- Concurrent LLM testing with configurable workers
- YAML-based attack pattern library
- JSON report generation with severity ratings
- Rate limiting per API endpoint
- Clean architecture with domain/service/handler layers"
```

**Architecture Review:**
```
"Review this Go security tool for:
- Clean architecture violations
- Proper error handling in concurrent code
- Resource cleanup (deferred Close calls)
- Race conditions
- Input validation"
```

-----

## Checkpoint

After completing this track, you should be able to:

- [ ] Direct Claude Code to build offensive security tools in Go
- [ ] Review Go security tools for architecture and security issues
- [ ] Describe Go concurrency patterns for parallel security scanning
- [ ] Design extensible security tool architectures
- [ ] Combine Go architecture + AI security knowledge into unique tools
- [ ] Produce a portfolio piece that differentiates you (Go + AI Red Team)

-----

## What's Next?

**Congratulations — you've completed the 44-week plan!**

You now have:
- **Software architecture expertise** to direct Claude Code effectively
- **AI/ML security skills** to red team AI systems
- **Go security tool portfolio** that differentiates you
- **Python understanding** to review and direct Python-based AI tools
- **A unique niche:** AI Red Teamer who builds tools in Go
