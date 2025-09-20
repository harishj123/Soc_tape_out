# Summary of Task 1 - Video

---

#  Chip Modeling and SoC Design Flow
---
 
## 1. Application Stage (C Code)
 
* Applications like **Firefox, Mozilla** are written in **C language**.
* Compiled using **GCC** which is a compiler that converts human readable source code into machine-readable instructions.
* **Output of this stage is considered as O0**

---

## 2. Specification Verification

* Application behavior is verified against the **(SPECS) Specifications**.
* **Output of this stage is considered as O1**
* Checks
  ```
  O0 == O1
  ```
---

## 3. RTL Design (Soft Hardware)

* Hardware is described in **RTL (Verilog/VHDL)** that is the softcopy of hardware in code.
* **Output of this stage is considered as O2**
* Checks
  ```
  O0 == O1 == O2
  ```
---

## 4. SoC Integration

* Processor, macros, and analog IPs are combined into a **microcontroller/SoC**.
* Processor has Gate level Netlist(Systh P1).
* While writing a code for processor make sure that no constructs(Verilog Primitives) are used because processor we use it for synthesize the gate
* pheripherals/IPs has Macros(Synthesizable RTL) and Analog IPs(Function RTL).
    *Macros:
        *Macros are Synthesizable RTL.
        *It is a block which is writtwn only once in a code so it can be instantiated at any time in anywhere.
     *Analog IPs:
        *Analog Ips are functional RTL.
        *Analog Ips like 10 bit ADC,PLL,Clock multipliers.
        *PLL (Phase Locked Loop) can also be used because processor works at high frequency but chips does not works with high frequency.
*  **Output of this stage is considered as O3**
* checks:
  ```
  O0 == O1 == O2 == O3
  ```
  
---

## 5. Physical Design (RTL → GDS)

* Steps:
   1. Floorplanning
   2. Placement
   3. Clock Tree Synthesis(CTS)
   4. Routing

---

## 6. Tapeout & Fabrication

* GDSII checked with **DRC/LVS** and it is sent to foundry. This process is called **Tapeout Process**.
* Fabricated chip received from factory is called **Tape-in process**.

---

## 7. Post-Silicon Testing with Peripherals

* The **same C testbench** is applied to the **fabricated chip with peripherals** on the board.
* **Output of this stage is considered as O4**
* Final verification:

  ```
  O0 == O1 == O2 == O3 == O4
  ```
  
## 8. Market Applications

* Chip runs at **100–130 MHz** and is placed on a board.
* Target applications:

  *  Smartwatches (iWatch)
  *  TV Panels
  *  AC Controllers
  *  **Arduino Boards** →  Most promising market

---

## Chip Journey Summary

```
C Code → GCC Compile → Output0
     ↓
Specification Verification → Output1
     ↓
RTL Architect → Output2
     ↓
Soc Design Flow
     ↓
ASIC Design Synthesis
     ↓
SoC Integration → Output3
     ↓
Physical Design → Output4
     ↓
Post-Silicon Testing → GDSII → Tapeout → Tape-in
     ↓
Market Deployment (Arduino, IoT, Consumer Electronics)
```

**C Code → RTL → Integrated SoC → Verified Chip → Real-World Applications**

---

