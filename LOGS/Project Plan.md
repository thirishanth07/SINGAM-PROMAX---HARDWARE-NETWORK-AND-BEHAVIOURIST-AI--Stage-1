# SINGAM PROMAX — Project Plan

## Hardware, Network & Behaviourist AI

**Team:** SINGAM PROMAX  
**Project:** Stage 1 — GitHub and Markdown Assignment  
**Repository Owner:** thirishanth07 (Thirishanth Veerasingam)  
**Repository Visibility:** Public  
**Learning Format:** Self-paced online module with weekly check-ins

---

## 1. Project Purpose

The purpose of this project is to develop a comprehensive, beginner-friendly educational module titled **Hardware, Network & Behaviourist AI**.

The module explores how computer hardware, network infrastructure, and behaviourist artificial intelligence work together to create intelligent systems capable of sensing, learning, making decisions, and responding to their environments.

The project is divided into three major components:

1. **Hardware — The Silicon:** Understanding the physical computing systems that execute AI operations.
2. **Network — The Bridge:** Understanding how neural networks, memory systems, sensors, and communication networks support AI applications.
3. **Behaviourist AI — The Intelligence:** Understanding how intelligent agents learn from environmental feedback and adapt their behaviour.

The final learning resources will include:

- A comprehensive Markdown study guide
- PowerPoint presentation slides
- Educational diagrams and illustrations
- Short video tutorials
- Worked examples and exercises
- Chapter-based knowledge assessments
- An integrated capstone project

The Markdown content stored in GitHub will serve as the primary source for all learning resources.

---

## 2. Target Learners

### Primary Audience

Undergraduate students interested in:

- Artificial intelligence
- Edge AI
- Embedded machine learning
- Computer architecture
- Internet of Things (IoT)
- Intelligent systems
- Robotics and behavioural computing

### Prerequisite Knowledge

Learners should have:

- Basic programming knowledge in Python or C
- Understanding of variables, loops, and functions
- Basic familiarity with vectors and matrices
- Basic computer literacy

No prior experience in computer hardware, networking, or artificial intelligence is required.

### Learning Environment

The module is designed for:

- Self-paced online learning
- University coursework
- Laboratory-based learning
- Group projects
- Capstone project preparation

### Learning Constraints

| Requirement | Description |
|---|---|
| Total Duration | Approximately 12–15 hours |
| Learning Format | Asynchronous, with weekly check-ins |
| Software | Free simulators and development tools |
| Hardware | Physical boards optional |
| Accessibility | Captions required for all videos |
| Cost | Prefer free and open-source resources |
| Assessment | Chapter activities and final capstone |

---

## 3. Intended Learning Outcomes

By the end of this module, learners should be able to:

1. Explain the **von Neumann bottleneck** and why AI workloads place heavy demands on memory bandwidth and data movement.

2. Compare **CPU, GPU, ASIC, NPU, TPU, and FPGA architectures** using performance metrics such as TOPS, TOPS/W, FLOPS, and latency.

3. Describe how neural network computations are mapped onto hardware accelerators.

4. Explain the importance of memory hierarchy and Network-on-Chip (NoC) architecture in AI processing efficiency.

5. Select appropriate communication technologies, including **5G, Wi-Fi, Bluetooth Low Energy (BLE), and MQTT**, for different edge AI and IoT applications.

6. Distinguish behaviourism from cognitivism and explain the **agent–environment interaction loop** involving perception, action, and reward.

7. Develop a basic behaviourist AI pipeline involving sensor data, feature extraction, sequence modeling, and real-time inference.

8. Apply model optimization techniques such as quantization and pruning to meet hardware performance requirements.

9. Evaluate AI system performance based on processing speed, latency, memory requirements, energy efficiency, and scalability.

10. Assess ethical considerations involving surveillance, data privacy, algorithmic bias, and cloud-based versus on-device processing.

---

## 4. Team Members and Responsibilities

