# AI/ML Security Books — Table of Contents

## Book 1: Adversarial AI Attacks, Mitigations, and Defense Strategies

**Author:** John Sotiropoulos
**Publisher:** Packt (July 2024) | **Pages:** ~586 | **ISBN:** 9781835087985

-----

### Part 1: Introduction to Adversarial AI

#### Chapter 1: Getting Started with AI
- What is AI and ML
- Models, training, validation, testing, and inference
- Types of ML (supervised, unsupervised, etc.)
- Popular ML algorithms
- Deep learning fundamentals
- Neural networks: CNNs, RNNs, LLMs (BERT, ChatGPT)

#### Chapter 2: Building Our Adversarial Playground
- Setting up a Python development environment
- Creating a Python virtual environment
- Working with ML algorithms hands-on
- Building ML models
- Deploying a neural network as a REST prediction service
- Creating the "adversarial playground" target

#### Chapter 3: Security and Adversarial AI
- Technical requirements
- Security fundamentals
- Threat modeling
- Risks and mitigations
- DevSecOps
- Securing our adversarial playground
  - Host security
  - Network protection
  - Authentication
  - Data protection
  - Access control
- Securing code and artifacts
  - Secure code
  - Securing dependencies with vulnerability scanning
  - Secret scanning
  - Securing Jupyter Notebooks
  - Securing models from malicious code
  - Integrating with DevSecOps and MLOps pipelines
- Bypassing security with adversarial AI
- Our first adversarial AI attack
- Traditional cybersecurity and adversarial AI
- Adversarial AI landscape

-----

### Part 2: Model Development Attacks

#### Chapter 4: Poisoning Attacks
- Basics of poisoning attacks
  - Definition and examples
  - Types of poisoning attacks
  - Poisoning attack examples
  - Why it matters
- Staging a simple poisoning attack
  - Creating poisoned samples
- Backdoor poisoning attacks
  - Creating backdoor triggers with ART
  - Poisoning data with ART
- Hidden-trigger backdoor attacks
- Clean-label attacks
- Advanced poisoning attacks
- Mitigations and defenses
  - Cybercity defenses with MLOps
  - Anomaly detection
  - Robustness tests against poisoning
  - Advanced poisoning defenses with ART
  - Adversarial training
  - Creating a defense strategy

#### Chapter 5: Model Tampering with Trojan Horses and Model Reprogramming
- Trojan horse attacks on ML models
- Model reprogramming techniques
- Backdoor insertion methods
- Attack scenarios and demonstrations
- Defenses and mitigations

#### Chapter 6: Supply Chain Attacks and Adversarial AI
- Traditional supply chain risks and AI
  - Risks from outdated and vulnerable components
  - Risks from AI's dependency on live data
  - Securing AI from vulnerable components
  - Enhanced security — allow approved-only packages
  - Client configuration for private PyPI repositories
  - Additional private PyPI security
  - Use of SBOMs
- AI supply chain risks
  - The double-edged sword of transfer learning
  - Model poisoning
  - Model tampering
  - Secure model provenance and governance for pre-trained models
  - MLOps and private model repositories
  - Data poisoning
  - Using data poisoning to affect sentiment analysis
- Defenses and mitigations
  - AI/ML SBOMs

-----

### Part 3: Attacks on Deployed AI

#### Chapter 7: Evasion Attacks against Deployed AI
- Fundamentals of evasion attacks
  - Importance of understanding evasion attacks
  - Reconnaissance techniques for evasion attacks
  - Perturbations and image evasion attack techniques
- Evasion attack scenarios
  - One-step perturbation with FGSM
  - Basic Iterative Method (BIM)
  - Jacobian-based Saliency Map Attack (JSMA)
  - Carlini and Wagner (C&W) attack
  - Projected Gradient Descent (PGD)
  - Adversarial patches — bridging digital and physical evasion techniques
- NLP evasion attacks with BERT using TextAttack
- Universal Adversarial Perturbations (UAPs)
- Black-box attacks with transferability
- Defending against evasion attacks
  - Mitigation strategies overview
  - Adversarial training
  - Input preprocessing
  - Model hardening techniques
  - Model ensembles
  - Certified defenses

#### Chapter 8: Privacy Attacks — Stealing Models
- Model extraction attacks
- Query-based extraction techniques
- Attack scenarios and demonstrations
- Inference attacks
- Defenses and mitigations against model stealing

#### Chapter 9: Privacy Attacks — Stealing Data
- (Subsections not publicly available)

#### Chapter 10: Privacy-Preserving AI
- (Subsections not publicly available)

-----

