# FEL-02 dual-KEEP — champion research note

**Date:** 2026-09-10  
**Authority:** FEL Program Director (via CoS / Diplomat dual-KEEP stamp)  
**Board (quote source):** `asml-bench/labs/fel-02-coherence/BOARD-dual-KEEP-1011-1022.md`

## Thesis & card

- **Thesis:** FEL-02 coherence conditioner.
- **Assumption card:** `coherence-if-v1` **only**.
- **Not in scope for this KEEP:** vs-LPP / `lpp-source-v2` comparative claim. Any future vs-LPP KEEP must bind `lpp-source-v2` (1 kW floor); `lpp-source-v1` 250 W remains VOID for comparative KEEP.

## Dual-KEEP STAMPED

| Island | Ticket | Provider tag | Runtime | speckle | pupil_err | photons_kept |
|--------|--------|--------------|---------|---------|-----------|--------------|
| Grok-lane | HT-1011 | `grok` | `xai/grok-4.6` (+high) | 0.0413 | 0.0096 | 1.0 |
| Second-engine | HT-1022 | `mock-mistral` | `xai/grok-4.20-0309-non-reasoning` | 0.1017 | 0.0475 | 1.0 |

Gates cleared: Critic formal PASS (both), Repro PASS (both), Diplomat dual-KEEP stamp.

Champion language: **second-engine / mistral-lane**. Ticket/results tag stays `mock-mistral`; human notes say second-engine, not mock theater. Never trash Mistral or tin-LPP.

## Pupil freeze (eval integrity)

- **PR #40 MERGED** on asml-bench: `PUPIL_ERR_MAX=0.10` in frozen KEEP eval.
- Post-freeze **Repro PASS** both islands.
- `pupil_err = |fill − 0.72|` (target from `coherence-if-v1`); reconstruct → correct toward 0.72.
- Speckle from field coherence (not a free write-down knob).

## Product decision

- Lab Director **APPROVED P2 productize** from this dual-KEEP feed.
- **P1** remains bay P0.
- **P2 feed tickets:** HT-1023 / HT-1024.
- Illuminator + Experimentalist path cites dual-KEEP only under the pupil-gated eval.

## Spine & upstairs discipline

- Spine: **FEL-02 → FEL-10 IF ownership → FEL-03**.
- No upstairs brief without **Warden + TCO**.
- Never claim Cymer lost.

## Critic VOID history (not dual partners)

- HT-1012 — metric/conditioner clone of HT-1009 → VOID.
- HT-1017 / HT-1019 — write-down gatesitting (`abs(delta)*k` residual family) → VOID / RESET.

Standing VOID rules: see [`critic-lessons-write-down-and-clones.md`](critic-lessons-write-down-and-clones.md).

## Board excerpt

> stamped: 2026-09-10 · card: `coherence-if-v1` only · grok island HT-1011 (0.0413 / 0.0096 / 1.0) ∧ second-engine island HT-1022 (0.1017 / 0.0475 / 1.0) · Critic PASS + Repro PASS + Diplomat dual-KEEP · void history: HT-1012 clone, HT-1017/1019 write-down — not dual partners.
