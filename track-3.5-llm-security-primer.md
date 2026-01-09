# Track 3.5: LLM Security Primer

**Duration:** 1 week | **Total:** 18 hours
**Weekly breakdown:** 8 hrs weekdays + 5 hrs Sat + 5 hrs Sun
**Priority:** HIGH (Security Context Before Python)

**Weekly Schedule:**
- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why Between Claude Code and Python?

This week gives you **security context** before diving into 10 weeks of Python:

- Understand LLM vulnerabilities conceptually
- See WHY you need Python for AI red teaming
- Build motivation for the technical tracks ahead
- Use your new Obsidian system to capture insights
- Practice Claude Code on security concepts

**You'll start Python Core (Week 6) knowing exactly what you're building toward.**

-----

## Book You Own

**Developer's Playbook for LLM Security** by Wilson ✅

This is THE practical guide for LLM security, covering:
- Prompt injection attacks
- Jailbreaking techniques
- Data extraction vulnerabilities
- Model inversion
- Supply chain risks
- Defense strategies

-----

## Week 5 Schedule

### Weekdays (Mon-Fri): 8 hours

**Reading Strategy:**
- Use your new speed reading skills from Track 1
- Take notes in Obsidian as you read (Track 2 practice)
- Create permanent notes for key concepts
- Link to your "AI Red Teaming" area note

**Suggested Pace:**
- **Mon-Tue (4 hrs):** Part 1 - LLM Fundamentals & Threat Landscape
  - How LLMs work (high-level)
  - Threat modeling for AI systems
  - OWASP LLM Top 10 overview

- **Wed-Thu (4 hrs):** Part 2 - Attack Techniques
  - Prompt injection (direct & indirect)
  - Jailbreaking methods
  - Training data extraction
  - Model inversion attacks
  - Data poisoning