| Team Member | GitHub Username | Role | Assigned Chapters |
|---|---|---|---|
| Kuypheav | @brain-go-pew | Coordinator, Repository and Submission Lead | Chapters 3 and 4 |
| Panha | To be confirmed | Content Writer | Chapters 1 and 7 |
| Brain | To be confirmed | Content Writer | Chapters 2 and 6 |
| Pun | To be confirmed | Content Writer | Chapters 5 and 12 |
| Egshiglen | To be confirmed | Content Writer | Chapters 8 and 9 |
| Shark | To be confirmed | Content Writer | Chapters 10 and 11 |
| Samuel | @SamuelT8 | Quality Assurance Lead | Review and quality control |

### Team Responsibilities

**Project Coordinator**
- Monitor overall progress.
- Maintain the GitHub repository.
- Coordinate submissions.
- Ensure deadlines are met.

**Content Writers**
- Research assigned chapters.
- Prepare Markdown learning materials.
- Include explanations, examples, diagrams, and references.
- Develop chapter knowledge checks.
- Review assigned content.

**Quality Assurance Lead**
- Review technical accuracy.
- Check Markdown formatting.
- Identify missing information.
- Review references and citations.
- Ensure consistent terminology across chapters.

---

## 5. Content Outline

### Difficulty Levels

| Level | Expected Learning Achievement |
|---|---|
| Beginner | Explain concepts and follow worked demonstrations |
| Intermediate | Apply knowledge with some guidance |
| Advanced | Independently design solutions and justify decisions |

---

# Part I — Hardware (The Silicon)

## Chapter 1: Introduction to Computer Hardware for AI

**Owner:** Panha  
**Depth:** Beginner  
**Duration:** 45 minutes

### Key Topics
- Traditional computer architecture
- Von Neumann bottleneck
- AI training versus inference
- CPU and AI hardware fundamentals
- TOPS, TOPS/W, FLOPS, and latency

### Learning Activities
- Compare three AI accelerator specification sheets.
- Complete a latency-versus-throughput worksheet.

---

## Chapter 2: Digital Logic and Computer Organization

**Owner:** Brain  
**Depth:** Beginner  
**Duration:** 60 minutes

### Key Topics
- Transistors and logic gates
- Boolean operations
- Arithmetic Logic Units (ALUs)
- Registers and memory
- Instruction Set Architectures (ISA)
- Multiply-accumulate operations
- Matrix multiplication in digital hardware

### Learning Activities
- Trace a MAC operation.
- Complete a basic ISA walkthrough.

---

## Chapter 3: CPU and GPU Architectures (and ASICs)

**Owner:** Kuypheav  
**Depth:** Beginner–Intermediate  
**Duration:** 60 minutes

### Key Topics
- CPU architecture
- Sequential processing
- SIMD execution
- GPU parallel computing
- ASIC design
- Performance and energy trade-offs

### Learning Activities
- Benchmark or simulate CPU versus GPU matrix multiplication.
- Explain observed performance differences.

---

## Chapter 4: AI Accelerators — NPUs, TPUs and FPGAs

**Owner:** Kuypheav  
**Depth:** Intermediate  
**Duration:** 60 minutes

### Key Topics
- Neural Processing Units
- Tensor Processing Units
- Field-Programmable Gate Arrays
- Systolic arrays
- MAC units
- Reconfigurable hardware
- Specialized AI accelerators

### Learning Activities
- Map a small neural network layer onto a systolic array.
- Compare different AI accelerators.

---

# Part II — Network (The Bridge)

## Chapter 5: Neural Network Architectures

**Owner:** Pun  
**Depth:** Intermediate  
**Duration:** 75 minutes

### Key Topics
- Artificial neural networks
- Convolutional Neural Networks
- Transformer architectures
- Neural network computation graphs
- Mapping neural networks to hardware

### Learning Activities
- Implement a small CNN or attention forward pass using NumPy.
- Identify hardware operations required for neural network execution.

---

## Chapter 6: Memory Hierarchy, NoC and Low-Power Hardware

**Owner:** Brain  
**Depth:** Intermediate  
**Duration:** 60 minutes

### Key Topics
- Cache and memory hierarchy
- Memory bandwidth
- Data movement energy costs
- Network-on-Chip architecture
- Embedded computing
- Low-power AI hardware
- TinyML

### Learning Activities
- Estimate energy used for computation versus data movement.
- Sketch a Network-on-Chip architecture.

---

## Chapter 7: Edge Computing and IoT Networking

