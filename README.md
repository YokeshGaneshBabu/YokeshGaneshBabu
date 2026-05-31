<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=160&section=header" width="100%"/>

<h1>Yokesh Ganesh Babu</h1>

<p>Electronics Engineering (VLSI Design & Technology) · VIT Chennai · Batch of 2027</p>

</div>

---

## 🛠️ Technical Stack

<div align="center">

### HDL & Verification
![Verilog](https://img.shields.io/badge/Verilog-RTL%20%26%20TB-1e3a5f?style=flat-square)
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-UVM%201.2-1e3a5f?style=flat-square)
![UVM](https://img.shields.io/badge/UVM-Functional%20Verification-2c3e50?style=flat-square)
![Verilog-A](https://img.shields.io/badge/Verilog--A-Behavioral%20Modeling-1e3a5f?style=flat-square)

### Programming
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)
![Embedded C](https://img.shields.io/badge/Embedded%20C-Arduino-555?style=flat-square&logo=c&logoColor=white)
![Tcl](https://img.shields.io/badge/Tcl-EDA%20Scripting-e67e22?style=flat-square)
![Perl](https://img.shields.io/badge/Perl-EDA%20Scripting-39457E?style=flat-square&logo=perl&logoColor=white)

### EDA Tools
![Cadence Virtuoso](https://img.shields.io/badge/Cadence%20Virtuoso-Analog%20IC-c0392b?style=flat-square)
![Spectre](https://img.shields.io/badge/Spectre-Circuit%20Sim-c0392b?style=flat-square)
![ModelSim](https://img.shields.io/badge/ModelSim-Simulation-0078d7?style=flat-square)
![Riviera-PRO](https://img.shields.io/badge/Aldec%20Riviera--PRO-UVM%20Sim-0078d7?style=flat-square)
![Xilinx Vivado](https://img.shields.io/badge/Xilinx%20Vivado-FPGA-e74c3c?style=flat-square)
![Synopsys TCAD](https://img.shields.io/badge/Synopsys%20TCAD-Device%20Sim-2ecc71?style=flat-square)
![LTspice](https://img.shields.io/badge/LTspice-Circuit%20Sim-8e44ad?style=flat-square)

</div>

---

## 🚀 Projects

### ✅ UART Controller RTL Design & UVM Verification
`Apr 2026 – May 2026` &nbsp;|&nbsp; `SystemVerilog · UVM 1.2 · Aldec Riviera-PRO · EDA Playground`

Complete UVM 1.2 verification environment for a UART controller, including RTL design of both TX and RX modules.

| Test | Transactions | Pass | Fail | Coverage | UVM_ERROR |
|------|:-----------:|:----:|:----:|:--------:|:---------:|
| `uart_rand_test` | 20 | 20 | 0 | 75% | 0 |
| `uart_directed_test` | 28 | 28 | 0 | **100%** | 0 |

**RTL:**
- `uart_tx` — `IDLE → START → DATA → PARITY → STOP` state machine, configurable baud (9600/115200 at 50MHz), NONE/EVEN/ODD parity, LSB-first serialization
- `uart_rx` — mid-bit sampling, two-flop synchronizer for metastability, `rx_parity_err` and `rx_frame_err` flags

**Verification environment:**
- Full UVM agent: driver, sequencer, monitor, dual analysis-port scoreboard (`uvm_analysis_imp_decl`), coverage collector
- Constrained-random sequences (20 frames), directed corner-case sequences (0x00/0xFF/0xAA/0x55 × both baud rates × all parity modes), back-to-back sequences (10 frames)
- SVA assertions: TX unknown detection, post-reset idle check, frame-count cover property — zero violations
- 100% functional coverage closure across baud × parity cross-bins

🔗 [uart_controller_verification](https://github.com/YokeshGaneshBabu/uart_controller_verification)

---

### 📡 LC-VCO with Adaptive Body Biasing & Switched Capacitor Bank
`Jan 2026 – Mar 2026` &nbsp;|&nbsp; `Cadence Virtuoso · Spectre · gpdk180 · 180nm CMOS`

Replicated and extended a **2023 Micromachines publication** on a 0.6V LC-VCO with Adaptive Body Biasing (ABB) in 180nm CMOS. Extended the design with a **3-bit switched capacitor bank**, doubling frequency coverage for Bluetooth frequency hopping.

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
- Targeted Bluetooth frequency hopping with 8 discrete frequency bands

---

### 📶 Ultra-Low Power Wake-Up Receiver Front-End (WuRx)
`Jan 2026 – Mar 2026` &nbsp;|&nbsp; `Cadence Virtuoso · Spectre · Verilog-A · gpdk180 · 1.8V CMOS`

Mixed-signal wake-up receiver front-end based on Choi et al. IEEE Access 2025, implementing a 2.4 GHz OOK architecture in 180nm CMOS.

| Block | Result |
|-------|--------|
| Envelope detector power | 153 nW average |
| Differential output swing | ~40 mV |
| Comparator delay (Verilog-A model) | 66.56 ps |
| Comparator static power | 0 W |
| End-to-end wake detection | Verified in 500 µs transient sim |

**Architecture:**
- Subthreshold envelope detector with self-referencing replica bias branch
- Dynamic clocked comparator modeled in Verilog-A — resolves analog differential to full CMOS rail-to-rail output
- 4-stage master-slave NAND DFF shift register + 1010 sync-code correlator for digital back-end

---

### 🔍 Kernel-Optimized Sobel Filter for Satellite Imagery
`Jan 2026 – Mar 2026` &nbsp;|&nbsp; `Verilog · ModelSim · Python · PyTorch`

Hardware-accelerated Sobel edge detection pipeline in Verilog, targeting real-time satellite image processing for disaster assessment.

```
Architecture Progression:
  Basic (1-cycle latency) ──► Pipelined (3-stage) ──► Learned-Kernel (quantized ML weights)
                                      ↑
                     PyTorch training → integer quantization → .vh parameter file
```

**Key contributions:**
- Designed a streaming 3×3 window extractor with dual line buffers for row-by-row pixel input
- Built a fully pipelined datapath: Stage 1 (Gx/Gy), Stage 2 (|Gx|+|Gy|), Stage 3 (output register)
- Trained a PyTorch conv model on synthetic edge images to learn hardware-friendly quantized kernels
- Auto-generated `learned_kernel_params.vh` — directly loadable as Verilog parameters, no floating-point in hardware
- ModelSim verified across all three architectures

🔗 [kernel-optimized-sobel-filter](https://github.com/YokeshGaneshBabu/kernel-optimized-sobel-filter)

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

### 🔭 Exploration Reduction in Lee's Maze Routing Algorithm
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

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=100&section=footer" width="100%"/>

*"Design at the boundary of physics and logic."*

</div>
