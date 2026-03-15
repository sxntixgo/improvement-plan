# Gap Analysis: AI Security Books TOC vs Improvement Plan

**Date:** March 15, 2026
**Method:** Cross-referenced the full table of contents of 9 AI/ML security books against Track 7 (LLM Security Primer), Track 10 (AI/ML Security), and the future reading list to identify topics the plan doesn't adequately prepare you for.

---

## What the Plan Already Covers Well

Before identifying gaps, credit where it's due. These topics are well-covered across Track 7, Track 10, and supporting resources:

| Topic | Coverage |
|-------|----------|
| Prompt injection (direct + indirect) | Wilson Ch 4, Dursey Ch 6, Huyen Ch 5, HTB labs |
| Data poisoning | Dursey Ch 4, HTB labs |
| Evasion attacks at inference | Dursey Ch 5 |
| Model extraction/theft | Dursey Ch 8, Wilson Ch 7 |
| RAG & agent security | Huyen Ch 6, Dursey Ch 7, Week 25 hands-on |
| ML supply chain attacks | Wilson Ch 8, Track 10 Week 26 |
| OWASP LLM Top 10 | Wilson Ch 2, referenced throughout |
| Red team methodology & reporting | Dursey Ch 1-2, 9-10 |
| ML fundamentals | Fast.ai, Hugging Face NLP course |
| Professional frameworks | NIST AI RMF, MITRE ATLAS, Google SAIF |
| Evaluation methodology | Huyen Ch 3-4 |
| Automated red team tooling | Garak, PyRIT, Claude SDK |

**Verdict:** The plan's core LLM red teaming coverage is strong. The gaps are mostly in breadth (non-LLM AI attacks), depth (formal defense theory), and operational maturity (MLSecOps, incident response, regulation).

---

## Gap 1: Deepfakes and GAN-Based Attacks — NOT COVERED

**Severity: HIGH for an AI red teamer**

**What the TOC reveals:**
- Book 1 Ch 12 has extensive coverage: StyleGAN fake image generation, face verification evasion, voice deepfakes, password cracking with GANs, malware detection evasion, generating adversarial payloads with GANs
- Book 4 Ch 2 covers GANs, VAEs, and other generative model architectures
- Book 2 ("Not with a Bug, But with a Sticker") is literally about physical-world adversarial examples

**What the plan covers:** Nothing. Track 10 focuses exclusively on LLM/text-based attacks. Deepfakes, synthetic media, and GAN-based attacks are completely absent.

**Why it matters:** Deepfakes are one of the most visible AI threats. An AI red teamer who can't assess deepfake risks or test face verification systems has a significant blind spot. GANs are also used to generate adversarial examples, evade malware detectors, and crack passwords — all offensive security use cases.

**Recommendation:** Add a 2-day module to Track 10 Phase 2 or Phase 4 covering:
- GAN architecture basics (generator vs discriminator)
- Deepfake generation and detection techniques
- Face verification evasion
- Voice deepfake awareness
- Direct Claude Code to build a simple deepfake detector

**Books that cover this:** Sotiropoulos Ch 12 (Tier 1 future reading), Santos Ch 2 (Tier 2)

---

## Gap 2: Adversarial Attacks Beyond LLMs/NLP — MINIMAL COVERAGE

**Severity: MEDIUM-HIGH**

**What the TOC reveals:**
- Book 7 Part 5 covers attacks on: Graph Neural Networks, Recommender Systems, Reinforcement Learning, Speech Models, Multi-Modal Models, and non-neural-network ML models
- Book 1 Part 3 covers evasion attacks on deployed computer vision models (FGSM, BIM, JSMA, C&W, PGD, adversarial patches)
- Book 8 Ch 6 covers physical-world attacks on images and texts

**What the plan covers:** Dursey Ch 5 covers "evasive attacks at inference" generally, but the plan doesn't go deep on specific attack algorithms (FGSM, PGD, C&W) or attacks on non-text modalities (vision, speech, recommender systems, RL).

