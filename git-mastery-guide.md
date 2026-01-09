# Git Mastery Guide - Using Pro Git Book

**Book You Own:** Pro Git by Scott Chacon and Ben Straub

**Purpose:** Git is essential throughout ALL tracks (Python, JavaScript, Go). This guide provides a progressive learning path using your Pro Git book.

**Learning Strategy:** Learn Git progressively as you need it, not all at once.

-----

## Git Learning Timeline

### Week 5 (Go Crash Course): Git Basics - 2 hours
**When:** Friday of Week 5
**Why:** Immediate need for work contributions
**Pro Git:** Chapter 2 (Git Basics)
**Focus:** Daily workflow commands

### Week 7 (Python Core Start): Branching - 1 hour
**When:** Sunday of Week 7
**Why:** Managing Python projects and experiments
**Pro Git:** Chapter 3 (Git Branching)
**Focus:** Feature branches, merging

### Week 10 (Mid Python Core): Collaboration - 1 hour
**When:** Sunday of Week 10
**Why:** Contributing to open source, portfolio projects
**Pro Git:** Chapter 5 (Distributed Git)
**Focus:** Forking, pull requests, code review

### Week 16 (Before AI/ML): Advanced Topics - 1 hour
**When:** Sunday of Week 16
**Why:** Managing complex projects, undoing mistakes
**Pro Git:** Chapter 7 (Git Tools)
**Focus:** Stashing, rewriting history, debugging

### Ongoing: Reference as Needed
**Chapters 6, 8-10:** GitHub, server setup, internals (reference when needed)

-----

## Chapter 2: Git Basics (Week 5 - Friday)

**Time:** 2 hours
**Priority:** HIGH - Essential for work

### What to Read (Pages 18-52)

**Section 2.1: Getting a Git Repository (15 min)**
```bash
# Initialize new repo
git init

# Clone existing repo
git clone https://github.com/user/repo.git
```

**Section 2.2: Recording Changes (30 min) - MOST IMPORTANT**

**The Four File States:**
1. Untracked - Not in Git
2. Unmodified - Tracked, no changes
3. Modified - Changed but not staged
4. Staged - Ready to commit

**Essential Commands:**
```bash
# Check status
git status

# Stage files
git add filename.go
git add .              # Stage all

# Commit
git commit -m "Clear, descriptive message"

# Skip staging area (use carefully)
git commit -a -m "Message"

# Remove files
git rm filename.go
git rm --cached file   # Keep file but untrack it

# Move/rename files
git mv old_name.go new_name.go
```

**Section 2.3: Viewing Commit History (20 min)**
```bash
# View commits
git log
git log --oneline              # Condensed
git log --graph --oneline      # Visual branch structure
git log -p -2                  # Last 2 commits with diffs
git log --since=2.weeks        # Time-based filtering
git log --author="Your Name"   # By author
```

**Section 2.4: Undoing Things (30 min) - CRITICAL**
```bash
# Amend last commit (add forgotten file or fix message)
git commit --amend

# Unstage a file
git reset HEAD filename.go

# Discard changes in working directory (DESTRUCTIVE!)
git checkout -- filename.go

# Better alternative (Git 2.23+)
git restore --staged filename.go    # Unstage
git restore filename.go              # Discard changes
```

**Section 2.5: Working with Remotes (20 min)**
```bash
# View remotes
git remote -v

# Add remote
git remote add origin https://github.com/user/repo.git

# Fetch (download but don't merge)
git fetch origin

# Pull (fetch + merge)
git pull origin main

# Push
git push origin main
git push -u origin feature-branch  # Set upstream
```

**Section 2.6: Tagging (5 min) - SKIP for now**
Read later when you need releases

**Section 2.7: Git Aliases (5 min) - OPTIONAL**
```bash
# Useful shortcuts
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status
```

### Week 5 Exercises (30 min)

**After reading Chapter 2, practice:**

1. **Create test repository** (10 min)
```bash
mkdir git-practice
cd git-practice
git init
echo "# Git Practice" > README.md
git add README.md
git commit -m "Initial commit"
```