**Owner:** Panha  
**Depth:** Intermediate  
**Duration:** 60 minutes

### Key Topics
- Cloud computing versus edge computing
- Edge AI applications
- Internet of Things
- Wi-Fi
- Bluetooth Low Energy
- 5G connectivity
- MQTT communication
- Distributed inference

### Learning Activities
- Simulate an MQTT message between an edge device and a cloud service.
- Select networking protocols for different IoT scenarios.

---

## Chapter 8: Sensor Networks and Event-Based Sensing

**Owner:** Egshiglen  
**Depth:** Intermediate–Advanced  
**Duration:** 60 minutes

### Key Topics
- Sensor networks
- Event cameras
- Inertial Measurement Units
- Audio sensor arrays
- Event-driven processing
- Asynchronous sensor streams
- Sensor data processing

### Learning Activities
- Stream asynchronous sensor data into a processing pipeline.
- Handle missing, delayed, and out-of-order events.

---

# Part III — Behaviourist AI (The Intelligence)

## Chapter 9: Introduction to Behaviourist AI

**Owner:** Egshiglen  
**Depth:** Intermediate  
**Duration:** 60 minutes

### Key Topics
- Behaviourism
- Cognitivism
- Stimulus-response learning
- Agent–environment interaction
- Rewards and penalties
- Reinforcement learning
- Behavioural cloning

### Learning Activities
- Implement a simple gridworld environment.
- Develop an agent that responds to rewards.

---

## Chapter 10: Behavioral Signals, Sensing and Representation

**Owner:** Shark  
**Depth:** Intermediate–Advanced  
**Duration:** 75 minutes

### Key Topics
- Human behavioural signals
- Pose estimation
- Eye gaze
- Speech and audio
- Biometric signals
- Time-series data
- Multimodal features
- Sensor fusion

### Learning Activities
- Extract features from pose or audio time-series data.
- Combine information from two different sensors.

---

## Chapter 11: Behavioral Modeling, Learning and Real-Time Edge Inference

**Owner:** Shark  
**Depth:** Advanced  
**Duration:** 75 minutes

### Key Topics
- Behavioural prediction
- Recurrent Neural Networks
- Long Short-Term Memory networks
- Sequence modeling
- Model quantization
- Model pruning
- Real-time edge inference
- Latency optimization

### Learning Activities
- Train a small sequence model.
- Apply quantization and pruning.
- Measure inference latency.
- Attempt to achieve latency below 50 milliseconds.

---

## Chapter 12: Applications, Ethics, Privacy and Future Directions

**Owner:** Pun  
**Depth:** Advanced  
**Duration:** 60 minutes

### Key Topics
- Smart homes
- Healthcare applications
- Robotics
- Autonomous vehicles
- Edge AI applications
- Data privacy
- AI surveillance
- Algorithmic bias
- Responsible AI
- Future developments

### Learning Activities
- Develop an integrated behaviourist edge AI concept.
- Evaluate privacy and ethical trade-offs.

---

## 6. Total Learning Duration

| Part | Chapters | Duration |
|---|---|---|
| Hardware | Chapters 1–4 | 3 hours 45 minutes |
| Network | Chapters 5–8 | 4 hours 15 minutes |
| Behaviourist AI | Chapters 9–12 | 4 hours 30 minutes |
| **Chapter Total** | **12 chapters** | **12 hours 30 minutes** |
| Capstone Demonstration | Integrated project | 1 hour |
| **Overall Total** | | **13 hours 30 minutes** |

---

## 7. Scope Boundaries

### In Scope

**Hardware**
- Computer architecture
- Digital logic
- CPU and GPU processing
- AI accelerators
- Memory hierarchy
- Hardware performance metrics

**Networking**
- Neural network architectures
- Network-on-Chip systems
- Edge computing
- IoT networking protocols
- Sensor networks
- Event-based sensing

**Behaviourist AI**
- Behaviourism and cognitivism
- Agent–environment interaction
- Reinforcement learning
- Behavioural cloning
- Behavioural signal processing
- Sequence models
- Model optimization
- Real-time inference

**Learning Resources**
- Markdown lessons
- Educational diagrams
- Code examples
- Exercises
- 12 video tutorials
- Chapter assessments
- Integrated capstone project

