# AIRepo Quick Start

This guide is a non-authoritative operational projection of the canonical method in `framework/SO-06.md` and conformance semantics in `framework/SO-09.md`. If this guide conflicts with the canonical framework, the canonical semantic owners win.

## 1. Freeze the assessment subject

Resolve the target project's authority chain and identify the exact repository revision and evidence snapshot being assessed.

## 2. Identify active consumers and material assets

Inventory only repository surfaces that have an active consumer or a reproducible failure mode. Do not create speculative structure to satisfy AIRepo.

## 3. Classify the current state

For each material asset resolve, where applicable:

- semantic responsibility;
- authority owner;
- canonical System of Record;
- active consumer;
- lifecycle and durability;
- confidentiality/access class;
- compatibility boundary;
- generated versus manually owned state.

## 4. Resolve rule applicability

Use `framework/SO-04.md`. For every relevant Rule ID classify applicability as `applicable`, `not applicable`, or `unresolved`. A rule is not `not applicable` merely because evidence is missing.

## 5. Acquire evidence read-only and check fitness

When evidence is missing, stale, or ambiguous, acquire it read-only where safely possible. Do not convert missing evidence into an authority-bearing conclusion.

For a material Claim, confirm that the evidence binds the claimed subject at the needed precision and that the verification method can actually observe the property or boundary being claimed. A green test, mock, report, or exact SHA does not prove a broader property it cannot observe.

## 6. Record results

Use the validation results defined by `SO-09`:

- `satisfied`;
- `approved deviation`;
- `non-compliant`;
- `insufficient evidence`;
- `conflict`.

A useful finding records the Rule ID, exact evidence, current-state classification, failure mode, impact, and smallest safe target change.

## 7. Design the smallest change

Before adding a new directory, registry, manifest, validator, workflow, System of Record, or ownership layer, ask whether naming, navigation, configuration, composition, an existing contract, or an external capability already solves the problem.

Escalate to a full complexity review only when the proposal materially changes structural/lifecycle ownership, canonical locations, compatibility, validation, migration, operational support, or confidentiality controls.

## 8. Respect implementation authority

An assessment may propose remediation, but it does not authorize mutation. Apply changes only in a project-authorized implementation mode.

## 9. Validate closure

A completed assessment or adoption should leave:

- exact subject identity;
- per-rule applicability and evidence;
- explicit unresolved conflicts;
- migration/rollback where required;
- validation evidence;
- only the Human Decisions that existing authority genuinely requires.

## Routine Fast Path

For Class A/B low-risk work that does not touch authority, compatibility, safety, behavior/reproducibility, cross-revision evidence reuse, or Class C/D semantics, use the smallest path:

`authority as needed → concrete failure → applicable Rule → smallest change → focused validation → done`

Escalate to the full Claim/Evidence Fitness path only when the excluded concerns become material or a PASS is contested/materially relied upon.
