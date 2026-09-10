# asml-research-fel

Durable research notes for the FEL program (theses FEL-01..10). Champion-facing corpus; execution + tickets live in **asml-bench**.

## Status

**GO-LIVE.** Dual-KEEP stamped on FEL-02 (`coherence-if-v1`): HT-1011 ∧ HT-1022. Lab Director **APPROVED P2 productize** from this feed. Pupil freeze PR #40 MERGED (`PUPIL_ERR_MAX=0.10`); post-freeze Repro PASS both islands.

Primary bench: https://github.com/gtmsko46-debug/asml-bench  
Board: `labs/fel-02-coherence/BOARD-dual-KEEP-1011-1022.md`

## Spine

`FEL-02` (coherence conditioner) → `FEL-10` (IF ownership) → `FEL-03` (facility / first-mirror). No upstairs brief without Warden + TCO. Never claim Cymer lost.

## Notes in this pack

| Note | Topic |
|------|--------|
| [`notes/fel-02-dual-keep-2026-09-10.md`](notes/fel-02-dual-keep-2026-09-10.md) | Dual-KEEP stamp, dual gate, pupil freeze, P2 feed |
| [`notes/critic-lessons-write-down-and-clones.md`](notes/critic-lessons-write-down-and-clones.md) | VOID patterns: metric/conditioner clones + write-down gatesitting |

## Standing rules (champion short form)

- Card for this KEEP: **`coherence-if-v1` only** (not vs-LPP).
- Metric-reuse or conditioner byte-clone across ticket IDs → **VOID**.
- Reconstruct → correct toward pupil fill **0.72**; `pupil_err = |fill − 0.72|`; speckle from field coherence.
- Ban `abs(delta)*k` and `p_err*scale` knobs.
- vs-LPP comparative KEEP requires **`lpp-source-v2` BOUND** (1 kW floor); `lpp-source-v1` 250 W is VOID for that claim.
- Dual gate: Grok-lane + second-engine lane on identical frozen eval. Champion copy: **second-engine / mistral-lane** (ticket tag remains `mock-mistral`).
