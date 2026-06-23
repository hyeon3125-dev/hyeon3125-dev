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
Scalar builds the verification layer for AI execution —
deterministic systems that prove an action is safe *before* it runs.
Solo-built. 2-Layer patent (filed). Live in production.
```

**Seung-hyun Lee** — Founder, Scalar Inc. · Seoul, Korea · l0architect@scalar-inc.com

Orchestration, finance, copyright, kernel verification — every project answers one question: **can you trust the result of an execution?** Verify before you trust.
<br><sub>오케스트레이션·금융·저작권·커널 검증 — 모든 프로젝트가 답하는 하나의 질문: 실행 결과를 신뢰할 수 있는가. 신뢰하기 전에 검증한다.</sub>

---

## Background

```
R&D  →  Korea's largest manufacturing floors (Hyundai · Kia)  →  overseas auto production line (full-lot quality inspection)  →  ERP · logistics · CS  →  independent development  →  2 patents · LKML · open source
```

Across every floor — domestic and overseas, from R&D through quality, logistics, and customer support — the same problem kept surfacing: *how do you trust the result of an execution?* Scalar is the answer, built from that floor up.
<br><sub>국내 최대 제조현장(현대·기아)부터 해외 생산라인 품질 전수검사, ERP·물류·CS까지 — 전 공정에서 반복적으로 만난 단 하나의 질문: 실행 결과를 어떻게 신뢰하는가. 스칼라는 그 현장에서 출발한 답이다.</sub>

---

## Why Verification — Where the Market Is Moving

Enterprises don't stall on AI because the models are weak. They stall because **no one can prove what an action did** — so every AI action carries a *trust cost*: human review, audit, rollback, liability. Verification removes that cost. It is the layer that turns an impressive demo into something deployable in production — and the spend is moving from "a better model" to "an action you can prove."
<br><sub>AI 도입이 막히는 건 모델이 약해서가 아니라 "무엇을 실행했는지 증명할 수 없어서"다 — 검토·감사·롤백·책임이라는 **신뢰비용**. 검증은 그 비용을 제거해 데모를 프로덕션으로 바꾼다. 자본은 "더 좋은 모델"에서 "증명 가능한 실행"으로 이동 중.</sub>

| | Signal | Source |
|---|---|---|
| **Market** | AI orchestration **$11.0B (2025) → $30.2B (2030), 22.3% CAGR** · agentic orchestration **$6.3B → $46.8B by 2036, 22.1% CAGR** — shift from chat assistants to *governed* automation with audit trails | MarketsandMarkets · Fortune Business Insights · Fact.MR |
| **Capital** | Arcade.dev raised **$60M Series A** (SYN Ventures lead; $72M total) for a "secure action layer" — the verification/execution-control category is now funded | BusinessWire · WSJ `2026-06` |
| **Academia** | AGI-premise collapse → per-domain verification *harness* becomes mandatory, not optional | LeCun et al. — [arXiv:2602.23643](https://arxiv.org/abs/2602.23643) |
| **Governance** | Typed Planning → DAG → Validation Gate → Audit Trail as the enterprise pattern | POLARIS — [arXiv:2601.11816](https://arxiv.org/abs/2601.11816) |
| **The gap** | "Capability–Deployment **Verification Gap**" — *built ≠ trustable* | [arXiv:2605.14675](https://arxiv.org/abs/2605.14675) |
| **Product entry** | Sakana AI ships Fugu multimodel orchestration commercially — the category is real | `2026-06` |

> *"Agents don't fail in production because the model is wrong. They fail because no one can prove what an agent did."* — Alex Salazar, Arcade.dev CEO

**Where Scalar sits** — the execution-guarantee layer, not another framework:

```
L1  Orchestration   LangChain · CrewAI       connect models & tools          →  complement
L2  Guardrails      Guardrails AI · NeMo     output format / schema check     →  adjacent
L3  Deterministic   SCALAR MTP-L2            prove constraints BEFORE run     →  Scalar
    execution                                · reproduce · audit                 2-layer patent
