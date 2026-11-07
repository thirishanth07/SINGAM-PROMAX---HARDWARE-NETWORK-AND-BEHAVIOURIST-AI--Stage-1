# Chapter Quest Study Guide

**Chapter Quest - Singam Pro Max | Version 1.0**

**Team:** SINGAM PRO MAX - Module AI Hardware and Behaviorist AI

A beginner route through eleven game chapters. You will trace an AI system, choose hardware for a workload, and test how feedback changes an agent's decisions.

**Before you start:** Bring paper and a pencil or a notes app. You need basic arithmetic and web navigation. A calculator is optional. No programming is required.

**How to use each mission:** Read the briefing, make a prediction, try the task, then compare your reasoning with the debrief. Allow 10-15 minutes per mission, plus game time.

## Contents

1. Enter the Circuit Garden
2. Chapter 1 Battle Setup
3. Chapter 1 Practice Screen
4. Missions 1-2 Hardware and logic
5. Missions 3-4 Processors and acceleration
6. Missions 5-6 Memory and networks
7. Missions 7-8 Behavior and rewards
8. Missions 9-10 Algorithms and applications
9. Mission 11 and final review
10. Glossary and resources

---

## Enter the Circuit Garden

Open the hosted game in a browser. Choose a glowing portal or the Play chapter button on a chapter card. The menu shows all 11 chapters available, so you can revisit a topic directly.

