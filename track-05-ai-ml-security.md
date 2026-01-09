# Track 5: AI/ML Security

**Duration:** 8 weeks | **Hours/week:** 18 | **Priority:** HIGH
**Goal:** AI red teaming skills

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Phase Overview

|Phase|Weeks|Focus                   |
|-----|-----|------------------------|
|1    |16-17|ML Fundamentals         |
|2    |18-19|HTB Academy Labs        |
|3    |20-21|Adversarial ML          |
|4    |22-23|Advanced Red Teaming    |

-----

## Resources

### Primary Platform

|Resource             |Cost        |Focus                           |
|---------------------|------------|--------------------------------|
|HTB Academy AI Red Teamer|~$20/month × 2|Hands-on labs, prompt injection, model attacks|

### Free Resources

|Resource          |URL                  |Focus                    |
|------------------|---------------------|-------------------------|
|Fast.ai           |fast.ai              |ML fundamentals          |
|Hugging Face NLP  |huggingface.co/learn |Transformers, NLP        |
|OWASP LLM Top 10  |genai.owasp.org      |LLM vulnerabilities      |
|HackAPrompt       |hackaprompt.com      |Prompt injection practice|
|Dreadnode/Crucible|crucible.dreadnode.io|CTF-style challenges     |

### Books

|Resource                                      |Cost         |Status/Focus              |
|----------------------------------------------|-------------|--------------------------|
|Developer's Playbook for LLM Security (Wilson)|Already owned|✅ Read in Track 3.5      |
|AI Engineering (Huyen)                        |~$50         |Production AI systems     |
|Red Teaming AI (Dursey)                       |~$50         |Red teaming (July 2026)   |

### Optional Paid Courses

|Resource             |Cost|Focus                 |Note                     |
|---------------------|----|----------------------|-------------------------|
|NVIDIA Adversarial ML|$90 |Adversarial techniques|Optional - can use free resources|

-----

## Phase 1: ML Fundamentals (Weeks 16-17)

|Week|Focus                                |Resource               |
|----|-------------------------------------|-----------------------|
|16  |Deep Learning basics, neural networks|Fast.ai Part 1         |
|17  |NLP, transformers, attention         |Hugging Face NLP Course|

**Note:** You already understand LLM vulnerabilities from Track 3.5 (Wilson book). Now you're building the ML foundation to exploit them.

-----

## Phase 2: HTB Academy AI Red Teamer Labs (Weeks 18-19)

**Primary Resource:** HTB Academy AI Red Teamer Path (~$20/month subscription)

|Week|Focus                                |HTB Modules                      |
|----|-------------------------------------|---------------------------------|
|18  |Prompt injection, jailbreaking       |HTB: Introduction to Red Teaming AI, Prompt Injection labs|
|19  |Model privacy attacks, adversarial AI|HTB: Model extraction, Data poisoning labs|

**What You'll Do:**
- Complete hands-on labs attacking real AI systems
- Build prompt injection exploits (using Python from Track 4!)
- Test jailbreaking techniques against LLMs
- Execute model privacy attacks
- Document findings in Obsidian

**Key Skills Developed:**
- Practical exploitation (not just theory)
- Python for AI security tooling
- Attack documentation and reporting
- Defensive recommendations

**Supplement with OWASP LLM Top 10:** Review concepts as you encounter them in labs

-----

## Phase 3: Production LLM Apps & Adversarial ML (Weeks 20-21)

|Week|Focus                                 |Resource                    |
|----|--------------------------------------|----------------------------|
|20  |**LangChain security, RAG attacks**   |**LangChain docs + build vulnerable app**|
|21  |Adversarial ML & production systems   |AI Engineering (Huyen) Ch 7-10 + NVIDIA (optional)|

**Week 20: LangChain Security - NEW CRITICAL ADDITION**

**Why This Week:**
- Most production LLM apps use LangChain or similar frameworks
- RAG (Retrieval Augmented Generation) is everywhere
- Agent-based systems have unique vulnerabilities
- You need to understand the framework to attack it effectively

**What You'll Learn:**
- LangChain basics: Chains, Agents, Memory, Tools
- RAG architecture and attack surfaces
- How to build a vulnerable LLM app (to then attack it)
- Prompt injection in multi-step chains
- RAG poisoning techniques
- Agent exploitation

