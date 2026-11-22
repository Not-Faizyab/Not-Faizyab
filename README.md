### Hey, I'm Faizyab
**Systems Programmer · Security Researcher · Formal Verification**

I engineer low-level systems in Rust and C++, build offensive reconnaissance tooling, and investigate deterministic solver dynamics and edge-case vulnerabilities in production infrastructure.

---

### Security & Research Highlights
* **NASA Vulnerability Disclosure Program (VDP):** Identified and responsibly disclosed a security vulnerability on NASA infrastructure *(validated & in engineering remediation)*.
* **Deterministic CDCL SAT Solver Research:** Authored *Representation-Induced State Divergence in Deterministic CDCL SAT Solving* — reviewed by **Prof. Dr. Armin Biere** *(Creator of CaDiCaL/Kissat)* and **Dr. Alexander Nadel** *(Principal Research Scientist, NVIDIA)*.
* **Upstream MaxSAT Solver Engineering:** Authored and merged a C++ clause-threshold optimization (`preprocesslightmaxclauses`) into [Aperture](https://github.com/Not-Faizyab/Aperture), validated across 386 MSE'26 benchmark instances.

---

### Featured Research: CDCL State Divergence
**`Representation-Induced State Divergence in Deterministic CDCL SAT Solving` · `C++` · `MiniSat 2.2.0`**

Instrumented deterministic MiniSat in C++ to trace how syntactic representation changes (variable index permutations preserving exact semantic equivalence) alter internal solver trajectories on Bounded Model Checking (BMC) instances:
* **Empirical Variance:** Demonstrated a **21.9x swing in decision counts** (`2,845` to `62,320` decisions vs. `49,726` baseline) across 100 variable permutations of a single BMC instance.
* **Mechanistic Trace:** Isolated two distinct divergence regimes—**immediate divergence** triggered by binary-heap index tie-breaking on identical VSIDS activity scores, and **delayed divergence** occurring after hundreds of aligned conflict cycles.

---

### Core Systems & Security Tooling

| Repository | Stack | Architecture & Focus |
| :--- | :--- | :--- |
| **Breach** | `Rust` | Custom interpreted language and runtime with a hand-written lexer/parser, concurrency primitives, and **native HTTP/1.1 CL.0 request smuggling / desync** network sockets. |
| **CDCL-Trajectory-Sensitivity** | `C++` | Custom MiniSat instrumentation harness logging **VSIDS heap ordering**, branching decisions, and conflict-clause divergence across CNF permutations. |
| **Doomscan / Doomscan-CLI** | `Python · FastAPI · React` | Full-stack and headless CLI **attack-surface reconnaissance suite** for automated subdomain enumeration, DNS mapping, and perimeter auditing. |
| **Rover** | `C++ · ESP32-CAM` | Bare-metal embedded firmware for a 4x4 tactical recon rover featuring **low-latency MJPEG streaming** and servo-actuated pan-tilt laser targeting. |
| **Gavel** | `JavaScript` | High-speed **document indexing and corpus comparison engine** centralizing UN resolutions, treaty stances, and side-by-side bloc analysis. |

---

### Technical Stack & Focus Areas
* **Languages & Runtimes:** `Rust` · `C++` · `Python` · `JavaScript` · `Bash`
* **Frameworks & Tooling:** `Burp Suite` · `CaDiCaL / MiniSat` · `FastAPI` · `React` · `Linux / WSL2`
* **Core Domains:** Language Runtimes & Parsers · CDCL/MaxSAT Solvers & Formal Methods · Web Application Security · Attack-Surface Recon · Embedded Firmware (ESP32)

---

**Contact:** `notfaizyab@gmail.com` · [All Repositories](https://github.com/Not-Faizyab?tab=repositories)