### Out of Scope

- Advanced chip design
- RTL and Verilog programming
- PCB design and soldering
- Full mathematical derivations of deep learning algorithms
- Advanced network routing and VPN configuration
- Complex cloud infrastructure
- Production deployment
- Professional certification
- Live tutoring

---

## 8. Project Timeline

| Stage | Deadline | Main Deliverables |
|---|---|---|
| Stage 1 | 24 October 2026 | Project plan, GitHub repository, content outline, task assignments, initial Markdown chapters |
| Stage 2 | 7 November 2026 | All 12 Markdown chapters, study guide draft, PPT slides, video drafts, and assessments |
| Stage 3 | 28 November 2026 | Revised learning resources, completed videos, capstone demonstration, final review, and submission |

### Internal Checkpoints

**Stage 1**
- Finalize chapter assignments.
- Complete project planning.
- Establish GitHub folder structure.
- Prepare initial Markdown learning content.

**Stage 2**
- 3 November: Complete Markdown drafts and peer review.
- 6 November: Complete initial study guide, slides, assessments, and video drafts.
- 7 November: Stage 2 submission.

**Stage 3**
- 14 November: Collect learner feedback.
- 21 November: Complete content revisions.
- 25 November: Final quality review.
- 27 November: Prepare final submission.
- 28 November: Final project deadline.

---

## 9. Shared Markdown Content Plan

The GitHub Markdown files will serve as the project's **single source of truth**.

All slides, scripts, activities, and assessments should remain consistent with the Markdown chapters.

### Each Chapter Must Include

1. Chapter title
2. Learning objectives
3. Introduction and importance
4. Key terminology
5. Main content explanations
6. Diagrams or illustrations
7. Worked examples
8. Practical learning activities
9. Knowledge-check questions
10. Explained answers
11. References and sources

### Recommended Repository Structure

- `README.md` — Project overview
- `Project Plan.md` — Project planning document
- `Study Guide/` — Chapter Markdown files
- `assets/images/` — Educational illustrations
- `slides/` — PowerPoint presentations
- `videos/` — Tutorial scripts and resources
- `assessments/` — Questions and answer keys
- `capstone/` — Integrated project materials

---

## 10. PowerPoint Presentation Plan

### Objective

Create clear, visually engaging presentations that explain the technical concepts in all 12 chapters.

### Presentation Requirements

Each chapter presentation should contain:

- Learning objectives
- Essential concepts
- Relevant diagrams
- Hardware or system examples
- Practical applications
- Knowledge-check questions
- Chapter summary
- References

### Visual Materials

Examples include:

- Von Neumann architecture diagram
- CPU versus GPU comparison
- Systolic array illustration
- Memory hierarchy diagram
- IoT networking architecture
- Sensor processing pipeline
- Agent–environment interaction loop
- Behavioural AI inference pipeline

---

## 11. Video Tutorial Production Plan

### Objective

Develop 12 short educational video tutorials covering all chapters.

### Format

- One video per chapter
- Approximately 5–20 minutes per video
- Screen recordings and narrated slides
- Demonstrations where appropriate
- Captions required
- Beginner-friendly explanations

### Production Workflow

1. Finalize Markdown chapter.
2. Prepare video script.
3. Develop supporting slides and visuals.
4. Record narration and demonstrations.
5. Edit video.
6. Add captions.
7. Conduct technical and accessibility review.
8. Publish the completed tutorial.

### Important Dependency

Markdown content must be reviewed and sufficiently stable before video recording begins.

---

## 12. Live Mini-Lecture Plan

### Proposed Topic

**From Sensors to Intelligent Decisions: How Edge AI Works**

### Objective

Demonstrate how hardware, networking, and behaviourist AI can work together in a practical intelligent system.

### Duration

Approximately 15–20 minutes.

### Lecture Structure

**Introduction — 3 minutes**
- Introduce edge AI.
- Explain the role of sensors and intelligent agents.

**Technical Explanation — 5 minutes**
- Explain sensor data collection.
- Demonstrate basic feature extraction.
- Describe how AI models process incoming information.

**Practical Demonstration — 7 minutes**
- Show a simulated sensor input.
- Process the sensor data.
- Demonstrate a simple AI decision or agent response.

