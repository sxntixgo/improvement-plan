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

## Week 5 Schedule

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

### Thursday-Friday (4 hours): Concurrency + Git Essentials

**Thursday (2 hours): Go Concurrency Basics**
- Goroutines (concurrent functions)
- Channels (communication between goroutines)
- Select statements
- **Why:** Go's concurrency is unique and widely used

**Resources:**
- Go by Example: Goroutines, Channels, Channel Buffering, Select
- Tour of Go: Concurrency section

**Friday (2 hours): Git Essentials for Work**

**You have "Pro Git" book - use it as reference**

**Focus on practical commands you'll use daily:**

**Basic Workflow (30 min):**
```bash
# Clone repository
git clone [url]

# Create feature branch
git checkout -b feature/my-change

# Stage and commit
git add .
git commit -m "Description"

# Push to remote
git push origin feature/my-change
```

**Branching (30 min):**
```bash
# See all branches
git branch -a

# Switch branches
git checkout main
git checkout develop

# Pull latest
git pull origin main

# Merge branches
git merge feature/my-change
```

**Essential Commands (30 min):**
```bash
# Status
git status
git diff

# History
git log --oneline
git log --graph

# Undo changes
git checkout -- file.go  # Discard local changes
git reset HEAD file.go   # Unstage
git revert [commit]      # Undo commit

# Stash (save work temporarily)
git stash
git stash pop
```

**Company-Specific (30 min):**
- Ask team: What's your Git workflow? (GitFlow? Feature branches?)
- How to create pull requests?
- Any Git hooks or pre-commit checks?
- Code review process?

**Pro Git Book Reference:**
- Chapter 2: Git Basics (read this)
- Chapter 3: Git Branching (skim)
- Chapters 1, 4-10: Skip for now, reference later

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

## Git Integration Notes

**You'll use Git throughout all tracks:**
- Week 5 (Go): Learn basics for work
- Week 7+ (Python): Git for personal projects
- Week 25+ (JavaScript): Git for portfolio
- Ongoing: Pro Git book as reference

**Pro Git Reading Plan:**
- **Week 5 (now):** Chapter 2 (Git Basics) - 1 hour
- **Week 7:** Chapter 3 (Branching) - 1 hour
- **Week 10:** Chapter 5 (Distributed Git) - 1 hour
- **Later:** Reference as needed

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

### Books You Own
- **Pro Git** - For Git fundamentals (Chapter 2 this week)

### For Later (Week 53-64: Go Deep Dive)
- Learning Go, 2nd ed (Bodner) - $50
- Let's Go (Alex Edwards) - $40
- Black Hat Go - Already owned!
- 100 Go Mistakes (Harsanyi) - $40

-----

## Deliverables

**By end of Week 5, you should have:**
- [ ] Completed Tour of Go
- [ ] Worked through Go by Example (key sections)
- [ ] Built a simple Go tool (HTTP server or CLI)
- [ ] **Made first contribution to company codebase** (even if tiny!)
- [ ] Comfortable with basic Git workflow
- [ ] Can read and understand company's Go code with Claude Code

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

## Week 5 Checklist

### Learning
- [ ] Complete Tour of Go (3 hrs)
- [ ] Work through Go by Example (3 hrs)
- [ ] Understand goroutines and channels (2 hrs)
- [ ] Learn Git basics from Pro Git Ch 2 (2 hrs)

### Practice
- [ ] Build simple Go tool (5 hrs)
- [ ] Read company's Go codebase (2 hrs)
- [ ] Make first contribution to company repo (3 hrs)

### Skills Acquired
- [ ] Can read Go code
- [ ] Can make small changes
- [ ] Understand basic concurrency
- [ ] Know Git workflow for work
- [ ] Can use Claude Code with Go effectively

-----

## What's Next?

**Week 6: LLM Security Primer**
- Read Wilson's book
- Build security context for Python learning
- Continue using Go at work (with Claude Code assistance)

**Weeks 7-16: Python Core**
- Focus on AI red teaming skills
- Keep using Go at work daily
- You'll be functional in Go by now

**Weeks 53-64: Go Deep Dive**
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

**For Git:**
1. Commit often, push frequently
2. Write clear commit messages: "Fix bug in user handler"
3. Create small PRs (easier to review)
4. Pull before you push (avoid conflicts)
5. When stuck: `git status` is your friend

**For Learning:**
- You're NOT trying to master Go this week
- Goal: Be productive at work while continuing AI red teaming path
- Claude Code is your safety net
- Week 53-64 is when you'll become a Go expert

-----

## Cost

**This week: $0**
- All resources are free
- Using books you already own (Pro Git)
- Go books purchased later (Week 53-64)

-----

## Success Metrics

**Minimum viable success:**
- ✅ Can read Go code at work
- ✅ Can make small changes/fixes
- ✅ Submitted at least one PR (even if tiny)
- ✅ Comfortable with Git basics
- ✅ Can use Claude Code with Go

**Stretch goals:**
- Built a useful Go tool
- Fixed a real bug at work
- Understand company's Go architecture
- Comfortable with goroutines/channels

You're now ready to be productive at work while continuing your AI red teaming journey!
