# Track 10: AI/ML Security

**Duration:** 8 weeks | **Hours/week:** 18 | **Priority:** HIGH — THIS IS YOUR CAREER GOAL
**Goal:** AI red teaming skills — understand AI systems deeply enough to find and exploit their vulnerabilities

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Why Right After Architecture?

You just spent 12 weeks learning software architecture (Track 8). Now you apply that systems thinking to AI:

- **You understand system architecture** — RAG, agents, and production AI are systems with components, interfaces, and attack surfaces
- **You don't need Python syntax first** — Claude Code writes the Python for labs, scripts, and exploit code. You focus on understanding concepts and finding vulnerabilities
- **Architecture knowledge maps to AI systems** — dependency injection, service layers, and API design are how production AI systems are built. You already know how to think about them

**Your role as architect:** You study how AI systems work, identify architectural weaknesses, and direct Claude Code to build exploit tools and vulnerable test applications. You don't type Python — you think like a red teamer.

-----

## Phase Overview

|Phase|Weeks|Focus                           |AI Engineering Chapters|
|-----|-----|--------------------------------|-----------------------|
|1    |21-22|ML Fundamentals                 |Ch 2: Foundation Models|
|2    |23-24|HTB Academy Labs                |-                      |
|3    |25-26|RAG/Agents + Supply Chain       |Ch 5-6: Prompt Eng + RAG|
|4    |27-28|Evaluation + Advanced CTF       |Ch 3-4, 7, 9-10        |

**AI Engineering Book Usage (7 chapters, ~18 hours):**
- **Week 22:** Ch 2 (Foundation Models) - 4 hrs
- **Week 25:** Ch 6 (RAG and Agents) - 4 hrs CRITICAL
- **Week 26:** Ch 5 (Prompt Engineering) - 4 hrs CRITICAL for attacks
- **Week 27:** Ch 3-4 (Evaluation) + Ch 7, 10 (skim) - 8 hrs
- **Optional:** Ch 9 (Inference Optimization) — reference reading, not required

**Note:** Phase 5 (Go for AI Security) has moved to Track 11 as the capstone, where Go architecture skills + AI security knowledge combine.

-----

## Resources

### Primary Platform

|Resource             |Cost        |Focus                           |
|---------------------|------------|--------------------------------|
|HTB Academy AI Red Teamer|~$20/month x 2|Hands-on labs, prompt injection, model attacks|

### Free Resources

|Resource          |URL                  |Focus                    |
|------------------|---------------------|-------------------------|
|Fast.ai           |fast.ai              |ML fundamentals          |
|Hugging Face NLP  |huggingface.co/learn |Transformers, NLP        |
|OWASP LLM Top 10  |genai.owasp.org      |LLM vulnerabilities      |
|MITRE ATLAS       |atlas.mitre.org      |Adversarial ML threat framework (ATT&CK for AI)|
|HackAPrompt       |hackaprompt.com      |Prompt injection practice|
|Dreadnode/Crucible|crucible.dreadnode.io|CTF-style challenges     |

### Books

|Resource                                      |Cost         |Status/Focus              |
|----------------------------------------------|-------------|--------------------------|
|Developer's Playbook for LLM Security (Wilson)|Already owned|Read in Track 7           |
|AI Engineering (Huyen)                        |~$50         |Production AI systems     |
|Red Teaming AI (Dursey)                       |Already owned|Red teaming               |

-----

## Phase 1: ML Fundamentals (Weeks 21-22)

|Week|Focus                                |Resource               |Hours|
|----|-------------------------------------|-----------------------|-----|
|21  |Deep Learning basics, neural networks|Fast.ai Part 1         |18   |
|22  |NLP, transformers, foundation models |Hugging Face NLP + **AI Engineering Ch 2**|18|

**Week 21: Deep Learning Foundations**
- Fast.ai Practical Deep Learning Part 1
- Focus on understanding: neural networks, training, evaluation
- Understand loss functions, optimization concepts
- Claude Code runs the notebooks — you study the architecture and results

**Week 22: Foundation Models Deep Dive**

**Monday-Wednesday (6 hours): Hugging Face NLP Course**
- Transformers architecture — understand the system
- Attention mechanisms — how models "focus"
- Tokenization — how text becomes numbers
- Pre-training and fine-tuning concepts

**Thursday-Friday (4 hours): AI Engineering Chapter 2**
- **Training data curation** — How LLMs learn (and what can go wrong)
- **Model architecture decisions** — Understanding model internals
- **Scaling laws** — How model size affects capabilities and vulnerabilities
- **Post-training techniques** — Supervised and preference finetuning
- **Sampling and probabilistic nature** — Why outputs vary, temperature attacks