**Discussion and Q&A — 5 minutes**
- Discuss latency and hardware limitations.
- Explain privacy concerns.
- Answer audience questions.

---

## 13. Integrated Capstone Project

### Project Objective

Design a small intelligent system that combines:

- Sensor input
- Data processing
- Network communication
- AI inference
- Agent decision-making
- Environmental feedback

### Suggested Project

**Smart Behaviour-Aware Edge AI System**

A simulated smart environment detects user activity through sensors, processes the signals using an AI model, and generates an appropriate response.

### Project Pipeline

1. Collect sensor data.
2. Extract meaningful features.
3. Process data using an AI model.
4. Perform inference on an edge device or simulator.
5. Select an action.
6. Respond to environmental feedback.
7. Evaluate performance.

### Evaluation Criteria

- System functionality
- Inference latency
- Computational efficiency
- Appropriate networking decisions
- Privacy protection
- Ethical considerations
- Quality of technical explanation

---

## 14. Main Project Risks and Solutions

| Risk | Proposed Solution |
|---|---|
| Limited hardware knowledge | Provide beginner-level explanations and worked examples |
| Difficult technical topics | Use diagrams, demonstrations, and peer review |
| Lack of physical hardware | Use free simulators and software-based experiments |
| Programming difficulties | Provide starter code and guided activities |
| Uneven workload | Assign clear chapter ownership and review progress weekly |
| Delayed submissions | Use internal deadlines and early progress reporting |
| Inaccurate technical information | Verify claims using textbooks, research papers, and official documentation |
| Inconsistent learning resources | Use Markdown as the single source of truth |
| Excessive project scope | Prioritize core learning outcomes and simplified demonstrations |
| Video production delays | Finalize chapter content before recording |
| Accessibility issues | Include captions, readable fonts, and clear visual explanations |

---

## 15. Communication and Project Management

### Communication

- Primary communication through the team group chat.
- Weekly progress updates.
- Additional meetings before major deadlines.

### Task Tracking

- Members update task progress through the group chat.
- Approved updates are recorded in the GitHub repository.
- Chapter completion status is monitored regularly.

### Quality Assurance

Before approving a chapter:

1. Confirm technical accuracy.
2. Check that learning objectives are addressed.
3. Verify terminology.
4. Review worked examples.
5. Check diagrams and image references.
6. Test code examples where applicable.
7. Review knowledge-check answers.
8. Verify references.
9. Confirm Markdown displays correctly on GitHub.

---

## 16. Assessment Plan

### Formative Assessment

Each chapter will include:

- Short knowledge-check questions
- Practical exercises
- Worked examples
- Explained answers

### Final Assessment

A Google Forms assessment will evaluate understanding across:

1. Hardware fundamentals
2. Digital logic
3. CPU and GPU architecture
4. AI accelerators
5. Neural networks
6. Memory and NoC
7. IoT networking
8. Sensor networks
9. Behaviourist AI
10. Behavioural sensing
11. Edge inference
12. Applications and ethics

### Capstone Assessment

Learners will also demonstrate their ability to combine hardware, networking, and AI concepts in an integrated application.

---

## 17. Expected Final Deliverables

By the final submission, SINGAM PROMAX aims to produce:

- [ ] Completed project plan
- [ ] Public GitHub repository
- [ ] Twelve completed Markdown chapters
- [ ] Educational illustrations and diagrams
- [ ] PowerPoint slides
- [ ] Twelve captioned video tutorials
- [ ] Chapter exercises and answer keys
- [ ] Final Google Forms assessment
- [ ] Integrated capstone project
- [ ] Live mini-lecture presentation
- [ ] References and glossary
- [ ] Final quality assurance review

---

## 18. Conclusion

The Hardware, Network & Behaviourist AI project aims to provide learners with a practical understanding of how intelligent systems operate, from the underlying computer hardware to network communication and adaptive AI behaviour.

Through structured lessons, simulations, worked examples, and a capstone project, learners will develop the ability to understand, evaluate, and design basic intelligent systems.

The project emphasizes **technical understanding, practical application, energy efficiency, responsible AI development, and collaborative learning**.

**Prepared by:** SINGAM PROMAX  
**Project:** Hardware, Network & Behaviourist AI
