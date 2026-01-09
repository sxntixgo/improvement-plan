# Learning Plan Review & Recommended Improvements

**Review Date:** January 9, 2026
**Focus:** Project-based learning resources alignment

-----

## Executive Summary

Your learning plan is well-structured with good sequential logic. However, I've identified several opportunities to enhance it with more project-driven resources that align better with your learning style.

**Key Findings:**
- ✅ Strong foundation with owned books
- ✅ Good sequential progression
- ⚠️ Missing several cutting-edge 2026 resources
- ⚠️ Some tracks could benefit from more hands-on platforms
- ⚠️ Limited mention of interactive CTF/lab environments

-----

## Track-by-Track Improvements

### Track 4: Python Core - **HIGH IMPACT ADDITIONS**

#### Current Resources
- Test-Driven Development with Python (Percival) - FREE ✅
- Python Testing with pytest (Okken) - $40 ✅
- Architecture Patterns with Python - FREE ✅

#### Recommended Additions

**1. TestDriven.io Courses** (Project-driven platform)
- **Why:** Real-world microservices projects with TDD
- **Projects:** Flask REST API, Docker deployment, GitLab CI
- **Cost:** Paid subscription, but extremely project-focused
- **Link:** [TestDriven.io](https://testdriven.io/)

**2. Real Python - TDD with pytest Course**
- **Why:** Video-based hands-on course
- **Focus:** Creating tests, finding bugs, performance testing
- **Cost:** Real Python subscription (~$60/year)
- **Link:** [Test-Driven Development With pytest](https://realpython.com/courses/test-driven-development-pytest/)

**3. Test Automation University - Introduction to pytest**
- **Why:** FREE, hands-on coding exercises
- **Focus:** Fixtures, parameters, plugins
- **Cost:** FREE
- **Link:** [TAU pytest Course](https://testautomationu.applitools.com/pytest-tutorial/)

**Recommendation:** Add TestDriven.io as primary resource for Weeks 5-8, keeps Percival book as theory supplement.

-----

### Track 5: AI/ML Security - **CRITICAL ADDITIONS**

#### Current Resources
- Fast.ai ✅
- OWASP LLM Top 10 ✅
- HackAPrompt ✅
- Crucible ✅

#### Recommended Additions/Updates

**1. Hack The Box Academy - AI Red Teamer Path** ⭐ NEW!
- **Why:** Official Google collaboration, comprehensive hands-on labs
- **Coverage:** Prompt injection, model privacy attacks, adversarial AI, supply chain
- **Cost:** HTB subscription (~$14-20/month)
- **Link:** [HTB AI Red Teamer Path](https://academy.hackthebox.com/course/preview/introduction-to-red-teaming-ai)

**2. NDC Security Oslo 2026 - AI Red Teaming Workshop** ⭐ UPCOMING!
- **Why:** 2-day intensive by Microsoft AI Red Team members
- **Format:** Competitive CTF-style labs with leaderboards
- **Tools:** Hands-on with PyRIT framework
- **Cost:** ~$1,000-2,000 (workshop)
- **Link:** [NDC Security Oslo](https://ndcsecurity.com/workshops/ai-red-teaming-in-practice/2b86879b0a22)
- **Note:** Check if your employer will sponsor this

**3. Certified AI Security Professional (CAISP)** ⭐ NEW!
- **Why:** 30+ browser-based labs, practical exam
- **Coverage:** Prompt injection, model theft, data poisoning
- **Cost:** Check website for pricing
- **Format:** Self-paced with certification

**4. Maven AI Red Teaming Masterclass**
- **Why:** Hands-on projects with industry guest speakers
- **Bonus:** AI/ML Red-Teaming Certification Exam
- **Link:** [Maven Masterclass](https://maven.com/learn-prompting-company/ai-red-teaming-and-ai-safety-masterclass)

**5. OffSec LLM Red Teaming Path** ⭐ NEW!
- **Why:** Offensive Security reputation
- **Focus:** LLM unbounded consumption vulnerabilities
- **Cost:** OffSec subscription

**Critical Update:** Replace Week 21-22 CTF practice with structured HTB AI Red Teamer path, then supplement with HackAPrompt and Crucible.

-----

### Track 6: JavaScript/Node.js - **MODERATE IMPROVEMENTS**

#### Current Resources
- Eloquent JavaScript ✅
- Web Development with Node and Express ✅
- YDKJS 1st edition ✅

#### Recommended Additions

**1. Zero To Mastery - Complete Node JS Developer** ⭐ HIGHLY RECOMMENDED
- **Why:** Massive project-driven course
- **Projects:**
  - NASA Space Launch application
  - Full-stack multiplayer pong game with web sockets
  - Deploy to production with Docker + AWS
- **Cost:** ~$30-40 (or subscription)
- **Link:** [ZTM Node.js](https://zerotomastery.io/courses/learn-node-js/)

**2. The Odin Project - Node.js Path**
- **Why:** Completely FREE, comprehensive, project-based
- **Projects:** APIs, web apps, deployment
- **Cost:** FREE
- **Link:** [The Odin Project](https://www.theodinproject.com/paths/full-stack-javascript/courses/nodejs)

**3. Udemy - Learn Nodejs by Building 12 Projects**
- **Why:** 12 real-world projects
- **Focus:** Express, MongoDB, JWT
- **Link:** [12 Node Projects](https://www.udemy.com/course/learn-nodejs-by-building-10-projects/)

**Recommendation:** Use Zero To Mastery as primary for Weeks 31-34 (Node.js phase), supplement with your owned books as references.

-----

### Track 7: Python Advanced - **MINOR ADDITIONS**

#### Current Resources
- Using Asyncio in Python (Fowler) ✅
- Beazley workshops ✅

#### Recommended Additions

**1. Real Python - asyncio Hands-On Walkthrough** ⭐ UPDATED 2025!
- **Why:** Updated July 2025, downloadable code, interactive quiz
- **Focus:** Practical asyncio with scaling examples
- **Cost:** Real Python subscription
- **Link:** [Real Python asyncio](https://realpython.com/async-io-python/)

**2. LambdaTest Asyncio Guide** ⭐ VERY RECENT (Jan 2025)
- **Why:** Practical weather API + web scraping examples
- **Focus:** aiohttp, asyncio.gather()
- **Cost:** FREE
- **Link:** [LambdaTest asyncio](https://www.lambdatest.com/blog/python-asyncio/)

**3. Python SAST Tools Deep Dive** ⭐ NEW for 2026
- **Why:** Hands-on with Semgrep, Bandit for custom rules
- **Focus:** Building security scanners
- **Resources:**
  - [NO Complexity SAST Guide](https://nocomplexity.com/top-sast-tools-for-2026/)
  - [Semgrep Python SAST](https://www.johal.in/devsecops-pipelines-semgrep-python-sast-scans-2026/)

**Recommendation:** Add SAST tools project in Week 45-46 - build custom Semgrep rules for common security issues.

-----

### Track 8: Go/Golang - **GOOD AS IS**

#### Current Resources
- Learning Go (Bodner) ✅
- Black Hat Go ✅
- Let's Go (Edwards) ✅
- 100 Go Mistakes ✅

#### Supplemental Resources (Free)

**1. TutorialEdge - Building Security Tools in Go**
- **Why:** Step-by-step security tool tutorials
- **Projects:** Port scanner, network tools
- **Cost:** FREE
- **Link:** [TutorialEdge Go Security](https://tutorialedge.net/projects/building-security-tools-in-go/)

**2. Awesome Go Security Collections**
- **Why:** Real-world open source projects to study
- **Repos:**
  - [awesome-go-security](https://github.com/Binject/awesome-go-security)
  - [guardrails awesome-golang-security](https://github.com/guardrailsio/awesome-golang-security)

**Recommendation:** Your current plan is solid. Add TutorialEdge as Week 59 warmup before Black Hat Go projects.

-----

### Track 2: Note-Taking (Obsidian) - **MINOR ENHANCEMENT**

#### Current Resources
- How to Take Smart Notes ✅
- Building a Second Brain ✅

#### Recommended Additions

**1. Curtis McHale's 2026 Obsidian Setup** ⭐ VERY RECENT!
- **Why:** Updated for 2026, developer-focused with code snippets
- **Focus:** PARA implementation, plugins for developers
- **Cost:** FREE
- **Link:** [2026 Obsidian Setup](https://curtismchale.ca/2025/12/29/my-2026-obsidian-setup/)

**2. Obsidian PARA Starter Kit**
- **Why:** Ready-to-use GitHub template
- **Link:** [GitHub PARA Template](https://github.com/byarbrough/obsidian-para)

**3. Sam Julien's Developer Guide**
- **Why:** Specifically for developers
- **Link:** [Get Started with Obsidian as a Developer](https://www.samjulien.com/get-started-with-obsidian-as-a-developer/)

**Recommendation:** Add these as Week 3 Sunday reading (2 hours) for practical setup examples.

-----

## New Project Ideas (Security-Focused)

Based on your security background, here are project ideas that combine multiple tracks:

### Python Projects
1. **AI-Powered SAST Tool** (Track 4 + 5 + 7)
   - Use AST parsing + LLM to explain security issues
   - Integration: pytest for testing, asyncio for scanning multiple files

2. **LLM Prompt Injection Scanner** (Track 4 + 5)
   - Automated testing of LLM applications
   - TDD approach, pytest fixtures for test cases

3. **Security Findings Aggregator** (Track 4)
   - Already in your plan - GOOD ✅

### JavaScript Projects
4. **Node.js Security Scanner API** (Track 6)
   - REST API for security scans
   - Express + security best practices
   - Integrates with Python backend

### Go Projects
5. **High-Performance Security Scanner** (Track 8)
   - Port scanner with concurrency
   - Compare performance to Python version

-----

## Budget Impact

### Current Budget: ~$270
- Python Testing with pytest: $40
- AI Engineering: $50
- Using Asyncio in Python: $50
- Learning Go: $50
- 100 Go Mistakes: $40
- Let's Go: $40

### Recommended Additions: ~$350-500 (optional)
- **HTB Academy Subscription:** ~$14-20/month × 2 months = $30-40
- **Zero To Mastery:** ~$40 (one-time) or $39/month
- **TestDriven.io:** ~$30/month × 1-2 months = $30-60
- **Real Python:** ~$60/year (covers Track 4 + 7)
- **CAISP Certification:** TBD (check website)
- **NDC Security Workshop:** ~$1,000-2,000 (employer-sponsored?)

### Cost-Optimized Approach: ~$130 additional
1. HTB Academy (2 months): $40
2. Zero To Mastery (1 month): $40
3. Real Python (1 year): $60
4. **Total:** ~$140 + existing $270 = ~$410

-----

## Platform Subscriptions Recommendation

Consider these platform subscriptions that cover multiple tracks:

1. **Real Python** (~$60/year)
   - Covers Track 4 (TDD), Track 7 (asyncio)
   - Project-based video courses
   - Interactive quizzes

2. **Hack The Box Academy** (~$20/month)
   - Essential for Track 5 (AI Red Teaming)
   - 2-month subscription = $40

3. **Zero To Mastery** (~$40 one-time)
   - Track 6 (Node.js)
   - Project-heavy

**Total subscription cost:** ~$140 for platforms covering 3 tracks

-----

## Timeline Modifications

### No Major Changes Needed
Your 62-week timeline is solid. Minor adjustments:

**Week 21-22 (Track 5):**
- **Current:** HackAPrompt + Crucible only
- **Improved:** HTB AI Red Teamer labs (structured) → HackAPrompt (practice) → Crucible (advanced)

**Week 31-34 (Track 6):**
- **Current:** Brown book only
- **Improved:** Zero To Mastery course (primary) + Brown book (reference)

**Week 45-46 (Track 7):**
- **Current:** Semgrep documentation
- **Improved:** Build 3 custom Semgrep rules for common Python security issues (portfolio piece)

-----

## Priority Ranking for Additions

### Must-Have (High ROI)
1. ✅ **HTB Academy AI Red Teamer Path** - Essential for Track 5
2. ✅ **Zero To Mastery Node.js** - Best project-based JS course
3. ✅ **Real Python Subscription** - Covers 2 tracks

### Nice-to-Have (Good ROI)
4. **TestDriven.io** - Track 4 enhancement
5. **CAISP Certification** - Track 5 credential
6. **Curtis McHale Obsidian Setup** - Track 2 practical guide

### Optional (Lower Priority)
7. NDC Security Workshop - Only if employer-sponsored
8. Maven Masterclass - Alternative to HTB if preferred
9. OffSec LLM Path - Alternative to HTB

-----

## Free Resource Highlights

Don't overlook these FREE project-based resources:

1. **The Odin Project** - Full-stack JS (Track 6)
2. **Test Automation University** - pytest (Track 4)
3. **TutorialEdge Go Security** - Go projects (Track 8)
4. **LambdaTest asyncio** - Python async (Track 7)
5. **Fast.ai** - ML fundamentals (Track 5) ✅ Already in plan
6. **HackAPrompt** - LLM security (Track 5) ✅ Already in plan

-----

## Action Items

### Immediate (Before Starting Track 1)
- [ ] Review HTB Academy AI Red Teamer path curriculum
- [ ] Check if employer will sponsor NDC Security workshop
- [ ] Compare Real Python vs TestDriven.io subscriptions
- [ ] Download PARA Obsidian starter template

### Week 4 (After Claude Code)
- [ ] Sign up for Real Python (covers Track 4 + 7)
- [ ] Evaluate Zero To Mastery for Track 6

### Week 14 (Before Track 5)
- [ ] Subscribe to HTB Academy for 2 months
- [ ] Bookmark HackAPrompt challenges
- [ ] Set up Crucible account

### Week 22 (Before Track 6)
- [ ] Start Zero To Mastery Node.js course
- [ ] Review The Odin Project as supplement

-----

## Summary

Your plan is strong, but adding these project-based platforms will significantly enhance hands-on learning:

1. **HTB Academy** for AI security → Required for competitive AI red teaming skills
2. **Zero To Mastery** for Node.js → Best project-driven JS course available
3. **Real Python** for TDD + async → Video-based, complements books well

**Estimated additional investment:** ~$140-200 (high ROI)
**Time impact:** Minimal - these replace/enhance existing reading time
**Career impact:** Substantial - hands-on labs + certifications >> books alone

-----

## Sources

### Track 4: Python Core
- [TestDriven.io](https://testdriven.io/)
- [Real Python TDD Course](https://realpython.com/courses/test-driven-development-pytest/)
- [Test Automation University pytest](https://testautomationu.applitools.com/pytest-tutorial/)
- [Class Central pytest Courses](https://www.classcentral.com/subject/pytest)

### Track 5: AI/ML Security
- [HTB Academy AI Red Teamer](https://academy.hackthebox.com/course/preview/introduction-to-red-teaming-ai)
- [NDC Security Oslo Workshop](https://ndcsecurity.com/workshops/ai-red-teaming-in-practice/2b86879b0a22)
- [Maven AI Masterclass](https://maven.com/learn-prompting-company/ai-red-teaming-and-ai-safety-masterclass)
- [OffSec LLM Red Teaming](https://www.offsec.com/learning/paths/llm-red-teaming/)
- [Bishop Fox CTF Recommendations](https://bishopfox.com/blog/ready-to-hack-an-llm-our-top-ctf-recommendations)

### Track 6: JavaScript/Node.js
- [Zero To Mastery Node.js](https://zerotomastery.io/courses/learn-node-js/)
- [The Odin Project Node.js](https://www.theodinproject.com/paths/full-stack-javascript/courses/nodejs)
- [12 Node Projects Course](https://www.udemy.com/course/learn-nodejs-by-building-10-projects/)

### Track 7: Python Advanced
- [Real Python asyncio](https://realpython.com/async-io-python/)
- [LambdaTest asyncio Guide](https://www.lambdatest.com/blog/python-asyncio/)
- [NO Complexity SAST 2026](https://nocomplexity.com/top-sast-tools-for-2026/)
- [Semgrep Python SAST](https://www.johal.in/devsecops-pipelines-semgrep-python-sast-scans-2026/)

### Track 8: Go/Golang
- [TutorialEdge Go Security](https://tutorialedge.net/projects/building-security-tools-in-go/)
- [Awesome Go Security](https://github.com/Binject/awesome-go-security)
- [Guardrails Golang Security](https://github.com/guardrailsio/awesome-golang-security)

### Track 2: Obsidian
- [Curtis McHale 2026 Setup](https://curtismchale.ca/2025/12/29/my-2026-obsidian-setup/)
- [GitHub PARA Template](https://github.com/byarbrough/obsidian-para)
- [Sam Julien Developer Guide](https://www.samjulien.com/get-started-with-obsidian-as-a-developer/)
