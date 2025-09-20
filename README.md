# Digital VLSI SOC Design and Planning

# Task 1 – Chip Journey  

1. **C Code** → Compile with GCC → Verified (O1)  

2. **RTL Design** (Verilog/VHDL) → Verified (O2)  

3. **ASIC Synthesis** → Gate-level Netlist/Macros/Analog IPs → Verified (O3)  

4. **SoC Integration** → Processor + Peripherals + IPs  

5. **Physical Design** → GDSII Layout → Fabrication  

6. **Post-Silicon Test** → Run same C testbench → Verified (O4)  

7. **Applications** → Arduino, Smartwatches, TVs, ACs  


 Final Check:

```
O0 == O1 == O2 == O3 == O4
```

---

Code → RTL → Chip → Real-world products.

---


---

# Task 2 – Installation Steps

---

## 1. Setup Virtual Environment

* Install **Oracle VirtualBox**.
* Check system requirements:

  * **6 GB RAM**, **50 GB HDD**
  * **Ubuntu 20.04+**
  * **4 vCPUs**

---

## 2. Install Yosys

* Clone the **Yosys repository**.
* Install required dependencies (build tools, libraries).
* Build and install **Yosys** for RTL synthesis.

---

## 3. Install Icarus Verilog (Iverilog)

* Install **Iverilog** for simulation of Verilog designs.

---

## 4. Install GTKWave

* Install **GTKWave** to view simulation waveforms.

---

## 5. Optional: OpenSTA

* For timing analysis (not required for SFAL participants).
* Install **OpenSTA** from the OpenROAD project repository.

---

## Flow of Task 2:

1. Setup VirtualBox + Ubuntu → 2. Install Yosys → 3. Install Iverilog → 4. Install GTKWave → 5. (Optional) OpenSTA

---



