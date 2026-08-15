# AIRepo 1.0.0 — Public Release Manifest

Status: PUBLIC / CANONICAL / STABLE  
Release: 1.0.0  
Release Set ID: `AIREPO-1.0.0`  
Release date: 2026-08-15

## Release identity

AIRepo 1.0.0 is the first public release of **The AI-Ready Repository Framework**.

Public versioning starts at 1.0.0. Earlier `AIROF` identifiers were pre-public development, validation, and staging identities and are not public predecessor releases.

The public release preserves the semantic model, stable Rule IDs, authority boundaries, and validated behavior of the qualified pre-public lineage while changing the public project identity to AIRepo. Historical validation records remain unmodified under `release/provenance/`.

## Canonical public structure

- `framework/` — canonical semantic owners SO-01…SO-10.
- `generated/` — non-authoritative machine-readable projection and schema.
- `localization/` — non-authoritative revision-bound localized projections.
- `docs/` — non-authoritative operational guidance derived from canonical semantics.
- `release/` — release identity, publication assessment, and provenance evidence; not semantic authority.

## Canonical semantic source set

The following SHA-256 values bind the exact UTF-8 bytes of the canonical semantic owners for AIRepo 1.0.0:

- `SO-01`: `d2ffa9ea94ea7063493b9999aebe3ec7cdce20e8c8648f0ed734b7d08d3ea79b`
- `SO-02`: `7887cd04d4feb204e024e663115aa9478459dd549e063da5a3a7883f78022531`
- `SO-03`: `956eaf58a05ae59ad141e9777e11d240555f4d8dad9124c23d3d3dd739d8a217`
- `SO-04`: `fbf4768ea281b2ed05c9e04f55c472db24e75a1d9e7b54a4b9decae11cd22282`
- `SO-05`: `be8f76f4709ca33a47d389245ba83e699041331d34449f380f100c0009e6a272`
- `SO-06`: `e0de803648f113ee97b46ac60073109a8592b7cdb0025e3c3a295597394cadb6`
- `SO-07`: `f18b3c3c176e66c06d904ce61144458477191ecc9a2fe45a10964c64a60ab651`
- `SO-08`: `83e4d9a0010a5f00de1afcc1fcce3de8b757c871d66031ff4fafca75e2eed108`
- `SO-09`: `69d06c59f30f26789c4da4999dea8c5309226c456677d905558a010b06f7788e`
- `SO-10`: `629b217d363969729d3c668d6182d112bdabc4d5decefeee7c58def73408bf7b`

## Authority

Canonical framework semantics are owned only by the documents in `framework/` according to the authority model defined by AIRepo. Generated artifacts, localization, guides, validation evidence, repository paths, CI results, and model output do not redefine framework semantics.

## License and authorship

- License: Apache-2.0.
- Creator: Andrei Miliutin.
- Publisher/maintainer brand: MILIUTIN.
- Website: https://miliutin.com
- LinkedIn: https://www.linkedin.com/in/discoverer
- Citation metadata: `CITATION.cff`.
- MILIUTIN branding is attribution only and does not create framework authority or a runtime/platform dependency.

## Compatibility and provenance

Pre-public AIROF validation and qualification records are retained as immutable provenance under `release/provenance/`. Public consumers MUST NOT depend on historical AIROF paths or identifiers.

## Release invariants

- provider neutral;
- technology agnostic;
- no mandatory platform/runtime dependency;
- one semantic fact has one canonical owner;
- generated and localized projections cannot become semantic owners;
- consumer Systems of Record retain their authority;
- framework validation evidence does not assign consumer maturity or business approval.

## Validation basis

The semantic lineage promoted into this release completed semantic completeness, deterministic projection/staleness validation, localization validation, bounded-batch execution validation, two independent consumer validations, and independent qualification review before public assembly. The branding/publication transformation is editorial with regenerated hashes and derived projections.

## Version history

- 1.0.0 — first public stable release.