**Why it matters:** AI red teaming engagements don't only target chatbots. Organizations deploy computer vision (autonomous vehicles, medical imaging, surveillance), recommendation engines, speech recognition, and multi-modal systems. Understanding adversarial perturbation techniques (even conceptually) across modalities makes you a more complete red teamer.

**Recommendation:** No plan change needed for the 44-week timeline — LLM focus is correct for your career entry point. But flag this as the **first area to deepen after plan completion**. Specifically:
- Book 7 (Adversarial Robustness) Part 2 and Part 5 should be your first academic reading
- Sotiropoulos Ch 7 (evasion attacks) has hands-on attack walkthroughs

**Priority for future reading:** Move Sotiropoulos higher — it covers both LLM and classical ML attacks in one book.

---

## Gap 3: Privacy-Preserving AI Techniques — NOT COVERED

**Severity: MEDIUM**

**What the TOC reveals:**
- Book 1 Ch 10: Privacy-Preserving AI (full chapter)
- Book 3 Ch 10: Differential privacy, federated learning as defensive innovations
- Book 5 Ch 5: GenAI Data Security
- Book 7 Ch 27: Privacy and Watermarking
- Book 8 Ch 7: Adversarial Perturbation for Privacy Preservation

**What the plan covers:** The plan covers privacy *attacks* well (model extraction, data extraction, membership inference via Dursey Ch 8). It does NOT cover privacy-preserving *defenses*: differential privacy, federated learning, homomorphic encryption, secure multi-party computation.

**Why it matters:** A red teamer who understands privacy-preserving defenses can:
- Identify when differential privacy is implemented incorrectly (still leaks data)
- Find weaknesses in federated learning deployments (gradient attacks)
- Assess whether privacy claims in AI systems actually hold up
- Write more credible reports that acknowledge defense mechanisms

**Recommendation:** Add a half-day reading block in Track 10 Phase 1 (Week 22) or Phase 4 (Week 27):
- Conceptual overview of differential privacy, federated learning, and their known weaknesses
- No hands-on needed — just enough to recognize these defenses and know their limits
- Reference: NIST AI RMF already in the plan covers governance aspects

---

## Gap 4: AI Regulation, Legal, and Compliance Frameworks — THIN COVERAGE

**Severity: MEDIUM**

**What the TOC reveals:**
- Book 3 Ch 5: Aligning LLM Security with Organizational Objectives and Regulatory Landscapes
- Book 4 Ch 8: Extensive legal coverage — patentability, copyright, trademark, liability, ethical development, international standards
- Book 5 Ch 3: AI Regulations (full chapter)
- Book 3 Ch 10: The evolving regulatory landscape
- Book 6 Ch 16: Copyright-related risks in ML/AI systems

**What the plan covers:** NIST AI RMF and Google SAIF are referenced for report framing (Track 10 Week 28). EU AI Act, liability frameworks, copyright issues, and organizational compliance are not covered.

**Why it matters:** Professional red team reports increasingly need to map findings to regulatory requirements (EU AI Act, NIST AI RMF, industry-specific regulations). Understanding the regulatory landscape helps you:
- Frame findings in language that executives and legal teams understand
- Prioritize vulnerabilities based on compliance impact
- Advise on remediation that satisfies regulatory requirements
- Differentiate yourself from purely technical red teamers

**Recommendation:** Add a 2-hour reading block in Track 10 Week 28 (already the "reporting and frameworks" week):
- Overview of EU AI Act risk categories and how they apply to LLM deployments
- How to map red team findings to regulatory requirements
- Reference: Book 3 Ch 5 or Book 4 Ch 8 as future reading when you need depth

---

## Gap 5: MLSecOps and AI Security in the Development Lifecycle — SURFACE-LEVEL

**Severity: MEDIUM**

**What the TOC reveals:**
- Book 1 Part 5: Secure-by-Design AI (Ch 17), AI Security with MLSecOps (Ch 18), Maturing AI Security (Ch 19) — three full chapters
- Book 3 Ch 11: Integrating Security into LLM Development Lifecycle (data curation → deployment)
- Book 3 Ch 12: Monitoring, Incident Response, and Continuous Improvement — very detailed (anomaly detection, incident response plans, post-incident review, root cause analysis)
- Book 5 Ch 8: From LLMOps to DevSecOps for GenAI

