# 🧠 Single-Cycle RISC Processor (Verilog)

An implementation of a custom 32-bit single-cycle RISC processor designed in Verilog and simulated using Xilinx Vivado. This processor supports basic arithmetic, logic, memory, and branching operations with a fixed instruction format and unified memory.

## 🚀 Features

- **Instruction Format**: 32-bit fixed format.
- **Registers**: 32 General Purpose Registers (GPRs), 16-bit wide.
- **Memory**: 64KB unified instruction and data memory (16-bit words).
- **Supported Operations**:
  - Arithmetic: ADD, SUB
  - Logical: AND, OR, XOR, NOT
  - Shift: LSL, LSR
  - Memory: Load/Store
  - Branching: BEQ, BNE, JMP
- **ALU**: Fully integrated with control decoding logic.
- **Control Unit**: Hardcoded using opcode decoding and select logic.
- **Modular Design**: Includes data path, control unit, ALU, memory units, and testbench.

## 📁 File Overview

| File                 | Description                            |
|----------------------|----------------------------------------|
| `risc.v`             | Top-level module                       |
| `data_path.v`        | Full datapath logic                    |
| `control_unit.v`     | Opcode to control signal decoding      |
| `GPRs.v`             | Register file                          |
| `Data_Memory.v`      | 64KB unified memory module             |
| `Instruction_Memory.v` | ROM for instructions (loads .prog)  |
| `ALU.v`              | Arithmetic and logic unit              |
| `alu_control.v`      | ALU control decoder                    |
| `testbench.v`        | Verilog testbench with waveform output|

## 🧪 Simulation & Test

To run:
1. Launch Vivado and create a new simulation project.
2. Add all source and testbench `.v` files.
3. Place instruction binaries (`test.prog`) in the correct path.
4. Run behavioral simulation to verify results.

## 📷 Screenshot

![image](https://github.com/user-attachments/assets/ebf3668e-1774-4c1b-a4af-893c35719f9f)



