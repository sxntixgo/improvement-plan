# Track 4: Git Mastery (Week 5)

**Duration:** 1 week | **Total:** 18 hours
**Approach:** Hands-on, project-based learning

**You Own:** Pro Git by Scott Chacon and Ben Straub (reference)

-----

## Why Git Before Go?

Git is foundational for ALL development work:
- Essential for contributing to company Go projects (Week 6)
- Needed for managing Python, JavaScript projects
- Required for portfolio, open source contributions
- Concentrated learning beats scattered sessions

-----

## Learning Strategy: Hands-On First, Reference Second

**Primary Learning (12 hours):** Interactive, project-based tutorials
**Reference Reading (6 hours):** Pro Git book for depth and context

This approach matches your "learn by doing" preference while keeping Pro Git as valuable reference.

-----

## Week 5 Schedule

### Monday-Tuesday: Git Immersion Labs (6 hours)

**Resource:** [Git Immersion](https://gitimmersion.com/) - FREE ⭐

**50+ hands-on labs** that build real Git skills through practice.

**Monday (3 hours):**
- **Lab 1-10:** Setup and basics (30 min)
  - Install Git, configure
  - Create repository
  - Add, commit, status
  - Stage changes
- **Lab 11-20:** History and structure (1 hour)
  - View commit history
  - Aliases for efficiency
  - Getting old versions
  - Tagging versions
  - Understanding .git directory
- **Lab 21-30:** Branching basics (1.5 hours)
  - Undoing local changes
  - Undoing committed changes
  - Removing commits from branch
  - Amending commits
  - Moving files

**Tuesday (3 hours):**
- **Lab 31-40:** Advanced branching (1.5 hours)
  - Creating branches
  - Navigating branches
  - Merging branches
  - Resolving conflicts (CRITICAL)
  - Rebasing vs merging
- **Lab 41-50:** Remote repositories (1.5 hours)
  - Cloning repositories
  - Remote branches
  - Fetching changes
  - Pulling changes
  - Pushing to remotes
  - Hosting Git repos

**Deliverable:** Completed 50 Git Immersion labs, built real repositories

-----

### Wednesday-Thursday: Learn Git Branching (6 hours)

**Resource:** [Learn Git Branching](https://learngitbranching.js.org/) - FREE ⭐

**Visual, interactive sandbox** - perfect for understanding branching deeply.

**Wednesday (3 hours):**

**Main Section (2 hours):**
- **Introduction Sequence** (30 min)
  - 1.1: Introduction to Git Commits
  - 1.2: Branching in Git
  - 1.3: Merging in Git
  - 1.4: Rebase Introduction
- **Ramping Up** (45 min)
  - 2.1: Detach yo' HEAD
  - 2.2: Relative Refs (^)
  - 2.3: Relative Refs #2 (~)
  - 2.4: Reversing Changes
- **Moving Work Around** (45 min)
  - 3.1: Cherry-pick
  - 3.2: Interactive Rebase

**Remote Section (1 hour):**
- **Push & Pull** (30 min)
  - 1.1: Clone Intro
  - 1.2: Remote Branches
  - 1.3: Git Fetch
  - 1.4: Git Pull
  - 1.5: Simulating Collaboration
- **To Origin and Beyond** (30 min)
  - 2.1: Push Master
  - 2.2: Merging with Remotes
  - 2.3: Remote Tracking

**Thursday (3 hours):**

**Remote Advanced (1.5 hours):**
- **Advanced Origin** (45 min)
  - 3.1: Push Arguments
  - 3.2: Push Arguments Expanded
  - 3.3: Fetch Arguments
  - 3.4: Source of Nothing
  - 3.5: Pull Arguments
- **Remote Workflows** (45 min)
  - Complete remaining remote challenges

**Practice Scenarios (1.5 hours):**
- Work through all "Practice" levels
- Focus on scenarios you'll encounter at work
- Build muscle memory for common workflows

**Deliverable:** All main challenges completed, visual understanding of Git operations

-----

### Friday: Company Workflow + GitHub Practice (3 hours)

**Morning (1.5 hours): Learn Your Company's Git Workflow**

**Questions to Ask Team Lead:**
1. What branching strategy? (GitFlow, GitHub Flow, trunk-based?)
2. Branch naming convention? (feature/, bugfix/, hotfix/?)
3. Commit message format? (Conventional Commits?)
4. Pull request process?
5. Code review requirements?
6. Any Git hooks or pre-commit checks?
7. Main branch name? (main, master, develop?)

**Common Workflows:**

**GitHub Flow (Simple):**
```bash
1. git checkout -b feature/my-feature main
2. # Make changes
3. git add . && git commit -m "Add feature"
4. git push origin feature/my-feature
5. # Create PR on GitHub
6. # After approval, merge via GitHub UI
```

**GitFlow (Complex):**
```bash
1. git checkout -b feature/my-feature develop
2. # Make changes
3. git add . && git commit -m "Add feature"
4. git push origin feature/my-feature
5. # Create PR to develop branch
```

**Practice with real company repo:**
- Clone a company repository
- Create a test branch
- Make a small change (comment, docs)
- Push and create draft PR
- Ask teammate to review workflow (don't merge)

**Afternoon (1.5 hours): GitHub Real-World Practice**

**Exercise 1: Fork and Contribute (45 min)**
1. Find a beginner-friendly open source project
   - [First Timers Only](https://www.firsttimersonly.com/)
   - [Good First Issue](https://goodfirstissue.dev/)
2. Fork the repository
3. Clone your fork
4. Add upstream remote
5. Create feature branch
6. Make small contribution (fix typo, update docs)
7. Push to your fork
8. Create pull request

**Exercise 2: Handle Merge Conflicts (45 min)**
```bash
# Create test repo to practice conflicts
mkdir conflict-practice
cd conflict-practice
git init

# Create file on main
echo "Line 1" > file.txt
git add file.txt
git commit -m "Initial commit"

# Create branch 1
git checkout -b branch1
echo "Line 2 from branch1" >> file.txt
git add file.txt
git commit -m "Add line from branch1"

# Create branch 2 from main
git checkout main
git checkout -b branch2
echo "Line 2 from branch2" >> file.txt
git add file.txt
git commit -m "Add line from branch2"

# Try to merge - conflict!
git checkout main
git merge branch1  # Success
git merge branch2  # CONFLICT!

# Resolve conflict
# Edit file.txt
# Remove <<<<<<, ======, >>>>>> markers
# Keep desired content
git add file.txt
git commit -m "Resolve merge conflict"
```

**Deliverable:**
- Understand company Git workflow
- Created at least one real pull request
- Resolved merge conflicts successfully

-----

### Weekend: Pro Git Reference Reading (3 hours)

**Saturday (1.5 hours): Core Concepts**

**Pro Git Chapter 2: Git Basics (1 hour)**
- Pages 18-52
- Focus on sections you didn't fully understand from Git Immersion
- **2.2: Recording Changes** - Deep dive on staging area
- **2.4: Undoing Things** - When to use reset vs restore vs revert
- **2.5: Working with Remotes** - Understanding fetch vs pull

**Pro Git Chapter 3: Branching (30 min)**
- Pages 53-75 (Sections 3.1-3.2 only)
- **3.1: Branches in a Nutshell** - How Git stores branches
- **3.2: Basic Branching and Merging** - Theory behind what you practiced

**Sunday (1.5 hours): Collaboration & Tools**

**Pro Git Chapter 5: Distributed Git (45 min)**
- Pages 130-155 (Sections 5.1-5.2 only)
- **5.1: Distributed Workflows** - Different team structures
- **5.2: Contributing to a Project** - Best practices, commit guidelines

**Pro Git Chapter 7: Git Tools (45 min)**
- Pages 201-230 (Selected sections)
- **7.3: Stashing** - Saving work temporarily
- **7.6: Searching** - Finding code in history
- **7.7: Rewriting History** - When and when NOT to

**Deliverable:** Deeper understanding of Git internals, ready for advanced scenarios

-----

## Essential Git Commands Reference

### Daily Workflow
```bash
# Status and changes
git status
git diff                    # Changes not staged
git diff --staged           # Changes staged for commit

# Add and commit
git add filename
git add .                   # Add all changes
git commit -m "Message"
git commit -am "Message"    # Add and commit tracked files

# Push and pull
git pull origin main
git push origin feature-branch
git push -u origin feature-branch  # Set upstream
```

### Branching
```bash
# Create and switch
git branch feature-name              # Create
git checkout feature-name            # Switch
git checkout -b feature-name         # Create and switch
git switch feature-name              # Modern alternative
git switch -c feature-name           # Create and switch

# Merge and delete
git merge feature-name
git branch -d feature-name           # Delete (safe)
git branch -D feature-name           # Force delete

# List branches
git branch                  # Local
git branch -a               # All (including remote)
git branch -v               # With last commit
```

### Undoing Changes
```bash
# Unstage files
git restore --staged filename
git reset HEAD filename              # Old way

# Discard changes in working directory
git restore filename
git checkout -- filename             # Old way

# Amend last commit
git commit --amend
git commit --amend --no-edit         # Keep message

# Undo commits
git reset HEAD~1                     # Keep changes
git reset --hard HEAD~1              # Discard changes (DESTRUCTIVE!)
git revert HEAD                      # Create new commit that undoes
```

### Stashing
```bash
# Save work temporarily
git stash
git stash save "Description"

# List and apply
git stash list
git stash pop                        # Apply and remove
git stash apply                      # Apply and keep
git stash drop                       # Delete stash
```

### Remotes
```bash
# Remote management
git remote -v
git remote add origin URL
git remote add upstream URL
git remote remove origin

# Fetch and pull
git fetch origin
git fetch upstream
git pull origin main
git pull --rebase origin main        # Avoid merge commits
```

### History and Search
```bash
# View commits
git log
git log --oneline
git log --graph --oneline --all
git log -p                           # With diffs
git log --since=2.weeks
git log --author="Name"

# Search
git grep "search term"
git log --grep="commit message search"
git log -S "function_name"           # When code was added/removed
```

### Collaboration
```bash
# Forking workflow
git clone https://github.com/YOUR-USERNAME/repo.git
git remote add upstream https://github.com/ORIGINAL/repo.git
git fetch upstream
git merge upstream/main

# Creating PRs
git checkout -b feature/description
# Make changes
git push origin feature/description
# Create PR via GitHub UI
```

-----

## Troubleshooting Common Issues

### "Your branch is behind 'origin/main'"
```bash
git pull origin main
# Or if you have local commits:
git pull --rebase origin main
```

### "Merge conflict in file.txt"
```bash
# 1. Open conflicted file
# 2. Look for <<<<<<< HEAD and >>>>>>> markers
# 3. Edit file to resolve
# 4. Remove conflict markers
# 5. Stage and commit
git add file.txt
git commit -m "Resolve merge conflict"
```

### "I committed to wrong branch"
```bash
# If not pushed yet:
git log                              # Copy commit SHA
git checkout correct-branch
git cherry-pick <commit-SHA>
git checkout wrong-branch
git reset --hard HEAD~1              # Remove from wrong branch
```

### "I need to undo last commit but keep changes"
```bash
git reset HEAD~1
# Changes are now unstaged
```

### "I need to undo last commit completely"
```bash
git reset --hard HEAD~1              # DESTRUCTIVE!
```

### "I pushed sensitive data (API key, password)"
```bash
# 1. IMMEDIATELY rotate credentials
# 2. Contact team lead
# 3. May need to rewrite history and force push
# 4. Consider using git-secrets or pre-commit hooks
```

### "Detached HEAD state"
```bash
# You're not on a branch
# To keep changes:
git checkout -b new-branch-name

# To discard changes:
git checkout main
```

-----

## Success Metrics

### By End of Week 5:
- [ ] Completed Git Immersion (50 labs)
- [ ] Completed Learn Git Branching (all main challenges)
- [ ] Understand company Git workflow
- [ ] Created at least one pull request
- [ ] Can resolve merge conflicts
- [ ] Can use stash effectively
- [ ] Read Pro Git Chapters 2, 3, 5, 7 (selected sections)
- [ ] Confident with Git for daily work

### Skills Checklist:
- [ ] Clone, add, commit, push, pull
- [ ] Create and switch branches
- [ ] Merge branches
- [ ] Resolve conflicts
- [ ] Fork and sync repositories
- [ ] Create pull requests
- [ ] Use git stash
- [ ] Undo mistakes safely
- [ ] Search commit history
- [ ] Follow company workflow

-----

## Resources

### Primary (Hands-On):
- **[Git Immersion](https://gitimmersion.com/)** - FREE - 50 hands-on labs
- **[Learn Git Branching](https://learngitbranching.js.org/)** - FREE - Visual interactive
- **[GitHub Skills](https://skills.github.com/)** - FREE - Official GitHub tutorials

### Reference:
- **Pro Git Book** (you own this)
  - Online free version: https://git-scm.com/book/en/v2
  - Use for deep dives and reference
- **[Git Documentation](https://git-scm.com/doc)** - Official docs
- **[Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)** - Excellent guides

### Cheat Sheets:
- [GitHub Git Cheat Sheet (PDF)](https://education.github.com/git-cheat-sheet-education.pdf)
- [Atlassian Git Cheat Sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)

### Practice Projects:
- [First Timers Only](https://www.firsttimersonly.com/) - Beginner-friendly open source
- [Good First Issue](https://goodfirstissue.dev/) - Curated easy issues
- [Up For Grabs](https://up-for-grabs.net/) - Projects wanting contributions

-----

## Why This Approach Works

**Hands-On First:**
- Git Immersion: Learn by building real repos
- Learn Git Branching: Visual understanding of operations
- Muscle memory through repetition

**Reference Second:**
- Pro Git provides depth after hands-on practice
- Theory makes more sense after doing
- Use as reference throughout other tracks

**Project-Based:**
- Build real repositories
- Create actual pull requests
- Solve real merge conflicts
- Practice company workflow

**Matches Your Learning Style:**
- You prefer "learning using projects to follow along"
- Interactive tutorials > passive reading
- Do first, understand deeply second

-----

## Pro Git Reading Schedule (Reference)

Use Pro Git as reference throughout other tracks:

| When | Chapter | Topic | Why |
|------|---------|-------|-----|
| Week 5 | 2, 3, 5, 7 | Core Git | Foundation |
| Week 8 | 6 | GitHub | When starting Python projects |
| Week 18 | 8 | Customizing Git | When building AI/ML tools |
| Later | 1 | Getting Started | History and concepts |
| Later | 9 | Git Internals | Optional deep dive |

-----

## Next Steps

**After Week 5:**
- Use Git daily for all projects (Go, Python, JavaScript)
- Contribute to open source (builds portfolio)
- Practice advanced features as needed
- Reference Pro Git when stuck
- Share Git knowledge with colleagues

**Git Philosophy:**
- Commit early, commit often
- Write clear commit messages
- One logical change per commit
- Test before committing
- Pull before push
- Never force push to shared branches
- When in doubt, ask for help!

-----

## Week 5 Daily Schedule Summary

**Monday (3 hrs):** Git Immersion Labs 1-30
**Tuesday (3 hrs):** Git Immersion Labs 31-50
**Wednesday (3 hrs):** Learn Git Branching (Main Section)
**Thursday (3 hrs):** Learn Git Branching (Remote + Practice)
**Friday (3 hrs):** Company workflow + GitHub practice
**Saturday (1.5 hrs):** Pro Git Chapters 2-3 (reference reading)
**Sunday (1.5 hrs):** Pro Git Chapters 5, 7 (reference reading)

**Total: 18 hours of focused, hands-on Git mastery**
