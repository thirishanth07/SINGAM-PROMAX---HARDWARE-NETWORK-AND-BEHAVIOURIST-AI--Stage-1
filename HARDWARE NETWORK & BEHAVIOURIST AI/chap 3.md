# Chapter 3: CPU, GPU & ASIC Architectures

**Choosing how to organise computation.**

## Learning Objectives

By the end of this chapter, readers should be able to:

- Define the three processor categories.
- Compare serial and parallel execution.
- Explain SIMD and SIMT with simple examples.
- Choose hardware using workload, memory, power, and software needs.

## CPU: Flexible General Computing

**CPU** means Central Processing Unit: a general-purpose processor that executes program instructions.

- A **core** is a processing engine within a chip. Modern CPUs commonly have multiple cores.
- **Control flow** is the order in which instructions run, including choices and repeated steps. CPUs handle varied tasks and complex control flow well.

## Serial vs Parallel Processing

| Concept | Definition |
|---|---|
| **Serial processing** | Performs tasks one after another. |
| **Parallel processing** | Performs multiple tasks at the same time when their dependencies allow it. |
| **Dependency** | One step needs another step's result. More workers cannot remove this requirement. |

## GPU: Many Calculations Together

**GPU** means Graphics Processing Unit: a processor designed for high throughput across many parallel tasks.

- **Throughput** is the amount of work completed per unit of time.
- AI often repeats similar arithmetic across many numbers, making suitable operations a good fit for GPUs.

## SIMD: One Instruction, Many Values

**SIMD** means Single Instruction, Multiple Data: one instruction applies the same operation to several data values.

- Example: Add 1 to `[2, 4, 6, 8]` to obtain `[3, 5, 7, 9]`.
- CPUs can also support SIMD; this idea is not exclusive to GPUs.

## SIMT: Single Instruction, Multiple Threads

**SIMT** means Single Instruction, Multiple Threads: groups of threads execute instructions together on different data.

- A **thread** is one sequence of program execution. NVIDIA GPUs organise threads into groups called **warps**.
- **Branch divergence** occurs when threads in a group take different paths; paths may run with some lanes inactive, reducing efficiency.

## ASIC: Hardware for a Specific Purpose

**ASIC** means Application-Specific Integrated Circuit: a chip designed for a particular application or set of tasks.

- Specialised AI ASICs can dedicate more hardware to supported AI operations.
- **The tradeoff:** Reduced hardware flexibility and significant design effort. Supported software and models still matter.

## Which Processor Fits the Work?

| Processor | Useful for | Key tradeoff |
|---|---|---|
| **CPU** | Varied tasks; complex decisions | Less specialised for bulk arithmetic |
| **GPU** | Many similar parallel calculations | Transfers and irregular control |
| **AI ASIC** | Supported specialised operations | Narrower hardware flexibility |

## How Processors Work Together

- **Preprocessing:** Prepares raw input for a model, such as resizing an image.
- **Calculate:** The CPU can coordinate a task; a GPU or AI accelerator can run supported model calculations.
- **Postprocessing:** Turns model outputs into useful results, such as selecting an object label.

*Note: Data transfers and synchronisation add overhead.*

## Chapter Recap

- CPUs combine flexibility with several forms of parallelism.
- GPUs suit many large, regular parallel workloads.
- AI ASICs specialise hardware for a supported set of tasks.
- Workload, memory, software, and data movement determine practical performance.