2. **Practice workflow** (15 min)
```bash
# Create file
echo "Hello Git" > test.txt
git status
git add test.txt
git commit -m "Add test file"

# Modify file
echo "More content" >> test.txt
git status
git diff
git add test.txt
git commit -m "Update test file"

# View history
git log --oneline
```

3. **Practice undoing** (5 min)
```bash
# Make a mistake
echo "Oops" >> test.txt
git status

# Undo it
git restore test.txt
git status
```

### Week 5 Deliverable
- [ ] Read Pro Git Chapter 2 (Git Basics)
- [ ] Completed practice exercises
- [ ] Can: clone, add, commit, push, pull
- [ ] Understand: staging area, commit history, undoing changes

-----

## Chapter 3: Git Branching (Week 7 - Sunday)

**Time:** 1 hour
**Priority:** HIGH - Essential for feature development

### What to Read (Pages 53-90)

**Section 3.1: Branches in a Nutshell (20 min)**

**Key Concept:** Branches are lightweight pointers to commits

```bash
# Create branch
git branch feature-name

# Switch to branch
git checkout feature-name

# Create and switch (shortcut)
git checkout -b feature-name

# Modern alternative (Git 2.23+)
git switch feature-name
git switch -c feature-name  # Create and switch
```

**Section 3.2: Basic Branching and Merging (25 min) - MOST IMPORTANT**

**Workflow:**
```bash
# Start new feature
git checkout -b feature/add-login

# Make changes
git add .
git commit -m "Add login form"

# Switch back to main
git checkout main

# Merge feature
git merge feature/add-login

# Delete merged branch
git branch -d feature/add-login
```

**Handling Merge Conflicts:**
```bash
# When merge has conflicts
git merge feature-branch
# CONFLICT in file.py

# Open file, resolve conflicts
# Look for <<<<<<< HEAD markers
# Choose which code to keep
# Remove conflict markers

# Mark as resolved
git add file.py
git commit -m "Merge feature-branch, resolve conflicts"
```

**Section 3.3: Branch Management (10 min)**
```bash
# List branches
git branch              # Local branches
git branch -v           # With last commit
git branch -a           # Include remote branches

# See merged/unmerged
git branch --merged
git branch --no-merged

# Delete branch
git branch -d branch-name   # Safe delete (merged only)
git branch -D branch-name   # Force delete
```

**Section 3.4-3.5: Branching Workflows (5 min) - SKIM**
Read about common workflows:
- Long-running branches (main, develop)
- Topic branches (feature, bugfix)

**Section 3.6: Remote Branches (15 min)**
```bash
# Push branch to remote
git push origin feature-branch
git push -u origin feature-branch  # Set upstream

# Track remote branch
git checkout -b feature origin/feature

# Modern alternative
git switch -c feature origin/feature

# Delete remote branch
git push origin --delete feature-branch
```

**Section 3.7: Rebasing (SKIP for now)**
Read later when comfortable with merging

### Week 7 Exercises (15 min)

**Practice branching workflow:**
```bash
# Create feature branch
git checkout -b feature/test-feature

# Make changes
echo "Feature code" > feature.py
git add feature.py
git commit -m "Add feature"

# Switch to main
git checkout main

# Merge feature
git merge feature/test-feature

# Delete branch
git branch -d feature/test-feature
```

### Week 7 Deliverable
- [ ] Read Pro Git Chapter 3 (Branching)
- [ ] Can create and switch branches
- [ ] Can merge branches
- [ ] Can resolve merge conflicts
- [ ] Understand feature branch workflow

-----

## Chapter 5: Distributed Git (Week 10 - Sunday)

**Time:** 1 hour
**Priority:** MEDIUM - For collaboration

### What to Read (Pages 130-167)

**Section 5.1: Distributed Workflows (10 min) - SKIM**
Understand different team workflows:
- Centralized workflow
- Integration-manager workflow
- Dictator and lieutenants workflow

**Section 5.2: Contributing to a Project (30 min) - IMPORTANT**

**Forking Workflow:**
```bash
# 1. Fork repository on GitHub (web UI)

# 2. Clone YOUR fork
git clone https://github.com/YOUR-USERNAME/repo.git

# 3. Add upstream remote
git remote add upstream https://github.com/ORIGINAL-OWNER/repo.git

# 4. Keep your fork synced
git fetch upstream
git checkout main
git merge upstream/main

# 5. Create feature branch
git checkout -b feature/my-contribution

# 6. Make changes and commit
git add .
git commit -m "Add my contribution"

# 7. Push to YOUR fork
git push origin feature/my-contribution

# 8. Create Pull Request (web UI)
```

