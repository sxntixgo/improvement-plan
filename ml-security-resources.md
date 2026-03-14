# ML Security Resources - Comprehensive Research

**Date:** March 6, 2026
**Purpose:** Curated ML security resources for the AI Red Teamer learning path
**Source:** Compiled from training knowledge (no web lookups)

-----

## 1. Academic Papers (Free)

These are foundational papers that define the field. Read the ones relevant to your current track phase.

### Adversarial ML Foundations

| Paper | Authors | Year | Why It Matters |
|-------|---------|------|----------------|
| Intriguing Properties of Neural Networks | Szegedy et al. | 2013 | The paper that discovered adversarial examples. Started the entire field. |
| Explaining and Harnessing Adversarial Examples | Goodfellow, Shlens, Szegedy | 2014 | Introduced FGSM (Fast Gradient Sign Method). Most-cited adversarial ML paper. |
| Towards Evaluating the Robustness of Neural Networks | Carlini & Wagner | 2017 | The C&W attack — gold standard for evaluating model robustness. Nicholas Carlini is a key researcher to follow. |
| Adversarial Examples Are Not Easily Detected | Carlini & Wagner | 2017 | Shows why simple detection methods fail against sophisticated adversarial examples. |
| Certified Adversarial Robustness via Randomized Smoothing | Cohen, Rosenfeld, Kolter | 2019 | Provable robustness guarantees — the defense side of adversarial ML. |

### LLM Security

| Paper | Authors | Year | Why It Matters |
|-------|---------|------|----------------|
| Universal and Transferable Adversarial Attacks on Aligned Language Models | Zou et al. | 2023 | The "universal adversarial suffixes" paper. Automated jailbreak generation via gradient-based optimization. Directly referenced in Wilson's book. |
| Ignore This Title and HackAPrompt | Schulhoff et al. | 2023 | Systematic taxonomy of prompt injection techniques from the HackAPrompt competition. |
| Not What You've Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection | Greshake et al. | 2023 | Defines indirect prompt injection as an attack class. Essential reading. |
| Poisoning Language Models During Instruction Tuning | Wan et al. | 2023 | How attackers can poison instruction-tuned models with a small number of examples. |
| Scalable Extraction of Training Data from (Production) Language Models | Carlini et al. | 2023 | Extracting training data from ChatGPT. Demonstrates memorization risks in production LLMs. |
| Jailbroken: How Does LLM Safety Training Fail? | Wei, Haghtalab, Steinhardt | 2024 | Analyzes why safety training fails — competing objectives and mismatched generalization. |
| AutoDAN: Generating Stealthy Jailbreak Prompts on Aligned LLMs | Liu et al. | 2024 | Automated jailbreak prompt generation that evades perplexity-based defenses. |
| Many-shot Jailbreaking | Anthropic | 2024 | Demonstrates that long-context models are vulnerable to many-shot jailbreaking via in-context learning. |

### Data Poisoning & Backdoors

| Paper | Authors | Year | Why It Matters |
|-------|---------|------|----------------|
| Poisoning Attacks against Support Vector Machines | Biggio et al. | 2012 | Early foundational work on data poisoning. |
| BadNets: Identifying Vulnerabilities in the Machine Learning Model Supply Chain | Gu et al. | 2017 | Foundational backdoor attack paper. Shows how training-time attacks persist through transfer learning. |
| TrojAI: A Tool for Detecting Trojans in AI Models | IARPA | 2020+ | Government program for trojan detection — shows this is a national security concern. |
| Poisoning Web-Scale Training Datasets is Practical | Carlini et al. | 2023 | Shows that poisoning LAION-400M and other web-scraped datasets requires minimal resources. |

### Model Privacy & Extraction

