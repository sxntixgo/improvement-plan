# Track 4: Go Crash Course (For Work)

**Duration:** 1 week | **Total:** 18 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** HIGH (immediate work need)

**Weekly Schedule:**
- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why This Week?

Your company uses Go for development. This crash course gets you **functional at work** while you continue your AI red teaming path.

**Goal:** Minimum viable Go knowledge to:
- Read and understand Go codebases at work
- Make small changes and fixes
- Use Claude Code effectively with Go
- Collaborate with Go developers
- **NOT become a Go expert** (that's Week 53-64)

-----

## Week 6 Schedule

### Monday-Wednesday (8 hours): Go Fundamentals

**Monday (3 hours): Tour of Go + Setup**
- Complete [Tour of Go](https://go.dev/tour/) (official interactive tutorial)
- Install Go on your machine
- Set up VS Code with Go extension
- Write "Hello World" and run it

**Tuesday (3 hours): Go by Example**
- Work through [Go by Example](https://gobyexample.com/)
- Focus on these sections:
  - Variables, Constants, For loops
  - If/Else, Switch
  - Arrays, Slices, Maps
  - Functions, Multiple Return Values
  - Pointers
  - Structs, Methods, Interfaces
  - Errors

**Wednesday (2 hours): Read Your Company's Go Code**
- Clone company Go repository
- Use Claude Code to understand it:
  ```
  EXPLAIN: "Explain what this Go package does:
  [paste company code]
  Include: main functions, data structures, flow"
  ```
- Identify patterns used at work
- Ask senior devs for "good example files" to study

### Thursday-Friday (4 hours): Concurrency Basics

**Thursday (2 hours): Go Concurrency Basics**
- Goroutines (concurrent functions)
- Channels (communication between goroutines)
- Select statements
- **Why:** Go's concurrency is unique and widely used

**Resources:**
- Go by Example: Goroutines, Channels, Channel Buffering, Select
- Tour of Go: Concurrency section

**Friday (2 hours): Advanced Go Patterns**
- Error handling patterns
- Interface design
- Common Go idioms
- Read company Go code with Claude Code

**Resources:**
- [Effective Go](https://go.dev/doc/effective_go)
- Company codebase examples
- Ask senior devs for "good files to study"

### Weekend (10 hours): Practice + Company Projects

**Saturday (5 hours): Build a Simple Go Tool**

**Option 1: HTTP Server (Web focus)**
```go
// Simple REST API
package main

import (
    "encoding/json"
    "net/http"
)

type Response struct {
    Message string `json:"message"`
}

func handler(w http.ResponseWriter, r *http.Request) {
    response := Response{Message: "Hello from Go!"}
    json.NewEncoder(w).Encode(response)
}

func main() {
    http.HandleFunc("/", handler)
    http.ListenAndServe(":8080", nil)
}
```

**Option 2: CLI Tool (Systems focus)**
- File processor
- Log parser
- Configuration validator

**Use Claude Code to help:**
```
CREATE: "Build a simple Go HTTP server that:
- Has endpoints: GET /health, GET /api/users
- Returns JSON
- Includes error handling"
```

**Sunday (5 hours): Work on Company Codebase**

**Goal:** Make your FIRST contribution at work

**Steps:**
1. **Find a good first issue** (2 hours)
   - Ask team lead for "good first issue" or "beginner-friendly task"
   - Or: Fix a typo, update documentation, add a test
   - Small PR to learn the workflow

2. **Make the change** (2 hours)
   - Create feature branch
   - Make changes
   - Test locally
   - Use Claude Code if stuck

3. **Submit PR** (1 hour)
   - Commit with clear message
   - Push to remote
   - Create pull request
   - Address code review feedback

**If no task available:** Read company's Go style guide and contribution docs

-----

## Key Go Concepts (Crash Course Level)

**Syntax:**
- `:=` for variable declaration and assignment
- Multiple return values (esp. `result, err`)
- Exported vs unexported (capitalization matters)
- Package system

**Data Structures:**
- Slices (dynamic arrays): `[]int{1, 2, 3}`
- Maps: `map[string]int{"key": value}`
- Structs: Custom types

**Concurrency:**
- Goroutines: `go functionName()`
- Channels: `ch := make(chan int)`
- Select: Like switch but for channels

**Error Handling:**
```go
result, err := doSomething()
if err != nil {
    return err  // or log.Fatal(err)
}
```

**Common Patterns:**
- `if err != nil` everywhere
- Defer for cleanup: `defer file.Close()`
- Interfaces are implicit (no "implements" keyword)

-----

## Resources

### Free & Essential
- [Tour of Go](https://go.dev/tour/) - Interactive tutorial
- [Go by Example](https://gobyexample.com/) - Practical examples
- [Go Documentation](https://go.dev/doc/) - Official docs
- [Effective Go](https://go.dev/doc/effective_go) - Best practices

### For Later (Weeks 34-45: Go Deep Dive)
- Learning Go, 2nd ed (Bodner) - $50
- Let's Go (Alex Edwards) - $40
- Black Hat Go - Already owned!
- 100 Go Mistakes (Harsanyi) - $40

-----

## Deliverables

**By end of Week 6, you should have:**
- [ ] Completed Tour of Go
- [ ] Worked through Go by Example (key sections)
- [ ] Built a simple Go tool (HTTP server or CLI)
- [ ] **Made first contribution to company codebase** (even if tiny!)
- [ ] Can read and understand company's Go code with Claude Code
- [ ] Comfortable using Git from Track 4 for Go projects

**NOT expected:**
- ❌ Go expert
- ❌ Advanced concurrency patterns
- ❌ All Go idioms
- ❌ Deep understanding of Go internals

-----

## Using Claude Code with Go at Work

After this week, use Claude Code as your Go assistant:

**Daily Go Tasks:**
```
EXPLAIN: "Explain what this Go function does:
[paste code from work]"

REVIEW: "Review this Go code for:
- Idiomatic Go patterns
- Error handling
- Potential bugs"

FIX: "This Go code has a bug where [describe].
Debug and suggest a fix."

CREATE: "Write a Go function that [describe requirement]
Follow our company's style guide"
```

**Learning on the Job:**
- When stuck: Ask Claude Code
- When reviewing PRs: Ask Claude Code to explain
- When writing: Ask Claude Code to review before submitting

-----

## Week 6 Checklist

### Learning
- [ ] Complete Tour of Go (3 hrs)
- [ ] Work through Go by Example (3 hrs)
- [ ] Understand goroutines and channels (2 hrs)
- [ ] Learn Go patterns and idioms (2 hrs)

### Practice
- [ ] Build simple Go tool (5 hrs)
- [ ] Read company's Go codebase (2 hrs)
- [ ] Make first contribution to company repo (3 hrs)

### Skills Acquired
- [ ] Can read Go code
- [ ] Can make small changes
- [ ] Understand basic concurrency
- [ ] Know company's Git workflow (from Track 4)
- [ ] Can use Claude Code with Go effectively

-----

## What's Next?

**Week 8: LLM Security Primer**
- Read Wilson's book
- Build security context for Python learning
- Continue using Go at work (with Claude Code assistance)

**Weeks 9-18: Python Core**
- Focus on AI red teaming skills
- Keep using Go at work daily
- You'll be functional in Go by now

**Weeks 35-46: Go Deep Dive**
- Come back for advanced Go
- Security tool building (Black Hat Go)
- Become Go expert

-----

## Pro Tips

**For Go at Work:**
1. Keep Go by Example open in a tab - quick reference
2. Use Claude Code liberally - you're learning on the job
3. Ask senior devs to review your code - learn company patterns
4. Read other people's PRs - see how they write Go
5. Don't try to learn everything - focus on what you need today

**For Git at Work:**
1. You learned Git in Track 4 (Week 5) - apply those skills here
2. Use company's Git workflow (GitFlow, feature branches, etc.)
3. Write clear commit messages: "Fix bug in user handler"
4. Create small PRs (easier to review)
5. Reference Pro Git book when you encounter advanced scenarios

**For Learning:**
- You're NOT trying to master Go this week
- Goal: Be productive at work while continuing AI red teaming path
- Claude Code is your safety net
- Weeks 34-45 is when you'll become a Go expert

-----

## Cost

**This week: $0**
- All resources are free
- Git already learned in Track 4 (Week 5)
- Go books purchased later (Weeks 34-45)

-----

## Success Metrics

**Minimum viable success:**
- ✅ Can read Go code at work
- ✅ Can make small changes/fixes
- ✅ Submitted at least one PR (even if tiny)
- ✅ Using Git effectively (from Track 4)
- ✅ Can use Claude Code with Go

**Stretch goals:**
- Built a useful Go tool
- Fixed a real bug at work
- Understand company's Go architecture
- Comfortable with goroutines/channels

You're now ready to be productive at work while continuing your AI red teaming journey!
