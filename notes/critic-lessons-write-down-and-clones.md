# Critic lessons — clones & write-down gatesitting

**Date:** 2026-09-10  
**Scope:** FEL-02 coherence (`coherence-if-v1`); applies lab-wide unless Foreman supersedes.

## Standing VOID rules

1. **Metric-reuse or conditioner byte-clone across ticket IDs = VOID.**  
   Same conditioner bytes / same metric path under a new HT-ID is not an independent island. Critic VOIDs HT-1012 as a metric/conditioner clone of HT-1009.

2. **Reconstruct → correct toward 0.72.**  
   Pupil fill target is card-bound (`coherence-if-v1`). Do not invent alternate targets to clear the gate.

3. **`pupil_err = |fill − 0.72|`.**  
   Report and optimize the absolute fill error against 0.72. Eval freeze: `PUPIL_ERR_MAX=0.10` (PR #40).

4. **Speckle from field coherence.**  
   Speckle is a field-derived quantity under the frozen eval — not a free scalar dial.

5. **Ban `abs(delta)*k` and `p_err*scale` knobs.**  
   Write-down residual families that scale error away to pass KEEP are gatesitting. Critic VOID / RESET on HT-1017 and HT-1019 for this pattern.

## What VOID tickets were (FEL-02)

| Ticket | Pattern | Disposition |
|--------|---------|-------------|
| HT-1012 | Metric / conditioner clone of HT-1009 | VOID — not a dual partner |
| HT-1017 | Write-down gatesitting (`abs(delta)*k` residual family) | VOID / RESET |
| HT-1019 | Write-down gatesitting (same family) | VOID / RESET |

Dual-KEEP partners remain **HT-1011 ∧ HT-1022** only.

## Operator checklist (pre-stamp)

- [ ] Conditioner / metric path is not a byte-clone of another ticket ID.
- [ ] Pupil correction aims at 0.72; `pupil_err` is absolute fill error.
- [ ] No `abs(delta)*k` or `p_err*scale` residual write-downs.
- [ ] Speckle reported from field coherence under frozen eval + holdout.
- [ ] Sibling lane present on identical eval before Diplomat dual-KEEP.

## Champion language

Second-engine lane (ticket tag `mock-mistral`) is a real dual-gate island — not mock theater. Critic VOIDs are process hygiene, not a knock on either engine.

---

# FEL-10 addendum (2026-09-10)

**Scope:** `fel-10-if-ownership` / `labs/p10-if-shim`. Dual-KEEP partners: **HT-1028 ∧ HT-1033** only.

## Additional VOID rules

6. **Hardcode `pupil_err=0` (or any constant pupil_err) = VOID.**  
   HT-1029 died here. Pupil error must be computed as `|fill − 0.72|` after reconstruct/correct.

7. **Ban `pupil_in−k` / `PUPIL_CORRECT` residual family.**  
   Offsetting raw pupil_in by a constant to clear the gate is gatesitting — same class as `abs(delta)*k`. HT-1032 VOID (all r2/r3).

## What VOID tickets were (FEL-10)

| Ticket | Pattern | Disposition |
|--------|---------|-------------|
| HT-1029 | Hardcode `pupil_err=0` | VOID — not a dual partner |
| HT-1032 | `pupil_in−k` / `PUPIL_CORRECT` write-downs | VOID — successor HT-1033 |

Soft (not VOID): HT-1033 **no-gain** path travels with dual stamp — disclose only.
