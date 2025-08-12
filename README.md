# 32-bit Pipelined Wallace Tree Multiplier

## Overview
This project implements a high-speed 32-bit pipelined Wallace Tree multiplier in Verilog to improve throughput and reduce critical path delay compared to conventional multipliers.  
The design was synthesized, implemented, and analyzed using Xilinx Vivado, achieving excellent timing and power performance.  
It is suitable for high-speed DSP and AI workloads requiring efficient multiplication.

---

## Architecture
- Wallace Tree Structure: Minimizes partial product reduction delay using parallel carry-save adders.
- Pipelining: Multiple pipeline stages are inserted to balance delay and increase clock frequency.
- Final Stage Adder: Carry Lookahead Adder (CLA) used for final sum computation.
- Simulation & Verification: Functional verification performed using self-checking testbench.

Data Flow:
1. Partial product generation from input operands.
2. Reduction using carry-save adders in a tree structure.
3. Pipelined registers inserted between stages.
4. Final addition to produce 32-bit result.

---

## Features
- Fully pipelined architecture for high-speed operation.
- Positive timing slack: **3.262 ns**.
- Low power consumption: **0.189 W**.
- Synthesized and implemented on **Xilinx Artix-7 FPGA**.
- Optimized for both speed and area.

---

## Tools & Technologies
- Verilog HDL
- Xilinx Vivado 2023.1 (Synthesis, Implementation, STA)
- FPGA: Xilinx Artix-7
- Static Timing Analysis

---

## Results
- Timing Performance: Positive slack of 3.262 ns.
- Power Analysis: 0.189 W total power consumption.
- Resource Utilization(from Vivado Report):
  - LUTs: [Add number]
  - FFs: [Add number]
  - DSPs: [Add number]
- Clock Frequency: [Add frequency from report].


## Simulation & Testing
- Verified functionality with exhaustive test cases in Vivado Simulator.
- Compared simulation outputs with reference C model for accuracy.
- Observed waveform to confirm correct pipelined data propagation.

## Publication
Published in IEEE BIDA SCRS 2025 – Springer (Scopus Indexed).  
[Publication Link](#) *(Add the IEEE or Springer link if available)*

## Applications
- Digital Signal Processing (DSP)
- AI and Machine Learning accelerators
- Cryptography hardware implementations
- High-speed arithmetic units in processors


## Author
Eresh  
M.Tech in VLSI Design & Embedded Systems – RV College of Engineering  
[LinkedIn](https://linkedin.com/in/eresh-g-k-b97532244) | [GitHub](https://github.com/eresh-vlsi)
<img width="556" height="663" alt="Screenshot 2025-02-16 191527" src="https://github.com/user-attachments/assets/7c1f1a93-e8dd-4fd7-8ae0-122d9cf99899" />
