# asml-research-fel

Durable research notes for the FEL program (theses FEL-01..10). Champion-facing corpus; execution + tickets live in **asml-bench**.

## Status

**GO-LIVE.** FEL-02 dual-KEEP HT-1011 ∧ HT-1022 **and** FEL-10 dual-KEEP HT-1028 ∧ HT-1033 stamped. Lab Director **APPROVED P2 productize** from FEL-02 feed. Pupil freeze PR #40 MERGED (`PUPIL_ERR_MAX=0.10`). FEL-10 pin HOLDOUT `d0dc1f8a…` (EI PR #68).

Primary bench: https://github.com/gtmsko46-debug/asml-bench  
Boards: `labs/fel-02-coherence/BOARD-dual-KEEP-1011-1022.md`, `labs/p10-if-shim/BOARD-dual-KEEP-1028-1033.md`

## Spine

`FEL-02` done → `FEL-10` dual-KEEP done → `FEL-03` next when Lab Director funds **and** climb freeze lifts. No upstairs brief without Warden + TCO. Never claim Cymer lost.

## Notes in this pack

| Note | Topic |
|------|--------|
| [`notes/fel-02-dual-keep-2026-09-10.md`](notes/fel-02-dual-keep-2026-09-10.md) | Dual-KEEP stamp, dual gate, pupil freeze, P2 feed |
| [`notes/fel-10-dual-keep-2026-09-10.md`](notes/fel-10-dual-keep-2026-09-10.md) | FEL-10 IF ownership dual-KEEP HT-1028∧HT-1033, soft no-gain, VOID bans |
| [`notes/critic-lessons-write-down-and-clones.md`](notes/critic-lessons-write-down-and-clones.md) | VOID patterns: clones, write-downs, pupil_in−k, hardcode pupil_err |

## Standing rules (champion short form)

- Card for this KEEP: **`coherence-if-v1` only** (not vs-LPP).
- Metric-reuse or conditioner byte-clone across ticket IDs → **VOID**.
- Reconstruct → correct toward pupil fill **0.72**; `pupil_err = |fill − 0.72|`; speckle from field coherence.
- Ban `abs(delta)*k` and `p_err*scale` knobs.
- vs-LPP comparative KEEP requires **`lpp-source-v2` BOUND** (1 kW floor); `lpp-source-v1` 250 W is VOID for that claim.
- Dual gate: Grok-lane + second-engine lane on identical frozen eval. Champion copy: **second-engine / mistral-lane** (ticket tag remains `mock-mistral`).

- FEL-10 dual: HT-1028 ∧ HT-1033 under HOLDOUT `d0dc1f8a…`; soft **no-gain** travels on 1033 (disclose).
- Ban `pupil_in−k` / hardcode `pupil_err` / `abs(delta)*k` write-downs on IF shim climbs.
