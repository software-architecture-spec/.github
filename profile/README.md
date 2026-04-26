# Software Architecture Spec

An open specification for **SAM — Software Architecture Manifest**: a producer-signed, machine-readable declaration of what software was designed to do and the operational envelope it was designed for.

SBOM tells you what's *inside* the software. SLSA tells you *how* it was built. **SAM tells you what the producer designed it *to be*** — tenancy model, scaling axis, privilege posture, network requirements, operational dependencies, and ISO/IEC 25010:2023 quality claims, with industry-standard cross-references for auditors.

> **Working draft — not adoption-ready.** SAM is a v0 working proposal. Breaking changes are still possible; the stable target is v1. Engagement, technical review, and contributions welcome via [issues](https://github.com/software-architecture-spec/software-architecture-spec.github.io/issues) and [discussions](https://github.com/software-architecture-spec/software-architecture-spec.github.io/discussions).

## Live (v0.2 — current)

- [software-architecture-spec.github.io](https://software-architecture-spec.github.io/) — landing page
- [SPECIFICATION v0.2](https://software-architecture-spec.github.io/sam/v0.2/SPECIFICATION.md) — normative reference, §§1–9 (Scope, Terminology, Conformance language, Threat model, Conforming SAM, Versioning, Extensibility, Stability, **SAM Levels**)
- [JSON Schema v0.2](https://software-architecture-spec.github.io/sam/v0.2/schema.json) — Draft 2020-12
- [Example: SaaS API](https://software-architecture-spec.github.io/sam/v0.2/examples/saas.manifest.json) · [Example: internal enterprise](https://software-architecture-spec.github.io/sam/v0.2/examples/internal-enterprise.manifest.json)
- [Conformance test corpus](https://github.com/software-architecture-spec/software-architecture-spec.github.io/tree/main/sam/v0.2/conformance) — positive and negative cases per §5.1
- [Registries](https://github.com/software-architecture-spec/software-architecture-spec.github.io/tree/main/registry) — `standards.json`, `tensions.json` (advisory)

v0.1 frozen at [`/sam/v0.1/`](https://software-architecture-spec.github.io/sam/v0.1/SPECIFICATION.md) and remains valid per §6.3 same-MAJOR compatibility.

## Get involved

- [CONTRIBUTING.md](https://github.com/software-architecture-spec/software-architecture-spec.github.io/blob/main/CONTRIBUTING.md) — how to engage
- [ROADMAP.md](https://github.com/software-architecture-spec/software-architecture-spec.github.io/blob/main/ROADMAP.md) — feedback-driven future scope
- [Issue templates](https://github.com/software-architecture-spec/software-architecture-spec.github.io/issues/new/choose) — schema-change proposal, registry addition, bug report, real-world feedback

## Status

**v0.2 — working draft.** Breaking changes still possible while `MAJOR` is `0`. Stable target is v1.

## License

Dual-licensed: Apache-2.0 for code/schema/examples/conformance/registries, CC-BY-4.0 for prose docs.

---

The current namespace is hosted under `software-architecture-spec.github.io` as a working draft. The intent is for this to live eventually with a neutral host (CNCF / OpenSSF / IETF working group); existing URIs will redirect when that move happens.
