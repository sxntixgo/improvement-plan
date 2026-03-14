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

## Book 5: Learning Domain-Driven Design

**Author:** Vlad Khononov | **Foreword:** Julie Lerman
**Publisher:** O'Reilly (2021) | **Pages:** ~290 | **ISBN:** 9781098100131

-----

### Part I: Strategic Design

#### Chapter 1: Analyzing Business Domains
- What Is a Business Domain?
- What Is a Subdomain?
- Types of Subdomains
  - Core Subdomains
  - Generic Subdomains
  - Supporting Subdomains
- Comparing Subdomains
- Identifying Subdomain Boundaries
- Conclusion
- Exercises

#### Chapter 2: Discovering Domain Knowledge
- Business Problems
- Knowledge Discovery
- Communication
- What Is a Ubiquitous Language?
- Language of the Business
- Conclusion
- Exercises

#### Chapter 3: Managing Domain Complexity
- What Is a Bounded Context?
- Bounded Contexts Versus Subdomains
- Boundaries
  - Physical Boundaries
  - Ownership Boundaries
- Bounded Contexts in Real Life
- Conclusion
- Exercises

#### Chapter 4: Integrating Bounded Contexts
- Cooperation
  - Partnership
  - Shared Kernel
- Customer–Supplier
  - Conformist
  - Anticorruption Layer
  - Open-Host Service
- Separate Ways
  - Communication Issues
  - Generic Subdomains
  - Model Differences
- Context Map
- Conclusion
- Exercises

-----

### Part II: Tactical Design

#### Chapter 5: Implementing Simple Business Logic
- Transaction Script
  - Implementation
  - It's Not That Easy!
  - When to Use Transaction Script
- Active Record
  - Implementation
  - When to Use Active Record
- Be Pragmatic
- Conclusion
- Exercises

#### Chapter 6: Tackling Complex Business Logic
- History
- Domain Model
- Implementation
  - Complexity
  - Ubiquitous Language
  - Building Blocks
    - Value Objects
    - Entities
    - Aggregates
    - Domain Services
  - Complexity Management
- Conclusion
- Exercises

#### Chapter 7: Modeling the Dimension of Time
- Event Sourcing
  - Search
  - Analysis
  - Source of Truth
  - Event Store
- Event-Sourced Domain Model
  - Advantages
  - Disadvantages
- Conclusion
- Exercises

#### Chapter 8: Architectural Patterns
- Business Logic Versus Architectural Patterns
- Layered Architecture
  - Presentation Layer
  - Business Logic Layer
  - Data Access Layer
  - Communication Between Layers
  - Variation
  - When to Use Layered Architecture
- Ports & Adapters
  - Terminology
  - Dependency Inversion Principle
  - Integration of Infrastructural Components
  - Variants
  - When to Use Ports & Adapters
- Command-Query Responsibility Segregation (CQRS)
  - Polyglot Modeling
  - Implementation
  - Projecting Read Models
  - Challenges
  - Model Segregation
  - When to Use CQRS
  - Scope
- Conclusion
- Exercises

#### Chapter 9: Communication Patterns
- Model Translation
  - Stateless Model Translation
  - Stateful Model Translation
- Integrating Aggregates
  - Outbox
- Saga
- Process Manager
- Conclusion
- Exercises

-----

### Part III: Applying Domain-Driven Design in Practice

#### Chapter 10: Design Heuristics
- Heuristics
- Bounded Contexts
- Business Logic Implementation Patterns
- Architectural Patterns
- Testing Strategy
- Conclusion
- Exercises

#### Chapter 11: Evolving Design Decisions
- Changes in Subdomains
- Changes in the Domain's Complexity
- Strategic Design Concerns
- Tactical Design Concerns
- Organizational Changes
- Domain Knowledge
- Growth
- Conclusion
- Exercises

#### Chapter 12: EventStorming
- What Is EventStorming?
- Who Should Participate in EventStorming?
- What Do You Need for EventStorming?
- The EventStorming Process
  - Step 1: Unstructured Exploration
  - Step 2: Timelines
  - Step 3: Pain Points
  - Step 4: Pivotal Events
  - Step 5: Commands
  - Step 6: Policies
  - Step 7: Read Models
  - Step 8: External Systems
  - Step 9: Aggregates
  - Step 10: Bounded Contexts
