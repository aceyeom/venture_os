# BUILD PLAN — CASH-D1 · 책무구조도 Maintenance & Internal-Controls Execution Layer
> Cycle 21 (May 30, 2026) · MODE-CASH · the Prime Directive's deliverable for the board's lead idea.
> **STATUS: BUILD-ON-GREEN.** This plan is *promoted but gated* — each build phase unlocks only on the
> buyer signal named in its gate. Per §5, desk research cannot authorize a build; buyers do. Read with
> `LEDGER.md` (Cycle 17 = the idea; Cycle 19 = the validation kit that gates Phase 1).

---

## 0. WHY THIS IDEA, WHY NOW
- **Lead because:** fastest + hottest path on the board — a statutory mid-tier deadline (**책무구조도, 2026-07-02, 33 days out**), CEO *personal* liability, untooled at the mid-tier, warm channel via Ace's dad, async-buildable.
- **Forcing function:** decision date = 2026-07-02. On that date the top surviving idea is promoted to active build even if imperfect. This plan is the pre-positioned artifact so promotion is instant, not a scramble.
- **Subordinate ideas wait:** LEAD-1 (AI-compliance), MOAT-D1 (FSS benchmark), MOAT-A1 (security 소명), DATA-C1 (민원) are all the *same engine, different persona*. They become expansion SKUs only after this wedge has paying buyers. **Do not split Ace's 10-13 hr/wk.**

---

## 1. THE WEDGE (what we sell first)
Not the one-time map (Big-4/law firms own that) — the **continuous maintenance + 관리의무-이행 evidence** the consultants don't sell. Per refined **L1/L5**: own the unglamorous recurring workflow, not the headline deliverable.

**Buyer:** 준법감시인 / 내부통제 담당 / 소비자보호 총괄 at a mid-tier KR FI (저축은행 ≥₩7,000억, 캐피탈/카드 ≥₩5T 여전사, <₩5T 자산운용·증권 — all in the Jul-2-2026 cohort).
**Job-to-be-done:** keep the 책무구조도 current through every org/personnel change, and produce regulator-ready evidence that the CEO/임원 *did* their 관리의무 — the artifact that functions as a personal-liability defense (소명) in an FSS exam or post-incident.

---

## 2. MVP SCOPE (Phase-1, buildable in bandwidth)
| # | Capability | Why it's the wedge, not a doc tool |
|---|-----------|-----------------------------------|
| 1 | **책무 library** pre-built from 지배구조법 + 감독규정, templated by 업권 (저축은행/캐피탈/자산운용/증권) | Removes the blank-page problem; encodes the law so the buyer doesn't re-derive it |
| 2 | **임원 ↔ 책무 mapping editor with version control** — every change timestamped + diffed | The recurring pain: re-papering on personnel moves. This is the lock-in surface |
| 3 | **Auto-generate** 책무구조도 / 책무기술서 / 직책별 책무배분표 in FSS-submission format (PDF/HWP) | Turns hours of manual doc assembly into one click |
| 4 | **관리의무 이행 점검 workflow** — periodic checklists, evidence attachment, immutable audit log → CEO **소명 dossier** | The defensible artifact; this is what the buyer actually fears not having |
| 5 | **Change-triggered re-papering** — flag affected 책무 + regenerate docs when an 임원 changes | Converts a one-time submission into a recurring subscription reason |

**Explicitly OUT of MVP:** AI-compliance execution (LEAD-1), cross-client benchmark (MOAT-D1), 민원 (DATA-C1). Those are post-revenue SKUs.

---

## 3. ARCHITECTURE (Ace solo, full-stack + AI)
- **Stack:** Next.js + TypeScript, Postgres, an LLM layer (책무 derivation/mapping suggestions + doc generation), background jobs for change-detection.
- **Hosting:** KR cloud (NCP / NHN Cloud) for data-residency comfort; the **Apr-2026 망분리-for-SaaS relaxation** is what makes in-network FI SaaS viable — lean on it in the security narrative.
- **Trust posture (small-vendor mitigation):** strong per-FI tenant isolation; export-everything (no lock-in fear); KR liability entity on the contract.
- **Data model (core entities):** `Duty` · `Executive` · `Mapping{version}` · `Control` · `EvidenceItem` · `ReviewCycle` · `ChangeEvent` · `SubmissionPackage`.
- **Build estimate:** Phase-1 MVP ≈ 150–250 hrs ≈ ~3–4 months at 10–13 hr/wk. Fits G8 bandwidth.

---

## 4. PHASING — each gate is a buyer signal, not a date
| Phase | Unlock gate (build-on-green) | Scope | Bandwidth |
|-------|------------------------------|-------|-----------|
| **0 — now (pre-signal)** | none — but this is a **discovery aid**, shown only AFTER pain surfaces, never as the opening pitch (§5) | 1 sample 책무구조도 generated from public templates + clickable mock of the mapping editor | ~20–30 hrs |
| **1 — pilot MVP** | **≥1 STRONG signal** (buyer asks "얼마예요? / 언제 써요?" or describes ongoing-maintenance pain unprompted) | Items 1–3 + hand-in-loop for 1 design-partner FI | ~120 hrs |
| **2 — recurring engine** | **design partner commits** (paid pilot or LOI) | Items 4–5 (관리의무 evidence + change-triggered re-papering), multi-tenant | post-revenue |
| **3 — expansion SKUs** | **VoD #2 confirmed** (buyer wants vendor consolidation) | LEAD-1 / MOAT-D1 / DATA-C1 layered onto the same buyer | later |

