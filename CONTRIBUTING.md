# Contributing to AIRepo

Thank you for helping improve AIRepo. The framework is intentionally small and evidence-driven; contributions should improve a proven repository-facing engineering problem rather than expand scope for completeness.

## Before proposing a change

Please identify:

1. the consumer or reproducible failure mode;
2. the affected semantic owner or Rule ID;
3. supporting evidence or practice;
4. whether an existing rule, composition point, or external capability already addresses the need;
5. compatibility, migration, and authority impact.

## Contribution classes

- **Editorial / derived:** no semantic change.
- **Compatible clarification:** clarifies existing semantics without changing consumer obligations.
- **Material semantic / framework behavior:** changes requirements or materially changes behavior.
- **Authority / breaking / safety-critical:** changes authority boundaries, compatibility, or safety-critical behavior.

Assurance should be proportional to the highest applicable class. See `framework/SO-10.md`.

## Pull requests

A good pull request is bounded and includes:

- problem and evidence;
- affected files and Rule IDs;
- compatibility impact;
- validation performed;
- migration/rollback when required;
- confirmation that no project-specific assumption was promoted into reusable semantics.

Do not update generated or localized projections as independent semantic sources. They must remain derivable from canonical content and bound to exact source identity.

## Contributions and license

Unless explicitly stated otherwise, contributions intentionally submitted for inclusion are accepted under the Apache License 2.0, consistent with Section 5 of the license.