### Part 4: Generative AI and Adversarial Attacks

#### Chapter 11: Generative AI — A New Frontier
- (Subsections not publicly available)

#### Chapter 12: Weaponizing GANs for Deepfakes and Adversarial Attacks
- Use of GANs for deepfakes and deepfake detection
  - Using StyleGAN to generate convincing fake images
  - Creating simple deepfakes with GANs using existing images
  - Making direct changes to an existing image
  - Using Pix2PixHD to synthesize images
  - Fake videos and animations
  - Other AI deepfake technologies
  - Voice deepfakes
  - Deepfake detection
- Using GANs in cyberattacks and offensive security
  - Evading face verification
  - Compromising biometric authentication
  - Password cracking with GANs
  - Malware detection evasion
  - GANs in cryptography and stenography
  - Generating web attack payloads with GANs
  - Generating adversarial attack payloads
- Defenses and mitigations
  - Securing GANs
  - GAN-assisted adversarial attacks
  - Deepfakes, malicious content, and misinformation

#### Chapter 13: LLM Foundations for Adversarial AI
- A brief introduction to LLMs
- Developing AI applications with LLMs
  - Hello LLM with Python
  - Hello LLM with LangChain
  - Bringing your own data
- How LLMs change Adversarial AI

#### Chapter 14: Adversarial Attacks with Prompts
- Adversarial inputs and prompt injection
- Direct prompt injection
- Prompt override
- Style injection
- Role-playing

#### Chapter 15: Poisoning Attacks and LLMs
- (Subsections not publicly available)

#### Chapter 16: Advanced Generative AI Scenarios
- (Subsections not publicly available)

-----

### Part 5: Secure-by-Design AI and MLSecOps

#### Chapter 17: Secure by Design and Trustworthy AI
- (Subsections not publicly available)

#### Chapter 18: AI Security with MLSecOps
- (Subsections not publicly available)

#### Chapter 19: Maturing AI Security
- (Subsections not publicly available)

**Index**

-----

## Book 2: Not with a Bug, But with a Sticker

**Authors:** Ram Shankar Siva Kumar & Hyrum Anderson | **Foreword:** Bruce Schneier
**Publisher:** Wiley (2023) | **Pages:** ~300 | **ISBN:** 9781119883982

-----

**Foreword** (xv)

**Introduction** (xix)

### Chapter 1: Do You Want to Be Part of the Future? (1)
- Business at the Speed of AI
- Follow Me, Follow Me
- In AI, We Overtrust
- Area 52 Ramblings
- I'll Do It
- Adversarial Attacks Are Happening
- ML Systems Don't Jiggle-Jiggle; They Fold
- Never Tell Me the Odds
- AI's Achilles' Heel

### Chapter 2: Salt, Tape, and Split-Second Phantoms (29)
- Challenge Accepted
- When Expectation Meets Reality
- Color Me Blind
- Translation Fails
- Attacking AI Systems via Fails
- Autonomous Trap 001
- Common Corruption

### Chapter 3: Subtle, Specific, and Ever-Present (55)
- Intriguing Properties of Neural Networks
- They Are Everywhere
- Research Disciplines Collide
- Blame Canada
- The Intelligent Wiggle-Jiggle
- Bargain-Bin Models Will Do
- For Whom the Adversarial Example Bell Tolls

### Chapter 4: Here's Something I Found on the Web (85)
- Bad Data = Big Problem
- Your AI Is Powered by Ghost Workers
- Your AI Is Powered by Vampire Novels
- Don't Believe Everything You Read on the Internet
- Poisoning the Well

### Chapter 5: Why Is Defending Against Adversarial Attacks Hard? (107)
- Masking Is Important
- Because It Is Possible
- Masking Alone Is Not Good Enough
- An Average Concerned Citizen
- Security by Obscurity Has Limited Benefit
- The Opportunity Is Great; the Threat Is Real; the Approach Must Be Bold
- Swiss Cheese

### Chapter 6: Sailing for Adventure on the Deep Blue Sea (133)
- Why Be Securin' AI Systems So Blasted Hard?
- An Economics Perspective, Me Hearties!
- Tis a Sign, Me Mateys
- Here Be the Most Crucial AI Law Ye've Nary Heard Tell Of!
- Lies, Accursed Lies, and Explanations!
- No Free Grub
- Whatcha Measure Be Whatcha Get!
- Who Be Reapin' the Benefits?
- Cargo Cult Science

### Chapter 7: The Big One (159)
- This Looks Futuristic
- By All Means, Move at a Glacial Pace; You Know How That Thrills Me
- Waiting for the Big One
- Software, All the Way Down
- The Aftermath
- Race to AI Safety
- Happy Story
- In Medias Res
- Big-Picture Questions