**Game URL:** [https://chapter-quest-ai-seven-tk.tklm-sift.chatgpt.site](https://chapter-quest-ai-seven-tk.tklm-sift.chatgpt.site)

*Figure 1. The Circuit Garden portal map, cropped from the supplied menu screenshot. The top row shows Chapters 1-6 and the lower row shows Chapters 7-11. Singam stands on the central path.*

**Suggested route:** Begin with Missions 1-6 to see how AI runs. Then tackle Missions 7-11 to see how an agent learns and how to evaluate it. Play the chapter that matches your current mission.

**Offline route:** Complete the paper missions and use the separate Test Bank for retrieval practice. Record one mistake and one corrected explanation after each session.

---

## Chapter 1 Battle Setup

*Figure 2. The supplied Chapter 1 setup screen shows Start boss battle, Timed battle, and the three stages.*

For a first attempt, choose **Start boss battle**. Chapter 1 lists:
- **Doctor Doom** (10 easy questions)
- **Donkey Kong** (5 medium)
- **Kirby** (5 difficult)

Each correct answer powers one hit. The setup says a wrong answer costs 25 shield, and Try Again restarts the current level after a loss while retaining earlier cleared levels.

The screen also offers Timed battle and says the personal best is saved in this browser. Use the untimed practice view for the reflection task on the next page.

## Chapter 1 Practice Screen

*Figure 3. The supplied practice screen shows Doctor Doom at 10/10 HP, Singam at 100% shield, and a four-option hardware question. The header shows XP, streak, and No timer.*

**Play and observe:** Before choosing, explain how the software uses a physical processor. Select the answer that says hardware supplies the resources for computation. Compare the boss HP and shield before and after. Write down any feedback you see and one reason a different option is wrong.

**Offline check:** On paper, predict 9/10 boss HP after one correct answer from the pictured starting state. The setup's one-hit rule supports this prediction. The screenshots show the starting state. Post-answer displays, timing rules, and XP calculations were unavailable for verification.

---

## Missions 1-2 Hardware and logic

### Mission 1: Intro to AI Hardware Foundations

**Briefing:** Training adjusts model parameters using data or experience. Inference runs a trained model on new inputs. Both need physical processors and memory. An image classifier might train on thousands of pictures and later infer a label for one new photo.

**Your move:** Draw camera → memory → processor → label. Circle the part that carries out arithmetic. Label a separate step where model weights change.

**Hint:** Which step uses an already trained model?

**Debrief:** The processor performs the arithmetic. Training changes weights. Producing a label with fixed weights is inference.

### Mission 2: Digital Logic and Computer Organisation

**Briefing:** Bits represent 0 or 1. An AND gate outputs 1 when both inputs are 1, OR outputs 1 when either or both are 1, and NOT flips a bit. A processor fetches, decodes, and executes instructions using registers for immediate working values.

**Your move:** Build an access rule for a badge and supervisor approval. List input pairs 00, 01, 10, 11 and predict the output for each. Change the rule to accept either input and compare.

**Hint:** Which cases have exactly one input set?

**Debrief:** AND gives 0,0,0,1. OR gives 0,1,1,1. The 01 and 10 cases distinguish the rules.

---

## Missions 3-4 Processors and acceleration

### Mission 3: CPU, GPU and ASIC Architectures

**Briefing:** A CPU handles diverse instructions and control flow. A GPU can perform many similar operations in parallel. An ASIC is designed for a particular application. The best fit depends on workload, energy, cost, and flexibility.

**Your move:** Assign a processor to three tasks: varied operating-system work, thousands of independent pixel operations, and a stable high-volume sensor workload. State one trade-off for each.

**Hint:** Look for repeated independent work and for a stable task.

**Debrief:** A CPU fits varied work. A GPU fits many similar pixel operations. An ASIC may suit the stable sensor task if efficiency gains justify design cost.

### Mission 4: AI Accelerators

**Briefing:** An accelerator speeds up selected operations. Neural networks often use large groups of multiply-and-add operations. Data transfer and unsupported operations can limit speedups across a whole pipeline.

**Your move:** Predict the new runtime if a 100 ms pipeline spends 60 ms computing and 40 ms moving data, and an accelerator halves only compute time. Compare with a partner.

**Hint:** Change only one term in the sum.

**Debrief:** The new total is 30 + 40 = 70 ms. Measure the whole pipeline to check the improvement.

---

## Missions 5-6 Memory and networks

### Mission 5: Memory and Low Power Hardware

**Briefing:** Caches keep frequently needed data close to the processor. Memory bandwidth is data moved per unit time. Moving data costs energy. Quantization uses fewer bits for values and can save memory, with potential accuracy changes.

**Your move:** Calculate storage for 1,000 weights at 32 bits each and at 8 bits each. Then choose a measurement that would reveal a quality trade-off.

**Hint:** Eight bits make one byte.

**Debrief:** The arrays need 4,000 and 1,000 bytes before overhead. Compare accuracy on the same representative test set.

### Mission 6: Networks Internet and Cybersecurity Fundamentals

**Briefing:** A local network connects nearby devices. The Internet links networks. Latency is delay and bandwidth is transfer capacity. Phishing uses deceptive messages to obtain information or induce unsafe actions.

**Your move:** Sketch phone → Wi-Fi router → Internet → server. Imagine an urgent message asking you to sign in through an unfamiliar link. Mark where the request travels and rehearse a safe response.

**Hint:** Verify the request through a channel you already trust.

**Debrief:** An online request traverses the local network and wider networks. Avoid the message link, verify independently, and report it through the appropriate channel.

---

## Missions 7-8 Behavior and rewards

### Mission 7: Introduction to Behaviorist AI

**Briefing:** This guide uses behaviorist AI to explore observable action and feedback. A fixed reactive rule maps a situation to an action. A learning agent can adjust its future choices based on experience.

**Your move:** Role-play a robot. First follow "turn when blocked." Then keep scores for turning left and right after feedback across six trials. Describe what can change in the second version.

**Hint:** Separate the starting rule from the policy after experience.

**Debrief:** The first rule is fixed. The scored version can prefer whichever turn produced better outcomes in the trials.

### Mission 8: Fundamentals of Reinforcement Learning

**Briefing:** An agent observes a state, chooses an action, and receives a reward and a next state from its environment. A policy selects actions. Return measures accumulated rewards, often discounting later ones. Exploration tries alternatives, and exploitation uses current knowledge.

**Your move:** Compare two routes with rewards [2, 0] and [0, 5]. Compute each return with no discount and then with discount factor 0.2, weighting the second reward only.

**Hint:** Use first reward + discount × second reward.

**Debrief:** Without discount, 5 beats 2. With 0.2, the returns are 2 and 1, so the first route wins.

---

## Missions 9-10 Algorithms and applications

### Mission 9: Reinforcement Learning Algorithms

**Briefing:** Q-learning estimates the value of taking an action in a state and then choosing high-value actions. Its target uses immediate reward plus the discounted largest next-state Q-value. SARSA uses the value of the next action actually selected. In a terminal state the continuation term is zero.

**Your move:** Start with Q = 2, learning rate 0.5, reward 1, discount 0.5, and maximum next Q = 6. Compute the target and move halfway from the old value to it.

**Hint:** Compute the target before updating the estimate.

**Debrief:** The target is 1 + (0.5 × 6) = 4. The new Q is 2 + 0.5 × (4 - 2) = 3.

### Mission 10: Applications of Behaviorist AI

**Briefing:** Feedback-based policies can help in tasks with repeated decisions, such as routing a robot or controlling a simulated process. A simulator lets learners compare policies before risking physical equipment.

**Your move:** Draw a 3 × 3 grid with a start, goal, and blocked cell. Give +5 for reaching the goal and -1 per move including the goal move. Compare two valid routes of different lengths.

**Hint:** For each route subtract its move count from 5.

**Debrief:** A four-move route earns 1 and a six-move route earns -1. Keep the map and scoring fixed when comparing policies.

---

## Mission 11 and final review

### Mission 11: Challenges and Limitations of Behaviorist AI

**Briefing:** Sparse rewards provide little feedback during learning. A poorly chosen reward can produce undesirable behavior. A policy trained in one setting may struggle in a different setting. Unsafe actions need explicit limits and evaluation.

**Your move:** Give a delivery agent +1 for each parcel it moves. Predict a loophole, revise the reward, and design one test on an unfamiliar layout.

**Hint:** Ask whether the same parcel can earn points repeatedly.

**Debrief:** An agent could move one parcel back and forth. Reward verified delivery once per parcel, then test successful deliveries and safety on a new layout.

### Exit Challenge

Sketch a warehouse robot with a sensor, memory, processor, and a network link. Add an agent loop showing observation, action and reward. Explain one hardware trade-off and one reward loophole. Compare with Open Response 6 in the Test Bank.

*Check your sketch for both flows. Sensor data goes through computing hardware to produce a decision. In learning, feedback from the environment can change future decisions. A faster processor and a better reward address different problems.*

---

## Glossary and Resources

| Term | Definition |
|---|---|
| **Inference** | Using a trained model to generate an output. |
| **ASIC** | Application-specific integrated circuit. |
| **Cache** | Small, fast memory for frequently used data. |
| **Quantization** | Representing values at reduced precision, often with fewer bits. |
| **Latency and bandwidth** | Delay and transfer capacity per unit time. |
| **Phishing** | Deception intended to steal information or trigger an unsafe action. |
| **Agent and environment** | The decision maker and the world it interacts with. |
| **Policy and return** | How actions are selected and the accumulated reward, often discounted. |
| **Q-value** | Estimated return associated with a state and action. |
| **Reward loophole** | A way to increase measured reward while missing the intended goal. |

### Source Notes and Further Practice

Chapter Quest Team-supplied screenshots establish the chapter titles and visible interface. The paper missions extend those titles with beginner examples.

- **Nand to Tetris:** Try Project 1 truth tables, then preview Project 5 for CPU organization. [https://www.nand2tetris.org/course](https://www.nand2tetris.org/course)
- **Google ML Crash Course:** Open Exercises and compare the training and inference interactive activities. [https://developers.google.com/machine-learning/crash-course/exercises](https://developers.google.com/machine-learning/crash-course/exercises)
- **CISA Phishing Tip Sheet:** Find two warning signs and rehearse independent verification. [https://www.cisa.gov/sites/default/files/2024-09/Secure-Our-World-Phishing-Tip-Sheet.pdf](https://www.cisa.gov/sites/default/files/2024-09/Secure-Our-World-Phishing-Tip-Sheet.pdf)
- **Sutton and Barto:** Read the introductory examples, then identify the agent and environment in one. [https://www.incompleteideas.net/sutton/book/first/Chap1PrePub.pdf](https://www.incompleteideas.net/sutton/book/first/Chap1PrePub.pdf)
