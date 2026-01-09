# Getting Started: Tracks 1-3 (Weeks 1-4)

**Focus:** Meta-learning foundations before technical deep-dives
**Total Duration:** 4 weeks | 72 hours total
**Goal:** Set up learning infrastructure before starting Python/AI/JS

-----

## Why These Three First?

These aren't technical skills - they're **learning accelerators** that compound across everything else:

1. **Reading Skills** → Read technical books 2-3x faster
2. **Note-Taking** → Capture and retrieve knowledge across all 8 tracks
3. **Claude Code** → AI-assisted learning for all coding tracks

**Do these right, save 100+ hours later.**

-----

## Week 1: Reading Skills

**Books you own:**
- ✅ How to Read a Book (Adler & Van Doren)
- ✅ Speed Reading (Knight)

**Time:** 18 hours (8 weekday + 5 Sat + 5 Sun)

### Schedule

**Days 1-2 (Monday-Tuesday): Speed Reading (Knight) - 6 hours**

|Day|Time|Activity|
|---|----|----|
|Mon|3 hrs|Sections I-II (Chapters 1-6): Preview, Space Reading, Chunking|
|Tue|3 hrs|Sections III-V (Chapters 7-15): Fixation, Comprehension, Memory|

**Practice immediately:**
- Space Reading - Look between words, not at words
- Chunking - Read word groups
- Stop subvocalization - Don't "speak" every word in your head

**Days 3-5 (Wed-Fri): How to Read a Book (Adler) - 7 hours**

|Day|Time|Activity|Focus|
|---|----|----|-----|
|Wed|2 hrs|Part 1 (Ch 1-5)|4 levels of reading|
|Thu|3 hrs|Part 2 (Ch 6-12)|Analytical reading|
|Fri|2 hrs|Ch 13 + Part 4 (Ch 20-21)|Practical books + Syntopical reading|

**Skip:** Chapters 14-19 (fiction, philosophy, etc.)

**The 4 Questions (memorize these):**
1. What is the book about as a whole?
2. What is being said in detail, and how?
3. Is the book true, in whole or part?
4. What of it? (So what?)

**Weekend: Practice - 5 hours**

|Day|Time|Activity|
|---|----|----|
|Sat|3 hrs|Practice speed reading on articles/docs|
|Sun|2 hrs|Do inspectional reading on "How to Take Smart Notes"|

### Week 1 Deliverable
- [ ] Can speed read at least 50% faster than baseline
- [ ] Can do inspectional reading in 30-60 minutes
- [ ] Memorized the 4 questions

-----

## Week 2-3: Note-Taking System (Obsidian)

**Books you own:**
- ✅ How to Take Smart Notes (Ahrens)
- ✅ Building a Second Brain (Forte)

**Time:** 36 hours (18 hrs/week × 2 weeks)

### Week 2: Zettelkasten Method + Setup

**Weekdays (Mon-Fri): 8 hours**
- Read "How to Take Smart Notes" - all chapters
- Apply speed reading techniques from Week 1
- Take notes IN Obsidian as you read (meta!)

**Saturday: 5 hours**
- Install Obsidian
- Explore interface and core features
- Watch: "Linking Your Thinking" intro videos (YouTube)
- Set up basic vault structure

**Sunday: 5 hours**
- Install core plugins:
  - Dataview
  - Templater
  - Obsidian Git
  - Excalidraw (optional)
  - Kanban (optional)

### Week 3: PARA Method + Sync

**Weekdays (Mon-Fri): 8 hours**
- Read "Building a Second Brain" - all chapters
- Compare with Zettelkasten approach
- Decide on your hybrid system

**Saturday: 5 hours**
- Create PARA folder structure:
  - Projects (active learning tracks)
  - Areas (career, skills, AI security)
  - Resources (references, papers, code snippets)
  - Archives (completed projects)
- Design templates:
  - Daily note template
  - Book review template
  - Learning note template
  - Code snippet template
  - Security finding template

**Sunday: 5 hours**
- Set up sync:
  - Option 1: Obsidian Sync ($8/month, easiest)
  - Option 2: Your Synology + Möbius Sync (free, more complex)
  - Option 3: Obsidian Git plugin + private repo (free, tech setup)
- Test sync across devices
- Create your first "permanent note"

### Recommended Obsidian Setup