**Acknowledgments** (185)

**Index** (189)

-----

## Book 3: AI-Native LLM Security

**Authors:** Vaibhav Malik, Ken Huang & Ads Dawson
**Publisher:** Packt (December 2025) | **Pages:** ~400 | **ISBN:** 9781836203759

-----

### Part 1: Understanding the LLM Security Landscape

#### Chapter 1: Fundamentals and Introduction to Large Language Models

#### Chapter 2: Securing Large Language Models

#### Chapter 3: The Dual Nature of LLM Risks: Inherent Vulnerabilities and Malicious Actors

#### Chapter 4: Mapping Trust Boundaries in LLM Architectures

#### Chapter 5: Aligning LLM Security with Organizational Objectives and Regulatory Landscapes

-----

### Part 2: OWASP Top 10 for LLM Applications — Deep Dive

#### Chapter 6: Identifying and Prioritizing LLM Security Risks with OWASP

#### Chapter 7: Diving Deep: Profiles of the Top 10 LLM Security Risks

#### Chapter 8: Mitigating LLM Risks: Strategies and Techniques for Each OWASP Category

#### Chapter 9: Identifying Risk Profiles for Different LLM Application Types
- Adapting the Top 10 to chatbots and conversational AI systems
  - SaaS
  - Cloud AI platforms
  - Private deployments
- Applying the Top 10 to content generation and creative AI applications
- Scaling the Top 10 for enterprise-wide LLM deployment and governance
  - Framework for enterprise governance
  - Implementing best practices for security

-----

### Part 3: Emerging Threats and Operational Security

#### Chapter 10: Emerging Threats & Promising Defensive Innovations
- Emerging threats:
  - Attacks on AI agents
  - Deepfake
  - Automated social engineering
  - Advanced supply chain attacks and model poisoning
  - Zero-day vulnerabilities in LLM frameworks
  - Cross-model attacks and transferability
  - Quantum computing threats
  - AI-driven malware and autonomous attacks
  - Ethical manipulation and psychological impacts
  - Challenges in explainability and transparency
  - Integration with critical infrastructure
  - Globalization of threat actors
  - Evolution of attack tools and techniques
- Promising defensive innovations:
  - Reinforcement learning for safe and accurate LLMs
  - Differential privacy for protecting sensitive data in LLMs
  - Adversarial training for strengthening LLM defenses
  - Explainable AI (XAI)
  - Secure model architectures for inherent resistance to attacks
  - Federated learning for decentralized training and enhanced privacy
  - Additional frontier research topics in LLM security
  - The evolving regulatory landscape

#### Chapter 11: Integrating Security into the LLM Development Life Cycle: From Data Curation to Deployment
- Secure data collection, curation, and preprocessing
- Protecting model integrity during training and validation
- Conducting rigorous security testing and evaluation

#### Chapter 12: Monitoring, Incident Response, and Continuous Improvement
- Designing comprehensive monitoring and alerting strategies
  - The monitoring hierarchy for LLM systems
  - Key monitoring metrics and indicators
  - Building a monitoring architecture
  - Implementing effective alerting strategies
  - Case study — monitoring architecture for an enterprise LLM platform
- Detecting anomalies and potential security incidents in LLM systems
  - Understanding LLM anomaly types
  - Detection techniques for LLM security
  - Configuring detectors and alarms
- Developing and executing effective incident response plans
  - Fundamentals of LLM incident response planning
  - Investigation and analysis techniques for LLM incidents
  - Containment and remediation strategies
- Conducting post-incident reviews and root cause analysis
  - Structured post-incident review processes
  - Root cause analysis for LLM security incidents
  - Identifying actionable lessons and improvements
- Driving continuous improvement of LLM security posture
  - Establishing a security improvement framework
  - Leveraging threat intelligence and emerging best practices

#### Chapter 13: (Final chapter — title not publicly available)

**Index**

-----

## Book 4: Beyond the Algorithm: AI, Security, Privacy, and Ethics

**Authors:** Omar Santos & Petar Radanliev
**Publisher:** Pearson (January 2024) | **Pages:** ~400 | **ISBN:** 9780138268459

-----

#### Chapter 1: Historical Overview of Artificial Intelligence (AI) and Machine Learning (ML)
- The Story of Eva
- The Origins
- Advancements of AI
- Understanding AI and ML
- Comparison of ML Algorithms
- Problems to Consider When Choosing a Suitable Algorithm
- Applications of ML Algorithms
- Use Cases for AI and ML
- Ethical Challenges in AI and ML
- Privacy and Security Challenges
- AI and ML in Cybersecurity
- Cyber Risk from AI and ML
- Concluding the Story of Eva
- Summary
- Test Your Skills
- Exercises

