<!-- ═══════════════════════════════════════════════════════════
     hyeon3125-dev · GitHub Profile README
     Copy as-is → hyeon3125-dev/hyeon3125-dev/README.md
     ═══════════════════════════════════════════════════════════ -->

<div align="center">

```
 ░▒▓███████▓▒░  ░▒▓██████▓▒░  ░▒▓██████▓▒░  ░▒▓█▓▒░       ░▒▓██████▓▒░  ░▒▓███████▓▒░
░▒▓█▓▒░        ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░      ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░
░▒▓█▓▒░        ░▒▓█▓▒░       ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░      ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░
 ░▒▓██████▓▒░  ░▒▓█▓▒░       ░▒▓████████▓▒░░▒▓█▓▒░      ░▒▓████████▓▒░ ░▒▓██████▓▒░
       ░▒▓█▓▒░░▒▓█▓▒░       ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░      ░▒▓█▓▒░░▒▓█▓▒░       ░▒▓█▓▒░
       ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░      ░▒▓█▓▒░░▒▓█▓▒░       ░▒▓█▓▒░
░▒▓███████▓▒░  ░▒▓██████▓▒░  ░▒▓█▓▒░░▒▓█▓▒░░▒▓████████▓▒░░▒▓█▓▒░░▒▓█▓▒░░▒▓███████▓▒░
```