**Weekend (8 hours):**
- Continue Hugging Face course
- Study transformer architecture diagrams
- Document foundation model concepts in Obsidian
- Read relevant sections of Red Teaming AI (Dursey)

**Why This Matters:**
You already understand LLM vulnerabilities from Track 7 (Wilson book). Now you build the ML foundation to:
- Understand HOW models work internally (better attacks)
- Know training data vulnerabilities
- Exploit model architecture weaknesses
- Understand sampling and temperature manipulation

-----

## Phase 2: HTB Academy AI Red Teamer Labs (Weeks 23-24)

**Primary Resource:** HTB Academy AI Red Teamer Path (~$20/month subscription)

|Week|Focus                                |HTB Modules                      |
|----|-------------------------------------|---------------------------------|
|23  |Prompt injection, jailbreaking       |HTB: Introduction to Red Teaming AI, Prompt Injection labs|
|24  |Model privacy attacks, adversarial AI|HTB: Model extraction, Data poisoning labs|

**What You'll Do:**
- Complete hands-on labs attacking real AI systems
- Direct Claude Code to build prompt injection exploits
- Test jailbreaking techniques against LLMs
- Execute model privacy attacks
- Document findings in Obsidian

**Your Architect Approach:**
For each lab:
1. **Understand the target architecture** — What system am I attacking? What components?
2. **Identify the attack surface** — Where are the interfaces? What inputs do I control?
3. **Direct Claude Code to build the exploit** — "Write a Python script that tests this LLM endpoint for prompt injection using these techniques..."
4. **Analyze results** — Did the attack work? Why or why not? What does this tell you about the architecture?
5. **Document findings** — Professional red team notes in Obsidian

**Supplement with OWASP LLM Top 10:** Review concepts as you encounter them in labs

-----

## Phase 3: Production LLM Apps & Supply Chain (Weeks 25-26)

|Week|Focus                                 |Resource                    |
|----|--------------------------------------|----------------------------|
|25  |**RAG & Agent security**              |**AI Engineering Ch 6 + LangChain hands-on**|
|26  |**ML Supply Chain + Production**      |**Ch 5, 7, 9, 10 + hands-on exploits**|

**Week 25: RAG & Agent Security - CRITICAL**

**Why This Week:**
- Most production LLM apps use RAG (Retrieval Augmented Generation)
- Agent-based systems have unique vulnerabilities
- You need to understand the ARCHITECTURE to attack it effectively
- This is where your Track 8 systems thinking pays off

**Monday-Tuesday (4 hours): AI Engineering Chapter 6 - RAG and Agents** MUST READ
- **Retrieval-Augmented Generation (RAG):**
  - Term-based retrievers (BM25, TF-IDF)
  - Embedding-based retrievers (vector databases)
  - Hybrid retrieval approaches
  - RAG architecture and components
  - **Attack surfaces:** Document injection, retriever manipulation, context poisoning

- **Agentic Patterns:**
  - Tool access and function calling
  - Reflection mechanisms
  - Planning and reasoning loops
  - **Attack surfaces:** Tool misuse, infinite loops, prompt injection via tools

- **Memory Systems:**
  - Short-term vs long-term memory
  - Conversation history management
  - **Attack surfaces:** Memory poisoning, history injection

**Wednesday-Friday (6 hours): Direct Claude Code to Build RAG App**
Now that you understand RAG/agent architecture, direct Claude Code to build one:

1. **Document QA System (3 hours)** — Direct Claude Code:
   ```
   "Build a Python RAG application with:
   - ChromaDB vector database
   - Document embedding and storage
   - Retrieval chain: query → embed → retrieve → generate
   - Use LangChain for orchestration
   - Include logging for all retrieval steps (for later attack analysis)"
   ```

2. **LLM Agent (3 hours)** — Direct Claude Code:
   ```
   "Build a LangChain agent with:
   - Tools: calculator, web search, Wikipedia
   - Conversational memory
   - Multi-step reasoning
   - Tool execution logging"
   ```

**Weekend (8 hours): Attack Your Own Apps**

Direct Claude Code to build attack scripts, then analyze results:

1. **RAG Attacks (4 hours)**
   - Inject malicious documents into vector database
   - Context poisoning (manipulate retrieval results)
   - Embedding attacks (adversarial documents)
   - Prompt injection via retrieved context
   - Test different retrievers (term-based vs embedding)

2. **Agent Attacks (4 hours)**
   - Make agent call wrong tools
   - Cause infinite reasoning loops
   - Exploit tool execution vulnerabilities
   - Memory poisoning attacks
   - Jailbreak via multi-step chains

**Deliverable:**
- Working RAG app + agent (GitHub — built by Claude Code, reviewed by you)
- Attack documentation (Obsidian + blog post)
- 5+ attack vectors documented
- Defensive recommendations