| Paper | Authors | Year | Why It Matters |
|-------|---------|------|----------------|
| Stealing Machine Learning Models via Prediction APIs | Tramer et al. | 2016 | Foundational model extraction paper. Shows how to clone ML models through API queries. |
| The Secret Sharer: Measuring Unintended Neural Network Memorization | Carlini et al. | 2019 | Quantifies how much training data neural networks memorize. |
| Extracting Training Data from Large Language Models | Carlini et al. | 2021 | Demonstrated training data extraction from GPT-2. Led to the 2023 production-scale follow-up. |

**Where to find them:** Search paper titles on arxiv.org or Google Scholar. All are freely available.

-----

## 2. Online Courses (Free)

### Already in Your Plan

| Course | Platform | Status |
|--------|----------|--------|
| Fast.ai Practical Deep Learning | fast.ai | Track 10, Week 21 |
| Hugging Face NLP Course | huggingface.co/learn | Track 10, Week 22 |

### Additional Recommendations

| Course | Platform | Cost | Focus | When to Take |
|--------|----------|------|-------|-------------|
| Machine Learning Security (Nicholas Carlini) | YouTube lectures | Free | Adversarial ML from one of the top researchers | During Track 10 Weeks 21-22 (ML Fundamentals) |
| Intro to ML Safety | Center for AI Safety | Free | Robustness, monitoring, alignment, systemic safety | After Track 10 for broader safety context |
| MLSecOps Top 10 | OWASP | Free | ML pipeline security vulnerabilities | During Track 10 Week 26 (Supply Chain) |
| AI Red Teaming with Azure AI | Microsoft Learn | Free | Hands-on AI red teaming using Azure tools, PyRIT integration | During Track 10 Week 28 (PyRIT week) |
| Prompt Engineering for Security | Various (YouTube) | Free | Offensive prompt engineering techniques | Track 10 Week 26 supplement |

-----

## 3. CTF Platforms & Practice Labs

### Already in Your Plan

| Platform | Status |
|----------|--------|
| HTB Academy AI Red Teamer | Track 10, Weeks 23-24 |
| HackAPrompt | Track 10, Week 27 |
| Crucible (Dreadnode) | Track 10, Week 28 |

### Additional Platforms

| Platform | URL | Cost | Focus | Difficulty |
|----------|-----|------|-------|-----------|
| Gandalf (Lakera) | gandalf.lakera.ai | Free | Progressive prompt injection levels — excellent beginner-friendly intro | Easy-Medium |
| Damn Vulnerable LLM Agent | GitHub (OWASP) | Free | Deliberately vulnerable LLM-powered web app for practicing OWASP LLM Top 10 | Medium |
| AI Goat | GitHub (OWASP) | Free | Vulnerable AI environment for practicing adversarial attacks on ML models | Medium |
| Prompt Airlines | promptairlines.com | Free | Multi-level prompt injection challenge with airline booking scenario | Medium |
| Tensor Trust | tensortrust.ai | Free | Competitive prompt injection/defense game — attack and defend | Medium-Hard |
| DEFCON AI Village CTFs | YouTube/archive | Free | Annual AI security CTF challenges — study past solutions | Hard |
| Adversarial Robustness Toolbox (ART) | GitHub (IBM) | Free | Not a CTF but provides attack/defense implementations you can experiment with | Tool |

**Recommended progression:**
1. Gandalf (Week 23, warm-up before HTB)
2. HTB Academy (Weeks 23-24, structured labs)
3. Prompt Airlines (Week 25, supplement)
4. HackAPrompt (Week 27, as planned)
5. Tensor Trust (Week 27, supplement)
6. Crucible (Week 28, as planned)

-----

## 4. Tools & Frameworks

### Already in Your Plan

| Tool | Status |
|------|--------|
| Garak (NVIDIA) | Track 10, Weeks 23-24 |
| PyRIT (Microsoft) | Track 10, Week 28 |

### Additional Tools