**Folder Structure:**
```
📁 improvement-plan/
├── 📁 Projects/
│   ├── Track-1-Reading-Skills.md
│   ├── Track-2-Obsidian.md
│   ├── Track-3-Claude-Code.md
│   └── [future tracks...]
├── 📁 Areas/
│   ├── AI-Red-Teaming.md
│   ├── Python-Skills.md
│   ├── JavaScript-Skills.md
│   └── Career-Development.md
├── 📁 Resources/
│   ├── Books/
│   ├── Courses/
│   ├── Papers/
│   └── Code-Snippets/
└── 📁 Archives/
    └── [completed projects]
```

**Templates to Create:**

1. **Learning Note Template**
```markdown
---
type: learning-note
track: [Track 1-8]
week: [Week number]
tags: [python, security, ai, etc.]
created: {{date}}
---

# {{title}}

## Key Concepts

## Code Examples

## Questions/Gaps

## Links
-
```

2. **Daily Note Template**
```markdown
---
type: daily-note
date: {{date}}
---

# {{date:YYYY-MM-DD}}

## What I Learned Today

## What I Built Today

## Challenges/Questions

## Tomorrow's Focus
```

3. **Book Review Template**
```markdown
---
type: book-review
book: {{title}}
author:
track:
rating: /10
completed: {{date}}
---

# {{title}} Review

## Summary (3-5 sentences)

## Key Takeaways
1.
2.
3.

## Best Quotes

## How I'll Apply This

## Would I Recommend?
```

### Week 2-3 Deliverable
- [ ] Obsidian installed with PARA structure
- [ ] 5 core plugins configured
- [ ] 3 templates created (daily, learning, book review)
- [ ] Sync working across devices
- [ ] Notes from Week 1-2 captured in system

-----

## Week 4: Claude Code Mastery

**Resources you have:**
- Your guides/02 (Beginner guide)
- Your guides/17 (Advanced guide)

**Time:** 18 hours (8 weekday + 5 Sat + 5 Sun)

### Schedule

**Weekdays (Mon-Fri): 8 hours**

|Day|Time|Activity|
|---|----|----|
|Mon|2 hrs|Read guides/02 - 4-Part Formula|
|Tue|2 hrs|Read guides/02 - 7 Core Patterns|
|Wed|2 hrs|Read guides/17 - Chain-of-Thought|
|Thu|1 hr|Read guides/17 - Few-Shot prompting|
|Fri|1 hr|Read guides/17 - Cost-aware strategies|

