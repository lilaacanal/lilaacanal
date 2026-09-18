## Hi, I'm Lea 👋

EIE student at Imperial College London · Functional Safety Engineering Intern at Arm · I build things at the hardware/software boundary — FPGAs, fault-tolerant systems, compilers, and real-time rendering pipelines.

---

### Tech stack
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-blue?style=flat-square)
![C/C++](https://img.shields.io/badge/C%2FC%2B%2B-purple?style=flat-square)
![Python](https://img.shields.io/badge/Python-teal?style=flat-square)
![RISC-V](https://img.shields.io/badge/RISC--V-grey?style=flat-square)
![Vivado](https://img.shields.io/badge/Vivado%2FPYNQ-orange?style=flat-square)
![AWS](https://img.shields.io/badge/AWS-coral?style=flat-square)
![MATLAB](https://img.shields.io/badge/MATLAB-crimson?style=flat-square)

---
### Projects I am working/have worked on:

| Project | Description | Stack |
|---|---|---|
| **8-Lane Analytic Ray Tracer** | Independent extension of a group FPGA renderer — rebuilt from scratch with fully analytic ray–box intersection to remove a shared-BRAM bottleneck, scaling 2→8 parallel lanes, closing a −15.7 ns timing violation, and hitting 489 fps on hardware (150–270× a single-core ARM reference) | SystemVerilog · Vivado |
| **FPGA Hybrid Renderer** | Team-built dual-mode real-time renderer for a Cornell-box scene — division-free voxel ray-marching preview and a Monte Carlo path tracer with soft shadows and global illumination, pipelined in custom Q16.8 fixed-point hardware at 75 MHz | SystemVerilog · Python |
| **Formula 2D** | Real-time 2-player racing game across three PYNQ boards (1 server + 2 clients) over UDP — owned the tile-based graphics renderer end-to-end, taking a 7.7 fps software prototype to a 10,000 fps-capable hardware pipeline | SystemVerilog · PYNQ · UDP |
| **RISC-V RV32I Processor** | 5-stage pipelined RV32I CPU — designed the memory subsystem, including a 2-way set-associative write-back cache with shadow registers to resolve write-miss data loss | SystemVerilog |
| **C90 → RISC-V Compiler** | Compiler built from scratch with Flex & Bison — a ~3,500-line hand-written AST/codegen layer supporting arrays, structs, pointers, and full control flow, verified against a public regression suite | C++ · Flex · Bison |

---

Currently at Arm: building FVP and gem5 fault-injection infrastructure and designing fault-tolerance mechanisms (ABFT, parameter redundancy) that cut vector-register SDCs by up to 99.4%.

Imperial College London · EIE Year 3 · Arm, Cambridge
