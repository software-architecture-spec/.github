# Software Architecture Spec

An open specification for **SAM — Software Architecture Manifest**: a producer-signed, machine-readable declaration of what software was designed to do and the operational envelope it was designed for.

SBOM tells you what's *inside* the software. SLSA tells you *how* it was built. **SAM tells you what the producer designed it *to be*** — tenancy model, scaling axis, privilege posture, network requirements, operational dependencies, and ISO/IEC 25010:2023 quality claims, with industry-standard cross-references for auditors.

> **Working draft — not adoption-ready.** SAM is a v0 working proposal. Breaking changes are still possible; the stable target is v1. Engagement, technical review, and contributions welcome via [issues](https://github.com/software-architecture-spec/sam/issues) and [discussions](https://github.com/software-architecture-spec/sam/discussions).

## Live (v0.1 — first public draft)

- [Landing page](https://software-architecture-spec.github.io/sam/) — rendered README
- [SPECIFICATION v0.1](https://software-architecture-spec.github.io/sam/v0.1/SPECIFICATION.md) — normative reference, §§1–9 (Scope, Terminology, Conformance language, Threat model, Conforming SAM, Versioning, Extensibility, Stability, **SAM Levels**)
- [JSON Schema v0.1](https://software-architecture-spec.github.io/sam/v0.1/schema.json) — Draft 2020-12
- [Example: SaaS API](https://software-architecture-spec.github.io/sam/v0.1/examples/saas.manifest.json) · [Example: internal enterprise](https://software-architecture-spec.github.io/sam/v0.1/examples/internal-enterprise.manifest.json)
- [Conformance test corpus](https://github.com/software-architecture-spec/sam/tree/main/v0.1/conformance) — positive and negative cases per §5.1
- [Registries](https://github.com/software-architecture-spec/sam/tree/main/registry) — `standards.json`, `tensions.json` (advisory)

Future versions land alongside (`v0.2/`, `v0.3/`, …) at frozen URIs per §6.3.

## Get involved

- [CONTRIBUTING.md](https://github.com/software-architecture-spec/sam/blob/main/CONTRIBUTING.md) — how to engage
- [ROADMAP.md](https://github.com/software-architecture-spec/sam/blob/main/ROADMAP.md) — feedback-driven future scope
- [Issue templates](https://github.com/software-architecture-spec/sam/issues/new/choose) — schema-change proposal, registry addition, bug report, real-world feedback

## Status

**v0.1 — working draft.** Breaking changes still possible while `MAJOR` is `0`. Stable target is v1.

## License

Dual-licensed: Apache-2.0 for code/schema/examples/conformance/registries, CC-BY-4.0 for prose docs.

---

The current namespace is hosted under `software-architecture-spec.github.io` as a working draft. The intent is for this to live eventually with a neutral host (CNCF / OpenSSF / IETF working group); existing URIs will redirect when that move happens.
