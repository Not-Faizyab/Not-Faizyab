# Hey, I'm Faizyab 👋

**Systems Programmer · Security Researcher · Formal Verification**

I engineer low-level systems in **Rust** and **C++**, build offensive reconnaissance tooling, and investigate deterministic solver dynamics and edge-case vulnerabilities in production infrastructure.

---

### 🛡️ Security & Research Highlights

* **NASA Vulnerability Disclosure Program (VDP):** Identified and responsibly disclosed a security vulnerability on NASA infrastructure *(validated & currently in engineering remediation)*.
* **Deterministic CDCL SAT Solver Research:** Authored ***[Representation-Induced State Divergence in Deterministic CDCL SAT Solving](https://github.com/Not-Faizyab/CDCL-Trajectory-Sensitivity)*** — reviewed by **Prof. Dr. Armin Biere** *(Creator of CaDiCaL/Kissat)* and **Dr. Alexander Nadel** *(Principal Research Scientist, NVIDIA)*.

---

### 🔬 Featured Research: CDCL State Divergence

**[Representation-Induced State Divergence in Deterministic CDCL SAT Solving](https://github.com/Not-Faizyab/CDCL-Trajectory-Sensitivity)** · `C++` · `MiniSat 2.2.0`

Instrumented deterministic MiniSat in C++ to trace how syntactic representation changes (variable index permutations that preserve exact semantic equivalence) alter internal solver trajectories on Bounded Model Checking (BMC) instances:
* **Empirical Variance:** Demonstrated a **21.9x swing in decision counts** (`2,845` to `62,320` decisions vs. `49,726` baseline) across 100 variable permutations of a single BMC instance.
* **Mechanistic Trace:** Isolated two distinct divergence regimes—**immediate divergence** triggered by binary-heap index tie-breaking on identical VSIDS activity scores, and **delayed divergence** occurring after hundreds of aligned conflict cycles.

---

### ⚙️ Core Systems & Security Tooling

| Repository | Stack | Architecture & Focus |
| :--- | :--- | :--- |
| **[Breach](https://github.com/Not-Faizyab/Breach)** | `Rust` | Custom interpreted scripting language featuring a hand-written lexer/parser, runtime execution engine, concurrency primitives, and low-level networking sockets. |
| **[CDCL-Trajectory-Sensitivity](https://github.com/Not-Faizyab/CDCL-Trajectory-Sensitivity)** | `C++` | Custom MiniSat instrumentation harness logging VSIDS heap ordering, branching decisions, and conflict-clause divergence across CNF permutations. |
| **[Doomscan](https://github.com/Not-Faizyab/Doomscan)** / **[Doomscan-CLI](https://github.com/Not-Faizyab/Doomscan-CLI)** | `Python` · `FastAPI` · `React` | Full-stack and headless CLI attack-surface reconnaissance suite for automated subdomain enumeration, DNS mapping, and perimeter auditing. |
| **[Gavel](https://github.com/Not-Faizyab/Gavel)** | `JavaScript` | High-speed document indexing and intelligence platform for Model UN delegates, centralizing UN resolutions, treaty stances, and side-by-side bloc comparisons. |
| **[Rover](https://github.com/Not-Faizyab/Rover)** | `C++` · `ESP32-CAM` | Bare-metal embedded firmware for a 4x4 tactical recon rover featuring low-latency MJPEG video streaming and servo-actuated pan-tilt laser targeting. |

---

### 🧰 Technical Stack & Focus Areas

* **Languages & Runtimes:** `Rust` · `C++` · `Python` · `JavaScript` · `Bash`
* **Frameworks & Tooling:** `Burp Suite` · `MiniSat` · `FastAPI` · `React` · `Linux / WSL2`
* **Core Domains:** `Language Runtimes & Parsers` · `CDCL SAT Solvers & Formal Methods` · `Web Application Security` · `Attack-Surface Reconnaissance` · `Embedded Firmware (ESP32)`
