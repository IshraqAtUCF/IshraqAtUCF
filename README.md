<img align="right" width="44" src="https://cdn.simpleicons.org/intel/0071C5" alt="Intel">

<h1 align="center">ISHRAQ TASHDID</h1>
<p align="center"><sub>PART NO. IT-1 · HUMAN-GRADE HARDWARE SECURITY RESEARCHER · PRELIMINARY DATASHEET, REV 2.6</sub></p>
<p align="center"><sub>All specifications self-reported and subject to change without notice, typically near conference deadlines.<a href="https://www.linkedin.com/in/ishraqtashdid">&#8203;</a></sub></p>

<p align="center">
  <a href="https://ishraqtashdid.com"><img alt="site" src="https://img.shields.io/badge/site-ishraqtashdid.com-1e2d5a?style=flat-square"></a>
  <a href="https://ishraqtashdid.com/cv.html"><img alt="cv" src="https://img.shields.io/badge/CV-download-c9a84c?style=flat-square"></a>
  <a href="mailto:tashdid.ishraq@gmail.com"><img alt="email" src="https://img.shields.io/badge/contact-email-30363d?style=flat-square"></a>
</p>

<table align="center">
<tr><td><b>Device type</b></td><td>Ph.D. candidate, Computer Engineering, University of Central Florida</td></tr>
<tr><td><b>Core function</b></td><td>LLM-assisted threat modeling · formal verification · chiplet authentication</td></tr>
<tr><td><b>Process history</b></td><td>BUET EEE &rarr; XCelerium (RISC-V verification) &rarr; UCF Hardware Security Lab</td></tr>
<tr><td><b>Current deployment</b></td><td>Intel Corp., XPU Security Research, Folsom, CA (summer 2026)</td></tr>
<tr><td><b>Root of trust</b></td><td>Dr. Sazadur Rahman, UCF (advisor)</td></tr>
</table>

<br>

### 1. General Description

