## Hi, I'm Lea 👋

EIE student at Imperial College London · Functional Safety Engineering Intern at Arm · I build things at the hardware/software boundary — FPGAs, CPUs, compilers, low-latency systems, and everything in between.

---

### Tech stack
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-blue?style=flat-square)
![C/C++](https://img.shields.io/badge/C%2FC%2B%2B-purple?style=flat-square)
![Python](https://img.shields.io/badge/Python-teal?style=flat-square)
![OCaml](https://img.shields.io/badge/OCaml-amber?style=flat-square)
![RISC-V](https://img.shields.io/badge/RISC--V-grey?style=flat-square)
![Vivado](https://img.shields.io/badge/Vivado%2FPYNQ-orange?style=flat-square)
![POSIX](https://img.shields.io/badge/POSIX%2Fpthreads-slategray?style=flat-square)
![AWS](https://img.shields.io/badge/AWS-coral?style=flat-square)

---
### Projects I am working/have worked on:

| Project | Description | Stack |
|---|---|---|
| **NASDAQ ITCH 5.0 Feed Handler** | Streaming Ethernet/IPv4/UDP → MoldUDP64 → ITCH 5.0 decoder for FPGA, parsing headers in flight at 10G with no store-and-forward buffering — first field decoded 51.2 ns after SOF, top-of-book maintained for 1,024 symbols / 16K live orders, verified against ~250M messages of replayed public ITCH data | Hardcaml (OCaml) · Verilator · Vivado |
| **8-Lane Analytic Ray Tracer** | Independent rebuild of a group FPGA renderer — fully analytic ray–box intersection to remove a shared-BRAM bottleneck, scaling 2→8 parallel lanes, closing a −15.7 ns timing violation, and hitting 489 fps on hardware (150–270× a single-core ARM reference) | SystemVerilog · Vivado |
| **FPGA Hybrid Renderer** | Dual-mode real-time renderer for a Cornell-box scene — division-free voxel ray-marching preview and a Monte Carlo path tracer with soft shadows and global illumination, pipelined in custom Q16.8 fixed-point hardware at 75 MHz | SystemVerilog · Python |
| **Formula 2D** | Real-time 2-player racing game across three PYNQ boards over UDP — server-authoritative networking with per-player sequence validation, and a tile-based graphics renderer driven by 40 bytes of register writes per frame, taking 7.7 fps in software to 60 fps in hardware | Verilog · UDP · AWS · Python |
| **C90 → RISC-V Compiler** | Compiler built from scratch with Flex & Bison — ~2,600 lines lowering C90 to RV32IMFD assembly, with a scoped symbol table, `typedef` disambiguation, and structs/pointers/recursion/floats supported; passes all 86 public tests across 14 categories | C++ · Flex · Bison |
| **RISC-V RV32I Pipelined Processor** | 5-stage pipelined core with hazard detection and forwarding — owned integration and a 4 KB 2-way write-back cache, fixing a refill race with shadow registers and formally verifying the fix via model checking | SystemVerilog · Verilator · SymbiYosys |
| **Multithreaded UDP Chat Server** | Custom text protocol over a detached-thread-per-datagram server — broadcast/private messaging, mute lists, admin kicks, reader-writer locks, a circular buffer for message history, and a heartbeat thread for O(1) inactivity lookup with auto-eviction | C · pthreads · POSIX sockets |
| **Unix Shell** | Shell supporting N-stage pipelines, I/O redirection, `;` batches, `cd`/`cd -`, and arbitrarily nested subshells — depth-aware parser splits on operators outside parentheses, subshells isolated via re-exec | C · POSIX |
| **Autonomous Rover** | 3-wheeled rover with electromagnetic, infrared, ultrasound, and radio sensors — interrupt-driven real-time motor control plus a Wi-Fi web interface for live control and sensor visualization | C++ · Arduino |
| **Robot Arm via Mobile App** | 5-DOF robotic arm with Bluetooth control and a companion Android app (MIT App Inventor) supporting manual and automated step-recording modes | Arduino C++ · MIT App Inventor |

---

Currently at Arm: building FVP and gem5 fault-injection infrastructure and designing fault-tolerance mechanisms (ABFT, parameter redundancy) that cut vector-register and targeted model-parameter SDCs by ~99%.

Imperial College London · EIE Year 3 · Arm, Cambridge
