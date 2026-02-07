# Track 3: Claude Code Advanced Mastery

**Duration:** 1 week | **Total:** 18 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** CRITICAL

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why This Week?

You already build tools with Claude Code — you know the basics (prompt patterns, model selection, core workflows). This week levels you up to **power-user status** with features that compound across every future track.

Claude Code accelerates everything else. Mastering it now means:

- Faster code review and understanding
- Assisted project building in Python/JS/Go tracks
- Better prompt engineering for AI/ML security work
- Automated workflows for your Go development at work

-----

## Self-Assessment: Skip What You Know

Before starting, check your current level:

```
Already comfortable with:
- [ ] 4-Part Formula (Intent, Context, Constraints, Success criteria)
- [ ] 7 Core Patterns (CREATE, FIX, REFACTOR, REVIEW, EXPLAIN, TEST, OPTIMIZE)
- [ ] Model selection (Haiku for simple, Sonnet for moderate, Opus for complex)
- [ ] Cost-aware prompting

If you checked all 4: Skip to Day 3 (CLAUDE.md + MCP servers).
If you checked 2-3: Skim Days 1-2, focus on gaps.
If you checked 0-1: Start from Day 1.
```

-----

## Week 4 Schedule

### Monday-Tuesday (6 hours): CLAUDE.md Project Configuration

**Why This Matters:**
CLAUDE.md files give Claude Code persistent project context — they are the single biggest productivity multiplier. Every Go project at work and every learning project should have one.

**Monday (3 hours): CLAUDE.md Fundamentals**
- Understand CLAUDE.md structure and placement
- Project-level vs directory-level CLAUDE.md files
- What to include: build commands, test commands, code style, architecture
- What NOT to include: secrets, credentials, large file contents

**Hands-on: Create CLAUDE.md for your Go work repo:**
```markdown
# Project Context
Go microservice for [service name]. Uses [framework/patterns].

# Build & Test
- `go build ./...` to build
- `go test ./...` to run all tests
- `go test -race ./...` to run tests with race detector
- `golangci-lint run` for linting

# Code Style
- Follow company style guide
- Error wrapping: fmt.Errorf("context: %w", err)
- Table-driven tests preferred
- Interfaces defined by consumers, not producers
- Package names: short, lowercase, no underscores

# Architecture
- cmd/ for entry points
- internal/ for private packages
- pkg/ for shared libraries (if applicable)
```

**Tuesday (3 hours): Advanced CLAUDE.md Patterns**
- Multi-directory CLAUDE.md for monorepos
- Including dependency context (go.mod, key packages)
- Linking to style guides and architecture docs
- Create CLAUDE.md for your learning journal repo
- Create a template CLAUDE.md for future portfolio projects

**Deliverable:** Working CLAUDE.md files for your Go work repo and learning repo

-----

### Wednesday (2 hours): MCP Servers

**Why This Matters:**
MCP (Model Context Protocol) servers connect Claude Code to external tools — databases, APIs, your Obsidian vault. This creates a connected workflow where Claude Code can query your notes, check databases, and interact with services.

**Setup Obsidian MCP Integration (from Track 2):**
1. Install and configure MCP server for Obsidian (60 min)
   - Configure path to vault
   - Test querying from Claude Code
2. Test connected workflow (60 min)
   - Ask Claude Code to search your notes
   - Synthesize concepts across notes
   - Document the workflow

**Test Query:**
```
"Search my Obsidian vault for all notes about Go error handling patterns.
Synthesize the key patterns I've documented."
```

-----

### Thursday (2 hours): Hooks & Custom Slash Commands

**Why This Matters:**
Hooks automate pre/post actions on tool calls. Custom slash commands create reusable workflows. Together they streamline your daily Go development.

**Hooks (1 hour):**
- Pre-tool hooks: auto-format Go code before commits
- Post-tool hooks: run `golangci-lint` after file edits
- Notification hooks: alert on test failures