#### Chapter 2: Fundamentals of AI and ML Technologies and Implementations
- What Are the Leading AI and ML Technologies and Algorithms?
- Understanding Generative AI
- Generative Adversarial Networks (GANs)
- Variational Autoencoders (VAEs)
- Autoregressive Models
- Restricted Boltzmann Machines (RBMs)
- Normalizing Flows

#### Chapter 3: Emerging AI Trends
- OpenAI's GPT-4 and Beyond: A Breakthrough in Large Language Models
- Prompt Engineering
- Hugging Face
- Contributions to the NLP Landscape
- Auto-GPT: A Revolutionary Step in Autonomous AI Applications
- Responsibilities and Limitations

#### Chapter 4: The Cornerstones of AI and Machine Learning Security
- (Fundamental principles and best practices for safeguarding AI systems; goes beyond the OWASP Top 10 for LLMs)

#### Chapter 5: Hacking AI Systems
- (Deep dive into techniques and methodologies for exploiting AI vulnerabilities; prompt injection and other attacks)

#### Chapter 6: System and Infrastructure Security
- (Securing the underlying platforms on which AI and ML models operate)

#### Chapter 7: Privacy and Ethics: Navigating Privacy and Ethics in an AI-Infused World
- (Data collection, storage, security risks; personal privacy violations; algorithmic bias; user autonomy; accountability challenges)

#### Chapter 8: Legal and Regulatory Compliance for Artificial Intelligence (AI) Systems
- Conversational AI
- Patentability of AI Algorithms
- Copyright Protection for AI-Generated Content
- Trademark Protection for AI Systems
- Trade Secret Protection for AI Development
- Liability and Accountability
- Ethical Development and Deployment
- International Collaboration and Standards in AI
- Future Trends and Outlook in AI Compliance

**Index**

-----

## Book 5: Generative AI Security: Theories and Practices

**Authors:** Ken Huang, Yang Wang, Ben Goertzel, Yale Li, Sean Wright & Jyoti Ponnapalli
**Publisher:** Springer (April 2024) | **ISBN:** 9783031542510

### Part 1: Foundations of GenAI

#### Chapter 1: Foundations of Generative AI (3–30)

#### Chapter 2: Navigating the GenAI Security Landscape (31–58)

-----

### Part 2: Securing GenAI

#### Chapter 3: AI Regulations

#### Chapter 4: Build Your Security Program for GenAI (99–132)

#### Chapter 5: GenAI Data Security (133–162)

#### Chapter 6: GenAI Model Security (163–198)

#### Chapter 7: GenAI Application Level Security (199–237)

-----

### Part 3: Operationalizing GenAI Security

#### Chapter 8: From LLMOps to DevSecOps for GenAI (241–269)

#### Chapter 9: Utilizing Prompt Engineering to Operationalize Cybersecurity (271–303)

#### Chapter 10: Use GenAI Tools to Boost Your Security Posture (305–338)

-----

## Book 6: Large Language Models in Cybersecurity

**Editors:** Andrei Kucharavy, Octave Plancherel, Valentin Mulder, Alain Mermoud & Vincent Lenders
**Publisher:** Springer (May 2024) | **Pages:** ~247 | **ISBN:** 9783031548260 | **FREE** (Open Access)

-----

### Part I: Introduction

#### Chapter 1: From Deep Neural Language Models to LLMs
#### Chapter 2: Adapting LLMs to Downstream Applications
#### Chapter 3: Overview of Existing LLM Families
#### Chapter 4: Conversational Agents
#### Chapter 5: Fundamental Limitations of Generative LLMs
#### Chapter 6: Tasks for LLMs and their Evaluation

-----

### Part II: LLMs in Cybersecurity

#### Chapter 7: Private Information Leakage in LLMs
#### Chapter 8: Phishing and Social Engineering in the Age of LLMs
#### Chapter 9: Vulnerabilities Introduced by LLMs through Code Suggestions
#### Chapter 10: LLM Controls Execution Flow Hijacking
#### Chapter 11: LLM-Aided Social Media Influence Operations
#### Chapter 12: Deep(er) Web Indexing with LLMs

-----

### Part III: Exposure

