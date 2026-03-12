# Track 3: Claude Code Advanced Mastery

**Duration:** 1 week | **Total:** 18 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** CRITICAL — THIS IS YOUR PRIMARY TOOL

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why This Is the Most Important Week

**Claude Code is how you build everything.** You don't write code — you direct Claude Code to write it. This week determines how effective you are for the entire 44-week plan and your career.

The difference between a mediocre architect and a great one is the quality of their direction. This week teaches you to:

- **Give Claude Code precise architectural instructions** via CLAUDE.md files
- **Review code systematically** instead of accepting whatever Claude Code produces
- **Build automated workflows** that make your direction more efficient
- **Use extended thinking** for complex architectural decisions
- **Build AI agents** (directly relevant to your AI red teaming career)

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

## Claude Code as Your Implementation Partner

After this week, Claude Code is your implementation tool in every track:

**Track 5 (Go Crash Course):** CLAUDE.md for company repos, Go code review
**Track 8 (Software Architecture):** Direct Claude Code to build Go projects, review output
**Track 10 (AI/ML Security):** Build exploit tools, vulnerable apps, red team agents
**Track 9 (Python Core):** Build Python projects, review for architecture patterns
**Track 11 (Go Security + AI Capstone):** Build security tools, AI red team CLI tool

-----

## Expected ROI

- 30-60% cost reduction (smart model selection)
- 40-60% time savings per task (CLAUDE.md context)
- 10-20x productivity in first month
- Automated workflows save hours/week at work

-----

## Resources

### Official Documentation (Start Here)

- [Claude Code Best Practices](https://code.claude.com/docs/en/best-practices) — Anthropic's official Explore → Plan → Implement → Verify workflow
- [Claude Code Quickstart](https://code.claude.com/docs/en/quickstart) — Getting started guide
- [Create Custom Subagents](https://code.claude.com/docs/en/sub-agents) — Official guide to defining subagents in `.claude/agents/`
- [Agent SDK Overview](https://platform.claude.com/docs/en/agent-sdk/overview) — Official Claude Agent SDK documentation
- [How Anthropic Teams Use Claude Code (PDF)](https://www-cdn.anthropic.com/58284b19e702b49db9302d5b6f135ad8871e7658.pdf) — Internal Anthropic practices and workflows

### Prompting & Advanced Usage Patterns (Mon-Tue)

- [Prompting Best Practices](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices) — Official prompt engineering guide
- [Claude Code Prompting Guide 2025](https://smartscope.blog/en/generative-ai/claude/claude-code-prompting-official-guidelines-2025/) — 10 essential prompting techniques
- [The Ultimate Guide to Claude Code (Medium)](https://medium.com/@tonimaxx/the-ultimate-guide-to-claude-code-production-prompts-power-tricks-and-workflow-recipes-42af90ca3b4a) — Battle-tested templates and production prompts
- [Agentic Coding Recommendations (Armin Ronacher)](https://lucumr.pocoo.org/2025/6/12/agentic-coding/) — Practical agentic coding advice from Flask creator
- [50 Claude Code Tips & Tricks](https://www.geeky-gadgets.com/claude-code-tips-2/) — Quick reference of power-user patterns

### Hooks, Slash Commands & Automation (Thu)

- [Claude Code Hooks: Complete Guide](https://www.ksred.com/claude-code-hooks-a-complete-guide-to-automating-your-ai-coding-workflow/) — All 15 hook events and handler types
- [Mastering Claude Hooks (DEV Community)](https://dev.to/bredmond1019/mastering-claude-hooks-building-observable-ai-systems-part-2-2ic4) — Deep-dive on building observable AI systems
- [awesome-claude-code (GitHub)](https://github.com/hesreallyhim/awesome-claude-code) — Curated list of skills, hooks, slash commands, and plugins
- [Claude Code System Prompts (GitHub)](https://github.com/Piebald-AI/claude-code-system-prompts) — All system prompts, sub-agent prompts, and tool descriptions extracted from Claude Code

### Claude Agent SDK & AI Agent Building (Fri)

- [Claude Agent SDK Demos (GitHub)](https://github.com/anthropics/claude-agent-sdk-demos) — Official demo repository
- [DataCamp: Claude Agent SDK Tutorial](https://www.datacamp.com/tutorial/how-to-use-claude-agent-sdk) — Build three projects from one-shot to custom-tool agents
- [KDnuggets: Getting Started with the Claude Agent SDK](https://www.kdnuggets.com/getting-started-with-the-claude-agent-sdk) — Build a multi-tool CLI agent step by step
- [The Complete Guide to Building Agents (Nader Dabit)](https://nader.substack.com/p/the-complete-guide-to-building-agents) — Build a code review agent from scratch
- [Claude Code Everything You Need to Know (GitHub)](https://github.com/wesammustafa/Claude-Code-Everything-You-Need-to-Know) — All-in-one repo: setup, prompt engineering, hooks, BMAD method

### Sub-Agents & Multi-Agent Workflows (Sat)

- [Guide to Claude Code Subagents & Hooks (Arsturn)](https://www.arsturn.com/blog/a-beginners-guide-to-using-subagents-and-hooks-in-claude-code) — Beginner-friendly intro to subagents
- [Best Practices for Claude Code Subagents (PubNub)](https://www.pubnub.com/blog/best-practices-for-claude-code-sub-agents/) — Production patterns for subagent orchestration
- [Claude Code Workflow (GitHub)](https://github.com/catlog22/Claude-Code-Workflow) — JSON-driven multi-agent development framework
- [Agents: Multi-agent Orchestration (GitHub)](https://github.com/wshobson/agents) — 112 specialized agents, 16 orchestrators, 146 skills

### Security Testing with Claude Code (Relevant for AI Red Teaming)

- [Red Team Agent Skills (GitHub)](https://github.com/yechao-zhang/red-team-agent-skills) — Claude Code skills for automated red team operations
- [AI Red Teaming: Attacking Claude Code Using PyRIT](https://breakpoint-labs.com/ai-red-teaming-part-3-attacking-claude-code-using-pyrit/) — Prompt injection attacks via malicious files in repos
- [AI for Cyber Defenders (Anthropic Red Team)](https://red.anthropic.com/2025/ai-for-cyber-defenders/) — Anthropic's red team research
- [How to Red Team Claude (Promptfoo)](https://www.promptfoo.dev/blog/red-team-claude/) — YAML-config-based adversarial testing

### Video Courses & Tutorials

- [Claude Code in Action (Anthropic Official)](https://anthropic.skilljar.com/claude-code-in-action) — Official training covering architecture, implementation, and MCP integration
- [Video Tutorials (Claude Help Center)](https://support.claude.com/en/collections/10548294-video-tutorials) — Official video collection
- [Anthropic Academy: Build with Claude](https://www.anthropic.com/learn/build-with-claude) — Official learning hub

-----

## Checkpoint

You should be able to:
- [ ] Create effective CLAUDE.md files for any Go project
- [ ] Connect Claude Code to Obsidian via MCP
- [ ] Set up hooks for automated linting and formatting
- [ ] Build a simple AI agent with Claude Code SDK
- [ ] Use extended thinking for complex analysis
- [ ] Apply Claude Code effectively across all subsequent tracks
