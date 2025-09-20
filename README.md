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
---

# ⚙️ Task 2 – Installation Guide

## 🖥️ System Requirements

* **RAM:** 6 GB
* **Disk:** 50 GB
* **CPU:** 4 vCPUs
* **OS:** Ubuntu 20.04+

Download VirtualBox: [Oracle VM](https://www.virtualbox.org/wiki/Downloads)

---

## 🔧 Tool Setup

### 1️⃣ Yosys (Synthesis Tool)

```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install
```

### 2️⃣ Icarus Verilog (Simulator)

```bash
sudo apt-get update
sudo apt-get install iverilog
```

### 3️⃣ GTKWave (Waveform Viewer)

```bash
sudo apt-get update
sudo apt-get install gtkwave
```

### 4️⃣ OpenSTA (Static Timing – optional)

🔗 [OpenSTA GitHub](https://github.com/The-OpenROAD-Project/OpenSTA)

---

✅ Now your environment is ready!

---


