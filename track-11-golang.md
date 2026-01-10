# Track 11: Go/Golang

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
|1    |35-38|Go Fundamentals|
|2    |39-42|Web Development|
|3    |43-46|Security Tools |

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

## Phase 1: Go Fundamentals (Weeks 35-38)

**Primary Resource:** Learning Go, 2nd ed (Bodner)

|Week|Focus                            |
|----|---------------------------------|
|35  |Syntax, types, control flow      |
|36  |Functions, structs, interfaces   |
|37  |Concurrency: goroutines, channels|
|38  |Error handling, testing          |

**Supplement:** Go by Example + Exercism for practice

-----

## Phase 2: Web Development (Weeks 39-42)

**Primary Resource:** Let's Go (Alex Edwards) - ~$40

|Week|Focus                   |
|----|------------------------|
|39  |HTTP basics, routing    |
|40  |Templates, middleware   |
|41  |Database integration    |
|42  |Authentication, sessions|

**Project:** Simple web application

-----

## Phase 3: Security Tools (Weeks 43-46)

**Primary Resource:** Black Hat Go - Already owned

|Week|Focus                      |
|----|---------------------------|
|43  |TCP/UDP clients and servers|
|44  |HTTP clients, scraping     |
|45  |DNS, SMB, databases        |
|46  |Packet processing, plugins |

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
