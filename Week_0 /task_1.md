# Summary of Task 1 - Video

---

#  Chip Modeling and SoC Design Flow
---
 
## 1. Application Stage (C Code)

* Applications (e.g., **Firefox, Mozilla**) are written in **C/C++**.
* Compiled using **GCC** → converts human readable source code into machine-readable instructions.
* **Output 0: Compiled Application (GCC)**

---

## 2. Specification Verification

* Application behavior is verified against the **C-model specifications**.
* **Output 1: Verified Specifications**

---

## 3. RTL Design (Soft Hardware)

* Hardware is described in **RTL (Verilog/VHDL)** → blueprint of the chip in code.
* **Output 2: Softcopy of Hardware (RTL Model)**

---

## 4. SoC Integration

* Processor, macros, and analog IPs are combined into a **microcontroller/SoC**.
* Step-by-step check:

  ```
  Output0 == Output1 == Output2 == Output3
  ```
* **Output 3: Integrated SoC**

---

## 5. Post-Silicon Testing with Peripherals

* The **same C testbench** is applied to the **fabricated chip with peripherals**.
* **Output 4: Verified Silicon Chip**
* Final verification:

  ```
  Output0 == Output1 == Output2 == Output3 == Output4
  ```

---

## 6. Physical Design (RTL → GDSII)

* Steps: Floorplanning → Placement → Clock Tree Synthesis → Routing
* Output: **GDSII file (chip layout with metal layers)**

---

## 7. Tapeout & Fabrication

* GDSII checked with **DRC/LVS** → sent to foundry (**Tapeout**)
* Fabricated chip received (**Tape-in**)

---

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
RTL Design → Output2
     ↓
SoC Integration → Output3
     ↓
Post-Silicon Testing → Output4
     ↓
Physical Design → GDSII → Tapeout → Tape-in
     ↓
Market Deployment (Arduino, IoT, Consumer Electronics)
```
---

✨ **C Code → RTL → Integrated SoC → Verified Chip → Real-World Applications**

---

