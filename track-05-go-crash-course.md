# Track 5: Go Crash Course (For Work)

**Duration:** 1 week | **Total:** 18 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** HIGH (immediate work need)

**Weekly Schedule:**
- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why This Week?

Your company uses Go for development. Claude Code writes the Go, but you need to **understand Go well enough to**:
- Read and review what Claude Code produces
- Give Claude Code effective Go-specific direction
- Understand company Go codebases in code reviews
- Collaborate with Go developers using the right vocabulary
- **NOT become a Go expert** (that's Track 8: Software Architecture, Weeks 9-20)

-----

## Self-Assessment: Skip What You Already Know

You've been directing Claude Code to write Go at work. Don't waste time on material you can already recognize.

```
Before starting, can you:
- [ ] Read and understand Go code at work (with or without Claude Code help)?
- [ ] Identify what a Go function does when you see it?
- [ ] Understand goroutine/channel concepts (even if you can't write them)?
- [ ] Navigate your company's Go codebase structure?
- [ ] Review Go code in PRs and give meaningful feedback?

If you checked 4-5: Skip to Saturday (review company codebase deeply).
If you checked 2-3: Do the abbreviated version (skip Tour of Go, focus on gaps).
If you checked 0-1: Follow the full crash course below.
```

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

### For Track 8 (Go Foundations + Architecture, Weeks 9-20)
- Learning Go, 2nd ed (Bodner) - $50
- Let's Go (Alex Edwards) - $40
- Black Hat Go - Already owned!
- 100 Go Mistakes (Harsanyi) - $40

-----

## Deliverables

**By end of Week 6, you should have:**
- [ ] Completed Tour of Go (for reading comprehension)
- [ ] Reviewed Go by Example (key sections — understand, not memorize)
- [ ] Directed Claude Code to build a simple Go tool and reviewed the output
- [ ] Can read and understand company's Go code
- [ ] Can give Claude Code Go-specific direction at work
- [ ] Comfortable using Git from Track 4 for Go projects

**NOT expected:**
- You don't need to write Go from memory
- You don't need advanced concurrency patterns
- You don't need all Go idioms memorized
- Claude Code handles implementation — you handle direction and review

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

**Week 7: Docker Essentials (Track 6)**
- Container fundamentals for all future projects

**Week 8: LLM Security Primer (Track 7)**
- Read Wilson's book — security context for everything ahead

**Weeks 9-20: Software Architecture via Go (Track 8)**
- Deep architecture understanding: clean arch, DDD, testing
- Immediately applicable to your daily work

**Weeks 21-28: AI/ML Security (Track 10)**
- Your career goal — AI red teaming
- Architecture knowledge from Track 8 helps you understand AI systems

**Weeks 30-37: Python Core + TDD (Track 9)**
- Deepen Python understanding after using it in Track 10

**Weeks 38-43: Go Security Tools + AI Capstone (Track 11)**
- Combine everything into a unique portfolio piece

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
- Weeks 9-24 is when you'll become a Go expert

-----

## Cost

**This week: $0**
- All resources are free
- Git already learned in Track 4 (Week 5)
- Go books purchased for Track 8 (Week 9)

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
