# Full_Adder_using-CMOS
This project demonstrates the design and analysis of a **1-bit Full Adder** using CMOS logic. A Full Adder is a fundamental building block in digital electronics, used to perform binary addition of three input bits.
The project includes:
- Boolean logic derivation
- Truth table
- CMOS schematic design
- Simulation waveforms
- Layout design
- Power, delay, and area analysis
- Optional comparison with pass transistor logic

---
## 📚 Table of Contents

- [1. What is a Full Adder?](#1-what-is-a-full-adder)
- [2. Truth Table](#2-truth-table)
- [3. Boolean Expressions](#3-boolean-expressions)
- [4. CMOS Schematic Design](#4-cmos-schematic-design)
- [5. Simulation Results](#5-simulation-results)
- [6. Layout Design](#6-layout-design)
- [7. Performance Analysis](#7-performance-analysis)
- [8. Tools and Technologies](#8-tools-and-technologies)
- [9. File Structure](#9-file-structure)
- [10. Author](#10-author)

---
## 1. What is a Full Adder?

A **Full Adder** adds three binary bits:
- Input A
- Input B
- Carry-In (Cin)
  
![Full Adder Circuit using Gate](.c:\Users\ACER\OneDrive\Pictures\Cmos_days\Full_adder_schamtic_by_gate.png)
- **Sum**
- **Carry-Out (Cout)**

---

## 2. Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 |  0  |  0  |  0   |
| 0 | 0 |  1  |  1  |  0   |
| 0 | 1 |  0  |  1  |  0   |
| 0 | 1 |  1  |  0  |  1   |
| 1 | 0 |  0  |  1  |  0   |
| 1 | 0 |  1  |  0  |  1   |
| 1 | 1 |  0  |  0  |  1   |
| 1 | 1 |  1  |  1  |  1   |

![Truth Table](.c:\Users\ACER\OneDrive\Pictures\Cmos_days\Truth Table of Full Adder.png)

---

## 3. Boolean Expressions

### Sum:
Sum = A ⊕ B ⊕ Cin

### Carry-Out:
Cout = AB + BCin + ACin

## 4. CMOS Schematic Design

- Designed using **nMOS** and **pMOS** transistors.
- XOR implemented using combination of basic CMOS logic.
- Organized in a modular way: First XOR gate → Second XOR → Carry logic.

📷 **Schematic View:**

![Schematic](.C:\Users\ACER\OneDrive\Pictures\Cmos_days\Full_Adder_schematic.png)

---

## 5. Simulation Results

- Input waveform: `A`, `B`, `Cin`
- Output waveform: `Sum`, `Cout`

---
## 6. Layout Design

- Created using **[Microwind/Cadence/Custom Tool]**
- DRC-clean and LVS passed

📷 **Layout View:**

![Layout](.C:\Users\ACER\OneDrive\Pictures\Cmos_days\Full_adder_Physical_layout.png)
