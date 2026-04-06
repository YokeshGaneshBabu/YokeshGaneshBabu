<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=160&section=header" width="100%"/>

<h1>Yokesh Ganesh Babu</h1>
<p><b>VLSI Design &nbsp;·&nbsp; Analog IC &nbsp;·&nbsp; RTL & Verification</b></p>
<p><i>3rd Year B.Tech EE (VLSI Design and Technology) · VIT Chennai ·</i></p>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yokesh--ganesh--babu-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yokesh-ganesh-babu)
[![GitHub](https://img.shields.io/badge/GitHub-YokeshGaneshBabu-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/YokeshGaneshBabu)
[![Email](https://img.shields.io/badge/Email-yokeshsgar@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yokeshsgar@gmail.com)
[![Location](https://img.shields.io/badge/Chennai,%20India-📍-6366f1?style=for-the-badge)](.)

</div>

---

## 👋 About Me

I'm a 3rd-year B.Tech Electronics Engineering student at **VIT Chennai**, specializing in **VLSI Design and Technology** . I work across the analog-digital stack — from transistor-level analog IC design in Cadence Virtuoso to pipelined processor RTL in Verilog, with a focus on building things that are grounded in real silicon constraints.

Currently working on:
- 🔬 **Gas sensor research** with faculty — fabrication + characterization 
- 🔁 **LC-VCO with Switched Capacitor Bank** — extending a 2023 Micromachines paper in 180nm CMOS
- ⚡ **Sobel Edge Detection** hardware architecture in Verilog targeting satellite image processing

---

## 🛠️ Technical Stack

<div align="center">

### HDL & Programming
![Verilog](https://img.shields.io/badge/Verilog-RTL%20%26%20TB-1e3a5f?style=flat-square&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyTDIgN2wxMCA1IDEwLTV6TTIgMTdsOSA0LjkgOS00LjlWN0wxMiAxMiAyIDd6Ii8+PC9zdmc+)
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-Verification-1e3a5f?style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Embedded C](https://img.shields.io/badge/Embedded%20C-8051%20%7C%20Arduino-555?style=flat-square&logo=c&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)

### EDA Tools
![Cadence Virtuoso](https://img.shields.io/badge/Cadence%20Virtuoso-Analog%20IC-c0392b?style=flat-square)
![ModelSim](https://img.shields.io/badge/ModelSim-Simulation-0078d7?style=flat-square)
![Xilinx Vivado](https://img.shields.io/badge/Xilinx%20Vivado-FPGA-e74c3c?style=flat-square)
![Synopsys TCAD](https://img.shields.io/badge/Synopsys%20TCAD-Device%20Sim-2ecc71?style=flat-square)
![LTspice](https://img.shields.io/badge/LTspice-Circuit%20Sim-8e44ad?style=flat-square)

</div>



### 📡 LC-VCO with Adaptive Body Biasing & Switched Capacitor Bank
`Jan 2026 – May 2026 (ongoing)` &nbsp;|&nbsp; `Cadence Virtuoso · Spectre · gpdk180 · 180nm CMOS`

Replicated and extended a **2023 Micromachines publication** on a 0.6V LC-VCO with Adaptive Body Biasing (ABB) in 180nm CMOS. Extended the design with a **3-bit switched capacitor bank**, doubling the frequency coverage for Bluetooth frequency hopping applications.

| Parameter | Baseline (Paper) | Extended (This Work) |
|-----------|:-:|:-:|
| Oscillation Frequency | 2.4 GHz | 2.4 GHz |
| Supply Voltage | 0.6 V | 0.6 V |
| Tuning Range | 80 MHz | ~160 MHz across 8 bands |
| Phase Noise @ 1 MHz offset | −107 dBc/Hz | −107 dBc/Hz |
| Power Consumption | ~400 µW | ~400 µW |

**Key contributions:**
- Replaced fixed tank capacitor with 3-bit binary-weighted switched cap bank
- Demonstrated faster frequency settling with ABB vs. constant body bias during band switching
- Targeted **Bluetooth frequency hopping** with 8 discrete frequency bands

---

### ⚙️ 5-Stage Pipelined 32-bit MIPS Processor
`Dec 2025 – Feb 2026` &nbsp;|&nbsp; `Verilog · ModelSim`

Full 5-stage pipelined MIPS processor (IF → ID → EX → MEM → WB) with complete hazard handling.

```
Pipeline Stages:   IF ──► ID ──► EX ──► MEM ──► WB
                              ↑              │
                    Forwarding Unit ◄────────┘
                    Hazard Detection → Stall / Bubble
```

- ✅ **Forwarding unit** — resolves ALU-ALU data hazards with zero stall penalty
- ✅ **Hazard detection** — load-use dependencies handled with bubble insertion
- ✅ **Full datapath** — register file, ALU control, branch logic, memory interface
- ✅ **ModelSim verified** — forwarding paths, stall cycles, write-back timing

---

### 🧭 Single-Cycle 32-bit RISC-V Processor
`Jul 2025 – Nov 2025` &nbsp;|&nbsp; `Verilog · ModelSim`

Single-cycle RISC-V processor supporting **28 instructions** — the architectural foundation that the MIPS pipeline was built on top of conceptually.

- Built complete datapath: ALU, register file, control unit, branch logic
- Developed RTL modules and functional testbenches from scratch
- Verified instruction execution and control flow through simulation

---

### 🔍 Exploration Reduction in Lee's Maze Routing Algorithm
`Jul 2025 – Nov 2025` &nbsp;|&nbsp; `Python · EDA Algorithms`

Optimized the classical Lee routing algorithm used in PCB/IC layout tools.

```
Standard Lee:    5008 cells explored
Optimized:       3200 cells explored
Reduction:       36% fewer cells  ──► faster routing, lower memory
Technique:       Bidirectional BFS + pruning heuristics
```

Benchmarked across multiple net configurations and grid densities.

---

### 🔧 Varactor Diode Design & Simulation
`Mar 2025 – Apr 2025` &nbsp;|&nbsp; `Synopsys TCAD`

Device-level design and simulation of a voltage-controlled varactor diode using TCAD process simulation.

- Swept C–V characteristics across doping concentrations and reverse bias conditions
- Analyzed junction capacitance tuning range vs. doping profile
- Validated device behavior against theoretical semiconductor models

---

### 🚦 Smart Adaptive Traffic Light Controller
`Jul 2024 – Oct 2024` &nbsp;|&nbsp; `Arduino · Embedded C`

FSM-based adaptive traffic controller with emergency vehicle override capability.

- Sensor-driven FSM logic for dynamic signal timing
- Real-time emergency override using interrupt-driven embedded C
- Demonstrated on physical Arduino setup

---




## 💼 Experience

**Summer Intern — vTitan Corporation Pvt Ltd** &nbsp;`May 2025 – Jun 2025`

Worked on CPLD-to-FPGA migration for legacy digital designs — RTL porting, Vivado implementation, waveform-based debugging, and functional verification against design specs.

---

## 🔭 Currently Working On

```
[■■■■■■■░░░] LC-VCO Extended Design          — Cadence Virtuoso (ongoing)
[■■■░░░░░░░] Sobel Edge Detection in Verilog  — targeting satellite image processing
[■■■■■■░░░░] ZnO Gas Sensor Research          — fabrication + publication (with faculty)
```

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=100&section=footer" width="100%"/>

*"Design at the boundary of physics and logic."*

</div>
