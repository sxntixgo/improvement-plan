# Improvement Areas Review - Golang & Claude Code Focus

**Date:** February 7, 2026
**Focus:** Areas of improvement considering daily Go usage at work and existing Claude Code tooling experience
**Status:** IMPLEMENTED - All recommendations applied to the plan

---

## Summary

The plan is well-structured (9/10 from previous review), but it has significant blind spots around **two things you already do every day**: write Go and build with Claude Code. The plan treats both as things to "learn later" rather than strengths to build on. Below are 10 improvement areas, ranked by impact.

---

## 1. Go is Massively Underweighted for a Daily Work Language

**The Problem:**
Go gets a 1-week crash course (Week 6) and a 12-week deep dive starting at **Week 35**. That's a **29-week gap** where you're writing Go at work every day without structured learning to back it up. Meanwhile, JavaScript/TypeScript gets 20 weeks despite being less relevant to both your job and your AI red teaming goal.

**Current allocation:**
| Language | Weeks | Your Daily Usage |
|----------|-------|------------------|
| Python | 26 weeks (Tracks 8, 9, 10) | None yet |
| JavaScript/TypeScript | 20 weeks (Track 12) | None |
| **Go** | **13 weeks (Tracks 5, 11)** | **Every day at work** |

**Recommendation:**
- Move the Go Deep Dive (Track 11) earlier — start at **Week 27** instead of Week 35. You'll have Python Core + AI/ML Security done, and your Go crash course skills will be fresher (21-week gap vs 29-week gap).
- Reduce JavaScript/TypeScript from 20 weeks to **12-14 weeks** by compressing Phases 1-2 (you'll learn JS faster after mastering Python and Go). Use the freed weeks to deepen Go + AI security integration.
- Change Track 11 priority from "LOWER" to **"HIGH"** — it's your work language.

**Revised timeline option:**
```
Weeks 9-18:   Python Core (10 weeks) — unchanged
Weeks 19-26:  AI/ML Security (8 weeks) — unchanged
Weeks 27-38:  Go Deep Dive (12 weeks) — moved up from Week 35
Weeks 39-40:  Break + portfolio consolidation
Weeks 41-54:  JavaScript/TypeScript (14 weeks) — compressed from 20
Weeks 55-56:  Final portfolio + job prep
```

---

## 2. Claude Code Track is Outdated Given Your Experience

**The Problem:**
Track 3 is a 1-week "learn Claude Code" course based on prompt patterns you already documented. You've been **building tools** with Claude Code — you're well past the "4-Part Formula" and "7 Core Patterns" stage. This week would be largely wasted.

**What the track covers:**
- 4-Part Formula (Intent, Context, Constraints, Success criteria)
- 7 Core Patterns (CREATE, FIX, REFACTOR, REVIEW, EXPLAIN, TEST, OPTIMIZE)
- Model cascading (Haiku, Sonnet, Opus)
- Cost-aware prompting

**What it misses entirely:**
- **CLAUDE.md project configuration** — per-repo instructions that make Claude Code dramatically more effective
- **MCP servers** — connecting Claude Code to external tools (databases, APIs, Obsidian)
- **Hooks** — automating pre/post actions on tool calls
- **Extended thinking** — leveraging deep reasoning for complex problems
- **Sub-agents** — parallel task execution for complex workflows
- **Custom slash commands** — building reusable workflows
- **Claude Code SDK** — building custom AI agents (directly relevant to AI red teaming)
- **Multi-file editing workflows** — scaffolding entire projects
- **Go-specific Claude Code patterns** — test generation, interface extraction, error handling patterns

**Recommendation:**
Replace the current Track 3 content with an **advanced Claude Code track** that builds on your existing knowledge:

| Day | Focus | Output |
|-----|-------|--------|
| Mon-Tue | CLAUDE.md mastery: build project configs for your Go work repos | Working CLAUDE.md files |
| Wed | MCP servers: set up Obsidian MCP + database MCP for your workflow | Connected knowledge system |
| Thu | Hooks + custom slash commands: automate your Go development workflow | Custom Go dev automation |
| Fri | Claude Code SDK: build a simple AI agent | Working agent prototype |
| Weekend | Apply everything to a real Go project at work | Productivity improvement |

---

## 3. No Go + AI Security Integration

**The Problem:**
All security tooling in the plan is Python-only. But Go is excellent for security tools (you own Black Hat Go!), and it's your work language. The plan treats Go security (Track 11, Phase 3) and AI security (Track 9) as completely separate tracks with no overlap.

**Missing intersection:**
- Building LLM security testing tools in Go (your daily language)
- Go-based API security scanners that test AI endpoints
- gRPC security testing (common in Go microservice architectures)
- Go tools that interact with LLM APIs for automated red teaming
- Using Go's concurrency model for parallel prompt injection testing (goroutines are perfect for this)

**Recommendation:**
Add a **"Go for AI Security"** mini-phase (2 weeks) at the end of the Go Deep Dive:

| Week | Focus | Output |
|------|-------|--------|
| Week 37-38 (new) | Build Go-based LLM security tools | CLI tool that runs prompt injection tests concurrently using goroutines |

This serves double duty: deepening Go skills while producing AI red teaming portfolio pieces in your work language.

---

## 4. Claude Code Not Integrated as a Learning Accelerator Across Tracks

**The Problem:**
Claude Code appears in Track 3 (learn it) and Track 5 (use it for Go), then mostly disappears. For someone who already builds tools with Claude Code, it should be woven into **every single track** as a force multiplier.

**Current mentions across tracks:**
- Track 3: Learn Claude Code (1 week)
- Track 5: "Use Claude Code with Go at work" (brief tips)
- Other tracks: Occasional "use Claude Code if stuck"

**Recommendation:**
Add a **"Claude Code Integration"** section to each track with specific, actionable patterns:

**Track 8 (Python Core):**
- Use Claude Code to generate pytest fixtures from your Go test patterns
- Have Claude Code explain Python idioms by comparing to Go equivalents
- Use Claude Code to review your Python code for "Go-isms"

**Track 9 (AI/ML Security):**
- Use Claude Code SDK to build automated prompt injection testers
- Build MCP servers that connect to HTB Academy for note-taking
- Use extended thinking for complex attack chain analysis

**Track 11 (Go Deep Dive):**
- CLAUDE.md configuration for each Go project
- Claude Code for Go code review with 100 Go Mistakes patterns
- Automated Go test generation with Claude Code
- Interface extraction and refactoring patterns

**Track 12 (JS/TS):**
- Use Claude Code to scaffold TypeScript projects with proper configs
- Compare patterns across Go/Python/TS using Claude Code's multi-language knowledge

---

## 5. JavaScript/TypeScript is Overallocated at 20 Weeks

**The Problem:**
20 weeks (30% of the entire plan) for JS/TS is disproportionate for someone targeting AI red teaming. The plan justifies it with "LangChain, Vercel AI SDK use TypeScript" — but you'll primarily use Python and Go for security work.

**Breakdown of the 20 weeks:**
- 6 weeks: JavaScript fundamentals (Eloquent JavaScript cover-to-cover)
- 6 weeks: Node.js/Express with TypeScript
- 4 weeks: Advanced TypeScript patterns
- 4 weeks: Security focus

**What can be compressed:**
- **JavaScript fundamentals (6 weeks):** After mastering Python and Go, you don't need 6 weeks for another language's basics. You understand variables, functions, loops, objects, async. Compress to **3 weeks** focusing on JS-specific concepts (prototypes, closures, event loop, `this`).
- **Advanced TypeScript patterns (4 weeks):** Mapped types, conditional types, and template literal types are deep TypeScript expertise. For a security engineer, **2 weeks** is sufficient.
- **Node.js/Express (6 weeks):** Keep as-is — web app security requires understanding server-side JS.
- **Security focus (4 weeks):** Keep as-is — this is the payoff.

**Compressed timeline: 14 weeks instead of 20**, freeing 6 weeks for Go + AI security work.

---

## 6. Go Crash Course Doesn't Account for Existing Experience

**The Problem:**
Track 5 assumes you're starting Go from zero: "Tour of Go", "Hello World", install Go. But you've been using Go at work and building tools with Claude Code. Some of this week may be unnecessary.

**Recommendation:**
Add a **self-assessment checkpoint** at the start of Track 5:

```
Before starting, can you:
- [ ] Read and understand Go code at work?
- [ ] Write basic Go functions with error handling?
- [ ] Use goroutines and channels?
- [ ] Write Go tests?
- [ ] Navigate your company's Go codebase?

If you checked 3+: Skip to the weekend (build a tool + contribute to company codebase).
If you checked 1-2: Do the abbreviated version (skip Tour of Go, focus on gaps).
If you checked 0: Follow the full crash course.
```

This prevents wasting 18 hours on material you already know.

---

## 7. Missing: CLAUDE.md Strategy for Go Projects

**The Problem:**
CLAUDE.md files are one of Claude Code's most powerful features — they give Claude Code persistent project context. The plan never mentions creating CLAUDE.md files for your Go projects at work, which would dramatically improve your daily development.

**Recommendation:**
Add a concrete task in Week 4 (Track 3) or Week 6 (Track 5):

**Create CLAUDE.md files for:**
1. Your primary Go work repository
2. Your learning journal repository
3. Each portfolio project

**Example Go project CLAUDE.md:**
```markdown
# Project Context
Go microservice for [service name]. Uses gRPC + PostgreSQL.

# Build & Test
- `go build ./...` to build
- `go test ./...` to run tests
- `golangci-lint run` for linting

# Code Style
- Follow company style guide at [link]
- Error wrapping with fmt.Errorf("context: %w", err)
- Table-driven tests preferred
- Interfaces defined by consumers, not producers

# Architecture
- cmd/ for entry points
- internal/ for private packages
- pkg/ for shared libraries
```

---

## 8. No Mention of Claude Code SDK for AI Agent Building

**The Problem:**
The Claude Code SDK (Claude Agent SDK) lets you build custom AI agents — this is directly relevant to AI red teaming (building automated attack agents, red team orchestration tools). The plan never mentions it.

**Why it matters for AI red teaming:**
- Build agents that systematically test LLM defenses
- Create red team orchestration tools that chain attacks
- Automate prompt injection testing with agent workflows
- Build defensive monitoring agents

**Recommendation:**
Add a **2-day mini-project** during Track 9 (AI/ML Security, Weeks 25-26):

| Day | Activity | Output |
|-----|----------|--------|
| Day 1 | Learn Claude Code SDK basics, build simple agent | Working agent that tests prompt injection patterns |
| Day 2 | Extend agent to chain attacks and log results | Automated red team agent (GitHub portfolio piece) |

This combines your Claude Code experience with your AI security learning for a unique portfolio piece.

---

## 9. Track References Are Inconsistent

**The Problem:**
Several tracks have mismatched internal references:

| File | Issue |
|------|-------|
| `track-05-go-crash-course.md` | Line 24: Says "NOT become a Go expert (that's Week 53-64)" — should be Weeks 35-46 |
| `track-05-go-crash-course.md` | Title says "Track 4" in the heading context but it's actually Track 5 |
| `track-05-go-crash-course.md` | "Go Deep Dive" reference says "Weeks 34-45" (line 279) and "Weeks 35-46" (line 192) — inconsistent |
| `track-09-ai-ml-security.md` | Line 100: References "Track 6 (Wilson book)" — Wilson book is Track 7 (LLM Security Primer) |
| `track-09-ai-ml-security.md` | Line 119: References "Track 4" for Python — Python Core is Track 8 |
| `track-10-python-advanced.md` | Line 1 header text says "Why After JavaScript?" — but it comes BEFORE JavaScript |

These create confusion during execution when you're trying to cross-reference material.

**Recommendation:** Fix all cross-references in a single pass. Each track should reference other tracks by both track number AND name (e.g., "Track 7: LLM Security Primer").

---

## 10. Missing: Leveraging Go Concurrency for Security Work Earlier

**The Problem:**
Go's goroutines and channels are ideal for concurrent security scanning — but the plan only teaches Go concurrency in Week 37 (fundamentals) and uses it in Weeks 43-46 (Black Hat Go). By that point, you've already built async Python scanners (Weeks 31-34) without the option to use Go's simpler concurrency model.

**Recommendation:**
During the Python Async track (Weeks 31-34), add a **comparison exercise**:

> Build the same concurrent scanner in both Python (asyncio) and Go (goroutines).
> Compare: lines of code, performance, error handling, readability.
> Blog post: "Python asyncio vs Go goroutines for Security Scanning"

This reinforces both languages, produces a great blog post, and helps you decide which tool to reach for in real-world red teaming work.

---

## Priority Ranking

| # | Improvement | Impact | Effort |
|---|-------------|--------|--------|
| 1 | Move Go Deep Dive earlier (Week 27) | High | Medium (restructure timeline) |
| 2 | Update Claude Code track for your experience level | High | Low (rewrite 1 file) |
| 3 | Add Go + AI Security integration | High | Low (add 2-week phase) |
| 4 | Weave Claude Code into every track | Medium | Low (add sections) |
| 5 | Compress JavaScript/TypeScript to 14 weeks | Medium | Medium (restructure track) |
| 6 | Add self-assessment to Go Crash Course | Medium | Low (add checklist) |
| 7 | Add CLAUDE.md strategy for Go projects | Medium | Low (add section) |
| 8 | Add Claude Code SDK for agent building | Medium | Low (add 2-day project) |
| 9 | Fix cross-reference inconsistencies | Low | Low (text fixes) |
| 10 | Add Go vs Python concurrency comparison | Low | Low (add exercise) |

---

## Implementation Status

All 10 recommendations have been implemented in the restructured plan:

| # | Improvement | Status | What Changed |
|---|-------------|--------|-------------|
| 1 | Go front-loaded | DONE | New Track 8: Go Foundations + Architecture (12 weeks, Weeks 9-20) |
| 2 | Claude Code track updated | DONE | Track 3 rewritten for advanced users (CLAUDE.md, MCP, SDK, hooks) |
| 3 | Go + AI Security integration | DONE | Track 11 Phase 2: Go for AI Security (Weeks 41-42) |
| 4 | Claude Code woven into all tracks | DONE | Integration sections added to Tracks 8, 9, 10, 11, 12 |
| 5 | JS/TS compressed to 14 weeks | DONE | Track 13: Weeks 49-62 (down from 20 weeks) |
| 6 | Self-assessment on Go Crash Course | DONE | Track 5 has skip-ahead checklist |
| 7 | CLAUDE.md strategy for Go | DONE | Track 3 and Track 8 both teach CLAUDE.md for Go projects |
| 8 | Claude Code SDK for agents | DONE | Track 10 Week 36 has SDK red team agent project |
| 9 | Cross-references fixed | DONE | All track numbers and week references updated |
| 10 | Go vs Python concurrency | DONE | Track 12 Week 48 comparison exercise |

**Implemented Timeline:**
```
Weeks 1-8:    Foundation (Tracks 1-7)
Weeks 9-20:   Go Foundations + Software Architecture (Track 8) ← NEW
Weeks 21-24:  Go Security Tools / Black Hat Go (Track 11) ← right after Track 8
              Break week
Weeks 25-32:  Python Core + TDD (Track 9, compressed)
Weeks 33-42:  AI/ML Security + Go for AI Security capstone (Track 10)
              Break week
Weeks 43-48:  Python Advanced (Track 12, compressed)
Weeks 49-62:  JavaScript/TypeScript (Track 13, compressed)
              Break week (mid-JS/TS)
```

**New allocation:**
| Language | Weeks | Change |
|----------|-------|--------|
| Go | 19 weeks (Tracks 5, 8, 11) | +6 weeks, front-loaded |
| Python | 14 weeks (Tracks 9, 12) | -4 weeks, architecture learned in Go |
| JavaScript/TypeScript | 14 weeks (Track 13) | -6 weeks, compressed |
| AI/ML Security | 8 weeks (Track 10) | unchanged |

---

## Bottom Line

The plan now treats Go and Claude Code as **existing strengths being deepened**, not future skills to acquire. Go is front-loaded as the work language with software architecture taught in Go first, then transferred to Python and other languages.
