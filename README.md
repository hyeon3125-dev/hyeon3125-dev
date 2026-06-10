<div align="center">

<img src="https://raw.githubusercontent.com/hyeon3125-dev/hyeon3125-dev/7109418d7ec4f7720e46157d2b40771b793817e8/assets/scalar/brand/scalar-lockup-vertical.png" width="160" alt="Scalar"/>

<br/><br/>

<!-- BENCHMARK: 재현 가능한 공정 벤치 (kibo_fair_test.py, N=2000) -->
[![](https://img.shields.io/badge/🛡️_Safety-100%25_bounds--safe_vs_~75%25_raw-F37021?style=for-the-badge&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/✓_Schema-100%25_conform_by_construction-F37021?style=for-the-badge&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/◈_Output-normalized_to_fixed_command-F37021?style=for-the-badge&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)

<br/>

[![](https://img.shields.io/badge/●_LIVE-SCALAR_FMS_24%2F7-F37021?style=flat-square&labelColor=111111)](https://fms.scalar-inc.com)
[![](https://img.shields.io/badge/Patent_①_Routing-10--2026--0105850-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/Patent_②_Execution-10--2026--0084899-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/LKML_RFC-BPF_DAG_Verifier-F37021?style=flat-square&labelColor=111111&logo=linux&logoColor=white)](https://lore.kernel.org/bpf/178004391665.3522.4865582628003357086@gmail.com/T/#u)

<br/><br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/hyeon3125)
[![Demo](https://img.shields.io/badge/Request_Demo-F37021?style=for-the-badge&logoColor=white)](https://mtp-l2-scalar.lovable.app)
[![Portfolio](https://img.shields.io/badge/scalar--inc.com-111111?style=for-the-badge&logo=netlify&logoColor=F37021)](https://scalar-inc.com)
[![Email](https://img.shields.io/badge/l0architect@scalar--inc.com-111111?style=for-the-badge&logo=gmail&logoColor=F37021)](mailto:l0architect@scalar-inc.com)

</div>

---

```
Scalar develops deterministic AI orchestration systems
for enterprise-grade automation and robotics.
Solo-built. 2-Layer patent (filed). Live in production.
```

**Seung-hyun Lee** — Founder, Scalar Inc. · Seoul, Korea · l0architect@scalar-inc.com

---

## Core Products

### [MTP-L2-mini](https://github.com/ScalarCore/MTP-L2-mini) — Deterministic AI Orchestration &nbsp;[![](https://img.shields.io/badge/LIVE-F37021?style=flat-square&labelColor=111111)](https://mtp-l2-scalar.lovable.app) [![](https://img.shields.io/badge/Patent_Pending-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)

A deterministic layer between the LLM and the executor: tokenize → validate → clamp → compile. Every downstream command is schema-conform and within physical bounds **by construction** — not by hoping the model behaves.

**Patents (KR, filed):**
- Routing Layer — KR 10-2026-0105850 (reasoning-profile vector routing)
- Execution Layer — KR 10-2026-0084899 (DSL parser-verified execution)

```
Input → [Routing Layer (patent ①)] → [Execution Layer (patent ②)] → Verified Output
```

Pipeline routing and execution are patented as separate layers — bypassing one infringes the other.

| Metric | MTP-L2 | Raw LLM output | Source |
|--------|:------:|:------:|:------:|
| Bounds-safe & schema-conform | **100%** | ~75% | fair bench N=2000 |
| Correct vs intent | **~91%** | ~75% | fair bench N=2000 |
| Output payload | **~53 B (fixed)** | 25–86 B (varies) | fair bench N=2000 |
| Parse overhead | ~7 µs | ~4 µs | LLM call paid by both paths |

*Fair benchmark: identical fuzzed input to both paths, reproducible offline (`python kibo_fair_test.py`). MTP-L2's edge is determinism & safety — not latency.*

**→ [Repo + benchmark](https://github.com/ScalarCore/MTP-L2-mini)** · [Live Demo](https://mtp-l2-scalar.lovable.app)

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

### Music Forensics — AI Music Copyright Evidence &nbsp;[![](https://img.shields.io/badge/B2B-F37021?style=flat-square&labelColor=111111)](https://scalar-inc.com) [![](https://img.shields.io/badge/Portfolio-111111?style=flat-square&labelColor=222222)](https://scalar-inc.com)

Hybrid audio similarity engine for AI music copyright disputes: math core + reverse-tracking + a second-stage filter, producing forensic reports for B2B legal use.

| | |
|---|---|
| **Engine** | Chroma Roll · fastDTW · HPSS (numerical similarity) |
| **Pipeline** | FAISS reverse-tracker → second-stage filter → forensic report |
| **Stack** | Python 3.12 · FastAPI · FAISS · Supabase |
| **Target** | Music-specialized law firms · AI-music copyright proof |

---

## Research

### [riemann_verify.c](https://github.com/hyeon3125-dev/riemann_verify) — BPF DAG Verifier &nbsp;[![](https://img.shields.io/badge/LKML_RFC-F37021?style=flat-square&labelColor=111111&logo=linux&logoColor=white)](https://lore.kernel.org/bpf/178004391665.3522.4865582628003357086@gmail.com/T/#u) [![](https://img.shields.io/badge/LWN-Coverage-F37021?style=flat-square&labelColor=111111)](https://lwn.net/SubscriberLink/1075067/6e0bbea2010794b8/)

Kernel-level transfer functions for BPF DAG state verification. RFC submitted to Linux kernel mailing list.

```
Reviewer : Alexei Starovoitov  (BPF subsystem maintainer · Meta)
Reply    : 17 hours direct  ← third-party technical validation
Pathway  : merge_verifier_state() confirmed upstream
Language : C · eBPF
```

**→ [LKML 스레드](https://lore.kernel.org/bpf/178004391665.3522.4865582628003357086@gmail.com/T/#u)** `2026-05-30` &nbsp;·&nbsp; **[LWN Coverage](https://lwn.net/SubscriberLink/1075067/6e0bbea2010794b8/)** `2026-06-03`

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
Month 6  →  7-project portfolio               2-layer patent filed · 24/7 live · funding track active
```

---

<div align="center">

<img src="https://github-readme-stats-lemon-one-13.vercel.app/api?username=hyeon3125-dev&amp;show_icons=true&amp;theme=dark&amp;hide_border=true&amp;bg_color=0d1117&amp;title_color=F37021&amp;icon_color=F37021&amp;text_color=e8eaf0&amp;hide=contribs&amp;v=2" height="130"/>
&nbsp;
<img src="https://github-readme-stats-lemon-one-13.vercel.app/api/top-langs/?username=hyeon3125-dev&amp;layout=compact&amp;theme=dark&amp;hide_border=true&amp;bg_color=0d1117&amp;title_color=F37021&amp;text_color=e8eaf0&amp;langs_count=6&amp;v=2" height="130"/>

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
