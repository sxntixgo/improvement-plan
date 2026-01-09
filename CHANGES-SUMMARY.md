# Changes Summary - January 9, 2026

## What Changed

Your learning plan has been updated based on your security focus and to better integrate theoretical and practical learning.

-----

## New Structure

### Before
```
Week 1:    Reading Skills
Week 2-3:  Note-Taking (Obsidian)
Week 4:    Claude Code
Week 5-14: Python Core
Week 15-22: AI/ML Security (with Wilson book)
...
Total: 62 weeks
```

### After
```
Week 1:    Reading Skills
Week 2-3:  Note-Taking (Obsidian) ← Improved hands-on approach
Week 4:    Claude Code ← More concrete practice examples
Week 5:    LLM Security Primer (Wilson book) ← NEW!
Week 6-15: Python Core
Week 16-23: AI/ML Security (HTB Academy + Huyen) ← Updated
...
Total: 63 weeks
```

-----

## Track 3.5: LLM Security Primer (NEW)

**Week:** 5
**Duration:** 18 hours
**Cost:** $0 (using owned Wilson book)

**Why Added:**
- Provides security context BEFORE learning Python
- Answers "Why am I learning Python?" before diving in
- Builds motivation for technical tracks
- Practice using Obsidian system for security concepts

**What You'll Do:**
- Read Wilson's "Developer's Playbook for LLM Security"
- Explore OWASP LLM Top 10
- Browse HackAPrompt challenges (don't solve yet)
- Create 15-20 Obsidian notes on LLM vulnerabilities
- Watch AI red teaming talks
- Write first blog post on LLM security landscape

**Deliverables:**
- Understanding of: prompt injection, jailbreaking, data extraction, model inversion
- Obsidian notes linking concepts together
- Clear motivation for why Python matters for AI security

-----

## Track 2: Obsidian - Improved Approach

**Changed:** Now install Obsidian on Week 2, Day 1 (Monday morning)

**Why:** Meta-learning - use the system while learning about it

**Old Approach:**
- Week 2: Read book → then install Obsidian on Saturday
- By end of week: No notes created yet

**New Approach:**
- Week 2, Monday: Install Obsidian first (30 min)
- Week 2, Mon-Fri: Take notes IN Obsidian while reading
- By end of week: 10-15 actual notes created

**Result:** Hands-on from Day 1, real practice instead of theory

-----

## Track 3: Claude Code - More Concrete

**Added:**
- Specific prompt templates for all 7 patterns
- Time allocation (40 min per pattern)
- Suggested repos for practice (Flask, Requests)
- Concrete examples instead of abstract patterns

**Example before:**
```
REVIEW - "Review this code for security issues"
```

**Example after:**
```
REVIEW (40 min)
Prompt: "Review this code for:
- Security vulnerabilities
- Performance issues
- Best practice violations
File: [path]"
```

-----

## Track 5: AI/ML Security - Major Update

### Resources Changed

**Removed from active reading:**
- ❌ Wilson book (moved to Track 3.5)

**Added:**
- ✅ HTB Academy AI Red Teamer Path ($20/month × 2 = $40)

**Kept:**
- ✅ Huyen "AI Engineering" book ($50)
- ✅ Fast.ai, Hugging Face (free)
- ✅ HackAPrompt, Crucible (free)

### Phase Structure Updated

**Phase 1 (Weeks 16-17): ML Fundamentals**
- Same as before: Fast.ai + Hugging Face
- Note: You already know vulnerabilities from Track 3.5

**Phase 2 (Weeks 18-19): HTB Academy Labs** ← NEW PRIMARY FOCUS
- Hands-on labs attacking real AI systems
- Build prompt injection exploits with Python
- Execute model privacy attacks
- Document findings professionally

**Phase 3 (Weeks 20-21): Adversarial ML + Production**
- NVIDIA course (optional) OR free Hugging Face tutorials
- Huyen book: Focus on security chapters (7-10 only, not cover-to-cover)

**Phase 4 (Weeks 22-23): Advanced Red Teaming**
- HackAPrompt challenges
- Crucible CTF
- HTB Academy capstone project

### Why This Is Better

**Before:**
- Week 17-18: Read Wilson book (theory)
- Week 21-22: Do CTF challenges (jump from theory to hard practice)
- Gap between learning and application

**After:**
- Week 5: Read Wilson book (early context)
- Week 18-19: HTB Academy (structured hands-on)
- Week 22-23: Advanced CTF (after building skills)
- Progressive difficulty curve

**Result:**
- Theory → Guided practice → Independent challenges
- Better skill progression
- HTB Academy provides structure between theory and CTF

-----

## Timeline Impact

All tracks after Week 4 shift by 1 week:

|Track|Old Weeks|New Weeks|Change|
|-----|---------|---------|------|
|1    |1        |1        |None  |
|2    |2-3      |2-3      |None  |
|3    |4        |4        |None  |
|3.5  |—        |5        |NEW   |
|4    |5-14     |6-15     |+1    |
|5    |15-22    |16-23    |+1    |
|6    |23-42    |24-43    |+1    |
|7    |43-50    |44-51    |+1    |
|8    |51-62    |52-63    |+1    |

**Total:** 62 weeks → 63 weeks (+1 week)

-----

## Cost Impact

### Original Plan
- Books to buy: $270
- Courses: $0
- **Total: $270**

### Updated Plan
- Books to buy: $220 (skip Huyen? Or keep it - your choice)
  - Okken (pytest): $40
  - Huyen (AI Engineering): $50 ← Kept per your request
  - Fowler (asyncio): $50
  - Go books: $130
- Courses to add: $40 (HTB Academy 2 months)
- **Total: $260** (-$10 if you keep all books)

**If you follow the optimization guide (courses > books):**
- Books: $170
- Courses: $220 (Real Python, TestDriven.io, HTB, ZTM)
- **Total: $390** (+$120 but way more hands-on)

-----

## Key Benefits

### 1. Better Motivation
- Week 5: See WHY you need Python for AI security
- Week 6+: Learn Python knowing exactly what you'll build
- Week 16+: Apply Python to AI security with clear purpose

### 2. Progressive Learning
```
Theory (Week 5 Wilson) →
Fundamentals (Week 6-15 Python) →
Guided Practice (Week 18-19 HTB) →
Independent Challenges (Week 22-23 CTF)
```

### 3. More Hands-On
- Obsidian: Practice while learning (not after)
- Claude Code: Specific prompts (not vague patterns)
- AI Security: HTB labs (not just books)

### 4. Better Portfolio
- HTB Academy completion/certification
- Python-based security tools
- Professional red team reports
- Blog posts throughout

-----

## What to Do Now

### Immediate (Before Week 1)
- ✅ You have all the files updated
- ✅ Track 3.5 is ready to use
- ✅ No purchases needed yet

### Week 5 (Track 3.5)
- ✅ Use Wilson book you already own
- ✅ Free resources (OWASP, HackAPrompt browsing)
- ✅ Practice Obsidian note-taking
- ✅ Cost: $0

### Before Week 16 (Track 5)
- Decide: Keep Huyen book ($50) or skip and use HTB only
- Subscribe to HTB Academy ($20/month × 2 = $40)
- Total investment: $40-90

### Optional: Course Optimization
- Review `BOOKS-VS-COURSES-OPTIMIZATION.md`
- Consider adding courses for Tracks 4, 6, 7
- Decisions can wait until you reach those tracks

-----

## Files Updated

1. **README.md** - Priority order table updated
2. **track-3.5-llm-security-primer.md** - New track added
3. **track-05-ai-ml-security.md** - Updated with HTB Academy focus
4. **GETTING-STARTED-TRACKS-1-3.md** - Improved Obsidian/Claude Code approach

-----

## Questions?

**"Should I buy Huyen's book?"**
- If you want comprehensive production AI knowledge: Yes ($50)
- If HTB Academy hands-on is enough: No (save $50)
- Decision point: Week 15 (before Track 5 starts)

**"Is 63 weeks too long?"**
- 1 extra week is minimal
- The security context in Week 5 saves time later
- Better to learn right than learn fast

**"Can I skip Track 3.5?"**
- Technically yes, but not recommended
- It's only 1 week and uses a book you own
- The motivation boost is worth it

**"Do I need HTB Academy?"**
- For AI red teaming: Highly recommended
- Best hands-on platform for 2026
- Only $40 for 2 months
- Certification potential adds resume value

-----

## Next Steps

1. ✅ Start Track 1 (Reading Skills) - Week 1
2. ✅ All materials ready through Week 5
3. ✅ Week 5: Use Wilson book (already owned)
4. Decide on Huyen book by Week 15
5. Subscribe to HTB Academy by Week 15

**You're all set to begin!**
