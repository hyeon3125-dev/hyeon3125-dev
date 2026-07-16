<div align="center">

<img src="https://raw.githubusercontent.com/hyeon3125-dev/hyeon3125-dev/7109418d7ec4f7720e46157d2b40771b793817e8/assets/scalar/brand/scalar-lockup-vertical.png" width="160" alt="Scalar"/>

<br/><br/>

<!-- BENCHMARK: 재현 가능한 공정 벤치 (kibo_fair_test.py, N=2000) -->
[![](https://img.shields.io/badge/🛡️_Safety-100%25_bounds--safe_vs_74.6%25_raw-F37021?style=for-the-badge&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/✓_Schema-100%25_conform_by_construction-F37021?style=for-the-badge&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/◈_Output-normalized_to_fixed_command-F37021?style=for-the-badge&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)

<br/>

[![](https://img.shields.io/badge/SCALAR_Atelier-RC_·_Soft--Open-F37021?style=flat-square&labelColor=111111)](https://atelier.scalar-inc.com)
[![](https://img.shields.io/badge/Patent_filed_①_Routing-10--2026--0105850-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/Patent_filed_②_Execution-10--2026--0084899-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)
[![](https://img.shields.io/badge/LKML_RFC-BPF_DAG_fast--path-F37021?style=flat-square&labelColor=111111&logo=linux&logoColor=white)](https://lore.kernel.org/bpf/178004391665.3522.4865582628003357086@gmail.com/T/#u)

<br/><br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/hyeon3125)
[![Demo](https://img.shields.io/badge/Request_Demo-F37021?style=for-the-badge&logoColor=white)](https://mtp-l2-scalar.lovable.app)
[![Portfolio](https://img.shields.io/badge/scalar--inc.com-111111?style=for-the-badge&logo=netlify&logoColor=F37021)](https://scalar-inc.com)
[![Email](https://img.shields.io/badge/l0architect@scalar--inc.com-111111?style=for-the-badge&logo=gmail&logoColor=F37021)](mailto:l0architect@scalar-inc.com)

</div>

---

```
Scalar builds deterministic AI orchestration systems —
the execution-verification layer that proves an action is safe *before* it runs.
Solo-built. Two patent applications filed (KR). Verified in the open.
```

**Seung-hyeon Lee** — Founder, SCALAR *(incorporation in progress)* · Seoul, Korea · l0architect@scalar-inc.com

Orchestration, robotics, finance, copyright, kernel verification — every project answers one question: **can you trust the result of an execution?** Verify before you trust.
<br><sub>오케스트레이션·로보틱스·금융·저작권·커널 검증 — 모든 프로젝트가 답하는 하나의 질문: 실행 결과를 신뢰할 수 있는가. 신뢰하기 전에 검증한다.</sub>

---

## Background

```
LED manufacturing R&D  →  overseas auto production line (full-lot quality inspection)  →  ERP · logistics · call-center CS  →  Korea's largest manufacturing floors (Hyundai · Kia)  →  independent development  →  2 patent applications · LKML RFC · open source
```

Across every floor — production lines, quality inspection, logistics, and customer support — the same problem kept surfacing three ways: equipment broken by an unverified command, customer trust broken by an unverifiable answer, audits impossible on an unrecorded execution. Scalar is the answer, built from that floor up.
<br><sub>생산라인·품질 전수검사·물류·CS까지 — 전 공정에서 같은 문제를 세 번 만났다: 검증 없는 명령이 부순 설비, 검증 불가한 답이 무너뜨린 고객 신뢰, 기록 없는 실행에 불가능한 감사. 스칼라는 그 현장에서 출발한 답이다.</sub>

---

## Why Verification — Where the Market Is Moving

Enterprises don't stall on AI because the models are weak. They stall because **no one can prove what an action did** — so every AI action carries a *trust cost*: human review, audit, rollback, liability. Verification removes that cost. It is the layer that turns an impressive demo into something deployable in production — and the spend is moving from "a better model" to "an action you can prove."
<br><sub>AI 도입이 막히는 건 모델이 약해서가 아니라 "무엇을 실행했는지 증명할 수 없어서"다 — 검토·감사·롤백·책임이라는 **신뢰비용**. 검증은 그 비용을 제거해 데모를 프로덕션으로 바꾼다. 자본은 "더 좋은 모델"에서 "증명 가능한 실행"으로 이동 중.</sub>

| | Signal | Source |
|---|---|---|
| **Market** | AI orchestration **$13.99B (2026) → $60.34B (2034), 20.05% CAGR** · agentic orchestration **$6.3B → $46.8B by 2036, 22.1% CAGR** — shift from chat assistants to *governed* automation with audit trails | Fortune Business Insights · Fact.MR (secondary: MarketsandMarkets $11.0B → $30.2B, 2025→2030) |
| **Beachhead** | First wedge: SMB-manufacturing ERP-gap automation (validated demand, pilots ₩50–100M) → expands into the orchestration TAM | Scalar GTM |
| **Capital** | Arcade.dev raised **$60M Series A** (SYN Ventures lead; $72M total) for a "secure action layer" — the verification/execution-control category is now funded | BusinessWire · WSJ `2026-06` |
| **Academia** | AGI-premise collapse → per-domain verification *harness* becomes mandatory, not optional | LeCun et al. — [arXiv:2602.23643](https://arxiv.org/abs/2602.23643) |
| **Governance** | Typed Planning → DAG → Validation Gate → Audit Trail as the enterprise pattern | POLARIS — [arXiv:2601.11816](https://arxiv.org/abs/2601.11816) |
| **The gap** | "Capability–Deployment **Verification Gap**" — *built ≠ trustable* | [arXiv:2605.14675](https://arxiv.org/abs/2605.14675) |
| **Product entry** | Sakana AI ships Fugu multimodel orchestration commercially — the category is real | `2026-06` |

> *"Agents don't fail in production because the model is wrong. They fail because no one can prove what an agent did."* — Alex Salazar, Arcade.dev CEO

**Where Scalar sits** — the execution-guarantee layer, not another framework:

```
L1  Orchestration   LangChain · CrewAI            connect models & tools          →  complement
L2  Guardrails      Guardrails AI · NeMo          output format / schema check     →  adjacent
L3  Deterministic   PromptPort · Lean-Agent        prove constraints BEFORE run     →  Scalar combines
    execution       SCALAR MTP-L2                  · reproduce · audit                 routing + execution
                                                                                       verification
```

Scalar combines a **deterministic L3 execution guarantee** with multimodel routing — two patent applications filed (KR) and the same verification methodology submitted to the Linux kernel (LKML RFC). Honest weakness, stated up front: as a new entrant, ecosystem and mindshare are early-stage.
<br><sub>L1 연결·L2 형식검증이 못 푸는 "실행 전 결정론적 보장(L3)"을 멀티모델 라우팅과 결합 — 특허 2건 출원(KR), 같은 검증 방법론을 리눅스 커널에 RFC로 제출. 정직한 약점: 신생 팀이라 생태계·인지도는 이제 시작.</sub>

---

## Core Products

### [SCALAR Atelier](https://atelier.scalar-inc.com) — Local BYOK AI Orchestration for macOS &nbsp;[![](https://img.shields.io/badge/RC_·_Soft--Open-555?style=flat-square&labelColor=111111)](https://atelier.scalar-inc.com) [![](https://img.shields.io/badge/Patent_filed_①_Routing-F37021?style=flat-square&labelColor=111111)](https://atelier.scalar-inc.com)

A local, single-user, BYOK AI orchestration app (Tauri 2). Every model call is deterministically routed and verified at the boundary *before it leaves the device* — each egress commits an AdmissionRecord to an Ed25519-signed local audit hash-chain (proof candidate). Your keys, conversations, and files stay on your machine; Scalar's servers can't see inside. Same routing patent application and Kani-proof methodology as MTP-L2, applied to a consumer desktop app.
<br><sub>로컬 단일유저 BYOK AI 오케스트레이션 macOS 앱. 모든 모델 호출은 기기를 떠나기 전 경계에서 결정론적으로 라우팅·검증되고, Ed25519 서명 로컬 감사 해시체인에 기록됩니다. 키·대화·파일은 전부 기기 안에 — 서버는 들여다보지 못합니다.</sub>

| | |
|---|---|
| **Landing** | [atelier.scalar-inc.com](https://atelier.scalar-inc.com) |
| **Routing** | Deterministic argmax, Kani-proven (55 checks · 2,000-case differential vs production code, 100% match) |
| **Boundary** | AdmissionRecord + Ed25519 signature per provider egress — local audit hash-chain (proof candidate) |
| **Status** | RC — notarized macOS build · 700+ tests · lineage: internal codename *Project Ratatouille*, split 2026-07-03 |

---

### [MTP-L2-mini](https://github.com/ScalarCore/MTP-L2-mini) — Deterministic AI Orchestration &nbsp;[![](https://img.shields.io/badge/LIVE_DEMO-F37021?style=flat-square&labelColor=111111)](https://mtp-l2-scalar.lovable.app) [![](https://img.shields.io/badge/Patent_Pending-F37021?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/MTP-L2-mini)

A deterministic layer between the LLM and the executor: tokenize → validate → clamp → compile. Every downstream command is schema-conform and within physical bounds **by construction** — not by hoping the model behaves.

**Patent applications (KR, filed):**
- Routing Layer — KR 10-2026-0105850 (reasoning-profile vector routing)
- Execution Layer — KR 10-2026-0084899 (DSL parser-verified execution)

```
Input → [Routing Layer (application ①)] → [Execution Layer (application ②)] → Verified Output
```

Routing and execution are covered by two separately filed applications.

| Metric | MTP-L2 | Raw LLM output | Source |
|--------|:------:|:------:|:------:|
| Bounds-safe & schema-conform | **100.00%** | 74.6% | fair bench N=2000 |
| Correct vs intent | **90.9%** | 74.6% | fair bench N=2000 |
| Output payload | **52–55 B (mean 53.6)** | 25–86 B (varies) | fair bench N=2000 |
| Parse overhead | 6.10 µs | 3.81 µs | LLM call paid by both paths |

*Fair benchmark: identical fuzzed input to both paths, reproducible offline (`python kibo_fair_test.py --n 2000`). Scope: 100.00% is bounds/schema conformance by construction; 90.9% is intent match — separate properties. MTP-L2's edge is determinism & safety, not latency.*

**→ [Repo + benchmark](https://github.com/ScalarCore/MTP-L2-mini)** · [Live Demo](https://mtp-l2-scalar.lovable.app)

---

### [SCALAR FMS](https://fms.scalar-inc.com) — Financial Market Intelligence &nbsp;[![](https://img.shields.io/badge/V8.3-Shadow--Mode_Ops-F37021?style=flat-square&labelColor=111111)](https://fms.scalar-inc.com) [![](https://img.shields.io/badge/B2B-111111?style=flat-square&labelColor=222222)](https://fms.scalar-inc.com)

Real-time BTC/USDT derivatives + on-chain + whale tracking. The signal engine runs continuously on Hetzner VPS; trading and auto-tuning currently run in **shadow mode** (signals computed, logged, and evaluated — not live-applied) while the public endpoint is being rewired.

| | |
|---|---|
| **Dashboard** | [fms.scalar-inc.com](https://fms.scalar-inc.com) *(public endpoint transition in progress)* |
| **Stack** | Python 3.12 · Supabase · Bybit API · Telethon · React 18 |
| **Signal Engine** | Taker CVD · OI% · Funding · ATR · EMA · Whale Events ($10M+) |
| **Ops** | PM2 · Hetzner VPS · data partition: public views only (internal ledger isolated) |
| **Version** | V8.3 — regime-switching engine · ATR-anchored TP/SL · GeminiTuner (24h cycle, shadow mode) |

---

### Music Forensics — AI Music Copyright Evidence &nbsp;[![](https://img.shields.io/badge/B2B-F37021?style=flat-square&labelColor=111111)](https://scalar-inc.com) [![](https://img.shields.io/badge/PoC-111111?style=flat-square&labelColor=222222)](https://scalar-inc.com)

Hybrid audio-similarity engine for AI-music copyright disputes, producing forensic reports for B2B legal use.

| | |
|---|---|
| **Engine** | Chroma CENS (HPSS pre-processing) · fastDTW · Melody Contour (60% of score) |
| **Pipeline** | Math core → GPT-4o-mini pattern check → hybrid scorer → forensic HTML report |
| **Stack** | Python · FastAPI · Supabase |
| **Target** | Music-specialized law firms · AI-music copyright proof · *(FAISS reverse-tracker: PoC, on hold)* |

---

### [SCALAR: NODE ZERO](https://github.com/hyeon3125-dev/snz-novel) — Deterministic Interactive Novel &nbsp;[![](https://img.shields.io/badge/Open_IP-F37021?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/snz-novel) [![](https://img.shields.io/badge/CC_BY--NC--SA_·_PolyForm_NC-555?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/snz-novel/blob/main/LICENSE-CONTENT.md)

A complete 16-volume psychological-SF novel released as a source-available interactive novel — the deterministic philosophy applied to storytelling: same choices, same story, every time. No AI, no server, no build, zero runtime dependencies. The full manuscript ships in the repo; non-commercial culture is free, commercial use is licensed.
<br><sub>완결 심리 SF 장편을 오픈 IP 인터랙티브 노벨로 공개 — 비영리 향유는 자유, 상업적 이용(출판·굿즈·영상화)은 라이선스.</sub>

| | |
|---|---|
| **Play / Read** | [hyeon3125-dev.github.io/snz-novel](https://hyeon3125-dev.github.io/snz-novel/) · manuscript in-repo |
| **Scale** | 16 vols · 200 chapters + 21 side stories · 1,366 scenes · 11,608 lines — structural parity KO = EN = JP, verbatim-verified by CI across all three languages |
| **Engine** | Vanilla JS 5-layer · 6 gesture interactions · 6 faction text-grammars · procedural Web Audio |
| **Model** | Content CC BY-NC-SA 4.0 + commercial licensing & merch · **Engine source-available (PolyForm Noncommercial)** — free for noncommercial authors, commercial licensed |

---

### [차이 — 단편집](https://github.com/hyeon3125-dev/hyeon3125-dev-scalar-shorts) — Deterministic Short Stories &nbsp;[![](https://img.shields.io/badge/Open_IP-F37021?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/hyeon3125-dev-scalar-shorts) [![](https://img.shields.io/badge/CC_BY--NC--SA_·_PolyForm_NC-555?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/hyeon3125-dev-scalar-shorts)

Four short stories (비효율 · 기억 라우터 · 차이 · 입술의 무게) running on the **same SNZ 5-layer engine** — proof the engine is a reusable noncommercial substrate any author can build their own interactive novel on. Korean · English · Japanese, with theme-native interactions (silence as record, manipulated choice, refrains as echo).
<br><sub>SNZ 엔진을 그대로 재사용한 결정론 단편집 — 엔진은 비영리 작가 누구나 자기 작품에 쓸 수 있는 토대(PolyForm Noncommercial). 한·영·일 3개 언어.</sub>

| | |
|---|---|
| **Play / Read** | [hyeon3125-dev.github.io/hyeon3125-dev-scalar-shorts](https://hyeon3125-dev.github.io/hyeon3125-dev-scalar-shorts/) · manuscript in-repo |
| **Engine** | shared SNZ 5-layer core — source-available (PolyForm Noncommercial) |
| **Model** | Content CC BY-NC-SA 4.0 · Engine PolyForm Noncommercial |

---

## Research

### [MTP-MetaEval](https://github.com/hyeon3125-dev/MTP-MetaEval) — Verification Efficiency under Bounded Risk &nbsp;[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20806118-F37021?style=flat-square&labelColor=111111)](https://doi.org/10.5281/zenodo.20806118)

A cross-domain study of *when verification should stop* — the methodology behind the deterministic-verification work, made falsifiable. A non-refutation overhead boundary with a **provable risk bound** (`miss_rate ≤ ε`), and one *assumed-not-earned* law tested across number theory, cosmology, control, statistics, and LLM evaluation. Pre-registered; reports its own negative results (headline: *windowed IDE falsified, MTP-MetaEval survived*). DOI-archived on Zenodo.
<br><sub>검증을 언제 멈춰야 하는가 — 비반증 오버헤드 경계의 위험 한계 증명과 *assumed-not-earned* 법칙, 5개 도메인 교차 검증. 사전등록·정직한 negative 보고. Zenodo DOI 아카이브.</sub>

### [bpf-verifier-rs](https://github.com/hyeon3125-dev/bpf-verifier-rs) — BPF Verifier Scalar Domain, Formally Verified &nbsp;[![](https://img.shields.io/badge/LKML_RFC-F37021?style=flat-square&labelColor=111111&logo=linux&logoColor=white)](https://lore.kernel.org/bpf/178004391665.3522.4865582628003357086@gmail.com/T/#u) [![](https://img.shields.io/badge/Rust_·_Kani-111111?style=flat-square&labelColor=222222)](https://github.com/hyeon3125-dev/bpf-verifier-rs)

Rust model of the Linux BPF verifier's scalar abstract domain (tnum × cnum) with **Kani soundness proofs** and differential tests against the unmodified kernel C (N=2000 × 11 ops, 0 mismatches). Companion LKML RFC:

```
RFC      : [PATCH RFC] bpf: add DAG fast-path in verifier to skip redundant state pruning
Sent to  : bpf@vger.kernel.org · linux-kernel@vger.kernel.org        2026-05-29
Reply    : Alexei Starovoitov (BPF subsystem maintainer · Meta) — direct reply in 17 hours
Language : Rust (model + proofs) · C (kernel patch)
```

**→ [LKML thread](https://lore.kernel.org/bpf/178004391665.3522.4865582628003357086@gmail.com/T/#u)** `2026-05-29`

### [MTP-Cosmology](https://github.com/hyeon3125-dev/MTP-Cosmology) — Windowed IDE Toy Model &nbsp;[![](https://img.shields.io/badge/negative_result-555?style=flat-square&labelColor=111111)](https://github.com/hyeon3125-dev/MTP-Cosmology)

Windowed interacting-dark-energy toy model fit to real DESI DR1 BAO data (emcee MCMC). Honest negative result, reported as such: coupling bounded at **β₀ < 0.27 (95%)**, no advantage over ΛCDM (**Δln Z = −1.9**) — the falsification that MTP-MetaEval's stopping rule was tested against.
<br><sub>DESI DR1 BAO 실데이터 피팅 — ΛCDM을 이기지 못했다는 정직한 negative result. MetaEval 중단 규칙의 실전 반증 사례.</sub>

### [MTP_Popw](https://github.com/hyeon3125-dev/MTP_Popw) — Proof of Physical Work

Monetary issuance anchored to verifiable physical energy. Unauthorized inflation structurally impossible.

```
Simulation (seed=42): Conservation 100%  ·  False issuance blocked 53.7%  ·  SNR +94.2%
```

---

## Open Source & Simulations

### [Scalar ERP](https://github.com/ScalarCore/Scalar-ERP-v1.0) — Serverless MES on Google Sheets &nbsp;[![](https://img.shields.io/badge/MIT-555?style=flat-square&labelColor=111111)](https://github.com/ScalarCore/Scalar-ERP-v1.0)

Full BOM/production tracking · 41 functions · Zero infrastructure cost.

### [sim_music_automation](https://github.com/hyeon3125-dev/sim_music_automation) — Cognitive Layer Simulation

Two-domain stress test: music industry vs. social discourse. When μ > 1.0, echo chamber lock-in is the rational response.

```
Cross-domain Δβ: +0.141 / +0.135  ·  Music golden-age: 8% ↓  ·  Social: 98% intact
(v0.5 snapshot — structured argument, not a proof; author-reported limits in-repo)
```

---

## Trajectory

```
Month 2  →  Multi-LLM production system       FastAPI · pm2 · Tailscale VPN · Hetzner
Month 4  →  LKML BPF DAG verifier RFC         Alexei Starovoitov · 17h direct reply
Month 6  →  7-project portfolio               2 patent applications filed · funding track active
Month 7  →  SCALAR Atelier RC                 notarized macOS build · Kani-proven routing · 700+ tests
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
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![eBPF](https://img.shields.io/badge/eBPF-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=black)
![Tauri](https://img.shields.io/badge/Tauri-24C8D8?style=flat-square&logo=tauri&logoColor=white)

<br/>

<img src="https://raw.githubusercontent.com/hyeon3125-dev/hyeon3125-dev/7109418d7ec4f7720e46157d2b40771b793817e8/assets/scalar/brand/scalar-corporate-identity.png" width="320" alt="Scalar"/>

<br/><br/>

*SCALAR · Seoul, Korea · 2026 — incorporation in progress*

![](https://komarev.com/ghpvc/?username=hyeon3125-dev&color=F37021&style=flat-square&label=profile+views)

</div>