#### Chapter 13: LLM Adoption Trends and Associated Risks
#### Chapter 14: The Flow of Investments in the LLM Space
#### Chapter 15: Insurance Outlook for LLM-Induced Risk
#### Chapter 16: Copyright-Related Risks in the Creation and Use of ML/AI Systems
#### Chapter 17: Monitoring Emerging Trends in LLM Research

-----

### Part IV: Mitigation

#### Chapter 18: Enhancing Security Awareness and Education for LLMs
#### Chapter 19: Towards Privacy-Preserving LLMs
#### Chapter 20–21: (Titles not publicly indexed — mitigation techniques for safe LLM deployment)
#### Chapter 22: LLM Detectors
#### Chapter 23–24: (Titles not publicly indexed — additional mitigation chapters)

-----

### Part V: Conclusion

#### Chapter 25: Standards for LLM Security
#### Chapter 26: Exploring the Dual Role of LLMs in Cybersecurity: Threats and Defenses

**Index**

-----

## Book 7: Adversarial Robustness for Machine Learning

**Authors:** Pin-Yu Chen & Cho-Jui Hsieh
**Publisher:** Elsevier (2022) | **ISBN:** 9780128240205

-----

### Part 1: Background

#### Chapter 1: Background and Motivation
- Mathematical notations and ML basics; motivating examples for adversarial robustness

-----

### Part 2: Adversarial Attacks

#### Chapter 2: White-Box Attack
#### Chapter 3: Soft-Label Black-Box Attack
#### Chapter 4: Decision-Based Attack
#### Chapter 5: Attack Transferability
#### Chapter 6: Attacks in the Physical World

-----

### Part 3: Verification

#### Chapter 7: Convex Relaxation Framework
#### Chapter 8: Layer-Wise Relaxation (Primal Algorithms)
#### Chapter 9: Dual Approach
#### Chapter 10: Probabilistic Verification

-----

### Part 4: Defense

#### Chapter 11: Adversarial Training
#### Chapter 12: Certified Defense
#### Chapter 13: Randomization
#### Chapter 14: Detection Methods

-----

### Part 5: Adversarial Examples Beyond Image Classification

#### Chapter 15: Robustness of Other Machine Learning Models Beyond Neural Networks
#### Chapter 16: NLP Models
#### Chapter 17: Graph Neural Network
#### Chapter 18: Recommender Systems
#### Chapter 19: Reinforcement Learning
#### Chapter 20: Speech Models
#### Chapter 21: Multi-Modal Models

-----

### Part 6: Other Threat Models and Applications

#### Chapter 22: Backdoor Attack and Defense
#### Chapter 23: Data Poisoning Attack and Defense
#### Chapter 24: Transfer Learning
#### Chapter 25: Explainability and Interpretability
#### Chapter 26: Representation Learning
#### Chapter 27: Privacy and Watermarking

**Index**

-----

## Book 8: Adversarial Machine Learning: Attack Surfaces, Defence Mechanisms, Learning Theories in Artificial Intelligence

**Authors:** Aneesh Sreevallabh Chivukula, Xinghao Yang, Bo Liu, Wei Liu & Wanlei Zhou
**Publisher:** Springer (March 2023) | **Pages:** ~302 | **ISBN:** 9783030997717

-----

#### Chapter 1: Adversarial Machine Learning
- Adversarial Learning Frameworks
- Adversarial Algorithms Comparisons
- Adversarial Security Mechanisms
- Adversarial Examples Taxonomies
- Stochastic Game Illustration

#### Chapter 2: Adversarial Deep Learning
- Learning Curve Analysis
- Adversarial Loss Functions
- Adversarial Examples in Deep Networks
- Generative Adversarial Networks
- Transfer Learning for Domain Adaptation

#### Chapter 3: Security and Privacy in Adversarial Learning

#### Chapter 4: Game Theoretical Adversarial Deep Learning
- Game theoretical strategies for generating adversarial manipulations

#### Chapter 5: Adversarial Defense Mechanisms for Supervised Learning

#### Chapter 6: Physical World Adversarial Attacks on Images and Texts
- Adversarial Attacks on Images (Gradient-Based, Score-Based, Decision-Based, Transformation-Based)
- Adversarial Attacks on Texts (Character-Level, Word-Level, Sentence-Level, Multilevel)
- Spam Filtering (Text Spam, Image Spam, Biometric Spam)

#### Chapter 7: Adversarial Perturbation for Privacy Preservation
- Visual Data Privacy Models
- Privacy Protection Mechanisms Using Adversarial Perturbations (File-Level, Object-Level, Feature-Level)

**Index**

-----

## Book 9: Adversarial Machine Learning (Joseph et al., 2019)

TOC: (To be researched)

-----
