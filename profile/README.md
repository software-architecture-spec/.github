# Software Architecture Spec

An open specification for **SAM — Software Architecture Manifest**: a producer-signed, machine-readable declaration of what software was designed to do and the operational envelope it was designed for.

SBOM tells you what's *inside* the software. SLSA tells you *how* it was built. **SAM tells you what the producer designed it *to be*** — tenancy model, scaling axis, privilege posture, network requirements, and ISO/IEC 25010:2023 quality claims, with industry-standard cross-references for auditors.

## Live

- [software-architecture-spec.github.io](https://software-architecture-spec.github.io/) — landing page
- [SPECIFICATION v0.1](https://software-architecture-spec.github.io/sam/v0.1/SPECIFICATION.md) — normative reference, §§1–8
- [JSON Schema v0.1](https://software-architecture-spec.github.io/sam/v0.1/schema.json) — Draft 2020-12
- [Example: SaaS API](https://software-architecture-spec.github.io/sam/v0.1/examples/saas.manifest.json) · [Example: internal enterprise](https://software-architecture-spec.github.io/sam/v0.1/examples/internal-enterprise.manifest.json)

## Status

**v0.1 — working draft.** Breaking changes expected before v1.

## License

Dual-licensed: Apache-2.0 for code/schema/examples, CC-BY-4.0 for prose docs.

---

The current namespace is hosted under `software-architecture-spec.github.io` as a working draft. The intent is for this to live eventually with a neutral host (CNCF / OpenSSF / IETF working group); existing URIs will redirect when that move happens.