**The 4-Part Formula:**
1. **Intent** → What action (fix, create, refactor)
2. **Context** → Where (file path, tech stack)
3. **Constraints** → How (requirements, don'ts)
4. **Success criteria** → Expected output

**7 Core Patterns:**
- CREATE - Build new features/files
- FIX - Debug and repair
- REFACTOR - Improve code structure
- REVIEW - Code quality analysis
- EXPLAIN - Understand complex code
- TEST - Generate test cases
- OPTIMIZE - Performance improvements

**Weekend: Practice - 10 hours**

**Saturday: 5 hours**
- Pick a codebase (GitHub repo or your own code)
- Practice all 7 patterns on it:
  - EXPLAIN - "Explain what this module does"
  - REVIEW - "Review this code for security issues"
  - REFACTOR - "Refactor this function for clarity"
  - TEST - "Generate pytest tests for this"
  - OPTIMIZE - "Find performance bottlenecks"
  - FIX - Find a bug, ask Claude to fix it
  - CREATE - "Add a new feature to this"

**Sunday: 5 hours**
- Practice cost-aware prompting:
  - Start with Haiku for simple tasks
  - Use Sonnet for complex tasks
  - Reserve Opus for critical/difficult work
- Practice model cascading:
  - Try same prompt on Haiku → Sonnet → Opus
  - Compare quality and cost
- Set up CLAUDE.md in a test project

### Week 4 Deliverable
- [ ] Comfortable with 4-Part Formula
- [ ] Used all 7 core patterns in practice
- [ ] Understand when to use Haiku vs Sonnet vs Opus
- [ ] Created CLAUDE.md for a project

-----

## Investment Summary (Weeks 1-4)

### Books
- ✅ All already owned - $0

### Software/Tools
- **Free options:**
  - Obsidian (free)
  - Obsidian Git plugin (free)
  - GitHub private repo (free)
  - **Total: $0**

- **Paid options (optional):**
  - Obsidian Sync: $8/month = $8
  - **Total: $8**

### Time Investment
- Week 1: 18 hours
- Week 2: 18 hours
- Week 3: 18 hours
- Week 4: 18 hours
- **Total: 72 hours over 4 weeks**

-----

## What's Next After Week 4?

You'll be ready for **Track 4: Python Core** (Weeks 5-14) with:

✅ Speed reading skills → Read Okken/Percival books 2x faster
✅ Obsidian system → Capture all Python/TDD learnings
✅ Claude Code mastery → AI-assisted coding for projects

**Everything you learn in Tracks 4-8 will be:**
- Read faster (Track 1)
- Captured in Obsidian (Track 2)
- Built with Claude Code assistance (Track 3)

-----

## Quick Start Checklist

### Week 1
- [ ] Day 1-2: Read Speed Reading (Knight)
- [ ] Day 3-5: Read How to Read a Book (Adler)
- [ ] Weekend: Practice speed reading + inspectional reading

### Week 2
- [ ] Weekdays: Read How to Take Smart Notes
- [ ] Saturday: Install Obsidian + explore
- [ ] Sunday: Install plugins (Dataview, Templater, Git)

### Week 3
- [ ] Weekdays: Read Building a Second Brain
- [ ] Saturday: Create PARA structure + templates
- [ ] Sunday: Set up sync + test workflow

### Week 4
- [ ] Weekdays: Read Claude Code guides (guides/02 + guides/17)
- [ ] Saturday: Practice 7 patterns on real code
- [ ] Sunday: Cost-aware prompting + model cascading

-----

## Success Metrics

After completing Tracks 1-3, you should be able to:

**Track 1 (Reading):**
- ✅ Read 50%+ faster than baseline
- ✅ Do inspectional reading in 30-60 min
- ✅ Ask the 4 questions automatically

**Track 2 (Obsidian):**
- ✅ Capture notes in <2 minutes
- ✅ Find any note in <30 seconds
- ✅ Connect ideas across topics

**Track 3 (Claude Code):**
- ✅ Use 4-Part Formula naturally
- ✅ Apply all 7 core patterns
- ✅ Choose right model for task (cost-aware)

-----

## Common Pitfalls to Avoid

### Week 1: Reading Skills
- ❌ Don't skip the practice exercises
- ❌ Don't try to read everything analytically (use inspectional first)
- ❌ Don't subvocalize - this is the #1 speed killer

### Week 2-3: Obsidian
- ❌ Don't over-organize - start simple, iterate later
- ❌ Don't create empty folders - only add folders when you have content
- ❌ Don't obsess over perfect structure - the links matter more
- ❌ Don't skip setting up sync - you WILL lose notes otherwise

### Week 4: Claude Code
- ❌ Don't use Opus for everything - expensive and often unnecessary
- ❌ Don't skip writing clear prompts - garbage in, garbage out
- ❌ Don't forget to review Claude's output - it makes mistakes
- ❌ Don't ignore cost - use Haiku first, escalate if needed

-----

## Resources for Tracks 1-3

### Week 1
- Books: How to Read a Book, Speed Reading (both owned)

### Week 2-3
- Books: How to Take Smart Notes, Building a Second Brain (both owned)
- Videos: [Linking Your Thinking](https://www.youtube.com/c/LinkingYourThinking) (YouTube, free)
- Setup guide: [Curtis McHale 2026 Setup](https://curtismchale.ca/2025/12/29/my-2026-obsidian-setup/)
- Template: [GitHub PARA Template](https://github.com/byarbrough/obsidian-para)

### Week 4
- Your guides: guides/02 (Beginner), guides/17 (Advanced)
- Practice repos: Any GitHub repo or your own code

-----

## Questions to Ask Yourself

### After Week 1
- Can I skim a 300-page book in under an hour?
- Do I know when to read inspectionally vs analytically?
- Am I using the 4 questions on everything I read?

### After Week 2-3
- Is my Obsidian vault set up and syncing?
- Can I capture a new idea in under 2 minutes?
- Am I using templates consistently?
- Have I created at least 10 notes?

### After Week 4
- Can I write a clear 4-part prompt?
- Have I used all 7 core patterns?
- Do I know when to use Haiku vs Sonnet?
- Have I saved money by using model cascading?

-----

## Ready to Start?

**Week 1 starts NOW:**
1. Grab your Speed Reading book
2. Set a timer for 3 hours
3. Read Chapters 1-6
4. Practice space reading immediately

**Don't overthink it - just start reading!**