```

Scalar is the only one combining a **deterministic L3 guarantee** with multimodel routing, a 2-layer patent, and **kernel-level external validation** (LKML). Same direction as the funded capital, the frontier papers, and Linux-kernel verifier research — already shipped as patents and a live service.
<br><sub>L1 연결·L2 형식검증이 못 푸는 "실행 전 결정론적 보장(L3)"을 멀티모델 라우팅·2-레이어 특허·커널 외부검증과 결합한 유일 포지션 — 자본·학술 최전선·커널 검증 연구와 같은 방향을 이미 특허·라이브 서비스로 구현.</sub>

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

### [SCALAR: NODE ZERO](https://github.com/hyeon3125-dev/snz-novel) — Deterministic Interactive Novel &nbsp;[![](https://img.shields.io/badge/Open_IP-F37021?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/snz-novel) [![](https://img.shields.io/badge/CC_BY--NC--SA_·_PolyForm_NC-555?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/snz-novel/blob/main/LICENSE-CONTENT.md)

A complete 16-volume psychological-SF novel released as an open-source interactive novel — the deterministic philosophy applied to storytelling: same choices, same story, every time. No AI, no server, no build, zero runtime dependencies. The full manuscript ships in the repo; non-commercial culture is free, commercial use is licensed.
<br><sub>완결 심리 SF 장편을 오픈소스 인터랙티브 노벨로 공개 — 비영리 향유는 자유, 상업적 이용(출판·굿즈·영상화)은 라이선스.</sub>

| | |
|---|---|
| **Play / Read** | [hyeon3125-dev.github.io/snz-novel](https://hyeon3125-dev.github.io/snz-novel/) · manuscript in-repo |
| **Scale** | 16 vols · 200 chapters + 46 side stories · 1,366 scenes · 11,608 lines (verbatim-verified by CI) |
| **Engine** | Vanilla JS 5-layer · 6 gesture interactions · 7 viewpoint text-grammars · procedural Web Audio |
| **Model** | Content CC BY-NC-SA 4.0 + commercial licensing & merch · **Engine PolyForm Noncommercial** (free for noncommercial authors, commercial licensed) |

---

### [차이 — 단편집](https://github.com/hyeon3125-dev/hyeon3125-dev-scalar-shorts) — Deterministic Short Stories &nbsp;[![](https://img.shields.io/badge/Open_IP-F37021?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/hyeon3125-dev-scalar-shorts) [![](https://img.shields.io/badge/CC_BY--NC--SA_·_PolyForm_NC-555?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/hyeon3125-dev-scalar-shorts)

Four short stories (비효율 · 기억 라우터 · 차이 · 입술의 무게) running on the **same SNZ 5-layer engine** — proof the engine is a reusable noncommercial substrate any author can build their own interactive novel on. Korean · English · Japanese, with theme-native interactions (silence as record, manipulated choice, refrains as echo).
<br><sub>SNZ 엔진을 그대로 재사용한 결정론 단편집 — 엔진은 비영리 작가 누구나 자기 작품에 쓸 수 있는 토대(PolyForm Noncommercial). 한·영·일 3개 언어.</sub>

| | |
|---|---|
| **Play / Read** | hyeon3125-dev.github.io/hyeon3125-dev-scalar-shorts · manuscript in-repo |
| **Engine** | shared SNZ 5-layer core — PolyForm Noncommercial (free for noncommercial use) |
| **Model** | Content CC BY-NC-SA 4.0 · Engine PolyForm Noncommercial |

---

## Research

### [MTP-MetaEval](https://github.com/hyeon3125-dev/MTP-MetaEval) — Verification Efficiency under Bounded Risk &nbsp;[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20806118-F37021?style=flat-square&labelColor=111111)](https://doi.org/10.5281/zenodo.20806118)

A cross-domain study of *when verification should stop* — the methodology behind the deterministic-verification work, made falsifiable. A non-refutation overhead boundary with a **provable risk bound** (`miss_rate ≤ ε`), and one *assumed-not-earned* law tested across number theory, control, statistics, and LLM evaluation. Pre-registered; reports its own negative results. Published preprint (CERN Zenodo, DOI).
<br><sub>검증을 언제 멈춰야 하는가 — 비반증 오버헤드 경계의 위험 한계 증명과 *assumed-not-earned* 법칙. 사전등록·정직한 negative 보고. 공개 프리프린트(DOI).</sub>

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
