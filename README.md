# 8 bit ALU RTL Design in Verilog

*The purpose of this project is to design and verify an 8-bit Arithmetic Logic Unit (ALU) using Verilog HDL to perform basic arithmetic and logical operations with status flag generation.*

---

## Introduction
This project implements an **8-bit ALU** using **RTL design methodology** in Verilog HDL. The ALU supports commonly used **arithmetic and logical operations** such as **addition, subtraction, AND, OR, and XOR**, along with **Zero and Carry flag** generation. The design is parameterized to allow easy scalability for different data widths.

---

## Design Methodology
- Designed the ALU using **combinational logic blocks**
- Used **opcode-based operation selection**
- Implemented arithmetic operations using binary adders
- Generated **status flags** based on output results
- Parameterized the data width for reusability

---

## ALU Operation Description
- The ALU accepts two 8-bit operands and a control opcode
- Each opcode maps to a specific arithmetic or logical operation
- Output flags indicate:
  - **Zero flag:** Result equals zero
  - **Carry flag:** Carry-out from arithmetic operations

---

## Opcode Table
| Opcode | Operation |
|------|-----------|
| 000  | Addition |
| 001  | Subtraction |
| 010  | AND |
| 011  | OR |
| 100  | XOR |

---

## Tools & Technologies
- **Language:** Verilog HDL
- **Design Style:** RTL Design
- **Simulation Tool:** Xilinx Vivado / ModelSim
- **Concepts Used:** Combinational logic, arithmetic circuits, parameterization

---

## Testbench & Verification
- Developed a **self-checking Verilog testbench**
- Applied multiple operand and opcode combinations
- Verified ALU outputs and flags using **simulation waveforms**
- Ensured functional correctness across all supported operations

---

## Output Waveforms
Simulation waveforms validate correct ALU functionality, including:
- Proper result generation for each opcode
- Accurate Zero and Carry flag behavior

<!-- Add waveform images here -->
<!-- Example:
![ALU Waveform](images/alu_waveform.png)
-->

---

## Results
The ALU successfully performs all defined arithmetic and logical operations for 8-bit inputs. Simulation results confirm correct opcode decoding, result computation, and flag generation. The parameterized design ensures flexibility and reusability for wider datapath implementations.

---

## How to Run
1. Open the project in **Xilinx Vivado**
2. Add ALU RTL and testbench files
3. Run behavioral simulation
4. Observe result and flag signals in the waveform viewer

---

## Future Work
- Extension to **16-bit / 32-bit ALU**
- Addition of **shift and comparison operations**
- Integration into a **simple processor datapath**
- Power and timing optimization

---

## Author
**Nischal Agarwal**  
Electronics and Communication Engineering  
Birla Institute of Technology, Mesra
