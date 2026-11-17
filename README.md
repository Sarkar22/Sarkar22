## Hi there 👋

I'm **Emon Sarkar**. I design digital hardware at the **University of Waterloo**, where I work on multicore RISC-V SoCs for real-time embedded systems.

I work from **RTL** to **bare-metal software**: RISC-V cores, SoC integration, computer arithmetic, and hardware for real-time systems and security. Where I can, I verify exhaustively or with formal proofs rather than with a handful of test vectors.

Also: I take designs all the way to layout. More than 40 of mine are placed and routed on sky130, DRC- and LVS-clean.

### 🧠 What I'm into
- RTL design and verification in SystemVerilog
- RISC-V cores and computer architecture
- SoC design: multicore, coherence, memory systems
- Embedded and real-time systems: bare metal, FreeRTOS, Linux
- Computer arithmetic: adders, multipliers, floating point
- Hardware security: side channels, masking, lightweight and post-quantum crypto

### 🏗️ Things I've built (selection)
- [**he-soc**](https://github.com/Rodolfo-Pellizzoni-Lab/he-soc): a quad-core CVA6 SoC with a coherent interconnect and a performance-monitoring architecture. I brought up its four cores, worked on the per-core event monitoring units and the central monitoring unit, and wrote much of its test suite.
- [**hades-v-plus**](https://github.com/Sarkar22/hades-v-plus): RISC-V core extended from TU Graz's HaDes-V to RV32IMB plus scalar crypto. Runs FreeRTOS; its arithmetic units are formally proved.
- [**sv-arith**](https://github.com/Sarkar22/sv-arith): parametric adders and multipliers, integer and floating point, with a 41-design area-delay sweep on sky130.
- [**ascon-glitch-leakage**](https://github.com/Sarkar22/ascon-glitch-leakage): a masked Ascon S-box that looks secure in a zero-delay model but leaks in transistor-level SPICE.
- [**shadow-lwe**](https://github.com/Sarkar22/shadow-lwe): post-quantum LWE encryptor that expands its mask on chip, for a 126x smaller ciphertext.
- [**gate-level-netlist-simulator**](https://github.com/Sarkar22/gate-level-netlist-simulator) and [**espresso-minimizer**](https://github.com/Sarkar22/espresso-minimizer): a small EDA toolkit for gate-level simulation, static timing and logic minimization.
- More: [**cordic-activation**](https://github.com/Sarkar22/cordic-activation), [**secure-edge-node**](https://github.com/Sarkar22/secure-edge-node), [**zero-shadow-aead**](https://github.com/Sarkar22/zero-shadow-aead) and [**simon-unroll-study**](https://github.com/Sarkar22/simon-unroll-study), plus classic [**AES**](https://github.com/Sarkar22/aes), [**DES**](https://github.com/Sarkar22/des-pipelined-verilog) and [**SHA-256**](https://github.com/Sarkar22/sha256) cores.