| Tool | Author | Focus | When to Use |
|------|--------|-------|-------------|
| Adversarial Robustness Toolbox (ART) | IBM Research | Comprehensive library for adversarial attacks and defenses on ML models. Supports evasion, poisoning, extraction, inference attacks across frameworks (PyTorch, TensorFlow, scikit-learn) | Track 10 Week 21-22 for experimentation |
| Counterfit | Microsoft | CLI tool for assessing ML model security. Builds on ART. Good for quick assessments | Track 10, alternative to Garak for specific models |
| TextAttack | QData Lab (UVA) | NLP-specific adversarial attack framework. Implements 16+ attack recipes for text classification, entailment, etc. | Track 10 Week 22 (NLP focus) |
| Rebuff | Protect AI | Self-hardening prompt injection detection. LLM-based detection + heuristics + vector DB for known attacks | Track 10 Week 26 (defense perspective) |
| ModelScan | Protect AI | Scan ML models for unsafe code (pickle exploits, etc.). Like a security scanner specifically for model files | Track 10 Week 26 (Supply Chain) |
| NB Defense | Protect AI | Security scanner for Jupyter notebooks — detects credentials, PII, licensing issues in ML workflows | Reference tool |
| Vigil | deadbits | LLM prompt injection detection and analysis tool | Track 10 Weeks 23-24 supplement |
| LLM Guard | Protect AI | Input/output guardrails for LLM apps — sanitization, toxicity detection, PII redaction | Track 10 Week 25 (defense side of RAG) |

**Protect AI ecosystem:** Protect AI (now Huntr for AI) has built multiple open-source ML security tools. Their GitHub org is worth following as a collection.

-----

## 5. Professional Frameworks & Standards

### Already in Your Plan

| Framework | Status |
|-----------|--------|
| OWASP LLM Top 10 | Track 7 + Track 10 |
| MITRE ATLAS | Track 10 |
| NIST AI RMF | Track 10 Week 28 |
| NIST Gen AI Profile | Track 10 Week 28 |
| Google SAIF | Track 10 Week 28 |
| AI Incident Database | Track 10 Week 28 |

### Additional Frameworks

| Framework | Source | Focus | When to Reference |
|-----------|--------|-------|------------------|
| OWASP ML Top 10 | OWASP | Classic ML (not just LLMs) — covers model stealing, data poisoning, model inversion, membership inference, neural net reprogramming, adversarial examples, model skewing, transfer learning attack, output integrity attack, model poisoning | Track 10 to complement LLM Top 10 |
| OWASP AI Exchange | OWASP | Broader AI security knowledge base connecting OWASP projects | Reference |
| EU AI Act | European Commission | Regulatory framework classifying AI systems by risk level. Defines "high-risk" AI and compliance requirements. Relevant for red team scope: what systems MUST be tested | Track 10 Week 28 (reporting context) |
| ISO/IEC 42001 | ISO | AI Management System standard. Emerging certification for AI governance | Reference for enterprise contexts |
| NIST SP 800-218A (SSDF for AI) | NIST | Secure Software Development Framework extended for AI systems | Track 10 supplement |
| Responsible AI Practices | Google | Practical guidelines for building responsible AI systems | Reference |
| Anthropic RSP | Anthropic | Responsible Scaling Policy — how frontier AI labs evaluate catastrophic risk | After Track 10 for broader context |

-----

## 6. Blogs, Newsletters & Community

### Researchers to Follow

| Person | Affiliation | Focus | Where to Follow |
|--------|-------------|-------|----------------|
| Nicholas Carlini | Google DeepMind | Adversarial ML, training data extraction, LLM security | Blog + papers |
| Simon Willison | Independent | LLM security, prompt injection research, practical AI | Blog (simonwillison.net) |
| Kai Greshake | CISPA | Indirect prompt injection (wrote the foundational paper) | Papers + social |
| Johann Rehberger | Red Team Director | Real-world LLM vulnerability discovery, indirect prompt injection demos | Blog (embracethered.com) |
| Daniel Miessler | Fabric / AI | AI security frameworks, practical security | Blog + newsletter |
| Elie Bursztein | Google | AI security research | Blog + papers |

