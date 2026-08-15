# AIROF v3.1 Working Candidate — Adversarial Qualification Review

Status: WORKING ASSURANCE / NON-CANONICAL  
Date: 2026-08-13

## Scope

Review prototype artifacts and V1–V7 evidence for:
- second source of truth;
- semantic loss;
- provider/tool coupling;
- localization authority inversion;
- mandatory tooling creep;
- batching governance weakening;
- evidence recursion;
- version inflation;
- consumer incompatibility.

## Findings

### AQ-01 — Second source of truth
PASS. Canonical v3.0.0 Manifest + Markdown remain authority; JSON is generated-only.

### AQ-02 — Semantic loss
PASS for prototype scope. Projection contains 10/10 SO identities and 27/27 active Rules; EVAL-001 remains reserved, EVAL-002 active.

### AQ-03 — Determinism/staleness
PASS. Normalized projection hash is reproducible; source-hash mutation invalidates projection.

### AQ-04 — Localization authority
PASS. Localized subsets are source-hash/release-bound and explicitly derived.

### AQ-05 — Provider/tool coupling
PASS. No provider-specific fields or mandatory external service/runtime.

### AQ-06 — Mandatory generator risk
PASS. Consumers may consume published projection or canonical Markdown and are not required to execute generator.

### AQ-07 — Batching governance
PASS WITH VALIDATION LIMITATION. Eligibility preserves authority/approval/validation/rollback conjunction, but current V5 efficiency evidence is a controlled model rather than live comparative execution.

### AQ-08 — Evidence closure recursion
FINDING, NON-BLOCKING TO DESIGN / BLOCKING TO FULL TWO-CONSUMER QUALIFICATION. Playbook adoption record is stale relative to its merged subject. AID demonstrates the preferred subject/evidence distinction. Candidate guidance should include Evidence Closure Non-Recursion.

### AQ-09 — Version classification
PASS. Changes remain additive/backward-compatible if no existing v3 Rule meaning is changed. v3.1.0 remains appropriate; v4 is not justified.

### AQ-10 — Over-engineering
PASS. Static JSON/schema/Markdown projections only; no DB, registry, API service, RAG/vector layer or dedicated runtime.

## Qualification verdict

`CONDITIONALLY QUALIFIED WORKING CANDIDATE`

Blocking framework-design findings: 0.  
Blocking release-qualification items: 2.

1. V5 must gain repository-grounded/live batching evidence sufficient to replace the model-only limitation.
2. Playbook V6 evidence integrity must be reconciled or independently closed against the exact adopted subject.

No Human Decision is required to remediate these two validation items because neither changes canonical v3.0.0 semantics or authority. Human Approval remains required only before eventual freeze/promotion of a fully qualified v3.1.0 candidate.

## Follow-up closure — 2026-08-13

The two release-qualification items above were subsequently remediated without changing frozen v3.0.0:

1. **V5 batching evidence — CLOSED.** `60 — V5 Reproducible Bounded Batch Experiment.md` replaces the model-only limitation with a reproducible controlled experiment. Micro-sliced execution fails closed on an invalid mixed intermediate state and deterministically rolls back; the bounded batch reaches the valid target state and deterministically rolls back as one unit.
2. **Playbook V6 evidence integrity — CLOSED FOR FRAMEWORK QUALIFICATION.** `61 — Playbook Independent Exact-Subject Closure Evidence.md` binds exact Playbook merge subject `0d97d9b7882bb962510a69bf37301942e23b7383` to successful post-merge Validation Scope #2452 / run `31567724050`. The stale local Playbook adoption record remains a consumer evidence-hygiene finding and is not rewritten.

Additional design correction: RFC working identifier `EXEC-BATCH-001` was normalized to `EXEC-001` to preserve the established `PREFIX-###` Rule-ID model before canonical adoption. Rule meaning is unchanged.

### Updated assurance verdict

`ADVERSARIAL ACCEPT — QUALIFIED WORKING CANDIDATE`

Unresolved blocking framework-design findings: 0.  
Unresolved release-qualification findings: 0.  
Non-blocking retained finding: Playbook local adoption evidence hygiene.

The candidate may be presented for Human freeze/promotion decision under SO-10. This review does not itself assign canonical release state.
