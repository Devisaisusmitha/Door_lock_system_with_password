# Automatic Door Lock System 🔐

**Applies CMOS VLSI Digital Design fundamental concepts to Embedded Systems**

## 🎯 VLSI Concepts Used
This project implements digital design fundamentals.
### **Demo**
![Working Demo](demo.gif)

| VLSI Topic | Implementation in Project |
| --- | --- |
| **Finite State Machine (FSM)** | System states: `IDLE → INPUT → VERIFY → UNLOCK/LOCKED` |
| **Sequential Logic** | 4-digit password stored & checked sequentially using registers |
| **Clocking & Timing** | Servo PWM control + `delay()` for debouncing = clocked operations |
| **Digital Comparators** | Password verification logic = 4-bit digital comparator |
| **Memory Elements** | Password stored in EEPROM, similar to memory design concepts |

## 🔧 Hardware
- Arduino UNO
- 4x4 Keypad 
- Servo Motor SG90
- 16x2 LCD

## ⚡ How It Works
1. **IDLE State**: Waits for keypad input
2. **INPUT State**: Captures 4 digits sequentially into buffer registers
3. **VERIFY State**: Compares input with stored password using combinational logic
4. **UNLOCK State**: Triggers servo for 3s if match, then auto-locks → back to IDLE
This demonstartes understanding of digital design fudamentals, not VLSI chip design.

## 🎓 Course Alignment
Built while pursuing **NPTEL CMOS Digital VLSI Design - Elite 69%** by Prof. Sudeb Dasgupta, IIT Roorkee. 
Course topics applied: MOS transistors, CMOS logic, sequential design, clocking strategies.

### **Circuit Diagram
![Circuit Diagram](circuit.png)

## 🏷️ Tags
`#VLSI` `#DigitalDesign` `#FSM` `#SequentialLogic` `#EmbeddedSystems` `#Arduino` `#NPTEL` `#IITRoorkee`