### Blogs & Newsletters

| Source | Focus | Frequency |
|--------|-------|-----------|
| Trail of Bits Blog | Security research including ML/AI | Weekly |
| Protect AI Blog | ML security tools, vulnerability research | Regular |
| Lakera Blog | LLM security, prompt injection defense | Regular |
| NVIDIA AI Red Team Blog | Practical AI red teaming | Occasional |
| The MLSecOps Podcast | ML security operations | Biweekly |
| Latent Space (Podcast) | AI engineering (already in your plan) | Weekly |
| Simon Willison's Weblog | LLM security observations, practical demos | Daily |
| Embracing the Red (Rehberger) | LLM vulnerability research, PoC demos | Regular |

### Communities

| Community | Platform | Focus |
|-----------|----------|-------|
| OWASP AI Security Slack | Slack | AI security standards, LLM Top 10 discussions |
| HTB Discord | Discord | Already in your plan |
| AI Village (DEFCON) | Discord + annual conference | AI security research community |
| MLSecOps Community | Various | ML pipeline security |
| Protect AI Community | Discord | ML security tooling |

-----

## 7. Conferences & Talks (Free Recordings)

| Conference/Talk | Where to Watch | Focus |
|----------------|----------------|-------|
| DEF CON AI Village | YouTube | Annual AI security talks, CTFs, tool demos |
| Black Hat AI Track | YouTube (select talks) | Enterprise AI security |
| NeurIPS ML Safety Workshop | Papers + recordings | Academic ML safety research |
| USENIX Security AI papers | Papers + recordings | Peer-reviewed AI security research |
| AdvML Workshop (various venues) | Papers + recordings | Adversarial ML research |
| AI Red Team Con | YouTube/recordings | Dedicated AI red teaming conference |

**Recommended talks to watch during Track 10:**
- Any Nicholas Carlini talk on adversarial ML or training data extraction
- DEF CON AI Village keynotes (2023-2025)
- "Hacking AI" talks from Black Hat / DEF CON main tracks
- Anthropic / OpenAI red teaming methodology talks

-----

## 8. Datasets & Benchmarks for Testing

| Resource | Focus | Use Case |
|----------|-------|----------|
| AdvBench | Harmful behaviors benchmark | Testing LLM safety alignment |
| JailbreakBench | Standardized jailbreak evaluation | Measuring jailbreak success rates |
| ToxiGen | Implicit toxic language | Testing content filters |
| RealToxicityPrompts | Toxicity generation | Evaluating output safety |
| TruthfulQA | Truthfulness measurement | Testing hallucination rates |
| LMSYS Arena | Model comparison | Understanding model-specific vulnerabilities |

-----

## 9. Architecture Katas for AI Security

Practice exercises you can do during Track 10 to sharpen AI security architecture thinking.

### Kata 1: Threat Model a RAG Application
Design the architecture of a RAG app, then identify every attack surface:
- Document ingestion pipeline (poisoning)
- Embedding model (adversarial inputs)
- Vector database (injection)
- Retrieval chain (manipulation)
- LLM generation (prompt injection via context)
- Output to user (insecure output handling)

### Kata 2: Design a Secure LLM Gateway
Architecture a gateway that sits between users and an LLM:
- Input validation layer
- Prompt injection detection
- Output filtering
- Rate limiting
- Cost controls (denial of wallet prevention)
- Logging and monitoring

### Kata 3: Red Team an AI Agent System
Map the attack surface of an LLM agent with tool access:
- Tool execution privileges
- Memory/state manipulation
- Multi-turn conversation exploitation
- Tool output injection
- Infinite loop triggering
- Privilege escalation via tool chains

### Kata 4: Secure ML Pipeline Assessment
Review a typical ML pipeline for security weaknesses:
- Training data provenance
- Model artifact integrity
- Dependency supply chain
- CI/CD for ML (MLOps)
- Model serving infrastructure
- Monitoring and drift detection

