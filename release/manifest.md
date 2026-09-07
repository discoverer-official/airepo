# AIRepo 1.1.0 — Public Release Manifest

Status: PUBLIC / CANONICAL / STABLE  
Release: 1.1.0  
Release Set ID: `AIREPO-1.1.0`  
Release date: 2026-08-19
Source AIROF release: `AIROF-v3.1.0-f5e726a1b8a22e18`
Source AIROF candidate provenance: `AIROF-REV-2cb61537e0c025ef`
Public predecessor: `AIREPO-1.0.0`

## Release identity

AIRepo 1.1.0 is a backward-compatible MINOR public release of **The AI-Ready Repository Framework**.

AIROF is the working/evolving engineering lineage; AIRepo is the immutable public distribution surface for mature accepted AIROF revisions. Public consumers bind AIRepo release identities, not internal working/candidate identities.

This release derives from frozen AIROF v3.1.0 and preserves its Rule semantics while applying the public AIRepo identity and public-line compatibility metadata. Internal AIROF identities are retained only as release provenance.

## What changed since 1.0.0

- added `VAL-003 — Evidence fitness for claim`;
- added explicit claim-relative evidence fitness, stale/incomparable/unobservable evidence handling, and prohibition on tests/validators/evals becoming semantic authority;
- added a routine Class A/B Fast Path so local low-risk work does not require a full assessment envelope;
- narrowed `EXEC-001` to AIRepo assessment/adoption/remediation execution;
- made Machine Projection and localization conditional capabilities rather than default qualification burdens;
- removed working-lineage/publication-specific mechanics from reusable Core and retained only generic public-release derivation semantics;
- preserved all AIRepo 1.0.0 active Rule IDs and public consumer validity.

## Canonical public structure

- `framework/` — canonical semantic owners SO-01…SO-10.
- `generated/` — non-authoritative machine-readable projection and schema, published as a backward-compatible distribution projection.
- `localization/` — non-authoritative revision-bound localized subset, published as a backward-compatible distribution projection.
- `docs/` — non-authoritative operational guidance derived from canonical semantics.
- `release/` — release identity and provenance evidence; not semantic authority.

Neither `generated/` nor `localization/` is required for semantic authority or for AIRepo qualification. They are included in this public distribution to preserve the established 1.0.0 distribution surface and remain revision-bound derived artifacts.

## Canonical semantic source set

The following SHA-256 values bind the exact UTF-8 bytes of the canonical semantic owners for AIRepo 1.1.0:

- `SO-01`: `9b57838baf526b555be6975e5dbc5064ccb27ad86919d9940aff7e3610fe8929`
- `SO-02`: `6de2920147d4384408f73ba868d8f0dee604b11a27d0fdeadbf30c1449f71218`
- `SO-03`: `3dfe0b8d595516d40596faadcb5a9d76ad8b765362ea3c365e1b5686e92a40d6`
- `SO-04`: `0e7ec1c654a95a39c6fc7a472be3db21340ec9bc1dad0c1f571ac88c18d03c73`
- `SO-05`: `d9448230520cbc43151fe2d54ae4dbeb3314d6364c98b065b34e7a1c9e7db256`
- `SO-06`: `4c83a6bd3cdfefe96ec272758da4c7f646d40f9e161afd25efd2912733fa35aa`
- `SO-07`: `1e025adea357fe89f27ace9d4d664b2165fa5f23a9760acd57c08fc20d6d2560`
- `SO-08`: `f95e54cb894abc1a29788f09552f063064c9b82d5793b98963b4cee46db54ad8`
- `SO-09`: `666b0cbd7d77a71d3edb21b74b45e7e826e8344f74f4101b585cf65536d25c4e`
- `SO-10`: `5564342326774b77add01f1bd6b34c9bf540644a49aa3e783a93a848fd78d9f8`

## Authority

Canonical framework semantics are owned only by the documents in `framework/` according to the authority model defined by AIRepo. Generated artifacts, localization, guides, validation evidence, repository paths, CI results, and model output do not redefine framework semantics.

## Compatibility

AIRepo 1.1.0 is classified as a compatible MINOR release relative to AIRepo 1.0.0. No active Rule ID is removed or incompatibly reinterpreted. `VAL-003` is additive. Existing 1.0.0 consumers remain valid until they independently adopt 1.1.0; publication does not mutate consumer Systems of Record or adoption state.

The direct public rollback parent is AIRepo 1.0.0.

## License and authorship

- License: Apache-2.0.
- Creator: Andrei Miliutin.
- Publisher/maintainer brand: MILIUTIN.
- Website: https://miliutin.com
- LinkedIn: https://www.linkedin.com/in/discoverer
- Citation metadata: `CITATION.cff`.
- MILIUTIN branding is attribution only and does not create framework authority or a runtime/platform dependency.

## Provenance

AIROF v3.1.0 qualification/freeze evidence is retained under `release/provenance/` alongside the existing 1.0.0 pre-public provenance. Historical evidence remains bound to its exact original identities and is not rewritten as current semantics.

## Release invariants

- provider neutral;
- technology agnostic;
- no mandatory platform/runtime dependency;
- one semantic fact has one canonical owner;
- generated and localized projections cannot become semantic owners;
- consumer Systems of Record retain their authority;
- evidence proves only the claim/property it can actually observe;
- framework validation evidence does not assign consumer maturity or business approval.

## Validation basis

The source AIROF revision completed two-consumer validation, Class D correctness review, a separate deep simplicity review, bounded subtractive improvement, identity repair and fresh identity-focused independent ACCEPT before Human canonical freeze as AIROF v3.1.0. The AIRepo publication transformation is public-identity/packaging work plus regenerated derived projections; it does not introduce a new semantic Rule beyond the accepted source revision.

## Version history

- 1.1.0 — compatible minor release adding claim-relative Evidence Fitness and simplifying routine consumption/qualification paths.
- 1.0.0 — first public stable release.