**Deterministic AI Orchestration · Financial Anomaly Detection · Kernel-level Systems**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/hyeon3125)
[![Demo](https://img.shields.io/badge/MTP--L2_Demo-live-brightgreen?style=flat-square)](https://mtp-l2-scalar.lovable.app)
[![Patent](https://img.shields.io/badge/Patent-Pending-orange?style=flat-square)](https://github.com/ScalarCore/MTP-L2-mini)
[![LKML](https://img.shields.io/badge/LKML-BPF_DAG_RFC-blueviolet?style=flat-square)](https://lkml.org)

</div>

---

## Architecture, not features.

> *"LLMs are powerful. Uncontrolled, they hallucinate. Controlled deterministically, they scale."*

I build systems at the intersection of **AI orchestration**, **financial infrastructure**, and **kernel-level verification** — solo, from scratch, in production.

---

## Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux_Kernel-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![BPF](https://img.shields.io/badge/eBPF-EE0000?style=for-the-badge&logo=linux&logoColor=white)
![Hetzner](https://img.shields.io/badge/Hetzner-D50C2D?style=for-the-badge&logo=hetzner&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Apps_Script-34A853?style=for-the-badge&logo=google&logoColor=white)

</div>

---

## Projects

### 🔴 [MTP-L2-mini](https://github.com/ScalarCore/MTP-L2-mini) — Deterministic AI Orchestration Layer
> *"The OS kernel for the LLM era"*

Multi-LLM routing with schema-enforced determinism. No hallucination leakage between layers.

```
Benchmark vs Legacy orchestration
─────────────────────────────────
Latency     :  10ms      ←  vs 2,000ms+   (200× faster)
Schema acc. :  100%      ←  vs ~60-80%
Model scale :  46B param routing confirmed
```

**[→ Live Demo](https://mtp-l2-scalar.lovable.app)** · Patent pending · Production-ready

---

### 🟡 [SCALAR FMS](https://github.com/hyeon3125-dev/scalar-fms) — Financial Anomaly Detection
> 24/7 live on Hetzner CPX32

Real-time financial monitoring with autonomous anomaly detection. B2B SaaS, always-on.

---

### 🟢 [Scalar ERP](https://github.com/ScalarCore/Scalar-ERP-v1.0) — Serverless MES on Google Sheets
> MIT Licensed · Zero infrastructure cost

Google Apps Script–based Manufacturing Execution System. 41 functions, shared utility layer, full BOM/production tracking — no backend required.

---

### 🔵 [MTP-riemann-z-explorer](https://github.com/hyeon3125-dev/MTP-riemann-z-explorer) — Runtime Non-Refutation Verifier
> C · Gödel · Chaitin · Landauer · Bekenstein

The Riemann Hypothesis has never been proved. It has never been disproved.

This repo argues — and demonstrates in C — that **runtime non-refutation is not a consolation prize. Under Gödel incompleteness and Landauer's thermodynamic constraints, it is the optimal available verification strategy.**

```
Stage 1  →  29 zeros located,  t ∈ [14.5, 98.9]
Stage 2  →  27/29 CONFIRMED on critical line (|Z| < 1e-6)
Stage 3  →  entropy cost per marginal zero: ~1.84e-19 J
Off-critical-line zeros detected: 0
```

*Proof may be structurally unavailable. This is the next best thing.*

---

### ⚪ [Scalar Market Analyzer](https://github.com/hyeon3125-dev/Scalar-Market-Analyzer) — Crypto Decision-Support Infrastructure
> Python · Gemini 1.5 Pro · Bybit + Coinglass APIs

Real-time BTC market intelligence system. Dual-layer engine: primary AI judge (Gemini) + OI-change fallback. FOMO Index (1–99) quantifies market sentiment. 24/7 autonomous operation, graceful fallback on API failure.

```
AI decision alignment  :  ~68% (500-interval validation)
Fallback stability     :  >95% API reliability
FOMO/volatility corr.  :  r ≈ 0.43 (p<0.05, rolling 24h)
```

*Decision support only. No trade execution.*

---

### 🟣 [MTP_Popw](https://github.com/hyeon3125-dev/MTP_Popw) — Proof of Physical Work: Numeric Consistency Simulation
> Python · MIT · Agent-based simulation

Stress-tests whether a **Proof of Physical Work** monetary issuance model is numerically consistent — and where it breaks.

Core claim: anchoring token issuance to verifiable physical energy expenditure makes unauthorized inflation structurally impossible — not just economically discouraged.

```
Value = Spec Complexity × Vision Check (0|1) × Energy Filter f(Work)
        ↑ reward size      ↑ output correct?   ↑ anti-forgery gate
```

```
Phase A  →  Conservation law Σ issued ≡ Σ(verified × spec)   ✅ 100% pass (0 violations)
Phase B  →  Attack resistance: padding / collusion / Sybil    ✅ 53.7% false issuance blocked
Phase C  →  Dynamic E_min calibration + transition attack     ✅ 0 oscillations, 0 bootstrap contamination
Phase D  →  Inflation filter: uniform ×2, non-uniform ×5     ✅ CV +23.0%, SNR +94.2%
Phase E  →  Parameter sensitivity sweep                       inflation intensity = most sensitive variable
```

*Open problem: self-certifying Spec — robotic sensor closure closes the governance loop.*

---

### ⬛ [riemann_verify.c](https://github.com/hyeon3125-dev/riemann_verify) — BPF DAG Verifier
> LKML RFC · Reviewed by Alexei Starovoitov (BPF maintainer, 17h reply)

Kernel-level BPF verifier extension implementing transfer functions for DAG state verification. `merge_verifier_state()` integration pathway confirmed upstream.

```c
// riemann_verify.c · thermal_controller.c · Makefile · README
// Math + Implementation + Production — vertical stack
```

---

## Trajectory

```
Month 2  →  Multi-LLM production system (FastAPI + pm2 + Tailscale VPN)
Month 4  →  LKML BPF DAG verifier RFC · Alexei Starovoitov direct reply (17h)
Month 6  →  6-project portfolio · patent pending · 24/7 live infra · funding track active
```

Solo-built. Patent pending. Live in production.  
Funding track active — 2026.

---

## Contact

**Business / B2B inquiries** → LinkedIn  
**Technical collaboration** → Issues / PRs welcome

<div align="center">

*Scalar Inc. · Seoul, Korea · Est. 2026*

![Profile views](https://komarev.com/ghpvc/?username=hyeon3125-dev&color=blueviolet&style=flat-square)

</div>