-----

## 10. Books: AI/ML Security Library

Your plan uses three books actively (Wilson in Track 7, Dursey + Huyen in Track 10). The broader field has a growing library of practitioner and academic books. These are catalogued here for reference; see `future-technical-reading.md` for reading order and prioritization.

### Books Already in Your Plan

| Book | Author | Publisher | Year | Status |
|------|--------|-----------|------|--------|
| The Developer's Playbook for Large Language Model Security | Steve Wilson | O'Reilly | 2024 | **Owned** — Track 7 |
| Red Teaming AI: A Field Manual for Attacking Intelligent Systems | Philip A. Dursey | No Starch Press | 2026 | **Owned** — Track 10 |
| AI Engineering | Chip Huyen | O'Reilly | 2025 | To purchase — Track 10 |

### Practitioner Books (Post-Plan Reading)

| Book | Author | Publisher | Year | ~Cost | Focus |
|------|--------|-----------|------|-------|-------|
| Not with a Bug, But with a Sticker | Ram Shankar Siva Kumar & Hyrum Anderson | Wiley | 2023 | ~$30 | Adversarial ML threats from Microsoft's AI Red Team founder. Accessible, real-world case studies. Foreword by Bruce Schneier. |
| Adversarial AI Attacks, Mitigations, and Defense Strategies | John Sotiropoulos | Packt | 2024 | ~$50 | Most hands-on guide bridging traditional adversarial ML with LLM/GenAI security. ~580 pages. OWASP LLM Top 10 co-lead. |
| Beyond the Algorithm: AI, Security, Privacy, and Ethics | Omar Santos & Petar Radanliev | Pearson | 2024 | ~$50 | Broad AI security reference. Cisco Distinguished Engineer, DEF CON Red Team Village lead. |
| AI-Native LLM Security | Vaibhav Malik, Ken Huang, Ads Dawson | Packt | 2025 | ~$50 | Most current LLM security guide. Trust boundaries, MLSecOps, CI/CD security. All authors OWASP Top 10 for LLM core team. |
| Generative AI Security: Theories and Practices | Ken Huang, Yang Wang, et al. | Springer | 2024 | ~$60 | GenAI architectures, DevSecOps for AI, global AI regulations. OWASP + NIST GenAI Working Group contributor. |
| Large Language Models in Cybersecurity | Kucharavy et al. | Springer | 2024 | **FREE** | Open-access. Swiss Cyber-Defence Campus. LLM threats from national security angle. |

### Academic References

| Book | Author | Publisher | Year | ~Cost | Focus |
|------|--------|-----------|------|-------|-------|
| Adversarial Robustness for Machine Learning | Pin-Yu Chen & Cho-Jui Hsieh | Elsevier | 2023 | ~$100 | Most complete academic textbook — attack algorithms, verification, defenses, threat models. |
| Adversarial Machine Learning: Attack Surfaces, Defence Mechanisms, Learning Theories | Chivukula et al. | Springer | 2023 | ~$80 | Game-theoretic adversarial deep learning, perturbation-based privacy, CV/NLP/cybersecurity defenses. |
| Adversarial Machine Learning | Joseph, Nelson, Rubinstein, Tygar | Cambridge UP | 2019 | ~$55 | Foundational reference. Most-cited comprehensive introduction. UC Berkeley, Google, UMelbourne researchers. |

### How the Books Relate to Each Other

```
Foundational Theory                    Practitioner Guides                  Your Plan (Active)
─────────────────                      ───────────────────                  ──────────────────
Joseph et al. (2019)                   Kumar & Anderson (2023)              Wilson (Track 7)
  └─ foundational concepts               └─ why adversarial ML matters       └─ OWASP LLM Top 10
Chen & Hsieh (2023)                    Sotiropoulos (2024)                  Dursey (Track 10)
  └─ attack/defense algorithms            └─ hands-on offense + defense       └─ red team methodology
Chivukula et al. (2023)                Santos & Radanliev (2024)            Huyen (Track 10)
  └─ game theory + deep learning          └─ broad AI security + compliance   └─ production AI systems
                                       Huang et al. (2024)
                                         └─ GenAI governance + DevSecOps
                                       Malik et al. (2025)
                                         └─ LLM-specific, latest OWASP
                                       Kucharavy et al. (2024) — FREE
                                         └─ national security perspective
```

