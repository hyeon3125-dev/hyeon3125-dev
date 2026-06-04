<div align="center">

<img src="https://raw.githubusercontent.com/hyeon3125-dev/hyeon3125-dev/7109418d7ec4f7720e46157d2b40771b793817e8/assets/scalar/brand/scalar-lockup-vertical.png" width="160" alt="Scalar"/>

<br/><br/>

<!-- BENCHMARK: 출처 명시 -->
[![](https://img.shields.io/badge/⚡_Latency-10ms_vs_2082ms_(internal_bench_N=10)-F37021?style=for-the-badge&labelColor=111111)](https://mtp-l2-scalar.lovable.app)
[![](https://img.shields.io/badge/✓_Schema-100%25_compliance_(internal_bench_N=10)-F37021?style=for-the-badge&labelColor=111111)](https://mtp-l2-scalar.lovable.app)
[![](https://img.shields.io/badge/◈_Scale-46B_params_(vs_380B_legacy)-F37021?style=for-the-badge&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)

<br/>

[![](https://img.shields.io/badge/●_LIVE-SCALAR_FMS_24%2F7-F37021?style=flat-square&labelColor=111111)](https://fms.scalar-inc.com)
[![](https://img.shields.io/badge/Patent-10--2026--0084899-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/LKML_RFC-BPF_DAG_Verifier-F37021?style=flat-square&labelColor=111111&logo=linux&logoColor=white)](https://lkml.org)

<br/><br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/hyeon3125)
[![Demo](https://img.shields.io/badge/Request_Demo-F37021?style=for-the-badge&logoColor=white)](https://mtp-l2-scalar.lovable.app)
[![Portfolio](https://img.shields.io/badge/scalar--inc.com-111111?style=for-the-badge&logo=netlify&logoColor=F37021)](https://scalar-inc.com)
[![Email](https://img.shields.io/badge/l0architect@scalar--inc.com-111111?style=for-the-badge&logo=gmail&logoColor=F37021)](mailto:l0architect@scalar-inc.com)

</div>

---

```
Building infrastructure for deterministic AI orchestration,
financial anomaly detection, and verifiable automation.
Solo-built. Patent pending. Live in production.
```

**Seung-hyun Lee** — Founder, Scalar Inc. · Seoul, Korea · l0architect@scalar-inc.com

---

## Core Products

### [MTP-L2-mini](https://github.com/ScalarCore/MTP-L2-mini) — Deterministic AI Orchestration &nbsp;[![](https://img.shields.io/badge/LIVE-F37021?style=flat-square&labelColor=111111)](https://mtp-l2-scalar.lovable.app) [![](https://img.shields.io/badge/Patent_Pending-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)

Multi-LLM routing via schema-enforced DSL. The OS kernel for the LLM era — no hallucination leakage between layers.

| Metric | MTP-L2 | Legacy | Source |
|--------|:------:|:------:|:------:|
| Latency | **10ms** | 2,082ms | internal benchmark N=10 |
| Schema compliance | **100%** | 0% | internal benchmark N=10 |
| Payload | **46B** | 380B | internal benchmark N=10 |

**→ [Live Demo](https://mtp-l2-scalar.lovable.app)** · [Repo](https://github.com/ScalarCore/MTP-L2-mini)

---

### [SCALAR FMS](https://fms.scalar-inc.com) — Financial Market Intelligence &nbsp;[![](https://img.shields.io/badge/●_24%2F7_LIVE-F37021?style=flat-square&labelColor=111111)](https://fms.scalar-inc.com) [![](https://img.shields.io/badge/V8.1-GeminiTuner-111111?style=flat-square&labelColor=222222)](https://fms.scalar-inc.com)

Real-time BTC/USDT derivatives + on-chain + whale tracking. B2B SaaS, always-on Hetzner CPX32.

| | |
|---|---|
| **Demo** | [fms.scalar-inc.com](https://fms.scalar-inc.com) |
| **Stack** | Python 3.12 · Supabase · Bybit API · Telethon · React 18 |
| **Signal Engine** | Taker CVD · OI% · Funding · ATR · EMA · Whale Events ($10M+) |
| **Uptime** | 24/7 automated (PM2 · Hetzner CPX32) |
| **Version** | V8.1 — GeminiTuner 24h auto-tuning · ATR-linked TP/SL |

---

## Research

### [riemann_verify.c](https://github.com/hyeon3125-dev/riemann_verify) — BPF DAG Verifier &nbsp;[![](https://img.shields.io/badge/LKML_RFC-F37021?style=flat-square&labelColor=111111&logo=linux&logoColor=white)](https://lkml.org)

Kernel-level transfer functions for BPF DAG state verification. RFC submitted to Linux kernel mailing list.

```
Reviewer : Alexei Starovoitov  (BPF subsystem maintainer · Meta)
Reply    : 17 hours direct  ← third-party technical validation
Pathway  : merge_verifier_state() confirmed upstream
Language : C · eBPF
```

### [MTP_Popw](https://github.com/hyeon3125-dev/MTP_Popw) — Proof of Physical Work &nbsp;[![](https://img.shields.io/badge/MIT-555?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/MTP_Popw)

Monetary issuance anchored to verifiable physical energy. Unauthorized inflation structurally impossible.

```
Conservation: 100%  ·  False issuance blocked: 53.7%  ·  SNR +94.2%
```

---

## Open Source

### [Scalar ERP](https://github.com/ScalarCore/Scalar-ERP-v1.0) — Serverless MES on Google Sheets &nbsp;[![](https://img.shields.io/badge/MIT-555?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/Scalar-ERP-v1.0)

Full BOM/production tracking · 41 functions · Zero infrastructure cost.

### [sim_music_automation](https://github.com/hyeon3125-dev/sim_music_automation) — Cognitive Layer Simulation

Two-domain stress test: music industry vs. social discourse. When μ > 1.0, echo chamber lock-in is the rational response.

```
Cross-domain Δβ: +0.141 / +0.135  ·  Music golden-age: 8% ↓  ·  Social: 98% intact
```

---

## Trajectory

```
Month 2  →  Multi-LLM production system       FastAPI · pm2 · Tailscale VPN · Hetzner live
Month 4  →  LKML BPF DAG verifier RFC         Alexei Starovoitov · 17h direct reply
Month 6  →  7-project portfolio               patent pending · 24/7 live · funding track active
```

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=hyeon3125-dev&amp;show_icons=true&amp;theme=dark&amp;hide_border=true&amp;bg_color=0d1117&amp;title_color=F37021&amp;icon_color=F37021&amp;text_color=e8eaf0&amp;hide=contribs" height="130"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=hyeon3125-dev&amp;layout=compact&amp;theme=dark&amp;hide_border=true&amp;bg_color=0d1117&amp;title_color=F37021&amp;text_color=e8eaf0&amp;langs_count=6" height="130"/>

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=hyeon3125-dev&amp;bg_color=0d1117&amp;color=F37021&amp;line=F37021&amp;point=111111&amp;area=true&amp;hide_border=true" width="100%"/>

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![eBPF](https://img.shields.io/badge/eBPF-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=black)
![Hetzner](https://img.shields.io/badge/Hetzner-D50C2D?style=flat-square&logo=hetzner&logoColor=white)

<br/>

<img src="https://raw.githubusercontent.com/hyeon3125-dev/hyeon3125-dev/7109418d7ec4f7720e46157d2b40771b793817e8/assets/scalar/brand/scalar-corporate-identity.png" width="320" alt="Scalar Inc."/>

<br/><br/>

*Scalar Inc. · Seoul, Korea · 2026*

![](https://komarev.com/ghpvc/?username=hyeon3125-dev&color=F37021&style=flat-square&label=profile+views)

</div>
