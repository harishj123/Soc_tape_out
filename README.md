# Digital VLSI SOC Design and Planning

# 🚀 Task 1 – Chip Journey  

A quick view of how a **C program becomes a real chip**:  

1️⃣ **C Code** → Compile with GCC → ✅ Verified (O1)  

2️⃣ **RTL Design** (Verilog/VHDL) → ✅ Verified (O2)  

3️⃣ **ASIC Synthesis** → Gate-level Netlist/Macros/Analog IPs → ✅ Verified (O3)  

4️⃣ **SoC Integration** → Processor + Peripherals + IPs  

5️⃣ **Physical Design** → GDSII Layout → 🏭 Fabrication  

6️⃣ **Post-Silicon Test** → Run same C testbench → ✅ Verified (O4)  

7️⃣ **Applications** → Arduino, Smartwatches, TVs, ACs  


✔️ Final Check:

```
O0 == O1 == O2 == O3 == O4
```

---

✨  Code → RTL → Chip → Real-world products.

---

# Project Tasks

- [Task 1: Chip Modeling]-(./week_0/task_1)

---

# 🛠️ Task 2 – Installation Steps

This task explains the tools and environment setup required for chip design and verification.

---

## 1️⃣ Setup Virtual Environment

* Install **Oracle VirtualBox**.
* Check system requirements:

  * **6 GB RAM**, **50 GB HDD**
  * **Ubuntu 20.04+**
  * **4 vCPUs**

---

## 2️⃣ Install Yosys

* Clone the **Yosys repository**.
* Install required dependencies (build tools, libraries).
* Build and install **Yosys** for RTL synthesis.

---

## 3️⃣ Install Icarus Verilog (Iverilog)

* Install **Iverilog** for simulation of Verilog designs.

---

## 4️⃣ Install GTKWave

* Install **GTKWave** to view simulation waveforms.

---

## 5️⃣ Optional: OpenSTA

* For timing analysis (not required for SFAL participants).
* Install **OpenSTA** from the OpenROAD project repository.

---

## Flow of Task 2:

1. Setup VirtualBox + Ubuntu → 2. Install Yosys → 3. Install Iverilog → 4. Install GTKWave → 5. (Optional) OpenSTA

---