**Hands-On Project:**
1. Build a simple RAG app with LangChain (8 hours)
   - Document QA system with vector database
   - LLM agent with tools (calculator, search, etc.)
   - Conversational memory
2. Attack your own app (10 hours)
   - Inject malicious documents into RAG
   - Manipulate agent behavior
   - Exploit chain vulnerabilities
   - Document findings in Obsidian

**Free Resources:**
- [LangChain Documentation](https://python.langchain.com/) - Official docs
- [LangChain Security Best Practices](https://python.langchain.com/docs/security)
- Build and break tutorial (hands-on)

**Week 21: Adversarial ML & Production**
- NVIDIA Adversarial ML (optional) OR Free: Hugging Face tutorials
- AI Engineering (Huyen) - Focus on Ch 7-10 (Safety, Security, Testing)

-----

## Phase 4: Advanced Red Teaming & CTF (Weeks 22-23)

|Week|Focus                        |Resource             |
|----|-----------------------------|---------------------|
|22  |HackAPrompt challenges       |hackaprompt.com      |
|23  |Crucible CTF + HTB capstone  |crucible.dreadnode.io + HTB final project|

**Week 22: HackAPrompt**
- Complete as many levels as possible
- Use Python skills to automate attacks
- Document successful prompts in Obsidian
- Blog post: "My HackAPrompt Solutions"

**Week 23: Advanced Challenges**
- Crucible CTF challenges
- HTB Academy capstone project (if available)
- Build final portfolio piece: Full AI red team assessment

-----

## Projects & Outputs

|Project                      |Output                               |Share             |
|-----------------------------|-------------------------------------|------------------|
|HTB Academy lab completions  |All modules completed                |HTB profile       |
|Prompt injection PoC (Python)|Working exploit with automation      |GitHub            |
|**Vulnerable LangChain app** |**RAG app + attack documentation**   |**GitHub + Blog** |
|**RAG poisoning exploit**    |**Inject malicious docs into vector DB**|**GitHub**     |
|HackAPrompt solutions        |Documented attack strategies         |Blog post + GitHub|
|Red team assessment          |Full AI security assessment report   |Blog post         |
|Jailbreak taxonomy           |Categorized attack techniques        |GitHub            |

-----

## Key Concepts

**You already learned these in Track 3.5 (Wilson book):**
- Prompt Injection (direct vs indirect)
- Jailbreaking techniques
- Training data extraction
- Model inversion
- Data poisoning

**New in Track 5 - Production LLM Security:**
- **RAG Architecture:** How Retrieval Augmented Generation works
- **RAG Poisoning:** Injecting malicious documents into vector databases
- **Chain Manipulation:** Exploiting multi-step LLM workflows
- **Agent Exploits:** Making LLM agents call unintended tools
- **Memory Attacks:** Corrupting conversation history
- **LangChain Security:** Framework-specific vulnerabilities

**Now you're applying them hands-on:**
- Building exploits with Python
- Testing real AI systems in HTB labs
- Building AND attacking LangChain apps
- RAG poisoning techniques
- Agent manipulation
- Automating attacks
- Writing security assessments
- Defensive recommendations

-----

## Checkpoint

Before moving to JavaScript (Track 6), you should be able to:

- ✅ Complete HTB Academy AI Red Teamer modules
- ✅ Build prompt injection exploits using Python
- ✅ **Build a LangChain RAG application from scratch**
- ✅ **Execute RAG poisoning attacks**
- ✅ **Exploit LLM agents and manipulate tool usage**
- ✅ Execute jailbreaking attacks against LLMs
- ✅ Document security findings professionally
- ✅ Provide defensive recommendations
- ✅ Solve HackAPrompt challenges
- ✅ Conduct full AI security assessment
- ✅ Explain adversarial ML attack vectors

**Portfolio pieces:**
- HTB Academy certification/completion (if available)
- **Vulnerable LangChain app + attack write-up** ← NEW
- **RAG poisoning PoC** ← NEW
- 3-5 blog posts on AI security
- GitHub repo with security tools and PoCs
- Professional red team assessment report