**Commit Guidelines:**
- Clear, descriptive commit messages
- One logical change per commit
- Test before committing
- Follow project's contribution guidelines

**Section 5.3: Maintaining a Project (20 min) - SKIM**
Read if you maintain open source projects:
- Reviewing pull requests
- Merging contributions
- Tagging releases

### Week 10 Exercises (15 min)

**Practice forking workflow:**
1. Fork a small open source project
2. Clone your fork
3. Add upstream remote
4. Create feature branch
5. Make small change (fix typo, update docs)
6. Push to your fork
7. Create pull request

### Week 10 Deliverable
- [ ] Read Pro Git Chapter 5 (Distributed Git)
- [ ] Understand forking workflow
- [ ] Can sync fork with upstream
- [ ] Created at least one pull request
- [ ] Understand contribution guidelines

-----

## Chapter 7: Git Tools (Week 16 - Sunday)

**Time:** 1 hour
**Priority:** MEDIUM - Advanced topics

### What to Read (Pages 201-270)

**Section 7.1: Revision Selection (10 min)**
```bash
# Specify commits
git show HEAD           # Latest commit
git show HEAD~2         # 2 commits ago
git show main~3         # 3 commits back on main
git show abc1234        # By SHA hash

# Ranges
git log main..feature   # Commits in feature not in main
```

**Section 7.2: Interactive Staging (10 min)**
```bash
# Interactively stage parts of files
git add -p

# Useful for committing related changes separately
```

**Section 7.3: Stashing (15 min) - VERY USEFUL**
```bash
# Save work temporarily
git stash

# List stashes
git stash list

# Apply stash
git stash pop            # Apply and remove
git stash apply          # Apply and keep

# Stash with message
git stash save "Work in progress on feature X"

# Apply specific stash
git stash apply stash@{1}

# Drop stash
git stash drop stash@{0}
```

**Section 7.4: Cleaning (5 min)**
```bash
# Remove untracked files (DESTRUCTIVE)
git clean -n     # Dry run (shows what would be deleted)
git clean -f     # Actually delete
git clean -fd    # Include directories
```

**Section 7.5: Signing Work (SKIP)**
Read if you need GPG signing

**Section 7.6: Searching (10 min)**
```bash
# Search code
git grep "function_name"
git grep -n "TODO"      # With line numbers

# Search commit messages
git log --grep="fix bug"

# Search code in history
git log -S "function_name"  # When function was added/removed
```

**Section 7.7: Rewriting History (15 min) - USE WITH CAUTION**
```bash
# Amend last commit
git commit --amend

# Interactive rebase (reorder, squash, edit commits)
git rebase -i HEAD~3

# NEVER rewrite history that's been pushed and shared!
```

**Section 7.8-7.14: Advanced Topics (5 min each) - SKIM**
- Reset Demystified
- Merging strategies
- Rerere (Reuse Recorded Resolution)
- Debugging with Git
- Submodules
- Bundling
- Replace

### Week 16 Deliverable
- [ ] Read Pro Git Chapter 7 (Git Tools)
- [ ] Can use git stash effectively
- [ ] Can search code and history
- [ ] Understand when NOT to rewrite history
- [ ] Know where to look for advanced features

-----

## Reference: Essential Git Commands

### Daily Workflow
```bash
# Status and changes
git status
git diff
git diff --staged

# Add and commit
git add filename
git add .
git commit -m "Message"

# Push and pull
git pull origin main
git push origin feature-branch
```

### Branching
```bash
# Branch management
git branch                    # List
git branch feature-name       # Create
git checkout feature-name     # Switch
git checkout -b feature-name  # Create and switch
git branch -d feature-name    # Delete

# Merging
git merge feature-name
```

### Undoing
```bash
# Unstage
git restore --staged filename

# Discard changes
git restore filename

# Amend commit
git commit --amend

# Stash
git stash
git stash pop
```

