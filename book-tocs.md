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

## Book 4: Build a Large Language Model (From Scratch)

**Author:** Sebastian Raschka
**Publisher:** Manning (2024) | **Pages:** ~368 | **ISBN:** 9781633437166

-----

### Chapter 1: Understanding Large Language Models
- 1.1 What is an LLM?
- 1.2 Applications of LLMs
- 1.3 Stages of building and using LLMs
- 1.4 Introducing the transformer architecture
- 1.5 Utilizing large datasets
- 1.6 A closer look at the GPT architecture
- 1.7 Building a large language model

### Chapter 2: Working with Text Data
- 2.1 Understanding word embeddings
- 2.2 Tokenizing text
- 2.3 Converting tokens into token IDs
- 2.4 Adding special context tokens
- 2.5 Byte pair encoding
- 2.6 Data sampling with a sliding window
- 2.7 Creating token embeddings
- 2.8 Encoding word positions

### Chapter 3: Coding Attention Mechanisms
- 3.1 The problem with modeling long sequences
- 3.2 Capturing data dependencies with attention mechanisms
- 3.3 Attending to different parts of the input with self-attention
- 3.4 Implementing self-attention with trainable weights
- 3.5 Hiding future words with causal attention
- 3.6 Extending single-head attention to multi-head attention

### Chapter 4: Implementing a GPT Model from Scratch to Generate Text
- 4.1 Coding an LLM architecture
- 4.2 Normalizing activations with layer normalization
- 4.3 Implementing a feed forward network with GELU activations
- 4.4 Adding shortcut connections
- 4.5 Connecting attention and linear layers in a transformer block
- 4.6 Coding the GPT model
- 4.7 Generating text

### Chapter 5: Pretraining on Unlabeled Data
- 5.1 Evaluating generative text models
  - 5.1.1 Using GPT to generate text
  - 5.1.2 Calculating the text generation loss
  - 5.1.3 Calculating the training and validation set losses
- 5.2 Training an LLM
- 5.3 Decoding strategies to control randomness
  - 5.3.1 Temperature scaling
  - 5.3.2 Top-k sampling
  - 5.3.3 Modifying the text generation function
- 5.4 Loading and saving model weights in PyTorch
- 5.5 Loading pretrained weights from OpenAI

### Chapter 6: Fine-tuning for Classification
- 6.1 Different categories of fine-tuning
- 6.2 Preparing the dataset
- 6.3 Creating data loaders
- 6.4 Initializing a model with pretrained weights
- 6.5 Adding a classification head
- 6.6 Calculating the classification loss and accuracy
- 6.7 Fine-tuning the model on supervised data
- 6.8 Using the LLM as a spam classifier

### Chapter 7: Fine-tuning to Follow Instructions
- 7.1 Introduction to instruction fine-tuning
- 7.2 Preparing a dataset for supervised instruction fine-tuning
- 7.3 Organizing data into training batches
- 7.4 Creating data loaders for an instruction dataset
- 7.5 Loading a pretrained LLM
- 7.6 Fine-tuning the LLM on instruction data
- 7.7 Extracting and saving responses
- 7.8 Evaluating the fine-tuned LLM
- 7.9 Conclusions
  - 7.9.1 What's next?
  - 7.9.2 Staying up to date in a fast-moving field
  - 7.9.3 Final words

-----

### Appendices

#### Appendix A: Introduction to PyTorch
- A.1 What is PyTorch?
  - A.1.1 The three core components of PyTorch
  - A.1.2 Defining deep learning
  - A.1.3 Installing PyTorch
- A.2 Understanding tensors
  - A.2.1 Scalars, vectors, matrices, and tensors
  - A.2.2 Tensor data types
  - A.2.3 Common PyTorch tensor operations
- A.3 Seeing models as computation graphs
- A.4 Automatic differentiation made easy
- A.5 Implementing multilayer neural networks
- A.6 Setting up efficient data loaders
- A.7 A typical training loop
- A.8 Saving and loading models
- A.9 Optimizing training performance with GPUs
  - A.9.1 PyTorch computations on GPU devices
  - A.9.2 Single-GPU training
  - A.9.3 Training with multiple GPUs

#### Appendix B: References and Further Reading

#### Appendix C: Exercise Solutions

#### Appendix D: Adding Bells and Whistles to the Training Loop
- D.1 Learning rate warmup
- D.2 Cosine decay
- D.3 Gradient clipping
- D.4 The modified training function

#### Appendix E: Parameter-Efficient Fine-tuning with LoRA
- E.1 Introduction to LoRA
- E.2 Preparing the dataset
- E.3 Initializing the model
- E.4 Parameter-efficient fine-tuning with LoRA

**Index**

-----
