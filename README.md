<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=venom&height=240&color=0:070b14,40:111b35,70:253b68,100:00e5ff&text=YOKESH%20GANESH%20BABU&fontColor=ffffff&fontSize=44&fontAlignY=42&desc=RTL%20DESIGN%20%E2%80%A2%20VERIFICATION%20%E2%80%A2%20AI%20%E2%80%A2%20SILICON&descSize=14&descAlignY=62&animation=twinkling" width="100%" alt="Yokesh Ganesh Babu banner"/>
</p>

<p align="center">
  <img src="./assets/binary-banner.svg" width="85%" alt="Scrolling binary banner"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=2800&pause=900&color=00E5FF&center=true&vCenter=true&width=760&height=50&lines=%3E+Building+RTL.+Checking+every+edge+case.;%3E+Exploring+AI%2FML+for+EDA.;%3E+From+transistor+physics+to+digital+systems.;%3E+Hardware+is+where+the+layers+meet.;%3E+01011001+01001111+01001011+%E2%86%92+YOK" alt="Typing tagline"/>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=YokeshGaneshBabu&label=PROFILE+VIEWS&color=00e5ff&style=for-the-badge" alt="Profile views"/>
  <img src="https://img.shields.io/badge/VIT-Chennai-253b68?style=for-the-badge&logo=googlescholar&logoColor=00e5ff" alt="VIT Chennai"/>
  <img src="https://img.shields.io/badge/Status-Open_to_VLSI_Internships-00e5ff?style=for-the-badge&labelColor=070b14" alt="Status"/>
</p>

<p align="center">
  <a href="https://github.com/YokeshGaneshBabu?tab=repositories"><img src="https://img.shields.io/badge/PROJECTS-070b14?style=for-the-badge&logo=github&logoColor=00e5ff&labelColor=070b14" alt="Projects"/></a>
</p>

<p align="center"><sub>Electronics Engineering · VLSI Design &amp; Technology</sub></p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%" alt="divider"/>

### `00` / WHOAMI

```verilog
module yokesh #(parameter PASSION = "VLSI") (
    input  wire coffee,
    input  wire curiosity,
    output reg  [31:0] ideas
);
    always @(posedge curiosity) begin
        if (coffee) ideas <= ideas + 1;   // never overflows
        else        ideas <= ideas;       // latch... avoid at all costs
    end

    // Currently: RTL design | verification | ML for EDA
endmodule
```

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%" alt="divider"/>

### `01` / ENGINEERING DOMAINS

<table>
<tr>
<td width="50%" valign="top">

**01 · DIGITAL DESIGN & VERIFICATION**

`Verilog` `SystemVerilog` `SVA` `UVM`

RTL design, self-checking testbenches, protocol checking, assertions, constrained-random stimulus, and functional coverage.

</td>
<td width="50%" valign="top">

**02 · AI / ML × EDA**

`Python` `PyTorch` `Scikit-learn`

CNN feature extraction, classical ML, lithography hotspot detection, routing congestion prediction, and semiconductor manufacturing analytics.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**03 · ANALOG & DEVICE ENGINEERING**

`Cadence Virtuoso` `Spectre` `Sentaurus TCAD`

Circuit simulation, oscillator design, mixed-signal blocks, FinFET characterization, and back-gate bias analysis.

</td>
<td width="50%" valign="top">

**04 · DIGITAL SYSTEMS & EMBEDDED**

`Processor Design` `Embedded C` `ESP32`

Processor microarchitecture, pipelining, FIFO design, peripheral protocols, and microcontroller-based automation.

</td>
</tr>
</table>

---

### `02` / FEATURED PROJECTS

<table>
<tr>
<td width="50%" valign="top">

### 01. UART Controller

**RTL Design + SystemVerilog Verification**

`Verilog` `SystemVerilog` `Simulation`

Designed UART transmitter and receiver RTL with configurable baud rates and parity modes.

- Directed and randomized frame testing
- Serial data and parity checking
- Reset and framing corner cases

<a href="https://github.com/YokeshGaneshBabu/uart_controller_verification">Explore UART repository ↗</a>