**What the plan covers:** Wilson Ch 10 gives a 1-hour overview of LLMOps. Track 10 doesn't go deeper into how security integrates into the ML pipeline, how to monitor AI systems in production, or how to respond to AI security incidents.

**Why it matters:** Red teamers who understand MLSecOps can:
- Recommend actionable remediation (not just "fix the vulnerability" but "add this to your CI/CD pipeline")
- Identify gaps in an organization's AI security posture beyond individual vulnerabilities
- Provide monitoring recommendations that detect the attacks they demonstrated
- Write reports that include operational security recommendations

**Recommendation:** No plan change needed for the 44-week timeline. This is operational security knowledge that deepens with professional experience. Flag Sotiropoulos Part 5 (Secure-by-Design, MLSecOps) and Book 3 Ch 11-12 (Monitoring, IR) as priority post-plan reading when you start doing professional engagements.

---

## Gap 6: Trojan Horse Attacks and Model Reprogramming — NOT COVERED

**Severity: MEDIUM-LOW**

**What the TOC reveals:**
- Book 1 Ch 5: Model Tampering with Trojan Horses and Model Reprogramming — distinct from data poisoning
- Book 7 Ch 22: Backdoor Attack and Defense — separate from data poisoning chapter
- Book 1 Ch 4: Distinguishes between backdoor poisoning, hidden-trigger backdoor attacks, and clean-label attacks

**What the plan covers:** Dursey Ch 4 covers "Poisoning the Well: Corrupting AI Data" but doesn't distinguish between simple data poisoning, backdoor/trojan insertion, hidden triggers, and model reprogramming. These are distinct attack classes with different techniques and defenses.

**Why it matters:** In professional red teaming, the distinction matters:
- **Data poisoning:** Corrupt training data to degrade model performance
- **Backdoor/Trojan:** Insert a hidden trigger that activates specific malicious behavior while the model appears normal otherwise
- **Model reprogramming:** Repurpose a model to perform a completely different task without retraining
- **Clean-label attacks:** Poison data without changing labels (harder to detect)

**Recommendation:** No plan change. Dursey Ch 4 provides sufficient exposure for the 44-week plan. Add Sotiropoulos Ch 4-5 to your Tier 1 reading list notes — they provide the granular attack taxonomy you'll want for professional depth.

---

## Gap 7: Formal Verification and Certified Defenses — NOT COVERED

**Severity: LOW (for practitioner, HIGH for researcher)**

**What the TOC reveals:**
- Book 7 Part 3 (4 full chapters): Convex Relaxation Framework, Layer-Wise Relaxation, Dual Approach, Probabilistic Verification
- Book 7 Ch 12: Certified Defense
- Book 1 Ch 7: Certified defenses (mentioned in evasion attack defenses)

**What the plan covers:** Nothing. The plan focuses on attacks and practical defenses (adversarial training, input preprocessing, model ensembles).

