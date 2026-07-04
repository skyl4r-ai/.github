<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/skyl4r-ai/skylar/main/docs/brand/skylar-logo-dark-2048.png">
  <img alt="SKYL4R" src="https://raw.githubusercontent.com/skyl4r-ai/skylar/main/docs/brand/skylar-logo-light-2048.png" width="500">
</picture>

<br><br>

# Sovereign AI specialists for the systems the world can't afford to break.

**Skyl4r builds proprietary, from-scratch vertical AI models.**
The first — **Skylar Cobol** — reads, explains, fixes and modernizes mission-critical legacy code
**without a single line ever leaving your infrastructure.**

*Legacy is the entry point, not the ceiling.*

[🌐 skyl4r.ai](https://skyl4r.ai) · [⚙️ The Framework](https://github.com/skyl4r-ai/skylar) · [🤗 Models](https://huggingface.co/collections/Sophia-AI/skylar)

</div>

---

### 🖥️ &nbsp; Skylar Cobol, at work

A rich-console workspace where the model reads, fixes and **verifies** mission-critical COBOL — on-prem, on a classic production failure:

```console
SKYLAR COBOL · SESSION 0847 · ON-PREM

USER>   Nightly batch INTFEE01 abends with SOC7 since the August release. Can you find why?

SKYLAR> Reading INTFEE01.cbl (1,214 lines) … done.
        The abend is a data exception in the COMPUTE at line 402:

          402   COMPUTE WS-FEE ROUNDED = WS-BAL * WS-RATE / 100

        WS-RATE is PIC S9(3)V99 COMP-3, loaded from RATE-FILE.
        The August release added rows where RATE is spaces —
        packed-decimal garbage → SOC7 on first arithmetic use.

        Proposed fix (behavior-preserving):
        +    IF WS-RATE NOT NUMERIC
        +        MOVE ZERO TO WS-RATE
        +        PERFORM 9000-LOG-RATE-WARN
        +    END-IF
             COMPUTE WS-FEE ROUNDED = WS-BAL * WS-RATE / 100

        ✓ cobc -fsyntax-only: 0 errors    ·    impact: 2 callers checked
```

|  |  |
|:--|:--|
| **📖 Reads the estate** | 40-year-old dialects, copybooks, packed decimal — explained in plain language. |
| **🧑‍💻 Fixes like a senior** | Behavior-preserving patches with impact analysis on every caller — not a generic guess. |
| **✅ Verifies before you ship** | Every answer checked against a **real COBOL compiler** before it gets near production. |

---

### 🧬 &nbsp; One startup, many models — COBOL is the first

|  | |
|:--|:--|
| **▸ Now · shipped** | **Skylar Cobol** — the COBOL specialist, live at [skyl4r.ai](https://skyl4r.ai). Open base models published & downloadable. |
| **▸ Next** | More legacy languages — **RPG · PL/I · HLASM · Natural** — same data pipeline, same buyers. |
| **▸ Later** | New sovereign verticals — regulated domains where generic cloud AI legally can't go. |

**Why COBOL first:** highest pain *(a retiring workforce on frozen, mission-critical systems)* · budgeted spend *(maintenance is already a line item)* · **zero sovereign rivals**.

---

### 🛠️ &nbsp; What we build

- 🧠 &nbsp;**From-scratch models** — our own weights, no third-party cloud, no lock-in. Trained on the open [**Skylar Framework**](https://github.com/skyl4r-ai/skylar) *(6M → 128B parameters, one codebase)*.
- 🔒 &nbsp;**Sovereign delivery** — on-premise / air-gapped. Your code never leaves the building. DORA-ready.
- ✅ &nbsp;**Compiler-verified** — COBOLEval-benchmarked, execution-checked. Not a wrapper around someone else's model.
- 🗣️ &nbsp;**A senior that never retires** — explains any program, extracts the real business rules, modernizes without rewriting.

<div align="center">

<br>

**Banking · Insurance · Government · Healthcare · Utilities · Logistics**
<sub>every industry that can't afford downtime runs on legacy code</sub>

<br>

*Built from first principles by **[Aleksandr Ivanovitch](https://www.linkedin.com/in/aleksandr-ivanovitch-brunelli)** — Founder & CEO.*

### **[→ See Skylar on your code · skyl4r.ai](https://skyl4r.ai)**

</div>