</td>
<td width="50%" valign="top">

### 02. APB Slave + Protocol Checker

**Assertion-Based Verification**

`SystemVerilog` `SVA` `APB`

Implemented an APB slave design with a separate protocol checker.

- Protocol property checking
- Reset and transfer behavior
- Directed simulation and assertion results

<a href="https://github.com/YokeshGaneshBabu?tab=repositories">Find repository ↗</a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 03. CNN Features + Classical ML

**Lithography Hotspot Detection**

`PyTorch` `CNN` `Classical ML`

Compared CNN architectures, learned feature representations, and classical classification heads across lithography hotspot benchmarks.

- Balanced accuracy and benchmark comparisons
- Ablation and statistical analysis
- Calibration and inference-latency evaluation

<a href="https://github.com/YokeshGaneshBabu?tab=repositories">Find repository ↗</a>

</td>
<td width="50%" valign="top">

### 04. VLSI Routing Congestion Prediction

**Machine Learning for EDA**

`Python` `Random Forest` `EDA`

Developed a synthetic layout-data and ML pipeline for predicting routing congestion.

- Layout and congestion-map generation
- Regression and classification models
- Evaluation on unseen layouts

<a href="https://github.com/YokeshGaneshBabu?tab=repositories">Find repository ↗</a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 05. Drift-Sense

**FinFET Pattern Localization**

`Python` `Computer Vision`

Built a classical computer-vision pipeline to recover pattern coordinates from larger inspection images under geometric variation and image degradation.

- Multi-scale and multi-rotation matching
- Phase-correlation assistance
- Candidate filtering and reproducible evaluation

<a href="https://github.com/YokeshGaneshBabu?tab=repositories">Find repository ↗</a>

</td>
<td width="50%" valign="top">

### 06. Kernel-Optimized Sobel Filter

**ML-to-RTL Hardware Exploration**

`Verilog` `PyTorch` `ModelSim`

Built a streaming edge-detection datapath with fixed and learned quantized kernels.

- 3 × 3 window extraction
- Three-stage pipelined implementation
- ML-generated integer kernel parameters

<a href="https://github.com/YokeshGaneshBabu/kernel-optimized-sobel-filter">Explore repository ↗</a>

</td>
</tr>
</table>

---

### `03` / RTL & MICROARCHITECTURE

| Project | Technical focus |
|:--|:--|
| **Single-Cycle RISC-V Processor** | RV32I microarchitecture, instruction decoding, datapath and control, simulated execution of compiled image-processing code |
| **Synchronous FIFO** | Parameterized RTL, wraparound pointers, full/empty detection, self-checking testbench |
| **UART · UVM Implementation** | UVM components, transaction-level stimulus, scoreboard, coverage collection, directed and constrained-random tests |
| **Lee's Maze Routing Optimization** | Dead-end pruning, bidirectional BFS, shortest-path reconstruction, bend minimization and algorithm benchmarking |

<p align="center"><a href="https://github.com/YokeshGaneshBabu?tab=repositories">Browse RTL repositories ↗</a></p>

---

### `04` / ANALOG, DEVICES & MIXED-SIGNAL

<details>
<summary><strong>LC-VCO with Adaptive Body Biasing</strong></summary>

180 nm CMOS oscillator design and simulation using Cadence Virtuoso and Spectre, extended with a switched-capacitor bank for discrete frequency tuning.

</details>

<details>
<summary><strong>Ultra-Low-Power Wake-Up Receiver</strong></summary>

2.4 GHz OOK receiver front-end exploration involving envelope detection, a behavioral comparator, and digital synchronization logic.

</details>

<details>
<summary><strong>Back-Gated FinFET Characterization</strong></summary>

TCAD investigation of transfer/output characteristics, threshold-voltage shifts, subthreshold swing, back-gate coupling, and buried-oxide thickness.

</details>

<sub>Some device and circuit projects are documented through simulation data, plots, schematics, and technical reports rather than public source-code repositories.</sub>

---

### `05` / EMBEDDED SYSTEMS

#### Smart Medicine Dispenser

