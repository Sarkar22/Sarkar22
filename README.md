Digital hardware engineer. I write RTL in SystemVerilog, check it against a reference model, and take it through synthesis and place and route, on FPGAs (Xilinx Artix-7 and Zynq UltraScale+) and on the open sky130 ASIC flow.

### Processors

- **[hades-v-plus](https://github.com/Sarkar22/hades-v-plus)**: a five-stage RISC-V soft core, extended from TU Graz's HaDes-V teaching core to rv32imb with Zicond, Zicntr and the Zbkb, Zbkx and Zknh crypto extensions. It runs unmodified FreeRTOS with an interactive shell on a cycle-accurate Verilator model, and its multiply/divide and bit-manipulation units are proved by k-induction.

### Computer arithmetic and EDA tools

- **[sv-arith](https://github.com/Sarkar22/sv-arith)**: parametric structural adders and multipliers (unsigned; signed Baugh-Wooley and radix-4 Booth; FP8, bf16 and fp16 floating point), checked exhaustively at 8 bits and with corner and random vectors at 16 and 32, and placed and routed on sky130 in a 41-design area-delay sweep.
- **[gate-level-netlist-simulator](https://github.com/Sarkar22/gate-level-netlist-simulator)**: a gate-level simulator and static timing analyzer for Icarus Verilog netlists, with bit-parallel simulation and OpenSTA-style timing reports.
- **[espresso-minimizer](https://github.com/Sarkar22/espresso-minimizer)**: the ESPRESSO heuristic Boolean minimizer in Python, with structural Verilog export. Checked on every 3-variable function (with don't-cares) and every 4-variable function: 72,097 covers, none wrong.

### Hardware security and cryptography

- **[ascon-glitch-leakage](https://github.com/Sarkar22/ascon-glitch-leakage)**: a masked Ascon S-box that a zero-delay model calls secure leaks at first order in transistor-level SPICE on sky130. Three leakage models, TVLA, and DRC/LVS-clean layouts re-tested after parasitic extraction.
- **[shadow-lwe](https://github.com/Sarkar22/shadow-lwe)**: an LWE encryptor that expands its random mask on chip from a 128-bit seed with Ascon-XOF128, so the ciphertext of one bit shrinks from 2524 bytes to 20.
- **[zero-shadow-aead](https://github.com/Sarkar22/zero-shadow-aead)**: Ascon-AEAD128 whose key-and-nonce initialization runs during the previous inference, off the critical path.
- **[secure-edge-node](https://github.com/Sarkar22/secure-edge-node)**: an MLP inference node that CTR-encrypts its output with no added latency, because the keystream is computed during the inference, and uses exactly one DSP slice.
- **[cordic-activation](https://github.com/Sarkar22/cordic-activation)**: one multiplier-free CORDIC datapath for both tanh and sigmoid in Q2.12, bit-exact on all 16,384 input codes, with zero DSP slices and zero block RAM.
- **[simon-unroll-study](https://github.com/Sarkar22/simon-unroll-study)**: a SIMON128/128 core with a parametric round-unroll factor, verified at 15 settings; its throughput optimum is a plateau, not a peak.
- Classic cores: pipelined [AES](https://github.com/Sarkar22/aes) (128/192/256-bit keys) and [DES](https://github.com/Sarkar22/des-pipelined-verilog), and an iterative [SHA-256](https://github.com/Sarkar22/sha256).

### Tools

SystemVerilog, Verilog, Python · Verilator, Icarus Verilog, SymbiYosys · Vivado · OpenLane and OpenROAD on sky130 · ngspice
