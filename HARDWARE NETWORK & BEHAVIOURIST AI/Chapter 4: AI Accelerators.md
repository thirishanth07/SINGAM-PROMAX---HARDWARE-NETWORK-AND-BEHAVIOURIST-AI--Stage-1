# Chapter 4: AI Accelerators

**Specialised hardware for repeated AI calculations. MAC / ARRAY / ACCELERATOR**

## Learning Objectives

By the end of this chapter, readers should be able to:

- Explain MAC units and systolic arrays.
- Define NPUs, TPUs, and FPGAs.
- Compare fixed circuit structures with reconfigurable hardware.
- Recognise why memory and software affect accelerator performance.

## What is an AI Accelerator?

An AI accelerator is hardware designed to speed up selected AI operations or improve their energy efficiency.

- An **operation** is a basic computation, such as addition or multiplication.
- Accelerators combine arithmetic units, local memory, and control logic. They still need data and compatible software.

## MAC Units

- **MAC** means multiply-accumulate: multiply two values, then add the product to a running total.
- An **accumulator** is storage that holds that running total.
- **Example:** Start at 0; add 2×3 to get 6; add 4×5 to get 26.

## Systolic Arrays: An Organised Flow

A systolic array is a grid of processing units that passes data between neighbours in timed steps.

- Each unit can perform multiply-accumulate work and reuse values as they move through the grid.
- A **clock cycle** is one timing step of a clocked circuit. Work advances across multiple cycles; the whole matrix is not finished instantly.

## Why Reusing Data Helps

- **Data reuse** means using a value several times after bringing it into nearby storage or a processing array.
- **Local memory** is storage close to the calculation units.
- Reuse can reduce repeated transfers from more distant memory. The benefit depends on array size, workload shape, and available storage.

## NPU: Neural Processing Unit

- Designed for neural networks.
- Handles learned parameters (adjustable values).
- Translates input data into model outputs.
- *Note: Operations and software vary by device.*

## TPU: Google's AI Accelerator

**TPU** means Tensor Processing Unit: Google's custom accelerator for machine learning.

- A **tensor** is an array of numbers; a vector is one-dimensional and a matrix is two-dimensional.
- Cloud TPU matrix units use systolic arrays. Supported workloads benefit from suitable shapes, data types, and software compilation.

## FPGA: Reconfigurable Hardware

**FPGA** means Field-Programmable Gate Array: a chip whose logic blocks and connections can be reconfigured after manufacture.

- A **pipeline** divides a task into stages so different inputs can occupy different stages at once.
- An FPGA can implement a custom AI pipeline, but design effort, resources, and software support constrain it.

## Choosing an Accelerator

| Type | Main idea | Check before use |
|---|---|---|
| **NPU** | Neural-network processing hardware | Operations and deployment tools |
| **TPU** | Google tensor processing hardware | Model shapes and software support |
| **FPGA** | Reconfigurable logic and connections | Design effort and available resources |

## Chapter Recap

- MAC units build results through repeated multiplication and accumulation.
- Systolic arrays coordinate neighbouring units and reuse moving data.
- NPUs and TPUs specialise AI computation; FPGAs allow circuit reconfiguration.
- An accelerator needs sufficient memory bandwidth and compatible software to stay useful.
