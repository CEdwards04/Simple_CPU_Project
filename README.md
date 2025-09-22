Project overview

A small, educational CPU implemented in VHDL for the CpE 271L Digital Logic Laboratory.
This project implements a simplified von-Neumann CPU that supports three instructions: LOADA, ADDA, and STOREA. The CPU uses a 5-bit address space (32 memory words) with 8-bit data words, and includes the following main components:

Accumulator (A)

Instruction Register (IR)

Program Counter (PC)

Memory Address Register (MAR)

Memory Data Registers (MDRI, MDRO)

ALU

Control Unit (CU)

RAM (from Lab 9 memory component)

The CPU operates in a classic fetch → decode → execute cycle. The handout contains diagrams and behavioral descriptions; this repo contains the VHDL templates and the pieces you must complete.

Features / behavior

8-bit instructions: top 3 bits = opcode, lower 5 bits = operand (memory address).

Supported opcodes: LOADA, ADDA, STOREA.

Memory: 5-bit address bus (32 addresses), 8-bit data width.

ALU operations: add, subtract, bitwise AND/OR, pass A/B (ALU created from Lab 9).

Control Unit implemented as a finite state machine controlling the fetch and execute sequences.
