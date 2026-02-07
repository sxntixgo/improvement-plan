# Track 10: AI/ML Security

**Duration:** 10 weeks | **Hours/week:** 18 | **Priority:** HIGH
**Goal:** AI red teaming skills

**Weekly Schedule:**

- Weekdays: 8 hours
- Saturday: 5 hours
- Sunday: 5 hours

-----

## Phase Overview

|Phase|Weeks|Focus                           |AI Engineering Chapters|
|-----|-----|--------------------------------|-----------------------|
|1    |33-34|ML Fundamentals                 |Ch 2: Foundation Models|
|2    |35-36|HTB Academy Labs                |-                      |
|3    |37-38|RAG/Agents + Supply Chain       |Ch 6: RAG/Agents       |
|4    |39-40|Evaluation + Advanced CTF       |Ch 3-5, 7, 9-10        |
|5    |41-42|Go for AI Security (Capstone)   |Hands-on projects      |

**AI Engineering Book Usage (7 chapters, ~18 hours):**
- **Week 34:** Ch 2 (Foundation Models) - 4 hrs
- **Week 37:** Ch 6 (RAG and Agents) - 4 hrs CRITICAL
- **Week 38:** Ch 5 (Prompt Engineering) - 4 hrs CRITICAL for attacks
- **Week 38:** Ch 7, 9, 10 (Production systems) - 6 hrs
- **Week 39:** Ch 3-4 (Evaluation) - 4 hrs

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
|HackAPrompt       |hackaprompt.com      |Prompt injection practice|
|Dreadnode/Crucible|crucible.dreadnode.io|CTF-style challenges     |

### Books

|Resource                                      |Cost         |Status/Focus              |
|----------------------------------------------|-------------|--------------------------|
|Developer's Playbook for LLM Security (Wilson)|Already owned|Read in Track 7           |
|AI Engineering (Huyen)                        |~$50         |Production AI systems     |
|Red Teaming AI (Dursey)                       |~$50         |Red teaming (July 2026)   |

### Optional Paid Courses

|Resource             |Cost|Focus                 |Note                     |
|---------------------|----|----------------------|-------------------------|
|NVIDIA Adversarial ML|$90 |Adversarial techniques|Optional - can use free resources|

-----

## Phase 1: ML Fundamentals (Weeks 33-34)

|Week|Focus                                |Resource               |Hours|
|----|-------------------------------------|-----------------------|-----|
|33  |Deep Learning basics, neural networks|Fast.ai Part 1         |18   |
|34  |NLP, transformers, foundation models |Hugging Face NLP + **AI Engineering Ch 2**|18|

**Week 33: Deep Learning Foundations**
- Fast.ai Practical Deep Learning Part 1
- Focus on neural networks, training, evaluation
- Hands-on: Build and train simple models
- Understand loss functions, optimization

**Week 34: Foundation Models Deep Dive**

**Monday-Wednesday (6 hours): Hugging Face NLP Course**
- Transformers architecture
- Attention mechanisms
- Tokenization
- Pre-training and fine-tuning concepts

**Thursday-Friday (4 hours): AI Engineering Chapter 2**
- **Training data curation** - How LLMs learn (and what can go wrong)
- **Model architecture decisions** - Understanding model internals
- **Scaling laws** - How model size affects capabilities and vulnerabilities
- **Post-training techniques** - Supervised and preference finetuning
- **Sampling and probabilistic nature** - Why outputs vary, temperature attacks

**Weekend (8 hours):**
- Continue Hugging Face course
- Build transformer model from scratch (tutorial)
- Document foundation model concepts in Obsidian

**Why This Matters:**
You already understand LLM vulnerabilities from Track 7: LLM Security Primer (Wilson book). Now you're building the ML foundation to:
- Understand HOW models work internally (better attacks)
- Know training data vulnerabilities
- Exploit model architecture weaknesses
- Understand sampling and temperature manipulation

-----

## Phase 2: HTB Academy AI Red Teamer Labs (Weeks 35-36)

**Primary Resource:** HTB Academy AI Red Teamer Path (~$20/month subscription)

