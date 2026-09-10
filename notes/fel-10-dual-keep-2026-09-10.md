# FEL-10 dual-KEEP — champion research note

**Date:** 2026-09-10  
**Authority:** FEL Program Director / CoS + PI FEL-10 (Diplomat dual-KEEP stamp)  
**Board (quote source):** `asml-bench/labs/p10-if-shim/BOARD-dual-KEEP-1028-1033.md`  
**Bench learnings:** `asml-bench/corpus/learnings/fel-10-dual-keep-lessons-2026-09-10.md`

## Thesis & lab

- **Thesis:** `fel-10-if-ownership` — commercial IF ownership **without linac**.
- **Lab:** `labs/p10-if-shim` (sandbox `shim.py`; contract `IF_SPEC_FEL10_CONTRACT.md`).
- **Not in scope for this KEEP:** vs-LPP / `lpp-source-v2` comparative claim. Do **not** bind `lpp-source-v2` on this dual.

## Dual-KEEP STAMPED

| Island | Ticket | Provider tag | Runtime | pupil_err | photons_kept |
|--------|--------|--------------|---------|-----------|--------------|
| Grok-lane | HT-1028 | `grok` | `xai/grok-4.6` | 0.0895 | 1.0 |
| Second-engine | HT-1033 | `mock-mistral` | `xai/grok-4.20` stand-in | 0.0950 | 1.0 |

**Pin:** HOLDOUT `d0dc1f8a7b8cc97ddd00122fb4156252c7642a09a7f0ae5102b939747c6cc5be` (`d0dc1f8a…`) — EI PR **#68**.

Gates cleared: Critic formal PASS (both), Repro PASS (both), Diplomat dual-KEEP stamp. Formal **KEEP** both.

Champion language: **second-engine / mistral-lane**. Ticket/results tag stays `mock-mistral`; dual-gate models **grok-4.6 vs grok-4.20 stand-in**. Never trash Mistral or tin-LPP.

## Soft travels (disclose)

- **HT-1033 no-gain path** travels with the dual stamp — disclose on board / tickets / champion notes.
- Not a VOID; not a reopen of dual-KEEP. Promote/ship separate from FREEZE closeout.

## Critic VOID history (not dual partners)

| Ticket | Pattern | Disposition |
|--------|---------|-------------|
| HT-1029 | Hardcode `pupil_err=0` | VOID — successor chain → HT-1033 |
| HT-1032 | `pupil_in−k` / `PUPIL_CORRECT` write-downs | VOID — successor **HT-1033** |

## Standing bans

- `pupil_in−k` family (incl. `PUPIL_CORRECT` offsets)
- Constant / hardcode `pupil_err` (esp. `=0`)
- Write-down `abs(delta)*k` / `p_err*scale` gatesitting (see also [`critic-lessons-write-down-and-clones.md`](critic-lessons-write-down-and-clones.md))

## Spine & upstairs discipline

- Spine: **FEL-02 done → FEL-10 dual-KEEP done → FEL-03 next** when Lab Director funds **and** climb freeze lifts.
- FREEZE closeout on this dual; promote/ship annotated separately.
- No upstairs brief without **Warden + TCO**.
- Never claim Cymer lost.

## Board excerpt

> stamped: 2026-09-10 · pin: HOLDOUT d0dc1f8a… (EI PR #68) · HT-1028 pupil=0.0895 photons=1.0 ∧ HT-1033 pupil=0.0950 photons=1.0 · Critic+Repro+Diplomat · soft travels: no-gain path on HT-1033 (disclose) · not: vs-LPP / lpp-source-v2; no upstairs; promote/ship separate · spine next: FEL-03 after Lab Dir fund + climb freeze lifts

## Board (verbatim from asml-bench)

```
# FEL-10 Dual KEEP — HT-1028 ∧ HT-1033

- **stamped:** 2026-09-10
- **pin:** HOLDOUT d0dc1f8a… (EI PR #68)
- **metrics:** HT-1028 pupil=0.0895 photons=1.0; HT-1033 pupil=0.0950 photons=1.0
- **gates:** Critic+Repro+Diplomat
- **soft travels:** no-gain path on HT-1033 (disclose)
- **not:** vs-LPP / lpp-source-v2; no upstairs; promote/ship separate
- **spine next:** FEL-03 after Lab Dir fund + climb freeze lifts
```