- Variants
- When to Use EventStorming
- Facilitation Tips
- Remote EventStorming
- Conclusion
- Exercises

#### Chapter 13: Domain-Driven Design in the Real World
- Strategic Analysis
- Understand the Business Domain
- Explore the Current Design
- Modernization Strategy
  - Strategic Modernization
  - Tactical Modernization
- Cultivate a Ubiquitous Language
- Pragmatic Domain-Driven Design
- Selling Domain-Driven Design
- Undercover Domain-Driven Design
- Conclusion
- Exercises

-----

### Part IV: Relationships to Other Methodologies and Patterns

#### Chapter 14: Microservices
- What Is a Service?
- What Is a Microservice?
- Method as a Service: Perfect Microservices?
- Design Goal
- System Complexity
- Microservices as Deep Services
- Microservices as Deep Modules
- Domain-Driven Design and Microservices' Boundaries
  - Bounded Contexts
  - Aggregates
  - Subdomains
- Conclusion
- Exercises

#### Chapter 15: Event-Driven Architecture
- Event-Driven Architecture
- Events
  - Event Types
  - Designing Events
- Conclusion
- Exercises

#### Chapter 16: Data Mesh
- Analytical Data Management Platforms
  - Operational Versus Analytical Data
- Analytical Models
  - Fact Tables
  - Dimension Tables
  - Analytical Models
- Data Management Challenges
- Data Mesh
  - Domain Ownership
  - Data as a Product
  - Self-Serve Data Infrastructure
  - Federated Computational Governance
- Conclusion
- Exercises

**Closing Words**

**Appendix A: Applying DDD: A Case Study**

**Appendix B: Answers to Exercise Questions**

**Index**

-----

## Book 6: Designing Data-Intensive Applications

**Author:** Martin Kleppmann
**Publisher:** O'Reilly (2017) | **Pages:** ~550 | **ISBN:** 9781449373320

-----

### Part I: Foundations of Data Systems

#### Chapter 1: Reliable, Scalable, and Maintainable Applications
- Thinking About Data Systems
- Reliability
  - Hardware Faults
  - Software Errors
  - Human Errors
  - How Important Is Reliability?
- Scalability
  - Describing Load
  - Describing Performance
  - Approaches for Coping with Load
- Maintainability
  - Operability: Making Life Easy for Operations
  - Simplicity: Managing Complexity
  - Evolvability: Making Change Easy
- Summary

#### Chapter 2: Data Models and Query Languages
- Relational Model Versus Document Model
  - The Birth of NoSQL
  - The Object-Relational Mismatch
  - Many-to-One and Many-to-Many Relationships
  - Are Document Databases Repeating History?
  - Relational Versus Document Databases Today
- Query Languages for Data
  - Declarative Queries on the Web
  - MapReduce Querying
- Graph-Like Data Models
  - Property Graphs
  - The Cypher Query Language
  - Graph Queries in SQL
  - Triple-Stores and SPARQL
  - The Foundation: Datalog
- Summary

#### Chapter 3: Storage and Retrieval
- Data Structures That Power Your Database
  - Hash Indexes
  - SSTables and LSM-Trees
  - B-Trees
  - Comparing B-Trees and LSM-Trees
  - Other Indexing Structures
- Transaction Processing or Analytics?
  - Data Warehousing
  - Stars and Snowflakes: Schemas for Analytics
- Column-Oriented Storage
  - Column Compression
  - Sort Order in Column Storage
  - Writing to Column-Oriented Storage
  - Aggregation: Data Cubes and Materialized Views
- Summary

#### Chapter 4: Encoding and Evolution
- Formats for Encoding Data
  - Language-Specific Formats
  - JSON, XML, and Binary Variants
  - Thrift and Protocol Buffers
  - Avro
  - The Merits of Schemas
- Modes of Dataflow
  - Dataflow Through Databases
  - Dataflow Through Services: REST and RPC
  - Message-Passing Dataflow
- Summary

-----

### Part II: Distributed Data

#### Chapter 5: Replication
- Leaders and Followers
  - Synchronous Versus Asynchronous Replication
  - Setting Up New Followers
  - Handling Node Outages
  - Implementation of Replication Logs
