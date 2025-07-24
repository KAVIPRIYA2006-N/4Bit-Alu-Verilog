# 4Bit-Alu-Verilog
Performs basic arithmetic and logic operations controlled by mode and select signals. Includes a testbench and waveform simulation using Icarus Verilog and EPWave
# 🛠 Simple 4-bit ALU in Verilog

This project implements a basic yet versatile **4-bit Arithmetic Logic Unit (ALU)** using Verilog.  
It performs fundamental **arithmetic** and **logic** operations controlled by mode and select signals, and is fully tested with a Verilog testbench.

---

## ✨ Features
✅ Arithmetic operations:
- Addition
- Subtraction
- Multiplication
- Division
- Modulo
- Increment
- Decrement
- Fixed value (for testing)

✅ Logic operations:
- OR
- AND
- NOR
- NAND
- XOR
- XNOR
- NOT a
- NOT b

✅ Mode (`m`) to switch between arithmetic and logic  
✅ Three select lines (`s2, s1, s0`) to choose the operation

---

## 📦 Files
| File | Description |
|--|--|
| `design.sv` | ALU design (using dataflow & behavioral model) |
| `testbench.sv` | Verilog testbench to apply test cases and print results |
| `images/alu_waveform.png` | Screenshot of simulation waveform (EPWave) |

---

## 🧪 How to run
You can simulate this project easily on:
- [EDA Playground](https://www.edaplayground.com/) (using Icarus Verilog 12.0)

Or locally, if you have Icarus Verilog:
```bash
iverilog -Wall -g2012 design.sv testbench.sv
vvp a.out
