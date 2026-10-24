
# Chapter 2 — Digital Logic and Computer Organization

## Learning Objectives

By the end of this chapter, readers should be able to:

- Explain how logic gates, ALUs, and registers form the building blocks of a processor.
- Describe what an Instruction Set Architecture (ISA) is and why it matters.
- Explain how matrix multiplication maps onto digital logic operations.
- Trace a simple multiply-accumulate operation through basic computer organization.

## Why This Chapter Matters

Chapter 1 described the hardware landscape. This chapter goes one level deeper: how does a processor actually compute? Beginners do not need to design a chip, but they do need to understand that AI math is ultimately built from simple logic operations — AND, OR, NOT, add, multiply, and store. That understanding explains why hardware accelerators are designed the way they are.

## Key Terms

| Term | Definition |
|---|---|
| Logic gate | A basic digital circuit that performs a logical operation such as AND, OR, or NOT. |
| Combinational logic | Logic whose output depends only on the current inputs. |
| Sequential logic | Logic that stores state and depends on past inputs, usually synchronized by a clock. |
| ALU | Arithmetic Logic Unit — the part of a processor that performs arithmetic and logical operations. |
| Register | A small, fast storage location inside the processor. |
| Clock | A timing signal that coordinates when sequential logic updates. |
| ISA | Instruction Set Architecture — the contract between software and hardware describing available instructions. |
| Instruction | A single operation the processor can execute, such as load, add, or store. |
| Datapath | The hardware path that carries data through the processor. |
| Control unit | The hardware that decodes instructions and tells the datapath what to do. |
| MAC | Multiply-Accumulate — an operation that multiplies two numbers and adds the result to an accumulator. |

## From Transistors to Logic Gates

Digital circuits are built from transistors acting as switches. Groups of transistors form logic gates. A gate takes one or more binary inputs and produces a binary output.

**Common gates:**

- **NOT** — inverts the input.
- **AND** — outputs 1 only if all inputs are 1.
- **OR** — outputs 1 if at least one input is 1.
- **NAND** — the inverse of AND; often used because it is efficient to build.

A truth table lists the output for every input combination. For example, a two-input AND gate outputs 1 only for inputs 1 and 1.

Combinational logic has no memory. Its output depends only on its current inputs. Adders, multiplexers, and decoders are combinational.

Sequential logic stores state. Registers and memory are sequential because they hold values across clock cycles. The clock tells them when to update.

**Figure suggestion:** A truth table and gate symbols for AND, OR, NOT, and NAND.

## ALUs and Registers

The Arithmetic Logic Unit (ALU) performs operations such as addition, subtraction, bitwise AND/OR, and comparison. It takes operands from registers, performs an operation, and writes the result back to a register.

Registers are tiny, fast storage locations inside the processor. They hold the operands and results of current instructions. Because registers are close to the ALU, accessing them is much faster than accessing main memory.

**A simple processor cycle looks like this:**

1. Fetch an instruction from memory.
2. Decode the instruction to determine what to do.
3. Execute the operation in the ALU.
4. Write back the result to a register or memory.

The control unit coordinates these steps. The datapath carries the data.

## Instruction Set Architecture (ISA)

An ISA is the set of instructions a processor understands. It is the contract between software and hardware. Common ISA families include x86, ARM, and RISC-V.

**An ISA defines:**

- What instructions exist, such as load, store, add, multiply, branch, and jump.
- What registers exist and how they are used.
- How memory is addressed.
- How exceptions and interrupts work.

**Two broad styles are often compared:**

- **CISC (Complex Instruction Set Computer)** — many complex instructions; x86 is the classic example.
- **RISC (Reduced Instruction Set Computer)** — fewer, simpler instructions; ARM and RISC-V are examples.

The ISA matters for AI because compilers and libraries must translate model operations into instructions the hardware can execute. Specialized accelerators often add their own instructions or programming models for matrix operations.

## How Matrix Multiplication Maps to Digital Logic

Matrix multiplication is built from dot products. For two matrices \(A\) and \(B\), each output element is a sum of products:

$$
C_{ij} = \sum_k A_{ik} \times B_{kj}
$$