**Key Concepts to Capture in Obsidian:**
- Prompt injection vs jailbreaking (what's the difference?)
- Direct vs indirect prompt injection
- Universal adversarial suffixes
- Training data memorization
- Model extraction techniques

-----

### Weekend: Exploration & Practice - 10 hours

**Saturday (5 hours):**

**Morning (2 hours):** Finish reading Wilson book
- Part 3 - Defense strategies
- Mitigation techniques
- Secure AI development practices

**Afternoon (3 hours):** Explore OWASP LLM Top 10
- Read all 10 vulnerability categories
- Compare with Wilson's coverage
- Create Obsidian note linking the two
- Identify which ones excite you most

**Resources:**
- [OWASP LLM Top 10](https://genai.owasp.org/) - FREE
- Create permanent notes for each vulnerability class

**Sunday (5 hours):**

**Morning (2 hours):** HackAPrompt Exploration
- Browse [HackAPrompt challenges](https://hackaprompt.com/)
- Don't try to solve yet - just explore
- Understand the types of challenges
- See what prompt injection looks like in practice

**Afternoon (3 hours):** AI Security Reading
- Read AI red teaming blog posts:
  - [HTB - AI Red Teaming Explained](https://www.hackthebox.com/blog/ai-red-teaming-explained)
  - [Mindgard - What is AI Red Teaming](https://mindgard.ai/blog/what-is-ai-red-teaming)
  - [Anthropic - AI Safety Research](https://www.anthropic.com/research)
- Watch: DEF CON AI Village talks (pick 1-2, ~1 hour)
- Take notes in Obsidian

-----

## Obsidian Note Structure for This Week

**Create these notes:**

1. **Main Area Note:** `AI-Red-Teaming.md`
   ```markdown
   # AI Red Teaming

   ## Overview
   My learning path to become an AI red teamer

   ## Key Vulnerability Classes
   - [[Prompt Injection]]
   - [[Jailbreaking]]
   - [[Training Data Extraction]]
   - [[Model Inversion]]
   - [[Data Poisoning]]

   ## Resources
   - [[Wilson LLM Security Book]]
   - [[OWASP LLM Top 10]]

   ## Skills Needed
   - Python (for exploit development)
   - Testing frameworks (pytest for AI testing)
   - Understanding ML pipelines
   ```

2. **Permanent Notes for Each Concept:**
   - `Prompt-Injection.md` - What it is, how it works, examples
   - `Jailbreaking.md` - Techniques, DAN prompts, encoding bypasses
   - `Training-Data-Extraction.md` - Memorization, model inversion
   - `OWASP-LLM-01-Prompt-Injection.md` - Link to your concept note

3. **Book Literature Note:**
   - `Wilson-LLM-Security-Book.md` - Key takeaways, quotes, page references

**By end of week:** 15-20 linked notes on LLM security

-----

## Projects & Outputs

**No coding projects this week** - this is pure learning and context-building

**Outputs:**
- Obsidian vault with 15-20 LLM security notes
- Understanding of OWASP LLM Top 10
- First blog post: "Week 5 - LLM Security Landscape Overview"

-----

## Key Questions to Answer

As you read Wilson's book, focus on answering these:

1. **What is prompt injection and why is it different from SQL injection?**
2. **What's the difference between direct and indirect prompt injection?**
3. **How does jailbreaking work and why is it so hard to prevent?**
4. **What are universal adversarial suffixes?**
5. **Why do LLMs memorize training data and how can attackers extract it?**
6. **What is model inversion and how does it threaten privacy?**
7. **How do defenders validate LLM outputs?**
8. **Why do we need Python for AI red teaming?** ← Critical question!

Write answers to these in your Obsidian notes.

-----

## Claude Code Practice

Use Claude to help you understand concepts:

**Example prompts:**
```
EXPLAIN: "Explain the difference between prompt injection and jailbreaking
in LLMs. Include concrete examples of each."

EXPLAIN: "How does indirect prompt injection work? Give me a real-world
attack scenario where an attacker uses a poisoned website."

REVIEW: "I'm reading about training data extraction attacks. Can you
explain how an attacker would actually execute this against a production
LLM like ChatGPT?"
```

**Benefit:** Practice Claude Code skills while learning security concepts

-----

## Checkpoint

Before moving to Track 4 (Python Core), you should be able to:

- ✅ Explain the OWASP LLM Top 10 vulnerability classes
- ✅ Describe how prompt injection attacks work
- ✅ Understand why jailbreaking is challenging to prevent
- ✅ Know what training data extraction means
- ✅ Articulate WHY you need Python for AI red teaming
- ✅ Have 15-20 linked notes in Obsidian on LLM security
- ✅ Feel motivated to learn Python for security tool building

-----

## What's Next?

**Week 6-15: Python Core**
- You'll learn TDD and pytest (for testing AI systems)
- Architecture patterns (for understanding ML pipelines)
- Security code review (essential for AI code)

**Every Python skill you learn will directly apply to AI red teaming:**
- pytest → Testing LLM outputs for vulnerabilities
- TDD → Building reliable security scanners
- Code review → Analyzing ML framework code
- Architecture → Understanding AI system design

**Now you know WHY you're learning Python - you've seen the security problems it will help you solve!**

-----

## Resources

### Primary
- Developer's Playbook for LLM Security (Wilson) - Already owned ✅

### Free Resources
- [OWASP LLM Top 10](https://genai.owasp.org/)
- [HackAPrompt](https://hackaprompt.com/)
- [HTB AI Red Teaming Explained](https://www.hackthebox.com/blog/ai-red-teaming-explained)
- [Mindgard AI Red Teaming Guide](https://mindgard.ai/blog/what-is-ai-red-teaming)
- [Anthropic AI Safety Research](https://www.anthropic.com/research)
- DEF CON AI Village (YouTube)

### Cost
**Total: $0** (using owned book + free resources)

-----

## Common Pitfalls to Avoid

❌ **Don't:** Try to build exploits yet - you don't have Python skills
❌ **Don't:** Skip note-taking - capturing concepts now saves time later
❌ **Don't:** Read passively - actively question and link concepts
❌ **Don't:** Rush - understanding fundamentals now accelerates Track 5

✅ **Do:** Take thorough notes in Obsidian
✅ **Do:** Link concepts together (e.g., prompt injection → OWASP LLM-01)
✅ **Do:** Use Claude Code to deepen understanding
✅ **Do:** Build excitement for Python learning ahead

-----

## Success Metrics

**Knowledge:**
- Can explain 5+ LLM vulnerability classes
- Understand attack vs defense perspectives
- Know why Python matters for AI security

**Systems:**
- 15-20 notes in Obsidian on LLM security
- Notes are linked together (knowledge graph)
- First blog post published

**Motivation:**
- Excited to start Python Core (Week 6)
- Clear vision of end goal (AI red teamer)
- Understand the path from here to there