**Reading order after plan completion:** Sotiropoulos → Kumar & Anderson → Malik et al. → then branch based on need (Santos for compliance, Huang for governance, academic texts for theory depth).

-----

## 11. How These Resources Map to Your Plan

```
Track 7 (Week 8): LLM Security Primer
  Already covered: Wilson book, OWASP LLM Top 10, HackAPrompt
  ADD: Gandalf (lakera.ai) as warm-up practice
  ADD: Simon Willison's blog for real-world prompt injection examples

Track 10 Phase 1 (Weeks 21-22): ML Fundamentals
  Already covered: Fast.ai, Hugging Face NLP, AI Engineering Ch 2
  ADD: Goodfellow 2014 (FGSM paper) - foundational reading
  ADD: ART (IBM) for hands-on adversarial example generation
  ADD: Carlini's YouTube lectures on ML security

Track 10 Phase 2 (Weeks 23-24): HTB Labs
  Already covered: HTB Academy, Garak
  ADD: Gandalf before HTB (warm-up)
  ADD: Vigil for prompt injection analysis
  ADD: Greshake 2023 paper (indirect prompt injection)

Track 10 Phase 3 (Weeks 25-26): RAG/Agents + Supply Chain
  Already covered: AI Engineering Ch 5-6, LangChain, MITRE ATLAS
  ADD: ModelScan (Protect AI) for model file scanning
  ADD: Carlini 2023 (poisoning web-scale datasets)
  ADD: Prompt Airlines for RAG-adjacent practice
  ADD: OWASP ML Top 10 (classic ML, not just LLMs)

Track 10 Phase 4 (Weeks 27-28): Evaluation + CTF
  Already covered: HackAPrompt, Crucible, PyRIT, NIST, Google SAIF
  ADD: Tensor Trust (competitive prompt attack/defense)
  ADD: JailbreakBench for standardized evaluation
  ADD: EU AI Act awareness (regulatory context for reports)
  ADD: Architecture Katas 1-4 (above)

Track 11 Phase 2 (Weeks 42-43): Go AI Security Capstone
  ADD: Reference ART attack patterns when designing Go tool
  ADD: Use JailbreakBench prompts as test input library
```

-----

## Summary: What to Add vs What's Already Covered

Your plan already covers the core tools and resources well. The main gaps are:

1. **Academic papers** — Your plan is practice-heavy (great) but light on the foundational research. Adding 5-8 key papers deepens your understanding of *why* attacks work.

2. **Additional CTF platforms** — Gandalf (warm-up) and Tensor Trust (competitive) complement HTB + HackAPrompt + Crucible nicely.

3. **Defense-side tools** — Your plan is offense-focused. Adding ModelScan, LLM Guard, and Rebuff gives you the defender's perspective (which makes you a better attacker).

4. **Classic ML attacks** — OWASP ML Top 10 covers adversarial examples, model extraction, etc. beyond just LLM prompt injection. Important for "AI Red Teamer" vs "LLM Red Teamer."

5. **Community and researchers** — Following Carlini, Willison, Rehberger, and the Trail of Bits blog keeps you current as the field evolves rapidly.

6. **Books beyond your plan** — Section 10 catalogues the broader AI/ML security book landscape. Your plan's three books (Wilson, Dursey, Huyen) cover the essentials; the post-plan reading list in `future-technical-reading.md` prioritizes what to read next.

**No additional cost for sections 1-9.** Everything except the books in section 10 is free.
