<div align="center">

<!-- ANIMATED SVG HEADER -->
<img src="https://readme-typing-svg.demolab.com?font=Space+Mono&size=13&duration=3000&pause=1000&color=00E5FF&center=true&vCenter=true&multiline=true&width=600&height=80&lines=SCALAR+%2F%2F+L0;Architecture%2C+not+features." alt="Scalar" />

<br/>

<!-- BENCHMARK BADGES -->
<img src="https://img.shields.io/badge/Latency-10ms_vs_2082ms-00E5FF?style=flat-square&labelColor=0d1117"/>
<img src="https://img.shields.io/badge/Schema-100%25_accuracy-00FF88?style=flat-square&labelColor=0d1117"/>
<img src="https://img.shields.io/badge/Scale-46B_params-7B61FF?style=flat-square&labelColor=0d1117"/>
<img src="https://img.shields.io/badge/Infra-24%2F7_live-00FF88?style=flat-square&labelColor=0d1117&logo=hetzner&logoColor=white"/>
<img src="https://img.shields.io/badge/LKML-Alexei_17h_reply-FF6F00?style=flat-square&labelColor=0d1117&logo=linux&logoColor=white"/>

<br/><br/>

<!-- LINK BADGES -->
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/hyeon3125)
[![MTP-L2 Demo](https://img.shields.io/badge/MTP--L2_Live_Demo-00E5FF?style=for-the-badge&logoColor=black)](https://mtp-l2-scalar.lovable.app)
[![Patent](https://img.shields.io/badge/Patent-Pending-FF6F00?style=for-the-badge)](https://github.com/ScalarCore/MTP-L2-mini)
[![Portfolio](https://img.shields.io/badge/scalar--dev.netlify.app-111?style=for-the-badge&logo=netlify&logoColor=00E5FF)](https://scalar-dev.netlify.app)

</div>

---

```
AI orchestration · financial anomaly detection · kernel-level verification
Solo-built. Patent pending. Live in production.
```

**Seung-hyun Lee** — Founder, Scalar Inc. · Seoul, Korea  
Building deterministic AI infrastructure at the intersection of LLM orchestration, FinTech, and kernel-level verification.

---

## Projects

<!-- MTP-L2 -->
<details open>
<summary><b>🔵 MTP-L2-mini — Deterministic AI Orchestration</b> &nbsp;<img src="https://img.shields.io/badge/LIVE-00FF88?style=flat-square"/> <img src="https://img.shields.io/badge/Patent_Pending-FF6F00?style=flat-square"/></summary>

<br/>

Multi-LLM routing via schema-enforced DSL. The OS kernel for the LLM era — no hallucination leakage between layers.

| Metric | MTP-L2 | Legacy |
|--------|--------|--------|
| Latency | **10ms** | 2,082ms |
| Schema accuracy | **100%** | 0% |
| Model scale | **46B** | 380B |

**→ [Live Demo](https://mtp-l2-scalar.lovable.app)** · [Repo](https://github.com/ScalarCore/MTP-L2-mini)

</details>

---

<!-- SCALAR FMS -->
<details>
<summary><b>🟢 SCALAR FMS — Financial Anomaly Detection</b> &nbsp;<img src="https://img.shields.io/badge/24%2F7_LIVE-00FF88?style=flat-square"/></summary>

<br/>

Real-time financial monitoring with autonomous anomaly detection. B2B SaaS, always-on Hetzner CPX32.

```
Uptime: 24/7  ·  Auto-recovery: enabled  ·  B2B ready
```

[Repo](https://github.com/hyeon3125-dev/scalar-fms)

</details>

---

<!-- riemann_verify.c -->
<details>
<summary><b>⬛ riemann_verify.c — BPF DAG Verifier · LKML RFC</b> &nbsp;<img src="https://img.shields.io/badge/LKML_RFC-7B61FF?style=flat-square&logo=linux&logoColor=white"/></summary>

<br/>

Kernel-level transfer functions for BPF DAG state verification. RFC submitted to Linux kernel mailing list.

```
Reviewer : Alexei Starovoitov  (BPF subsystem maintainer · Meta)
Reply    : 17 hours
Pathway  : merge_verifier_state() confirmed upstream
Language : C · eBPF
```

[Repo](https://github.com/hyeon3125-dev/riemann_verify)

</details>

---

<!-- Scalar ERP -->
<details>
<summary><b>🟡 Scalar ERP — Serverless MES on Google Sheets</b> &nbsp;<img src="https://img.shields.io/badge/MIT-gray?style=flat-square"/></summary>

<br/>

Full BOM/production tracking with 41 functions and shared utility layer. Zero infrastructure cost.

```
Functions: 41  ·  Infra cost: $0  ·  License: MIT
```

[Repo](https://github.com/ScalarCore/Scalar-ERP-v1.0)

</details>

---

<!-- sim_music_automation -->
<details>
<summary><b>🟠 sim_music_automation — Automation & Cognitive Layer Simulation</b></summary>

<br/>

Two-domain stress test across music industry and social discourse. When μ > 1.0, echo chamber lock-in is the rational response.

```
Cross-domain Δβ: +0.141 / +0.135  ·  Music golden-age: 8% ↓ collapse
Social golden-age: 98% intact (resistance mechanism confirmed)
```

[Repo](https://github.com/hyeon3125-dev/sim_music_automation)

</details>

---

<!-- MTP_Popw -->
<details>
<summary><b>🟣 MTP_Popw — Proof of Physical Work Simulation</b> &nbsp;<img src="https://img.shields.io/badge/MIT-gray?style=flat-square"/></summary>

<br/>

Monetary issuance anchored to verifiable physical energy. Unauthorized inflation structurally impossible — not just discouraged.

```
Conservation law: 100% pass  ·  False issuance blocked: 53.7%
SNR improvement: +94.2%  ·  CV improvement: +23.0%
```

[Repo](https://github.com/hyeon3125-dev/MTP_Popw)

</details>

---

<!-- Scalar Market Analyzer -->
<details>
<summary><b>⚪ Scalar Market Analyzer — Crypto Decision-Support Infrastructure</b></summary>

<br/>

Dual-layer engine: Gemini AI judge + OI-change fallback. FOMO Index (1–99) · 24/7 autonomous operation.

```
AI alignment: ~68%  ·  Fallback stability: >95%
FOMO/volatility r ≈ 0.43 (p<0.05)
```

[Repo](https://github.com/hyeon3125-dev/Scalar-Market-Analyzer)

</details>

---

## Trajectory

```
Month 2  →  Multi-LLM production system       FastAPI · pm2 · Tailscale VPN · live on Hetzner
Month 4  →  LKML BPF DAG verifier RFC         Alexei Starovoitov direct reply · 17h
Month 6  →  7-project portfolio               patent pending · 24/7 live · funding track active
```

---

<div align="center">

**Stack**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![eBPF](https://img.shields.io/badge/eBPF-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=black)
![Hetzner](https://img.shields.io/badge/Hetzner-D50C2D?style=flat-square&logo=hetzner&logoColor=white)

<br/>

*Scalar Inc. · Seoul, Korea · 2026*

![](https://komarev.com/ghpvc/?username=hyeon3125-dev&color=00e5ff&style=flat-square)

</div>
