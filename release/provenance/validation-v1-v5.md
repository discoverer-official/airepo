# AIROF v3.1 Working Candidate — V1–V5 Prototype Validation Evidence

Status: WORKING EVIDENCE / NON-CANONICAL  
Candidate Revision: `AIROF-v3.1.0-candidate-7ab910821b332f3a`  
Parent: frozen AIROF v3.0.0

## V1 — Machine projection completeness — PASS
- semantic owners represented: 10/10
- active Rule IDs represented: 28/28
- duplicate active Rule IDs: 0
- inherited v3.0.0 active Rules: 27/27
- new `EXEC-001`: active and owned by SO-04
- `EVAL-001`: reserved, not active
- `EVAL-002`: active
- all Rule owner references resolve

## V2 — Determinism — PASS
Normalized candidate machine projection SHA-256: `3c89a25f9e92ed6cad1ef5f8c6dea390762653f3a0d3becec5a63cd7ad5b9b68`.
Repeated normalized serialization from identical semantic input produces identical bytes/hash.

## V3 — Drift/staleness — PASS
A working-copy source-hash mutation without projection regeneration is detected deterministically as stale. The candidate contract fails closed on source-hash mismatch.

## V4 — Localization subset — PASS
Tested SO-01 and changed SO-04 in EN/RU bounded representations. Candidate metadata binds `AIROF-v3.1.0-candidate-7ab910821b332f3a`; SO-04 binds candidate source SHA. Stable identifiers including `EXEC-001`, `EVAL-001` and `EVAL-002` remain byte-identical across locales.

## V5 — Bounded batching — PASS (reproducible controlled experiment)
Executable experiment: `v5_bounded_batch_experiment.py`.

Scenario: four related repository changes share one authority owner, one approval boundary, one validation boundary and one rollback boundary. Validator rejects mixed intermediate states.

Micro-sliced mode:
- first independently validated micro-change creates ambiguous partial state;
- validation fails closed;
- deterministic rollback restores baseline.

Bounded-batch mode:
- all four changes applied as one execution unit;
- same validation boundary passes on complete target state;
- whole-unit rollback deterministically restores baseline.

Conclusion: where semantic/validation state is indivisible, mandatory micro-slicing is not only more expensive but invalid. `EXEC-001` correctly requires batching only when authority, approval, validation and rollback boundaries are shared; otherwise splitting remains mandatory.

## V1–V5 verdict
PASS.
