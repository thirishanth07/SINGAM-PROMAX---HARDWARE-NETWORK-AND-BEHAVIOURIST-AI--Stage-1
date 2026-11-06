# Chapter 1: Introduction to Computer Hardware for AI

**Physical Foundations of Intelligent Computing**

## Learning Objectives & Roadmap

By the end of this chapter, readers should be able to:

- Explain how computers represent data.
- Identify key hardware components.
- Understand the Von Neumann model.
- Compare traditional and AI workloads.
- Distinguish training and inference.
- Interpret TOPS, TOPS/W, and latency.

## Why Hardware Matters for AI

AI software runs on physical processors. No hardware, no AI.

- **Massive Arithmetic:** AI workloads demand massive arithmetic operations and high-speed data movement.
- **Real-World Examples:** ChatGPT responses and image recognition both rely on specialized hardware.

## Digital Information

Computers use **bits** to represent all data.

- A bit is **0 or 1**.
- 8 bits = **1 byte**.
- Example: `1010₂` = 10

| Binary Place Values | 8 | 4 | 2 | 1 |
|---|---|---|---|---|
| **Binary Digits** | 1 | 0 | 1 | 0 |

**Calculation:** 1×8 + 0×4 + 1×2 + 0×1 = 10

## Core Computer Hardware

| Component | Function |
|---|---|
| **CPU** | Executes instructions. |
| **RAM** | Temporary working memory. |
| **Storage** | Saves data and programs. |
| **I/O** | Input and output devices. |
| **GPU** | Parallel processing. |

## Von Neumann Architecture
<br> ![Computer System Block Diagram](https://github.com/user-attachments/assets/35a5d384-d54d-4053-b084-52139bf8277b)

- **CPU:** Fetches, decodes, and executes instructions. The Control Unit directs data flow, and the ALU performs arithmetic and logic operations.
- **Main Memory:** Shared store for both program instructions and data. The CPU reads from and writes to this single memory space—a defining feature of the model.
- **Input/Output:** Input/output devices connect the system to the outside world. The system bus carries data, addresses, and control signals between all components.

### Program Execution: How a Program Runs

Follow one instruction (e.g., `ADD`):

1. **FETCH:** Retrieve the instruction.
2. **DECODE:** Interpret the instruction.
3. **EXECUTE:** Perform the operation.

*A simplified instruction cycle.*

## Traditional vs AI Workloads

| Traditional Example | AI Example |
|---|---|
| Handle a user action. | Process many input values. |
| Follow varied program steps. | Repeat matrix arithmetic. |
| Can also use parallelism. | Still needs control and memory. |

*Best hardware depends on the actual workload.*

## Training vs Inference

| Aspect | Training | Inference |
|---|---|---|
| **Purpose** | Learns from data. | Uses trained model. |
| **Main Task** | Updates weights. | Predicts new outputs. |
| **Computation** | Very high. | Lower than training. |
| **Memory Demand** | High. | Lower. |
| **Speed Focus** | Throughput. | Fast response. |
| **Example** | Teaching the model. | Using the model. |

## CPU, GPU & AI Accelerators

| Hardware | Strength | Role |
|---|---|---|
| **CPU** | Flexible control. | General tasks. |
| **GPU** | Parallel processing. | Many calculations. |
| **AI Accelerator** | AI optimization. | Specialized tasks. |

## Performance Metrics

| Metric | Definition | Best For |
|---|---|---|
| **TOPS** | Computing Speed: How many operations per second? | AI Model Training: Processes large datasets, needs high computing throughput. |
| **TOPS/W** | Energy Efficiency: How much performance per watt? | Battery-Powered AI Devices: Operates with limited battery power, needs efficient computing. |
| **LATENCY** | Response Time: How long until a result? | Real-Time AI Cameras: Detects objects in real time, needs fast responses. |

## Voice Assistant Pipeline

1. Microphone input.
2. Interpret request.
3. Choose an action.
4. Device / spoken output.

## Summary

- Computers represent data in bits.
- CPU, RAM, storage, and I/O work together.
- Von Neumann architecture explains core structure.
- AI workloads differ from traditional workloads.
- Training and inference have different hardware needs.
- TOPS, TOPS/W, and latency help measure AI hardware.