### Remote
```bash
# Remote management
git remote -v
git remote add origin URL
git fetch origin
git pull origin main
git push origin main
```

### History
```bash
# View commits
git log
git log --oneline
git log --graph --oneline
git log -p

# Search
git grep "search term"
git log --grep="commit message search"
```

-----

## Company-Specific Git Workflow

**Week 5 Friday: Learn your company's workflow**

### Questions to Ask Team Lead:
1. What branching strategy? (GitFlow, GitHub Flow, trunk-based?)
2. Branch naming convention? (feature/, bugfix/, hotfix/?)
3. Commit message format? (Conventional Commits?)
4. Pull request process?
5. Code review requirements?
6. Any Git hooks or pre-commit checks?
7. Main branch name? (main, master, develop?)

### Common Workflows:

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
6. # After approval, merge to develop
7. # Release: merge develop → release → main
```

-----

## Troubleshooting Common Issues

### "Your branch is behind 'origin/main'"
```bash
git pull origin main
# Or if you have local commits:
git pull --rebase origin main
```

### "Merge conflict"
```bash
# 1. Open conflicted file
# 2. Look for <<<<<<< and >>>>>>> markers
# 3. Edit file to resolve
# 4. Remove markers
# 5. Stage and commit
git add filename
git commit -m "Resolve merge conflict"
```

### "I committed to wrong branch"
```bash
# If not pushed yet:
git log  # Copy commit SHA
git checkout correct-branch
git cherry-pick <commit-SHA>
git checkout wrong-branch
git reset --hard HEAD~1  # Remove commit from wrong branch
```

### "I need to undo last commit"
```bash
# Keep changes (unstage)
git reset HEAD~1

# Discard changes (DESTRUCTIVE)
git reset --hard HEAD~1
```

### "I pushed sensitive data"
```bash
# Contact team lead immediately!
# May need to rewrite history and force push
# Or rotate credentials if exposed
```

-----

## Pro Git Book Reading Schedule

| Week | Chapter | Topic | Time | When |
|------|---------|-------|------|------|
| 5 | 2 | Git Basics | 2 hrs | Friday |
| 7 | 3 | Branching | 1 hr | Sunday |
| 10 | 5 | Distributed Git | 1 hr | Sunday |
| 16 | 7 | Git Tools | 1 hr | Sunday |
| Later | 1 | Getting Started | 30 min | Reference |
| Later | 4 | Git Server | Skip | Unless managing servers |
| Later | 6 | GitHub | 1 hr | If using GitHub Enterprise features |
| Later | 8 | Customizing Git | 30 min | When needed |
| Later | 9 | Git Internals | 1 hr | Optional deep dive |
| Later | 10 | Appendices | - | Reference |

-----

## Success Metrics

### After Week 5 (Git Basics):
- [ ] Can clone, add, commit, push, pull
- [ ] Understand staging area
- [ ] Can view and search commit history
- [ ] Can undo mistakes safely

### After Week 7 (Branching):
- [ ] Can create and switch branches
- [ ] Can merge branches
- [ ] Can resolve merge conflicts
- [ ] Understand feature branch workflow

### After Week 10 (Collaboration):
- [ ] Can fork repositories
- [ ] Can sync fork with upstream
- [ ] Can create pull requests
- [ ] Understand code review process

### After Week 16 (Advanced):
- [ ] Can use git stash effectively
- [ ] Can search code and history
- [ ] Know advanced Git features
- [ ] Confident with Git for all projects

-----

## Additional Resources

**Free Online:**
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Skills](https://skills.github.com/)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)
- [Learn Git Branching](https://learngitbranching.js.org/) - Interactive visual tutorial

**Your Book:**
- Pro Git (free online): https://git-scm.com/book/en/v2
- Pro Git (your physical copy): Use for deep reading

**Cheat Sheets:**
- [GitHub Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [Atlassian Git Cheat Sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)

-----

## Remember

**Git Philosophy:**
- Commit early, commit often
- Write clear commit messages
- One logical change per commit
- Test before committing
- Pull before push
- Never force push to shared branches
- When in doubt, ask for help!

**Pro Git is your reference** - you don't need to memorize everything. Learn the basics, then look up advanced features when you need them.