|Week|Focus                                |HTB Modules                      |
|----|-------------------------------------|---------------------------------|
|35  |Prompt injection, jailbreaking       |HTB: Introduction to Red Teaming AI, Prompt Injection labs|
|36  |Model privacy attacks, adversarial AI|HTB: Model extraction, Data poisoning labs|

**What You'll Do:**
- Complete hands-on labs attacking real AI systems
- Build prompt injection exploits (using Python from Track 9!)
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

## Phase 3: Production LLM Apps & Supply Chain (Weeks 37-38)

|Week|Focus                                 |Resource                    |
|----|--------------------------------------|----------------------------|
|37  |**RAG & Agent security**              |**AI Engineering Ch 6 + LangChain hands-on**|
|38  |**ML Supply Chain security**          |**Hands-on exploits + verification tools**|

**Week 37: RAG & Agent Security - CRITICAL**

**Why This Week:**
- Most production LLM apps use RAG (Retrieval Augmented Generation)
- Agent-based systems have unique vulnerabilities
- You need to understand the architecture to attack it effectively
- LangChain is the most popular framework for building these apps

**Learning Strategy: Theory First, Then Attack**

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

**Why Read This First:**
Understanding the architecture from Huyen's book gives you:
- Knowledge of how RAG systems work internally
- Attack surface identification
- Different retriever types to exploit
- Agent patterns and their weaknesses

**Wednesday-Friday (6 hours): LangChain Hands-On - Build RAG App**
Now that you understand RAG/agent architecture, build one:

1. **Build Document QA System (3 hours)**
   - Vector database setup (ChromaDB or Pinecone)
   - Document embedding and storage
   - Retrieval chain setup
   - Query -> Retrieve -> Generate pipeline

2. **Build LLM Agent (3 hours)**
   - Agent with tools (calculator, search, Wikipedia)
   - Conversational memory
   - Multi-step reasoning
   - Tool execution workflow

