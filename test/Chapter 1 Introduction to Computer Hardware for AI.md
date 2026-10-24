
# Chapter 1: Introduction to Computer Hardware for AI

## Learning Objectives

By the end of this chapter, readers should be able to:

- Explain what computer hardware does in an AI system and why hardware choices affect AI performance.
- Describe the Von Neumann bottleneck and why AI workloads stress memory and data movement.
- Distinguish training hardware from inference hardware.
- Define TOPS, TOPS/W, and latency, and use them to compare accelerators.

## Why This Chapter Matters

Beginners often treat AI as pure software: you write a model, you run it, and it works. In practice, every AI system is limited by physical hardware — how fast it can multiply numbers, how quickly it can move data, and how much energy it consumes. Understanding hardware gives you a mental model for why some models run on a phone and others need a data center.

## Key Terms

| Term | Definition |
|---|---|
| Hardware | The physical components of a computer: processors, memory, storage, and input/output devices. |
| CPU | Central Processing Unit — a general-purpose processor that executes instructions. |
| GPU | Graphics Processing Unit — a processor with many simple cores designed for parallel work. |
| Accelerator | Specialized hardware designed to speed up a particular workload, often AI math. |
| Von Neumann architecture | A design where instructions and data share memory and travel over a common path to the processor. |
| Von Neumann bottleneck | The performance limit caused by moving instructions and data between memory and the processor. |
| Training | The process of adjusting a model’s parameters using data and gradients. |
| Inference | Using a trained model to produce an output for a new input. |
| TOPS | Tera Operations Per Second — a measure of how many operations a chip can perform per second. |
| TOPS/W | Operations per second per watt — a measure of energy efficiency. |
| Latency | The time it takes to produce one result, such as one inference. |
| Throughput | The amount of work completed per unit of time, such as inferences per second. |

If the model requires 2 trillion operations per inference, the **ideal compute time** is:

- **Accelerator A:** 2 / 100 = 0.02 seconds = 20 ms.
- **Accelerator B:** 2 / 20 = 0.10 seconds = 100 ms.

Accelerator A is faster in ideal compute time, but it uses far more power. Accelerator B is five times more energy-efficient. For a battery-powered camera, B may be the better choice. For a data-center server where power is available and throughput matters, A may be better.

This example also shows why TOPS alone is not enough. Real latency will be higher because of memory access, data movement, and software overhead.

**Figure suggestion:** A simple diagram showing processor, memory, and the shared bus, with an arrow labeled “Von Neumann bottleneck.”

## Chapter Recap

- AI hardware must handle compute, memory, communication, and control.
- The Von Neumann bottleneck limits performance when data movement cannot keep up with compute.
- Training prioritizes throughput and memory; inference prioritizes latency and energy efficiency.
- TOPS measures raw operation rate; TOPS/W measures efficiency; latency measures time per result.
- Hardware choice depends on the workload, not just the biggest number on a spec sheet.

## Knowledge Check

1. **Recall.** What is the Von Neumann bottleneck?
2. **Application.** Why might a chip with higher TOPS be a worse choice for a battery-powered device?
3. **Compare.** How do training and inference hardware priorities differ?
4. **Evaluate.** A spec sheet says a chip has 50 TOPS. Why is that number not enough to conclude it is fast for your model?

### Answers

**1. Recall — Von Neumann bottleneck.**

It is the performance limit caused by the shared path between processor and memory. The processor must fetch instructions and data from memory, and if memory bandwidth or the shared bus cannot keep up, the processor waits. AI workloads stress this because they move large tensors between memory and compute.

**2. Application — Higher TOPS but worse for battery.**

Higher TOPS often comes with higher power consumption. A battery-powered device needs high TOPS/W and low latency at low power. A chip with high peak TOPS but poor efficiency may drain the battery quickly or overheat. Efficiency and workload fit matter more than peak TOPS.

**3. Compare — Training vs inference.**

Training requires forward and backward passes, gradient storage, and weight updates. It needs high throughput, large memory, and fast interconnects. Inference only runs the trained model forward. It prioritizes low latency, low energy, small size, and cost. Training is usually centralized; inference is often distributed to edge devices.

**4. Evaluate — Why TOPS alone is insufficient.**

TOPS does not tell you which operations are counted, what precision is assumed, how much memory bandwidth is available, or what latency your model will achieve. A model may be memory-bound, so peak TOPS cannot be reached. You also need TOPS/W, memory bandwidth, latency measurements, and software support.

## References

Use these as starting points and verify the exact edition or URL before submission.

Von Neumann, J. First Draft of a Report on the EDVAC. 1945.

Internet Archive scan: https://archive.org/details/firstdraftofrepo00vonn

Alternative PDF (Stanford mirror): http://qss.stanford.edu/~godfrey/vonNeumann/vnedvac.pdf

Hennessy, J. L., and Patterson, D. A. Computer Architecture: A Quantitative Approach.

Google Books (7th edition, Morgan Kaufmann, 2025): https://books.google.com/books/about/Computer_Architecture.html?id=0gNHEQAAQBAJ

Patterson, D. A., and Hennessy, J. L. Computer Organization and Design.

Google Books (RISC-V Edition, Morgan Kaufmann, 2017): https://books.google.com/books/about/Computer_Organization_and_Design_RISC_V.html?id=w6ZaDwAAQBAJ

Horowitz, M. “Computing’s Energy Problem (and What We Can Do About It).” IEEE ISSCC, 2014.

DOI: https://doi.org/10.1109/ISSCC.2014.6757323

**NVIDIA. CUDA C Programming Guide. **

Official documentation: https://docs.nvidia.com/cuda/cuda-c-programming-guide/

Jouppi, N. P., et al. “In-Datacenter Performance Analysis of a Tensor Processing Unit.” ISCA, 2017.

DOI: https://doi.org/10.1145/3079856.3080246
    
