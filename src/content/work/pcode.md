---
title: MyC-to-PCode Compiler Project
publishDate: 2024-02-25 00:00:00
img: /assets/stock-2.jpg
img_alt: Visualization of the MyC to P-Code compilation process
description: |
  This project develops a compiler for a small imperative language called MyC, translating it into P-Code. The compiler covers the first six phases of compilation and includes features to automate the comparison of outputs against correct reference solutions.
tags:
  - Compilation
  - MyC
  - P-Code
  - GCC
---

## MyC-to-PCode Compiler Project

> A project to build a compiler for the MyC language targeting P-Code.

This project aims to implement a compiler for a mini imperative language named **MyC**, which is translated into **P-Code**. The current compiler handles the first six phases of compilation and supports up through example 17.

### Project Structure

The repository is organized as follows:

- **Reference Solutions**: The `correction` directory contains the correct outputs for all example files. A shell script (`./test`) automatically compares the compiler’s results against these reference solutions.
  
- **Modifications**: All examples in the `PCode` folder compile without errors. Adjustments were made to fix issues in the provided example files—specifically, replacing references to `stack[bp]+1` with `stack[bp].int_value+1`.

### Compilation Instructions

#### Compiling MyC to P-Code

1. Run `make` to build the compiler.  
2. Use `./run ExX` to compile a specific example, where **X** is the example number (for example, `Ex01`, `Ex02`, …, `Ex17`).

#### Compiling P-Code Files with GCC

1. Change into the `PCode` directory.  
2. Run `make ExX` to compile a specific P-Code file, or `make all` to compile all examples in one command.

### Contact

For questions or support, please reach out to the project maintainer.  