The IT-1 is a single-core, human-grade security researcher, originally fabricated on BUET's
Electrical & Electronic Engineering process and now in extended characterization at the
University of Central Florida (Trustee's Doctoral Fellow · Future Faculty Laureate). The device
integrates an LLM-driven threat-modeling front-end with a formal-verification back-end, on-die
PUF-based authentication, and two years of production RISC-V verification history. It operates
across the hardware/firmware/software boundary, where field data confirms all the interesting
bugs live.

### 2. Features & Applications

<table>
<tr>
<td valign="top" width="55%">

**Features**
<ul>
<li>Native CWE / CVE / CAPEC decode; auto-compiles threat models into JasperGold-verified security properties</li>
<li>On-package PUF + MPC authentication, raw signatures never leave the device</li>
<li>Post-fabrication adaptive logic (eFPGA) for reverse-engineering and Trojan resistance</li>
<li>RL-based macro-placement coprocessor, reward-tuned on human design intuition</li>
<li>Hardened RISC-V / AXI / APB verification interfaces (UVM, cocotb)</li>
<li>Pin-compatible with whiteboards, napkins, and most flat surfaces</li>
</ul>

</td>
<td valign="top">

**Applications**
<ul>
<li>SoC security verification and sign-off</li>
<li>Chiplet / SiP supply-chain integrity</li>
<li>Peer review (external reviewer: ICCD 2025, HOST 2026)</li>
<li>Teaching & mentoring, two undergraduate co-processors integrated to date, since licensed to AMD and Northrop Grumman</li>
<li>Root-causing household appliances (see §7, Errata)</li>
</ul>

</td>
</tr>
</table>

### 3. Absolute Maximum Ratings

| Symbol | Parameter | Rating |
|---|---|---|
| `T_A` | Ambient operating temperature | Orlando, FL, no upper bound observed |
| `V_CAFF` | Caffeine supply | 2 cups sustained · 4 cups burst |
| `N_DL` | Concurrent paper deadlines | 2 nominal · 4 survived, not re-attempted |
| `t_TRUST` | Time to accept "it passed simulation" as proof | unbounded |

<sub>Stresses beyond those listed may cause permanent degradation. These are stress ratings only;
functional operation at these conditions is not implied, though it has been observed near major
conference deadlines.</sub>

### 4. Functional Blocks

| Block | Function | Silicon proof |
|---|---|---|
| `ATLAS` | Ingests CWE/CVE/CAPEC, auto-generates structured threat models for any SoC asset, and translates them into formal security properties | **DAC 2026** |
| `InterPUF` | Differential-delay PUF in the interposer fabric, evaluated under multi-party computation for chiplet authentication | **HOST 2026** |
| `ECOLogic` | Circular, obfuscated, adaptive logic via eFPGA-augmented SoCs | **ICCD 2025** |
| `SAFE-SiP` / `AuthenTree` | MPC-based distributed trust for heterogeneous SiPs | **GLSVLSI · PAINE 2025** |
| `BeyondPPA` | Human-inspired RL for reliability-aware macro placement | **MLCAD 2025, Best Paper Nominee** |

<sub>Full block-level documentation available on request.
An invited book chapter on LLMs for SoC design and security is currently in fabrication with collaborators at the University of Florida.</sub>

### 5. Performance Characteristics

| Parameter | Conditions | Min | Typ | Max |
|---|---|---|---|---|
| Known-CWE detection (`ATLAS`) | 3x HACK@DAC benchmark SoCs | -- | 39 / 48 | -- |
| Correct property generation | same | 82% | -- | -- |
| Area overhead (`InterPUF`) | reconfigurable interposer | -- | -- | 0.23% |
| Power overhead (`InterPUF`) | | -- | -- | 0.072% |
| ML modeling-attack accuracy vs. PUF | state-of-the-art adversary | -- | ~47%&sup1; | -- |
| Communication complexity (`AuthenTree`) | *n* chiplets | -- | O(log n) | -- |

<sub>&sup1; Indistinguishable from a coin flip. This is the specification, not a defect.</sub>

### 6. Revision History

| Rev | Period | Change summary |
|---|---|---|
| 0.9 | 2017-2022 | Initial fabrication, B.Sc. EEE, BUET. Basic functionality verified. |
| 1.0 | 2022-2023 | Production deployment at XCelerium: RISC-V ISA & system-level verification, AXI/APB bring-up. Discovered where the interesting bugs live; roadmap permanently revised. |
| 2.0 | 2024 | Migrated to UCF's Ph.D. process node. Trustee's Doctoral Fellowship (4-year) and Future Faculty Laureate designation fused at tapeout. |
| 2.1 | 2024-2025 | Undergraduate co-processor interface added. NSF travel grant (HOST 2025). |
| 2.5 | Feb 2026 | Field characterization: invited talks at the Intel AI Forum (Folsom, CA) and the 4th Florida Semiconductor Summit (Orlando, FL). |
| 2.6 | May-Aug 2026 | On allocation to Intel, XPU Security Research, Folsom, CA. **Current revision.** |

### 7. Errata

| ID | Description | Workaround |
|---|---|---|
| `ERR-001` | Device cannot fully explain a research result without drawing on something. | Provide whiteboard. Napkin acceptable in emergencies. |
| `ERR-002` | Internal clock scales with deadline proximity; PLL may overshoot at night. | None known. Characteristic of the process. |
| `ERR-003` | Applies assertion-based verification to household appliances described as "flaky." | Choose adjectives carefully within earshot of the device. |
| `ERR-004` | Refuses to treat "passed simulation" and "works in silicon" as the same claim. | None required. This is correct behavior. |

### 8. Ordering Information

| Part number | Package option | Availability |
|---|---|---|
| `IT1-RES` | Research collaboration / co-authorship | In stock |
| `IT1-TALK` | Invited talks, guest lectures | Lead time: one email |
| `IT1-IND` | Industry research & internships | On allocation |
| `IT1-BIB` | Citation, BibTeX format | Always in stock |

<p align="center">
  <a href="mailto:tashdid.ishraq@gmail.com">tashdid.ishraq@gmail.com</a> ·
  <a href="mailto:ishraq.tashdid@ucf.edu">ishraq.tashdid@ucf.edu</a> ·
  <a href="https://ishraqtashdid.com">ishraqtashdid.com</a>
</p>

<br>

<p align="center"><sub>This datasheet was written by the device under test. All parameters self-reported;
independent verification encouraged; peer reviewers, see §4.<a href="https://scholar.google.com/citations?user=gYcWmKYAAAAJ&hl=en">&#8203;</a></sub></p>