Each term \(A_{ik} \times B_{kj}\) is a multiplication. Adding it to a running total is an accumulation. Together, multiply and accumulate form a MAC operation.

**On a basic processor, one MAC operation can be performed by:**

1. Loading \(A_{ik}\) into a register.
2. Loading \(B_{kj}\) into another register.
3. Multiplying the two values in the ALU.
4. Adding the result to an accumulator register.
5. Repeating for each \(k\).

This is why matrix multiplication is slow on a simple serial processor: it requires many loads, multiplies, and adds. GPUs and AI accelerators speed it up by performing many MAC operations in parallel and by reusing data close to the compute units.

**Figure suggestion:** A diagram showing two input matrices, a dot product, and a MAC unit with multiplier and adder.

## Worked Example: Tracing a 2×2 Matrix Multiply

Suppose:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix},
\qquad
B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}
$$

The output element \(C_{00}\) is:

$$
C_{00} = (1 \times 5) + (2 \times 7) = 5 + 14 = 19
$$

**A simple processor would:**

1. Load 1 and 5 into registers.
2. Multiply: \(1 \times 5 = 5\).
3. Store 5 in the accumulator.
4. Load 2 and 7 into registers.
5. Multiply: \(2 \times 7 = 14\).
6. Add 14 to the accumulator: \(5 + 14 = 19\).
7. Write 19 to \(C_{00}\).

The same pattern repeats for \(C_{01}\), \(C_{10}\), and \(C_{11}\). Each output element is a sequence of MAC operations. Hardware accelerators are designed to perform many of these sequences at once.

## Chapter Recap

- Logic gates are built from transistors and perform basic logical operations.
- Combinational logic has no memory; sequential logic stores state and uses a clock.
- The ALU performs arithmetic and logic; registers hold operands and results.
- The ISA defines the instructions software can use.
- Matrix multiplication is a sequence of multiply-accumulate operations.
- Hardware accelerators speed up matrix math by parallelizing MACs and reusing data.

## Knowledge Check

1. **Recall.** What is the difference between combinational and sequential logic?
2. **Application.** Why does matrix multiplication require many MAC operations?
3. **Explain.** What role does the ISA play between software and hardware?
4. **Trace.** For \(C_{01}\) in the worked example, what is the result?

### Answers

**1. Recall — Combinational vs sequential.**

Combinational logic’s output depends only on current inputs and has no memory. Sequential logic stores state and updates based on a clock, so its output can depend on past inputs.

**2. Application — Why many MACs.**

Each output element of a matrix product is a sum of products. Each product is a multiplication, and each addition accumulates the result. A large matrix multiply therefore contains a very large number of MAC operations.

**3. Explain — Role of ISA.**

The ISA defines the instructions the processor can execute and how software uses registers, memory, and operations. Compilers translate high-level code into ISA instructions. It is the contract that lets software run on hardware.

**4. Trace — \(C_{01}\).**

$$
C_{01} = (1 \times 6) + (2 \times 8) = 6 + 16 = 22
$$

## References

Patterson, D. A., and Hennessy, J. L. Computer Organization and Design.

Google Books (RISC-V Edition, 2017): https://books.google.com/books/about/Computer_Organization_and_Design_RISC_V.html?id=w6ZaDwAAQBAJ

**Harris, D., and Harris, S. Digital Design and Computer Architecture. **

Google Books (Morgan Kaufmann, 2010): https://books.google.com/books/about/Digital_Design_and_Computer_Architecture.html?id=H3BQAAAAMAAJ

Hennessy, J. L., and Patterson, D. A. Computer Architecture: A Quantitative Approach.

Google Books (7th edition, 2025): https://books.google.com/books/about/Computer_Architecture.html?id=0gNHEQAAQBAJ

RISC-V International. The RISC-V Instruction Set Manual.

Official documentation (Unprivileged ISA, latest version): https://docs.riscv.org/reference/isa/unpriv/

ARM. ARM Architecture Reference Manual.

Official Arm documentation service (A-profile): https://documentation-service.arm.com/static/6770a3f5a7f5de067f4b2c7e

Intel. Intel 64 and IA-32 Architectures Software Developer’s Manual.

Combined volumes download page: https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html
    
