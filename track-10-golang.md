# Track 8: Go/Golang

**Duration:** 12 weeks | **Hours/week:** 18 | **Priority:** LOWER
**Goal:** Build security tools

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Phase Overview

|Phase|Weeks|Focus          |
|-----|-----|---------------|
|1    |51-54|Go Fundamentals|
|2    |55-58|Web Development|
|3    |59-62|Security Tools |

-----

## Resources (Project-Driven)

|Resource                    |Cost         |Project-Driven?         |
|----------------------------|-------------|------------------------|
|Learning Go, 2nd ed (Bodner)|~$50         |✅ Yes (structured intro)|
|Black Hat Go                |Already owned|✅ Yes (security tools)  |
|100 Go Mistakes (Harsanyi)  |~$40         |✅ Yes (anti-patterns)   |
|Let's Go (Alex Edwards)     |~$40         |✅ Yes (web app)         |
|Go by Example               |Free         |✅ Yes (exercises)       |
|Exercism Go Track           |Free         |✅ Yes (mentored)        |

**Recommended reading order:**

1. Learning Go (fundamentals)
1. Let's Go (web dev)
1. Black Hat Go (security tools)
1. 100 Go Mistakes (code review, reference throughout)

-----

## Phase 1: Go Fundamentals (Weeks 51-54)

**Primary Resource:** Learning Go, 2nd ed (Bodner)

|Week|Focus                            |
|----|---------------------------------|
|51  |Syntax, types, control flow      |
|52  |Functions, structs, interfaces   |
|53  |Concurrency: goroutines, channels|
|54  |Error handling, testing          |

**Supplement:** Go by Example + Exercism for practice

-----

## Phase 2: Web Development (Weeks 55-58)

**Primary Resource:** Let's Go (Alex Edwards) - ~$40

|Week|Focus                   |
|----|------------------------|
|55  |HTTP basics, routing    |
|56  |Templates, middleware   |
|57  |Database integration    |
|58  |Authentication, sessions|

**Project:** Simple web application

-----

## Phase 3: Security Tools (Weeks 59-62)

**Primary Resource:** Black Hat Go - Already owned

|Week|Focus                      |
|----|---------------------------|
|59  |TCP/UDP clients and servers|
|60  |HTTP clients, scraping     |
|61  |DNS, SMB, databases        |
|62  |Packet processing, plugins |

-----

## Projects & Outputs

|Project                |Output   |Share             |
|-----------------------|---------|------------------|
|Port scanner           |CLI tool |GitHub            |
|DNS enumeration tool   |CLI tool |GitHub            |
|Custom security scanner|Full tool|GitHub + Blog post|

-----

## Go Code Review Checklist

**Reference:** 100 Go Mistakes and How to Avoid Them (Harsanyi) — use throughout

- [ ] Error handling (not ignoring errors)?
- [ ] Race conditions (proper mutex usage)?
- [ ] Resource leaks (defer for cleanup)?
- [ ] Input validation?
- [ ] Crypto: using crypto/rand not math/rand?
- [ ] SQL injection (parameterized queries)?
- [ ] Command injection (proper escaping)?
- [ ] Memory safety (bounds checking)?

-----

## Checkpoint

You should be able to build security tools in Go and conduct Go code reviews.
