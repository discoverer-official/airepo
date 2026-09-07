# AIRepo

**The AI-Ready Repository Framework**  
**by MILIUTIN**

AIRepo is an open, provider-neutral framework for organizing software repositories so humans and AI agents can work with explicit authority, ownership, lifecycle, provenance, compatibility, and validation boundaries.

It is not a prescribed folder tree, an agent runtime, an orchestration platform, or a replacement for a project's own architecture and governance. It is a repository assessment and design framework for making repository-facing engineering work safer and more deterministic in AI-centred development.

## Why AIRepo

AI agents can generate code quickly, but repository structure often leaves critical questions implicit:

- Which artifact is authoritative?
- Who owns a semantic decision?
- What is durable state versus generated or transient output?
- Which rules actually apply to this repository?
- When is a structural change justified?
- What evidence is sufficient before an agent may make an authority-bearing claim or change?

AIRepo makes those boundaries explicit without imposing a universal technology stack or directory layout.

## Core model

The canonical framework is organized into ten semantic owners:

| ID | Responsibility |
|---|---|
| SO-01 | Framework Charter and Scope |
| SO-02 | Principles, Authority and Ownership |
| SO-03 | Semantic Model |
| SO-04 | Normative Rules |
| SO-05 | Adoption Profiles |
| SO-06 | Assessment and Repository Design Method |
| SO-07 | AI Agent Execution |
| SO-08 | Migration and Compatibility |
| SO-09 | Validation and Conformance |
| SO-10 | Release and Governance |

Start with [`framework/SO-01.md`](framework/SO-01.md), then use the [Quick Start](docs/QUICKSTART.md) for an assessment.

## Principles

- **Project authority wins.** Applying AIRepo does not make the framework part of a consumer project's authority hierarchy.
- **Semantic before physical.** Repository organization follows responsibility, ownership, consumers, lifecycle, and compatibility—not a preferred folder pattern.
- **Evidence must fit the claim.** Exact revision binding is necessary but not sufficient: evidence must be capable of observing the property/boundary being claimed. Missing, stale, incomparable, or unobservable evidence cannot be promoted to PASS.
- **Minimal structural change.** Preserve acceptable organization and introduce structure only for real consumers or reproducible failure modes.
- **Provider and technology neutrality.** AIRepo does not depend on a specific LLM, repository host, language, runtime, or project-management system.
- **Generated views are not authority.** Machine-readable and localized projections are derived from canonical semantic owners and must detect staleness.

## Release 1.1.0

`1.1.0` is a backward-compatible minor release derived from the accepted AIROF v3.1.0 working lineage. It adds claim-relative Evidence Fitness (`VAL-003`) and simplifies routine usage through a Class A/B Fast Path while preserving all 1.0.0 active Rule IDs and consumer validity.

Canonical public semantics live only in [`framework/`](framework/).

- [`release/manifest.md`](release/manifest.md) binds the exact canonical source hashes and source AIROF release provenance.
- [`generated/airepo.machine.json`](generated/airepo.machine.json) is a non-authoritative deterministic machine projection published to preserve the established public distribution surface.
- [`localization/`](localization/) contains revision-bound localized projections published as an optional distribution surface.
- [`release/provenance/`](release/provenance/) contains historical qualification/freeze evidence.

Machine and localized projections are not required for AIRepo semantic authority or qualification. They are included in this public distribution for compatibility and convenience.

## Machine consumption

Agents and tools may consume [`generated/airepo.machine.json`](generated/airepo.machine.json) for discovery, stable identities, applicability metadata, and validation support. Canonical Markdown remains authoritative; the machine projection must fail validation when its manifest or source hashes become stale.

## Adoption

AIRepo can be used in three broad ways:

1. **Read-only assessment** — evaluate an existing repository and produce evidence-backed findings without modifying it.
2. **Repository design** — propose the smallest structural changes required to resolve proven failure modes.
3. **Adoption** — bind an exact AIRepo revision to a project-owned profile while preserving the project's own authority and Systems of Record.

See [`docs/QUICKSTART.md`](docs/QUICKSTART.md).

## Contributing

Issues and pull requests are welcome. Contributions must preserve explicit authority boundaries, technology/provider neutrality, stable rule identity, evidence-backed reasoning, and proportional complexity. See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## Security

Do not submit secrets, credentials, customer data, production traces, personal data, or protected project decisions. See [`SECURITY.md`](SECURITY.md).

## Citation and authorship

AIRepo was created by **Andrei Miliutin** and published under the **MILIUTIN** brand.

- Website: <https://miliutin.com>
- LinkedIn: <https://www.linkedin.com/in/discoverer>
- Citation metadata: [`CITATION.cff`](CITATION.cff)

MILIUTIN is the creator/publisher brand, not a framework dependency or authority source.

## License

Licensed under the **Apache License 2.0**. See [`LICENSE`](LICENSE) and [`NOTICE`](NOTICE).