**Why it matters:** Certified defenses provide mathematical guarantees that a model's prediction won't change within a certain perturbation radius. Understanding these helps a red teamer:
- Assess whether a claimed "robust" model actually has provable guarantees
- Know the limits of certification (it doesn't scale well, has restricted threat models)
- Communicate intelligently about robustness guarantees in reports

**Recommendation:** No plan change. This is academic/research territory. Reference-only if you encounter certified defense claims in an engagement. Book 7 Part 3 is where to go if needed.

---

## Gap 8: Social Engineering and Influence Operations with LLMs — NOT COVERED

**Severity: MEDIUM**

**What the TOC reveals:**
- Book 6 Ch 8: Phishing and Social Engineering in the Age of LLMs
- Book 6 Ch 11: LLM-Aided Social Media Influence Operations
- Book 3 Ch 10: Automated social engineering as an emerging threat
- Book 3 Ch 10: Ethical manipulation and psychological impacts

**What the plan covers:** Nothing explicit. The plan focuses on attacking AI systems, not using AI systems as attack tools for social engineering.

**Why it matters:** AI red teaming increasingly includes assessing whether an organization's AI systems can be weaponized for:
- Automated phishing at scale (LLM-generated spear phishing)
- Social media manipulation campaigns
- Impersonation and pretexting
- Psychological manipulation of users

**Recommendation:** Add awareness-level coverage. A 1-hour reading block during Track 10 Week 27-28 on:
- How LLMs enable scaled social engineering
- Red team scenarios: "Can this chatbot be made to phish users?"
- Reference: Book 6 Ch 8 (free, open access) is the perfect resource

---

## Gap 9: LLM-Generated Code Vulnerabilities — NOT COVERED

**Severity: MEDIUM (directly relevant to your Claude Code workflow)**

**What the TOC reveals:**
- Book 6 Ch 9: Vulnerabilities Introduced by LLMs through Code Suggestions

**What the plan covers:** Nothing. Ironic given that your entire workflow is "Claude Code writes the code." The plan doesn't address the security implications of AI-generated code.

**Why it matters:** You're an architect who directs Claude Code to write all your code. Understanding the systematic vulnerabilities that LLMs introduce through code suggestions is directly relevant to:
- Your daily work (reviewing Claude Code output for security flaws)
- Your red teaming career (assessing organizations that use AI-assisted development)
- Your portfolio (unique angle: "I red team the code my AI writes")

**Recommendation:** Add a 2-hour awareness module to Track 10 Phase 4 (Week 27) or even Track 3 (Claude Code Advanced):
- Common vulnerability patterns in LLM-generated code
- How to review AI-generated code for security issues
- OWASP considerations for AI-assisted development
- Reference: Book 6 Ch 9 (free, open access)

---

## Gap 10: Game-Theoretic Adversarial ML — NOT COVERED

**Severity: LOW**

**What the TOC reveals:**
- Book 8 Ch 4: Game Theoretical Adversarial Deep Learning — game-theoretic strategies for generating adversarial manipulations
- Book 9 Ch 3: A Framework for Secure Learning (formal framework)

**What the plan covers:** Nothing. The plan takes a practical/applied approach to adversarial ML.

**Why it matters:** Game theory provides the mathematical framework for understanding adversarial interactions as strategic games between attacker and defender. This is primarily academic but helps in:
- Understanding why the arms race between attacks and defenses is inherently difficult
- Formalizing threat models
- Advanced research if you pursue academic work

**Recommendation:** No plan change. This is research-level content. Reference only.

---

## Summary: Priority-Ranked Gaps

| # | Gap | Severity | Action | Effort |
|---|-----|----------|--------|--------|
| 1 | Deepfakes and GAN-based attacks | HIGH | Add 2-day module to Track 10 | Medium |
| 2 | Adversarial attacks beyond LLMs | MEDIUM-HIGH | Flag for post-plan; reprioritize future reading | None (plan) |
| 3 | Privacy-preserving AI defenses | MEDIUM | Add half-day reading block | Low |
| 4 | AI regulation and compliance | MEDIUM | Add 2-hour block to Week 28 | Low |
| 5 | MLSecOps / AI security lifecycle | MEDIUM | Flag for post-plan reading | None (plan) |
| 6 | Trojan/backdoor attack taxonomy | MEDIUM-LOW | No change; Dursey Ch 4 sufficient | None |
| 7 | Formal verification / certified defense | LOW | No change; reference only | None |
| 8 | Social engineering with LLMs | MEDIUM | Add 1-hour awareness block | Low |
| 9 | LLM-generated code vulnerabilities | MEDIUM | Add 2-hour module (high relevance to workflow) | Low |
| 10 | Game-theoretic adversarial ML | LOW | No change; academic only | None |

---

## Recommended Plan Changes

### Changes Worth Making (fit within existing timeline)

1. **Track 10 Week 27 — Add "AI-Generated Code Vulnerabilities" (2 hours)**
   - Directly relevant to your Claude Code workflow
   - Reference: Book 6 Ch 9 (free, open access)
   - Replace 2 hours of catch-up time in Week 27

2. **Track 10 Week 28 — Add "AI Regulatory Landscape" (2 hours)**
   - Strengthen your reporting week with compliance context
   - Reference: EU AI Act overview + NIST AI RMF (already in plan)
   - Fits naturally with the existing "professional frameworks" block

3. **Track 10 Week 22 — Add "Privacy-Preserving AI Concepts" (2 hours)**
   - Conceptual only: differential privacy, federated learning, their weaknesses
   - Makes you a better attacker by understanding defenses
   - Reference: Conceptual overview, no book purchase needed

4. **Track 10 Week 27 — Add "LLMs as Social Engineering Tools" (1 hour)**
   - Awareness-level: how LLMs enable scaled phishing and manipulation
   - Reference: Book 6 Ch 8 (free, open access)

**Total time added:** ~7 hours across 3 weeks. This fits within existing slack/catch-up time without extending the plan.

### Changes to Defer (post-plan)

5. **Deepfakes and GAN-based attacks** — Most significant gap, but adding a full module would overload Track 10. Instead:
   - Add to Tier 1 future reading notes: "Sotiropoulos Ch 12 is your first priority after plan completion"
   - Consider adding a standalone 1-week "Deepfakes & Synthetic Media" mini-track between Track 10 and Track 9 if you find you have extra capacity

6. **Adversarial attacks beyond LLMs** — Reprioritize future reading order:
   - Sotiropoulos should be read FIRST after plan completion (covers both LLM and classical ML attacks)
   - Book 7 (Chen & Hsieh) Part 2 and Part 5 for cross-modality attack depth
   - "Not with a Bug, But with a Sticker" for physical-world adversarial context

7. **MLSecOps depth** — Operational knowledge that deepens with professional experience. Sotiropoulos Part 5 and Book 3 Ch 11-12 when you start professional engagements.

---

## Impact on Future Reading Priorities

Based on this gap analysis, the post-plan reading order should be adjusted:

**Current Tier 1 order (no explicit priority):**
All 7 books listed equally.

**Recommended Tier 1 order:**
1. **Sotiropoulos** — Covers the most gaps: deepfakes (Ch 12), classical ML attacks (Part 2-3), MLSecOps (Part 5), trojan attacks (Ch 5). The single most gap-filling book.
2. **Kumar & Anderson ("Not with a Bug, But with a Sticker")** — Physical-world adversarial examples, strategic perspective on AI red teaming.
3. **Malik et al. (AI-Native LLM Security)** — OWASP deep profiles, regulatory alignment, trust boundary mapping, monitoring/IR.
4. **Raschka (Build LLM From Scratch)** — Model internals for deeper attack understanding.
5. **Shostack (Threat Modeling)** — Formal methodology for professional engagements.
6. **Khononov (DDD)** — Architecture depth.
7. **Kleppmann (DDIA)** — Systems depth.

**Also:** Book 6 (LLMs in Cybersecurity) is free and open access. Move it from Tier 2 to a "read anytime" recommendation — Chapters 8, 9, and 11 directly address Gaps 8 and 9 at zero cost.

---

## Bottom Line

The plan's **LLM-focused red teaming core is solid** — no critical gaps in the primary career path. The gaps are:
- **Breadth gaps** (non-LLM AI attacks, deepfakes, physical-world adversarial) that matter as you grow from "LLM red teamer" to "AI red teamer"
- **Contextual gaps** (regulation, privacy defenses, social engineering) that make you a more complete professional
- **Meta gap** (LLM-generated code vulnerabilities) that's uniquely relevant to your Claude Code workflow

The 4 recommended in-plan changes add ~7 hours of awareness-level content. The bigger gaps (deepfakes, cross-modality attacks) are correctly deferred to post-plan reading, but Sotiropoulos should be explicitly prioritized as the #1 post-plan book since it fills the most gaps.
