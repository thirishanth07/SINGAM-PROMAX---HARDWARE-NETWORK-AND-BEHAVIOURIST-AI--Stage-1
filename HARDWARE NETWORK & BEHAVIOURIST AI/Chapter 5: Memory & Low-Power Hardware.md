# Chapter 5: Memory & Low-Power Hardware

**Memory hierarchy, Network-on-Chip and small AI devices. STORE / MOVE / REUSE**

## Learning Objectives

By the end of this chapter, readers should be able to:

- Explain the memory hierarchy and SRAM versus DRAM.
- Connect data movement to energy and performance.
- Explain reuse, tiling, and communication inside a chip.
- Describe embedded systems and TinyML, then bridge to Chapter 7.

## The Memory Hierarchy

A memory hierarchy arranges storage levels with different speed, capacity, and cost characteristics.

| Level | Function |
|---|---|
| **Registers** | Hold immediate processor values. |
| **Cache** | Keeps copies of useful data close to a processor. |
| **Main Memory** | Holds active programs and data. |
| **Storage** | Keeps files when power is off. |

*Nearer levels are generally smaller and faster.*

## SRAM vs DRAM

| Feature | SRAM | DRAM |
|---|---|---|
| **Definition** | Static Random-Access Memory: powered memory that retains bits without periodic refresh. | Dynamic Random-Access Memory: memory whose stored charge needs periodic refresh. |
| **Common Use** | Cache and local buffers. | Main memory. |
| **Speed** | Faster. | Slower. |
| **Density/Cost** | Less dense, more costly per bit. | More dense, cheaper per bit. |
| **Volatility** | Both are volatile (lose contents without power). | Both are volatile (lose contents without power). |

## Data Movement Can Be the Bottleneck

- **Memory bandwidth:** The amount of data a memory connection can transfer per unit of time.
- **Memory latency:** The delay before requested data becomes available.

If a processor needs values faster than memory supplies them, calculation units can wait. Moving data, especially across longer distances, can cost more energy than simple arithmetic.

## Data Reuse: Keep Useful Values Close

- A **buffer** is temporary storage used while data is processed or transferred.
- **Data reuse** keeps a value nearby for several calculations before replacing it.
- **Example:** A learned weight (model coefficient) used for 16 inputs can be loaded into a local buffer and reused instead of fetched from distant memory 16 times.

## Tiling

For matrix multiplication, load small matrix blocks, reuse them for several MAC operations, and save or retain partial results.

- A **partial result** is an unfinished output total.
- Tile size must fit local memory together with inputs and working values.

## Network-on-Chip: Communication Inside

**NoC** means Network-on-Chip: a communication network connecting components within one chip.

- A **link** carries data between connected components.
- A **router** forwards data toward its destination.
- A **packet** is a unit of transferred data with routing information. Some NoCs use packets to connect cores, memory controllers, and accelerators.

## Embedded Systems and Microcontrollers

- An **embedded system** is a computer built into a larger product for a specific purpose, such as monitoring a machine.
- A **microcontroller** is a small chip integrating a CPU, memory, and input/output interfaces for controlling a device.
- A **sensor** measures a physical quantity. Example: A vibration sensor supplies measurements to a machine-monitoring device.

## TinyML: Small Models, Small Devices

**TinyML** means tiny machine learning: running machine-learning workloads, commonly inference, on highly resource-constrained devices.

- **Inference** uses a trained model to produce an output from new data.
- **Example:** A microcontroller analyses short vibration samples and flags a possible machine fault.
- Training usually happens on a more capable system.

## Low-Power Design Techniques

| Technique | Definition |
|---|---|
| **Quantisation** | Represents values using a lower-precision numeric format; it can reduce storage and arithmetic cost on supported hardware. |
| **Duty cycling** | Keeps a component active only when needed and idle or asleep at other times. |

*Low-power design combines efficient models, data reuse, and careful measurement. Quantisation may affect accuracy; sleeping may delay a response.*

## From Inside the Chip to Chapter 7

- **Network-on-Chip** connects components within one chip.
- **Edge AI** processes data near where it is collected.
- **Cloud AI** uses remote computing services.
- **IoT** (Internet of Things) refers to physical devices connected to exchange data through networks.

*Chapter 7 explains how devices connect and share work beyond the chip.*

## Chapter Recap

- Memory levels balance speed, capacity, and cost.
- SRAM and DRAM serve different roles; both need power to retain data.
- Reuse and tiling can reduce costly data transfers.
- NoCs connect chip components; embedded systems and TinyML bring AI into small devices.