- Problems with Replication Lag
  - Reading Your Own Writes
  - Monotonic Reads
  - Consistent Prefix Reads
  - Solutions for Replication Lag
- Multi-Leader Replication
  - Use Cases for Multi-Leader Replication
  - Handling Write Conflicts
  - Multi-Leader Replication Topologies
- Leaderless Replication
  - Writing to the Database When a Node Is Down
  - Limitations of Quorum Consistency
  - Sloppy Quorums and Hinted Handoff
  - Detecting Concurrent Writes
- Summary

#### Chapter 6: Partitioning
- Partitioning and Replication
- Partitioning of Key-Value Data
  - Partitioning by Key Range
  - Partitioning by Hash of Key
  - Skewed Workloads and Relieving Hot Spots
- Partitioning and Secondary Indexes
  - Partitioning Secondary Indexes by Document
  - Partitioning Secondary Indexes by Term
- Rebalancing Partitions
  - Strategies for Rebalancing
  - Operations: Automatic or Manual Rebalancing
- Request Routing
- Summary

#### Chapter 7: Transactions
- The Slippery Concept of a Transaction
  - The Meaning of ACID
  - Single-Object and Multi-Object Operations
- Weak Isolation Levels
  - Read Committed
  - Snapshot Isolation and Repeatable Read
  - Preventing Lost Updates
  - Write Skew and Phantoms
- Serializability
  - Actual Serial Execution
  - Two-Phase Locking (2PL)
  - Serializable Snapshot Isolation (SSI)
- Summary

#### Chapter 8: The Trouble with Distributed Systems
- Faults and Partial Failures
  - Cloud Computing and Supercomputing
- Unreliable Networks
  - Network Faults in Practice
  - Detecting Faults
  - Timeouts and Unbounded Delays
  - Synchronous Versus Asynchronous Networks
- Unreliable Clocks
  - Monotonic Versus Time-of-Day Clocks
  - Clock Synchronization and Accuracy
  - Relying on Synchronized Clocks
  - Process Pauses
- Knowledge, Truth, and Lies
  - The Truth Is Defined by the Majority
  - Byzantine Faults
  - System Model and Reality
- Summary

#### Chapter 9: Consistency and Consensus
- Consistency Guarantees
- Linearizability
  - What Makes a System Linearizable?
  - Relying on Linearizability
  - Implementing Linearizable Systems
  - The Cost of Linearizability
- Ordering Guarantees
  - Ordering and Causality
  - Sequence Number Ordering
  - Total Order Broadcast
- Distributed Transactions and Consensus
  - Atomic Commit and Two-Phase Commit (2PC)
  - Distributed Transactions in Practice
  - Fault-Tolerant Consensus
  - Membership and Coordination Services
- Summary

-----

### Part III: Derived Data

#### Chapter 10: Batch Processing
- Batch Processing with Unix Tools
  - Simple Log Analysis
  - The Unix Philosophy
- MapReduce and Distributed Filesystems
  - MapReduce Job Execution
  - Reduce-Side Joins and Grouping
  - Map-Side Joins
  - The Output of Batch Workflows
  - Comparing MapReduce to Distributed Databases
- Beyond MapReduce
  - Materialization of Intermediate State
  - Graphs and Iterative Processing
  - High-Level APIs and Languages
- Summary

#### Chapter 11: Stream Processing
- Transmitting Event Streams
  - Messaging Systems
  - Partitioned Logs
- Databases and Streams
  - Keeping Systems in Sync
  - Change Data Capture
  - Event Sourcing
  - State, Streams, and Immutability
- Processing Streams
  - Uses of Stream Processing
  - Reasoning About Time
  - Stream Joins
  - Fault Tolerance
- Summary

#### Chapter 12: The Future of Data Systems
- Data Integration
  - Combining Specialized Tools by Deriving Data
  - Batch and Stream Processing
- Unbundling Databases
  - Composing Data Storage Technologies
  - Designing Applications Around Dataflow
  - Observing Derived State
- Aiming for Correctness
  - The End-to-End Argument for Databases
  - Enforcing Constraints
  - Timeliness and Integrity
  - Trust, but Verify
- Doing the Right Thing
- Summary

**Index**

-----
