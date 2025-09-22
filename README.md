# CPU in VHDL (CpE 271L)

## Project Overview
A small, educational CPU implemented in **VHDL**.  

This project implements a simplified **von Neumann CPU** that supports three instructions: `LOADA`, `ADDA`, and `STOREA`.  
The CPU uses a **5-bit address space** (32 memory words) with **8-bit data words**, and includes the following main components:

- Accumulator (A)  
- Instruction Register (IR)  
- Program Counter (PC)  
- Memory Address Register (MAR)  
- Memory Data Registers (MDRI, MDRO)  
- Arithmetic Logic Unit (ALU)  
- Control Unit (CU)  
- RAM (from Lab 9 memory component)  

The CPU operates in a classic **fetch → decode → execute** cycle.  
The provided handout contains diagrams and behavioral descriptions. This repository contains the **VHDL templates** and the pieces that must be completed.

---

## Features / Behavior
- **Instruction format:** 8-bit instructions  
  - Top 3 bits = opcode  
  - Lower 5 bits = operand (memory address)  

- **Supported opcodes:**  
  - `LOADA`  
  - `ADDA`  
  - `STOREA`  

- **Memory:**  
  - 5-bit address bus (32 addresses)  
  - 8-bit data width  

- **ALU operations:**  
  - Add  
  - Subtract  
  - Bitwise AND / OR  
  - Pass A / Pass B  

- **Control Unit:**  
  - Implemented as a **finite state machine**  
  - Controls **fetch** and **execute** sequences  