**Custom Slash Commands (1 hour):**
- Create `/go-review` command for Go code reviews
- Create `/go-test` command that runs tests and explains failures
- Create `/security-check` command for security-focused code review

-----

### Friday (2 hours): Claude Code SDK & AI Agent Building

**Why This Matters:**
The Claude Agent SDK lets you build custom AI agents — directly relevant to AI red teaming. Understanding the SDK now means you can build automated security testing agents later.

**Activities:**
- Understand the Claude Agent SDK architecture (30 min)
- Build a simple agent that reviews Go code for common mistakes (60 min)
- Extend the agent to suggest fixes based on "100 Go Mistakes" patterns (30 min)

**Output:** Working Go code review agent

-----

### Saturday (5 hours): Extended Thinking & Sub-Agents

**Extended Thinking (2 hours):**
- When to use extended thinking vs standard prompts
- Complex problem decomposition
- Architecture design sessions
- Security analysis with deep reasoning

**Sub-Agents for Parallel Work (3 hours):**
- Launching multiple agents for independent tasks
- Agent coordination patterns
- Practical use case: parallel security scanning
- Build workflow that scans multiple files concurrently

-----

### Sunday (5 hours): Apply Everything to Real Work

**Integration Day (5 hours):**

1. **Go work project (2 hours)**
   - Use CLAUDE.md-enhanced workflow on a real task
   - Apply hooks for auto-linting
   - Use extended thinking for an architecture decision

2. **Build a Claude Code workflow for learning (2 hours)**
   - Set up slash commands for each learning track
   - Create `/learn-summary` command that summarizes today's learnings
   - Create `/blog-draft` command that drafts weekly blog posts

3. **Document your setup (1 hour)**
   - Write blog post: "My Claude Code Power-User Setup"
   - Document all CLAUDE.md files, hooks, and commands in Obsidian
   - Share configurations on GitHub

-----

## Key Concepts

**CLAUDE.md Configuration:**
- Project context that persists across sessions
- Build/test/lint commands for Claude Code to use
- Architecture and style guide references
- Per-directory overrides for monorepos

**MCP Servers:**
- Connect Claude Code to external tools
- Obsidian integration for knowledge queries
- Database integration for data access
- Custom MCP servers for specialized workflows

**Hooks:**
- Pre-tool: Actions before Claude Code runs a tool
- Post-tool: Actions after Claude Code completes
- Automate formatting, linting, testing

**Claude Agent SDK:**
- Build custom AI agents
- Agent orchestration patterns
- Relevant for AI red teaming automation

**Extended Thinking:**
- Deep reasoning for complex problems
- Architecture design and security analysis
- When standard prompts aren't enough

-----

## Claude Code Integration Across Future Tracks

After this week, use Claude Code as a **continuous accelerator** in every track:

**Track 5 (Go Crash Course):** CLAUDE.md for company repos, Go code explanation
**Track 8 (Python Core):** Generate pytest fixtures, compare Python to Go patterns
**Track 9 (AI/ML Security):** Build automated red team agents with SDK
**Track 10 (Python Advanced):** AST analysis assistance, async pattern comparison
**Track 11 (Go Deep Dive):** CLAUDE.md for every project, Go test generation
**Track 12 (JS/TS):** Scaffold TypeScript projects, cross-language comparisons

-----

## Expected ROI

- 30-60% cost reduction (smart model selection)
- 40-60% time savings per task (CLAUDE.md context)
- 10-20x productivity in first month
- Automated workflows save hours/week at work

-----

## Checkpoint

You should be able to:
- [ ] Create effective CLAUDE.md files for any Go project
- [ ] Connect Claude Code to Obsidian via MCP
- [ ] Set up hooks for automated linting and formatting
- [ ] Build a simple AI agent with Claude Code SDK
- [ ] Use extended thinking for complex analysis
- [ ] Apply Claude Code effectively across all subsequent tracks