**Week 26: ML Supply Chain + Prompt Engineering**

**Monday-Tuesday (6 hours): ML Supply Chain Attacks**

**Theory (1 hour):**
Review supply chain concepts from Track 7 (Wilson book Chapter 8):
- Malicious models and backdoored weights
- Pickle exploits in PyTorch/TensorFlow
- Poisoned datasets
- ML-BOM and provenance
- Reference: [MITRE ATLAS](https://atlas.mitre.org/) — adversarial ML threat framework (the "ATT&CK for AI")

**Hands-On (5 hours):** Direct Claude Code to build:
1. **Malicious pickle file (2 hours)** — Understand the exploit architecture:
   - How pickle deserialization enables arbitrary code execution
   - Direct Claude Code to create PoC
   - Defensive: Convert to safetensors format

2. **Model verification tool (3 hours)** — Direct Claude Code:
   ```
   "Build a Python script that scans Hugging Face models for security:
   - Check for pickle files (unsafe)
   - Verify safetensors usage (safe)
   - Scan dependencies for known CVEs
   - Check model cards for red flags
   - Verify digital signatures"
   ```

**Wednesday-Thursday (4 hours): AI Engineering Ch 5 - Prompt Engineering** CRITICAL

This is THE chapter for AI red teaming:
- **Prompt Anatomy:** System prompts, user prompts, context
- **In-Context Learning:** Few-shot examples and their influence
- **Prompt Injection Attacks and Defenses:** ESSENTIAL
  - Direct vs indirect injection
  - Adversarial suffixes
  - Delimiter attacks
  - Defense strategies and why they often fail
- **Techniques for Improving Outputs:** Chain-of-thought (and how to exploit it)

**Friday (2 hours): Catch-up / HTB Academy**
- Finish any remaining HTB modules from Weeks 23-24
- Or catch up on Week 25 RAG attacks if needed

**Weekend (6 hours): Apply Prompt Engineering to Attacks**
- Revisit your RAG app and agent from Week 25
- Apply prompt engineering techniques from Ch 5 as attack vectors
- Test adversarial suffixes, delimiter attacks, chain-of-thought exploitation
- Document new attack findings in Obsidian

-----

## Phase 4: Evaluation & Advanced CTF (Weeks 27-28)

|Week|Focus                               |Resource             |
|----|------------------------------------|--------------------|
|27  |AI Engineering (remaining chapters) + HackAPrompt|Ch 3-4, 7, 10 + hackaprompt.com|
|28  |Crucible CTF + Automated Red Team Agent + Final Assessment|crucible.dreadnode.io + Claude SDK|

**Week 27: Evaluation + Production AI + HackAPrompt**

**Monday-Wednesday (6 hours): AI Engineering — Remaining Chapters**

- **Ch 3-4: Evaluation (3 hours)** — How to measure attack success objectively. Build evaluation pipeline for your attacks.
- **Ch 7: Finetuning (1.5 hours)** — Skim for attack implications of finetuned models. How does finetuning change model behavior and defenses?
- **Ch 10: AI Engineering Architecture (1.5 hours)** — Skim for attack surfaces in production AI systems. How are real systems deployed?
- **Ch 9: Inference Optimization** — OPTIONAL reference reading. Skim if time allows. Not critical for red teaming.

**Thursday-Weekend (12 hours): HackAPrompt CTF**
- Complete as many levels as possible
- Direct Claude Code to automate attack attempts
- Apply evaluation techniques from Ch 3-4
- Measure success rates across different attack vectors
- Document successful prompts in Obsidian
- Blog post: "My HackAPrompt Solutions + Success Rate Analysis"

**Week 28: Advanced CTF & Final Portfolio**

**Monday-Wednesday (6 hours): Crucible CTF**
- [Crucible by Dreadnode](https://crucible.dreadnode.io/)
- AI red teaming CTF challenges
- Apply all techniques from previous weeks

**Thursday-Friday (4 hours): Claude Code SDK - Automated Red Team Agent**

Direct Claude Code to build an automated red team agent:
```
"Build an automated prompt injection testing agent using the Claude Agent SDK:
- Input: target API endpoint + test case library (YAML)
- Agent systematically tests LLM defenses
- Chains multiple attack patterns automatically
- Logs all attempts and responses
- Classifies results (success/partial/blocked)
- Output: structured JSON report with findings and severity"
```

Review the agent's architecture. Does it follow clean architecture? Is it testable?

**Weekend (8 hours): Final Red Team Assessment Portfolio Piece**

1. **Target Selection (2 hours)** — Choose or build a complex vulnerable application
2. **Red Team Engagement (6 hours):**
   - Reconnaissance (model identification, architecture)
   - Vulnerability assessment (prompt injection, RAG poisoning, etc.)
   - Exploitation (demonstrate impact)
   - Professional report writing

**Deliverable:**
- Professional red team assessment report
- PoC exploits (GitHub)
- Defensive playbook
- Blog post on findings
- Portfolio piece for job applications

-----

## Projects & Outputs

|Week|Project                      |Output                               |Share             |
|----|-----------------------------|-------------------------------------|------------------|
|23-24|HTB Academy lab completions |All modules completed                |HTB profile       |
|23-24|Prompt injection PoC        |Working exploit with automation      |GitHub            |
|25  |**Vulnerable RAG app**       |**Document QA + LLM agent**          |**GitHub**        |
|25  |**RAG/Agent attacks**        |**5+ attack vectors documented**     |**GitHub + Blog** |
|26  |**Malicious pickle exploit** |**PyTorch RCE demonstration**        |**Demo only**     |
|26  |**Model verification tool**  |**Scan Hugging Face models**         |**GitHub**        |
|27  |**Attack evaluation pipeline**|**Automated testing framework**     |**GitHub**        |
|27  |HackAPrompt solutions        |Documented strategies + success rates|Blog + GitHub     |
|28  |Crucible CTF solutions       |Novel attack vectors                 |GitHub            |
|28  |**Automated red team agent** |**Claude SDK agent**                 |**GitHub**        |
|28  |**Red team assessment**      |**Professional security report**     |**Portfolio**     |

-----

## Key Concepts

**From Track 7: LLM Security Primer (Wilson book — Theory):**
- Prompt Injection (direct vs indirect)
- Jailbreaking techniques
- OWASP LLM Top 10
- Zero Trust for LLMs
- Supply Chain Security (ML-BOM)

**From AI Engineering Book (Production):**
- **Ch 2:** Foundation model internals, training data, scaling laws
- **Ch 3-4:** Evaluation methodology, testing AI systems objectively
- **Ch 5:** Prompt engineering, injection attacks and defenses
- **Ch 6:** RAG architecture, agents with tools, memory systems
- **Ch 7:** Finetuning techniques and attack surfaces
- **Ch 9:** Inference optimization, quantization exploits
- **Ch 10:** Production architecture, monitoring, attack surfaces

**From HTB Academy (Hands-On):**
- Practical prompt injection exploitation
- Jailbreaking real LLM systems
- Model extraction attacks
- Data poisoning demonstrations
- Attack automation

**Production LLM Security:**
- **RAG Architecture:** Term-based vs embedding retrievers
- **RAG Poisoning:** Inject malicious documents into vector DBs
- **Agent Exploits:** Tool misuse, infinite loops, prompt injection via tools
- **Memory Attacks:** Conversation history poisoning
- **LangChain Security:** Framework-specific vulnerabilities
- **ML Supply Chain:** Pickle RCE, malicious models, backdoored weights
- **Model Verification:** SafeTensors vs pickle, provenance checking
- **Evaluation Pipelines:** Automated attack testing, success rate measurement
- **Production Attacks:** API exploits, inference DoS, cache poisoning

-----

## Claude Code Integration

Use Claude Code throughout this track as your implementation tool:

**Building Targets:**
```
"Build a vulnerable RAG application with LangChain that I can
test for prompt injection. Include: vector database, document
ingestion, retrieval chain, and response generation."
```

**Building Exploits:**
```
"Write a Python script that tests an LLM API endpoint
for prompt injection using these attack patterns:
[list]. Log all responses for analysis."
```

**Analysis:**
```
"Explain how RAG poisoning works at a technical level.
I understand vector databases from reading about them.
How do adversarial documents manipulate embedding similarity?"
```

-----

## Checkpoint

Before moving to Track 9: Python Core, you should be able to:

**Conceptual Understanding:**
- Explain foundation model internals (training, scaling, sampling)
- Describe RAG architecture and its attack surfaces
- Explain how LLM agents work and their vulnerabilities
- Understand ML supply chain risks
- Design evaluation pipelines for measuring attack effectiveness

**Practical Experience (via Claude Code):**
- Complete HTB Academy AI Red Teamer modules
- Direct Claude Code to build prompt injection exploits
- Direct Claude Code to build RAG applications + attack them
- Direct Claude Code to build model verification tools
- Solve HackAPrompt and Crucible challenges
- Conduct professional AI red team assessment

**Portfolio Pieces:**
- HTB Academy profile with completed modules
- Vulnerable RAG app + LLM agent (GitHub)
- RAG/Agent attack documentation (blog post)
- Model verification tool (GitHub)
- Attack evaluation pipeline (GitHub)
- Automated red team agent built with Claude Code SDK (GitHub)
- Professional red team assessment report (portfolio)
- 5+ blog posts on AI security topics