---

## 5. UNIT ECONOMICS (MODE-CASH)
- **ACV:** ₩50–100M ($35–70K) — priced on the recurring maintenance + evidence, NOT the one-time map.
- **2026 target:** 3–5 design partners → **₩200–400M ARR**; gross margin high (SaaS); burn ≈ 0 (Ace solo, no hires).
- **Why not chase $30M here:** this is the *cash leg* — the anti-gaming resolution (Cycle 17) put the $30M thesis on the expansion/benchmark legs, which are separately gated and unvalidated. Don't relitigate.

---

## 6. RISKS → MITIGATIONS (from the harden pass)
| Watch-risk | Mitigation baked into the plan |
|-----------|-------------------------------|
| **Recurring-WTP unproven** (pay once for the map, maintain in Excel) — *the load-bearing risk* | Price the *maintenance + 소명 evidence*, not the map; Phase-2 gate = a paid commitment, so we never build the recurring engine on faith |
| Big-4 / law firm owns the initial map | **Integrate, don't fight** — accept their map as import; own the part they don't sell (continuous upkeep + evidence) |
| Small-vendor trust at a regulated FI | KR entity + data residency + export-everything + start with 1 warm design partner via Ace's dad |
| Bandwidth drift (A8) | Hard MVP cut-line (items 1–5 only); expansion SKUs forbidden until post-revenue |

---

## 7. DECISION-DATE PLAYBOOK (2026-07-02)
- **≥3 strong signals** → promote CASH-D1 to **active BUILD (Phase 1)**; sign the design partner.
- **<3 signals but pain confirmed** → extend validation 30 days; build only Phase-0 aid.
- **Pain absent / buyers shrug** → trust buyers over desk research (meta-loop §3): down-weight 책무구조도, and check the **MOAT-A1 activate-trigger** (is security-governance 소명 the real #1 pain instead?).

---

## 8. RED-TEAM FIXES (Cycle 22 — re-stress-test of the load-bearing assumptions)
The plan above passed the original harden. A harder re-attack surfaced four *new* failure modes and their fixes; these supersede the naïve framing where they conflict.

### FIX-1 — the timing trap (most important)
**New attack:** the Jul-2-2026 deadline that makes this idea look "hot" is the deadline for the *initial submission* — the one-time job we explicitly DON'T sell (Big-4/law firms own it, and they're being engaged *right now*, 33 days out). By the time we ship, the maps are filed. The why-now and the wedge are **misaligned in time.**
**Fix:**
- **Reframe the buying trigger** from "the deadline" → "the *first post-submission event*": the first personnel/org change that forces a re-paper, or the first FSS 점검. That's when maintenance pain (what we sell) actually bites.
- **Flip the validation ICP:** lead discovery with the **already-submitted cohort** (은행 Jan-2025, large 금투/보험 Jul-2025) — they're 6–18 months into the *maintenance* pain with no deadline-consultant competing for attention. They are the right teachers for VoD #1 (recurring WTP). Keep the Jul-2026 mid-tier as the sales *pipeline*, not the validation sample.

### FIX-2 — reframe the buyer & the value (raises WTP)
**New attack:** "maintenance" may be absorbed into existing 준법감시 headcount (a junior re-papers in Word) → soft WTP, sold to the analyst who wants to save time.
**Fix:** price it as **CEO liability-insurance, not an analyst productivity tool.** The 관리의무 소명 dossier reduces the CEO's *personal* criminal/sanction exposure. Sell to the CEO/board (who fear the ₩-billion/prison risk), not the analyst. Different, higher WTP; cheaper than the downside.

### FIX-3 — instrument the moat from day 1
**New attack:** the maintenance tool itself is thin and copyable (cash-mode tolerates this, but nothing compounds).
**Fix:** from the **first pilot**, capture the 책무→control→점검-outcome data the product naturally sees, so the cash wedge silently accretes the MOAT-D1 dataset. The cash leg funds the data that becomes the moat. *(Add `OutcomeObservation` to the §3 data model.)*

### FIX-4 — bandwidth containment
**New attack:** pixel-perfect FSS HWP templates + FI-grade security certs (ISMS-class) for procurement could blow the 150–250 hr estimate.
**Fix:** Phase-1 exports **PDF + structured data, not pixel-perfect HWP**; defer security certs until a design partner *requires* them, and fund that work from pilot revenue. Hard MVP cut-line holds.

### FIX-5 — the cross-board fix (see Cycle 22 in LEDGER + provisional Law L9)
**New attack (shared by the ENTIRE board):** every convergent idea has the *same* bear — enforcement-gated software-WTP (L6): FIs pay a consultant once and run Excel until an exam forces them. If that bear is right, this whole engine is YELLOW-forever.
**Fix / strategic option:** enter as a **service-wrapped-software (managed compliance service)** — David sells/presents the deliverable, Ace's software is the margin multiplier behind it — so revenue rides *proven consulting-WTP* instead of *unproven software-WTP*. Fewer clients, higher ACV (₩100–300M), faster to revenue, better bandwidth-fit. **This is the recommended entry posture if validation confirms software-WTP is soft.** (Regression-check: watch David's part-time bandwidth; MOAT leg still rides the software+data behind the service.)

---
*The binding constraint remains buyer signal (0/3). This plan exists so that the moment signals arrive, building starts the same day — and so that if they don't, we don't build the wrong thing.*
