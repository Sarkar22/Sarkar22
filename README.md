## Hi there 👋

I'm **Emon Sarkar**, a **PhD student** in computer hardware at the **University of Waterloo**.

I work from **RTL** to **Linux**: RISC-V cores, SoC integration, computer arithmetic and DSP hardware, and hardware for real-time systems and security. I've designed the digital core of a frequency-measurement SoC for MEMS sensors and worked on encryption hardware for implantable neurostimulators.

Also: I take designs all the way to layout. More than 40 of mine are placed and routed on sky130, DRC- and LVS-clean.

### 🧠 What I'm into
- RTL, ASIC and SoC design
- RISC-V cores and computer architecture
- HW/SW co-design and real-time systems
- Embedded systems: bare metal, FreeRTOS, Linux
- Computer arithmetic and DSP hardware
- Hardware security: side channels, masking, lightweight and post-quantum crypto

### 🔧 Research platform
- [**he-soc**](https://github.com/Rodolfo-Pellizzoni-Lab/he-soc): an open-source multicore RISC-V SoC from the PULP project, with CVA6 cores and a coherent interconnect. At Waterloo, I lead the team that develops it as our research platform: from four to eight cores, from bare metal to Linux 6.1, with performance-monitoring hardware and a test suite that runs in simulation, on bare metal and under Linux.

### 🏗️ Things I've built (selection)
- [**hades-v-plus**](https://github.com/Sarkar22/hades-v-plus): RISC-V core extended from TU Graz's HaDes-V to RV32IMB plus scalar crypto. Runs FreeRTOS; its arithmetic units are formally proved. Gold medal, RISC-V Community Challenge (TU Graz / The Linux Foundation).
- [**sv-arith**](https://github.com/Sarkar22/sv-arith): parametric adders and multipliers, integer and floating point, with a 41-design area-delay sweep on sky130.
- [**ascon-glitch-leakage**](https://github.com/Sarkar22/ascon-glitch-leakage): a masked Ascon S-box that looks secure in a zero-delay model but leaks in transistor-level SPICE.
- [**shadow-lwe**](https://github.com/Sarkar22/shadow-lwe): post-quantum LWE encryptor that expands its mask on chip, for a 126x smaller ciphertext.
- [**gate-level-netlist-simulator**](https://github.com/Sarkar22/gate-level-netlist-simulator) and [**espresso-minimizer**](https://github.com/Sarkar22/espresso-minimizer): a small EDA toolkit for gate-level simulation, static timing and logic minimization.
- More: [**cordic-activation**](https://github.com/Sarkar22/cordic-activation), [**secure-edge-node**](https://github.com/Sarkar22/secure-edge-node), [**zero-shadow-aead**](https://github.com/Sarkar22/zero-shadow-aead) and [**simon-unroll-study**](https://github.com/Sarkar22/simon-unroll-study), plus classic [**AES**](https://github.com/Sarkar22/aes), [**DES**](https://github.com/Sarkar22/des-pipelined-verilog) and [**SHA-256**](https://github.com/Sarkar22/sha256) cores.

### 🧰 Tools
- **Design and verification:** SystemVerilog, C, Python · Questa, Verilator, Icarus Verilog · Vivado, Vitis HLS
- **ASIC:** Synopsys VCS, Design Compiler · Cadence Xcelium, Virtuoso, Innovus · OpenLane, ngspice
- **Boards and systems:** VCU118, ZCU102, ZCU104, Kria KV260 · OpenSBI, Linux kernel modules
