# Chapter 2: Digital Logic & Computer Organisation

**From binary information to instructions and AI calculations. BITS / GATES / PROCESSOR**

## Learning Objectives

By the end of this chapter, readers should be able to:

- Represent different kinds of information using bits.
- Explain gates, circuits, and processor components.
- Follow an instruction from memory to its result.
- Connect matrix multiplication to digital hardware.

## Binary: Counting with Two Digits

A number system is a way of writing numbers using digits and place values.

- **Binary** uses only 0 and 1. A bit is one binary digit; eight bits form one byte.
- **Decimal** uses ten digits.
- Example: Binary `1010` means 1×8 + 0×4 + 1×2 + 0×1 = 10 in decimal.

## Encoding Information

Encoding means choosing rules that represent information as bit patterns.

- **Numbers:** Use numeric formats.
- **Text:** Uses character codes. ASCII is a coding standard; uppercase `A` has the decimal code 65.
- **Images:** A grid of pixels (picture elements) whose colours are stored as numbers.
- **Sound:** Audio sampling measures a sound signal at regular time intervals; each measurement becomes a number.
- **Video:** Represents changing images as a sequence of frames, usually with audio.

**Compression** reduces the number of bits needed.

- **Lossless compression** preserves the original data.
- **Lossy compression** discards some detail.

## Logic Gates: Rules for Bits

A logic gate is a circuit that produces an output bit from input bits using a rule. Boolean logic works with two logical values, represented here by 0 and 1.

| A | B | AND | OR | XOR |
|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 | 1 |
| 1 | 1 | 1 | 1 | 0 |

- **AND** gives 1 only if both inputs are 1.
- **OR** gives 1 if at least one input is 1.
- **NOT** reverses one input.

## From Gates to a Digital Circuit

A digital circuit connects gates to process or store bit values.

- **XOR (exclusive OR):** Produces 1 when its two input bits differ.
- **Half Adder:** Adds two bits. XOR produces the sum bit and AND produces the carry bit. A carry passes extra value to the next position.

**Example: 1 + 1**
- SUM: 0
- CARRY: 1

## Processor Components

| Component | Definition |
|---|---|
| **CPU** | Central Processing Unit: a processor that executes program instructions. |
| **ALU** | Arithmetic Logic Unit: the part that performs arithmetic and logical comparisons. |
| **Registers** | Small, fast storage locations inside a processor. |
| **Control Unit** | Directs the steps needed to execute instructions. |

## ISA: The Instructions Hardware Understands

**ISA** means Instruction Set Architecture: the software-visible rules defining instructions, registers, and memory access.

- An instruction tells the processor to perform an operation, such as `ADD`, `LOAD`, or `STORE`.
- **LOAD** copies data from memory into a register.
- **STORE** copies data from a register to memory.

## A Simple Computer Executes 2 + 3

A program is a sequence of instructions. The **program counter** is a register that tracks the address of an instruction.

1. **Fetch:** Retrieves an instruction from memory.
2. **Decode:** Identifies what it requests.
3. **Execute:** Performs the requested work.

**Example:**
- `LOAD` 2 and 3 into registers.
- `ADD` them to obtain 5.
- `STORE` the result in memory.
- **Result:** 5

## Matrix Multiplication and MAC

- A **matrix** is a rectangular table of numbers. Matrix multiplication combines a row from one matrix with a column from another.
- **MAC** means multiply-accumulate: multiply two values and add their product to a running total.
- **Example:** Row `[2, 4]` × Column `[3, 5]` gives (2×3) + (4×5) = 26. Repeat for other row-column pairs.

## Chapter Recap

- Bits represent numbers and other data through agreed encodings.
- Gates combine into circuits that calculate and store information.
- The control unit, registers, and ALU cooperate to execute ISA instructions.
- AI matrix calculations reduce to repeated multiply-accumulate operations.