**Resources:**
- [LangChain Documentation](https://python.langchain.com/)
- [LangChain RAG Tutorial](https://python.langchain.com/docs/tutorials/rag/)
- [LangChain Agents Guide](https://python.langchain.com/docs/tutorials/agents/)

**Weekend (8 hours): Attack Your Own Apps**

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
- Working RAG app + agent (GitHub)
- Attack documentation (Obsidian + blog post)
- 5+ attack vectors documented
- Defensive recommendations

**Week 38: ML Supply Chain & Production Security**

**Why This Week:**
- Most AI security incidents involve supply chain compromises (not novel attacks)
- Production systems have different attack surfaces than research models
- You need to verify model safety before deployment

**Monday-Tuesday (6 hours): ML Supply Chain Attacks - Hands-On**

**Theory (1 hour):**
Review supply chain concepts from Track 7: LLM Security Primer (Wilson book Chapter 8):
- Malicious models and backdoored weights
- Pickle exploits in PyTorch/TensorFlow
- Poisoned datasets
- ML-BOM and provenance

**Hands-On Exploitation (5 hours):**
1. **Create malicious pickle file (2 hours)**
   - Craft PyTorch model with embedded exploit
   - Test pickle deserialization attack
   - Demonstrate arbitrary code execution
   - **Defensive:** Convert to safetensors format

2. **Build model verification tool (3 hours)**
   - Python script to scan Hugging Face models
   - Check for pickle files (unsafe)
   - Verify safetensors usage (safe)
   - Scan dependencies for known CVEs
   - Check model cards for red flags
   - Verify digital signatures

**Resources:**
- [Hugging Face Model Security](https://huggingface.co/docs/hub/security)
- [SafeTensors Documentation](https://huggingface.co/docs/safetensors/)

**Wednesday-Thursday (4 hours): AI Engineering Ch 5 - Prompt Engineering** CRITICAL

**Why This Chapter:**
This is THE chapter for AI red teaming - covers prompt injection attacks!

- **Prompt Anatomy:**
  - System prompts, user prompts, context
  - Instruction following mechanisms
  - Role-playing and persona prompts

- **In-Context Learning:**
  - Few-shot examples and their influence
  - How models use context
  - **Attacks:** Manipulating examples, context injection

- **Prompt Injection Attacks and Defenses:** ESSENTIAL
  - Direct vs indirect injection
  - Adversarial suffixes
  - Delimiter attacks
  - Defense strategies and why they often fail
  - Real-world case studies

- **Techniques for Improving Outputs:**
  - Chain-of-thought prompting (and how to exploit it)
  - Role prompting (jailbreaking technique)
  - Output formatting (bypass content filters)

**Exercise:**
- Apply Chapter 5 techniques to HTB labs (retroactively)
- Document new attack vectors discovered
- Update your prompt injection taxonomy

**Friday-Weekend (8 hours): Production AI Systems**

**AI Engineering Ch 7, 9, 10 (6 hours):**

**Chapter 7: Finetuning (2 hours)**
- When companies finetune vs use RAG
- LoRA and PEFT techniques
- **Attack implications:** Finetuned models may have different vulnerabilities
- **Backdoor attacks:** Poisoning finetuning datasets

**Chapter 9: Inference Optimization (2 hours)**
- Latency and throughput metrics
- Quantization and distillation
- **Attacks:** Exploiting quantized models (different behavior)
- **DoS attacks:** Resource exhaustion via inference

**Chapter 10: AI Engineering Architecture (2 hours)**
- System architecture components
- Monitoring and observability
- **Attack surfaces:** API endpoints, queues, caches
- **Defensive monitoring:** Detecting attacks in production
- User feedback loops (poisoning risk)

**HTB Academy Capstone (2 hours):**
- Complete any remaining HTB modules
- Final project or capstone challenge
- Document portfolio piece

**Deliverables:**
- Malicious pickle exploit (demo only, not public)
- Model verification tool (GitHub)
- Updated prompt injection taxonomy
- Blog post: "ML Supply Chain Security"
- Notes on production AI security

-----

## Phase 4: Evaluation & Advanced CTF (Weeks 39-40)

|Week|Focus                               |Resource             |
|----|------------------------------------|--------------------|
|39  |Evaluation methodology + HackAPrompt|AI Engineering Ch 3-4 + hackaprompt.com|
|40  |Crucible CTF + Final Assessment     |crucible.dreadnode.io + Portfolio project|

**Week 39: Evaluation & HackAPrompt**

**Monday-Tuesday (4 hours): AI Engineering Ch 3-4 - Evaluation**

**Chapter 3: Evaluation Methodology (2 hours)**
- Challenges in evaluating foundation models
- Language modeling metrics (perplexity, etc.)
- Approaches for open-ended responses:
  - Functional correctness testing
  - Similarity scores (BLEU, ROUGE)
  - AI-as-a-judge (using LLMs to evaluate LLMs)
- Preference signals and human feedback
- **Red team application:** How to evaluate your attacks objectively

**Chapter 4: Evaluate AI Systems (2 hours)**
- Selecting appropriate models for applications
- Comparing hosting vs API approaches
- Analyzing public benchmarks (and their limitations)
- Building reliable evaluation pipelines
- **Red team application:** Build evaluation pipeline for your attacks

**Why This Matters:**
- Objectively measure attack success rates
- Build automated testing for prompt injections
- Evaluate defensive measures quantitatively
- Create reproducible red team assessments

**Wednesday-Weekend (14 hours): HackAPrompt CTF**
- Complete as many levels as possible
- Use Python to automate attack attempts
- Apply evaluation techniques from Ch 3-4
- Measure success rates across different attack vectors
- Document successful prompts in Obsidian
- **Build evaluation pipeline:** Automated testing of your solutions
- Blog post: "My HackAPrompt Solutions + Success Rate Analysis"

**Week 40: Advanced CTF & Final Portfolio**

**Monday-Wednesday (6 hours): Crucible CTF**
- [Crucible by Dreadnode](https://crucible.dreadnode.io/)
- AI red teaming CTF challenges
- Apply all techniques from previous weeks
- Document novel attack vectors discovered
- Compare with other solutions

**Thursday-Friday (4 hours): Claude Code SDK - Automated Red Team Agent**

**Why This Matters:**
You've been building tools with Claude Code throughout this plan. Now combine that experience with your AI security skills to build an automated red team agent using the Claude Agent SDK.

**Build: Automated Prompt Injection Testing Agent**
1. **Agent Design (1 hour)**
   - Define agent that systematically tests LLM defenses
   - Input: target API endpoint + test case library
   - Output: structured report with findings and severity

2. **Implementation (2 hours)**
   - Use Claude Agent SDK to build the agent
   - Agent chains multiple attack patterns automatically
   - Logs all attempts and responses
   - Classifies results (success/partial/blocked)

3. **Testing & Documentation (1 hour)**
   - Test against your own vulnerable RAG app (from Week 37)
   - Document the agent architecture
   - Add to GitHub portfolio

**Deliverable:** Working automated red team agent (unique portfolio piece combining Claude Code + AI security)

-----

**Weekend (8 hours): Final Red Team Assessment Portfolio Piece**

Build comprehensive AI security assessment:

1. **Target Selection (2 hours)**
   - Choose a real-world AI application (with permission)
   - OR build complex vulnerable application
   - Document scope and boundaries

2. **Red Team Engagement (6 hours)**
   - Reconnaissance (model identification, architecture)
   - Vulnerability assessment (prompt injection, RAG poisoning, etc.)
   - Exploitation (demonstrate impact)
   - Document findings professionally

3. **Report Writing (4 hours)**
   - Executive summary
   - Technical findings with severity ratings
   - Proof-of-concept code
   - Remediation recommendations
   - Defense-in-depth strategies

**Deliverable:**
- Professional red team assessment report
- PoC exploits (GitHub)
- Defensive playbook
- Blog post on findings
- Portfolio piece for job applications

-----

## Phase 5: Go for AI Security (Weeks 41-42)

**Why Now:**
You now have deep Go skills (Tracks 8 + 11) AND AI/ML security knowledge (Phase 1-4). This is where you combine them to build something no one else is building: AI security tools in Go.

Most AI red teamers only use Python. Your Go skills give you a unique edge:
- Go's concurrency model is ideal for parallel prompt injection testing
- Go binaries are easy to distribute (no Python environment needed)
- Go's performance handles high-volume API testing efficiently
- gRPC security testing is natural in Go (gRPC is a Go-native technology)

### Week 41: Go-Based LLM Security Testing Tools

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Build concurrent prompt injection tester|
|Wed-Thu|4|Go HTTP client for LLM API interaction (OpenAI, Anthropic APIs)|
|Fri|2|gRPC security testing patterns|
|Weekend|6|Project: LLM API fuzzer with goroutines|

**Concurrent Prompt Injection Tester:**
```go
type TestCase struct {
    Name     string
    Prompt   string
    Expected string // "blocked", "leaked", "safe"
}

type Result struct {
    TestCase TestCase
    Response string
    Status   string // "pass", "fail", "error"
    Duration time.Duration
}

func RunTests(ctx context.Context, cases []TestCase, workers int) []Result {
    // Fan-out: distribute test cases to worker goroutines
    // Fan-in: collect results through channel
    // Context: cancel all workers on timeout
}
```

**Key Features:**
- Fan-out/fan-in pattern for parallel testing
- Rate limiting to avoid API throttling
- Structured logging of all attempts
- JSON/CSV report generation
- Configurable test case library (YAML/JSON input)

### Week 42: Capstone — Go AI Red Team CLI Tool

|Day|Hours|Focus|
|---|-----|-----|
|Mon-Tue|6|Design and build complete AI red team CLI tool|
|Wed-Thu|4|Add reporting, configuration, Docker packaging|
|Fri|2|Write comprehensive tests|
|Weekend|6|Polish, document, blog post|

**Capstone: Go AI Red Team CLI Tool**

Combines Go mastery + AI security knowledge into a single portfolio piece:

**Features:**
- Concurrent LLM endpoint testing (goroutines)
- Multiple attack pattern libraries (prompt injection, jailbreak, exfiltration)
- Configurable via YAML
- Structured JSON reports with severity ratings
- Rate limiting and retry logic
- Docker multi-stage build
- Clean architecture (from Track 8)

**Tech Stack:**
- cobra for CLI framework
- slog for structured logging
- testify for testing
- net/http for API interaction
- goroutines + channels for concurrency
- CLAUDE.md for project configuration

**Deliverable:**
- GitHub repo with full codebase
- Blog post: "Building an AI Red Team Tool in Go"
- Docker image published
- Unique portfolio piece (AI security + Go = rare combination)

-----

## Projects & Outputs

|Week|Project                      |Output                               |Share             |
|----|-----------------------------|-------------------------------------|------------------|
|35-36|HTB Academy lab completions |All modules completed                |HTB profile       |
|35-36|Prompt injection PoC (Python)|Working exploit with automation      |GitHub            |
|37  |**Vulnerable RAG app**       |**Document QA + LLM agent**          |**GitHub**        |
|37  |**RAG/Agent attacks**        |**5+ attack vectors documented**     |**GitHub + Blog** |
|38  |**Malicious pickle exploit** |**PyTorch RCE demonstration**        |**Demo only**     |
|38  |**Model verification tool**  |**Scan Hugging Face models**         |**GitHub**        |
|39  |**Attack evaluation pipeline**|**Automated testing framework**     |**GitHub**        |
|39  |HackAPrompt solutions        |Documented strategies + success rates|Blog + GitHub     |
|40  |Crucible CTF solutions       |Novel attack vectors                 |GitHub            |
|40  |**Red team assessment**      |**Professional security report**     |**Portfolio**     |
|41  |LLM API fuzzer               |Concurrent prompt injection tester   |GitHub            |
|42  |**Go AI Red Team CLI Tool**  |**Complete AI security tool in Go**  |**GitHub + Blog** |

-----

## Key Concepts

**From Track 7: LLM Security Primer (Wilson book - Theory):**
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
- Attack automation with Python

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

Use Claude Code throughout this track:

**Attack Development:**
```
CREATE: "Build a Python script that tests an LLM API endpoint
for prompt injection vulnerabilities. Test these attack patterns:
[list patterns]. Log all responses for analysis."

REVIEW: "Review this prompt injection exploit for completeness.
What attack vectors am I missing? Reference OWASP LLM Top 10."
```

**Learning Acceleration:**
```
EXPLAIN: "Explain how RAG poisoning works at a technical level.
I understand vector databases from building one in LangChain.
How do adversarial documents manipulate embedding similarity?"
```

-----

## Checkpoint

Before moving to Track 12: Python Advanced, you should be able to:

**Technical Skills:**
- Understand foundation model internals (training, scaling, sampling)
- Complete HTB Academy AI Red Teamer modules
- Build prompt injection exploits using Python
- Build RAG applications with LangChain from scratch
- Execute RAG poisoning attacks (document injection, context poisoning)
- Exploit LLM agents (tool misuse, infinite loops)
- Attack memory systems (conversation history poisoning)
- Create malicious pickle exploits (RCE via model loading)
- Build model verification tools (scan Hugging Face for threats)
- Execute jailbreaking attacks against production LLMs
- Build automated attack evaluation pipelines
- Measure attack success rates objectively

**Practical Experience:**
- Solve HackAPrompt challenges with quantified success rates
- Complete Crucible CTF challenges
- Conduct full professional AI red team assessment
- Write security findings with severity ratings
- Build automated red team agent with Claude Code SDK

**Portfolio Pieces:**
- HTB Academy profile with completed modules
- Vulnerable RAG app + LLM agent (GitHub)
- RAG/Agent attack documentation (blog post)
- Model verification tool (GitHub)
- Attack evaluation pipeline (GitHub)
- Automated red team agent built with Claude Code SDK (GitHub)
- **Go AI Red Team CLI Tool (GitHub + Blog post)**
- Professional red team assessment report (portfolio)
- 5+ blog posts on AI security topics
