# Book Tables of Contents

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