`ESP32` `Embedded C` `RTC` `Sensors` `Actuation`

A scheduled medicine-dispensing prototype with two compartments for pre-meal and post-meal doses.

- DS3231 real-time clock for schedule tracking
- Servo-controlled compartment access
- IR-based pill-removal detection with interrupt debouncing
- LCD, LEDs, and audio prompts for user feedback

*Repository in preparation.*

---

### `06` / SEMICONDUCTOR DATA & AI

<details>
<summary><strong>Wafer Yield Analysis & Defect Classification</strong></summary>

Analyzed semiconductor manufacturing sensor data, including missing-value handling, feature selection, class imbalance, and pass/fail classification.

</details>

<details>
<summary><strong>Additional AI / ML Experiments</strong></summary>

Explorations in feature engineering, model comparison, image-based localization, and data-driven EDA workflows.

</details>

---

### `07` / TOOLCHAIN

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,pytorch,c,bash,linux,git,github,vscode,arduino&theme=dark" alt="Skill icons"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Verilog-RTL-19324d?style=for-the-badge" alt="Verilog"/>
  <img src="https://img.shields.io/badge/SystemVerilog-Verification-19324d?style=for-the-badge" alt="SystemVerilog"/>
  <img src="https://img.shields.io/badge/SVA-Assertions-19324d?style=for-the-badge" alt="SVA"/>
  <img src="https://img.shields.io/badge/UVM-1.2-19324d?style=for-the-badge" alt="UVM"/>
  <img src="https://img.shields.io/badge/Cadence-Virtuoso-19324d?style=for-the-badge" alt="Cadence Virtuoso"/>
  <img src="https://img.shields.io/badge/Synopsys-Sentaurus-19324d?style=for-the-badge" alt="Sentaurus"/>
  <img src="https://img.shields.io/badge/ModelSim-Simulation-19324d?style=for-the-badge" alt="ModelSim"/>
  <img src="https://img.shields.io/badge/Riviera--PRO-UVM_Simulation-19324d?style=for-the-badge" alt="Riviera-PRO"/>
</p>

---

### `08` / LIVE STATS

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=YokeshGaneshBabu&show_icons=true&hide_border=true&bg_color=070b14&title_color=00e5ff&icon_color=00e5ff&text_color=c9d1d9&ring_color=00e5ff" alt="GitHub stats"/>
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=YokeshGaneshBabu&layout=compact&hide_border=true&bg_color=070b14&title_color=00e5ff&text_color=c9d1d9" alt="Top languages"/>
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=YokeshGaneshBabu&theme=dark&hide_border=true&background=070b14&ring=00e5ff&fire=00e5ff&currStreakLabel=00e5ff&sideLabels=c9d1d9&currStreakNum=ffffff&sideNums=ffffff&dates=8b949e" alt="Streak stats"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=YokeshGaneshBabu&bg_color=070b14&color=00e5ff&line=00e5ff&point=ffffff&area=true&area_color=00e5ff&hide_border=true" alt="Contribution activity graph"/>
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=YokeshGaneshBabu&theme=onedark&no-frame=true&no-bg=true&margin-w=8&row=1&column=7" alt="Trophies"/>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/YokeshGaneshBabu/YokeshGaneshBabu/output/github-snake-dark.svg"/>
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/YokeshGaneshBabu/YokeshGaneshBabu/output/github-snake.svg" width="100%"/>
  </picture>
</p>

---

<p align="center">
  <a href="https://github.com/YokeshGaneshBabu?tab=repositories">
    <img src="https://img.shields.io/badge/EXPLORE_ALL_REPOSITORIES_↗-00e5ff?style=for-the-badge&logo=github&logoColor=070b14&labelColor=00e5ff" alt="Explore all repositories"/>
  </a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=120&section=footer&color=0:00e5ff,50:253b68,100:070b14&text=TRANSISTORS%20%E2%86%92%20LOGIC%20%E2%86%92%20SYSTEMS&fontColor=ffffff&fontSize=18&fontAlignY=70" width="100%" alt="Footer"/>
</p>
