# Software Architecture Spec

An open specification for **SAM — Software Architecture Manifest**: a producer-signed, machine-readable declaration of what software was designed to do and the operational envelope it was designed for.

SBOM tells you what's *inside* the software. SLSA tells you *how* it was built. **SAM tells you what the producer designed it *to be*** — tenancy model, scaling axis, privilege posture, network requirements, operational dependencies, and ISO/IEC 25010:2023 quality claims, with industry-standard cross-references for auditors.

> **Working draft — not adoption-ready.** SAM is a v0 working proposal. Breaking changes are still possible; the stable target is v1. Engagement, technical review, and contributions welcome via [issues](https://github.com/software-architecture-spec/sam/issues) and [discussions](https://github.com/software-architecture-spec/sam/discussions).

## Live (v0.3 — current)

- [Landing page](https://software-architecture-spec.github.io/sam/) — rendered README
- [SPECIFICATION v0.3](https://software-architecture-spec.github.io/sam/v0.3/SPECIFICATION.md) — normative reference, §§1–10 (Scope, Terminology, Conformance language, Threat model, Conforming SAM incl. **§5.5 design-context vs. graded claims**, Versioning, Extensibility, Stability, **SAM Levels**, **Quality characteristic definitions** — SAM's own plain-English definitions for each ISO/IEC 25010:2023 characteristic, anchored to the ISO names; original wording, CC-BY-4.0, informative, not a reproduction of the ISO text)
- [JSON Schema v0.3](https://software-architecture-spec.github.io/sam/v0.3/schema.json) — Draft 2020-12; adds `intent.deliveryForm`, `intent.architecturalStyle`, `intent.architecturalPatterns[]`, storage & concurrency detail, and the `dependencies[].type` → `deliveryForm` + `role` split
- [Example: SaaS API](https://software-architecture-spec.github.io/sam/v0.3/examples/saas.manifest.json) · [Example: internal enterprise](https://software-architecture-spec.github.io/sam/v0.3/examples/internal-enterprise.manifest.json) · [Example: Caddy (illustrative OSS)](https://software-architecture-spec.github.io/sam/v0.3/examples/caddy.manifest.json)
- [Conformance test corpus](https://github.com/software-architecture-spec/sam/tree/main/v0.3/conformance) — positive and negative cases per §5.1
- [Registries](https://github.com/software-architecture-spec/sam/tree/main/registry) — `standards.json`, `tensions.json`, `delivery-forms.json`, `patterns.json` (advisory)

v0.1 and v0.2 are frozen and remain valid at their own URIs per §6.3. Future versions land alongside (`v0.4/`, `v0.5/`, …) at frozen URIs.

## Get involved

- [CONTRIBUTING.md](https://github.com/software-architecture-spec/sam/blob/main/CONTRIBUTING.md) — how to engage
- [ROADMAP.md](https://github.com/software-architecture-spec/sam/blob/main/ROADMAP.md) — feedback-driven future scope
- [Issue templates](https://github.com/software-architecture-spec/sam/issues/new/choose) — schema-change proposal, registry addition, bug report, real-world feedback

## Status

**v0.3 — current working draft.** Breaking changes still possible while `MAJOR` is `0`. v0.3 adds delivery form, architectural style / patterns, and storage / concurrency detail, and splits `dependencies[].type` into `deliveryForm` + `role` (§6.6). v0.1 and v0.2 are frozen; their manifests remain conforming under their own URIs. Stable target is v1.

## License

Dual-licensed: Apache-2.0 for code/schema/examples/conformance/registries, CC-BY-4.0 for prose docs.

---

The current namespace is hosted under `software-architecture-spec.github.io` as a working draft. The intent is for this to live eventually with a neutral host (CNCF / OpenSSF / IETF working group); existing URIs will redirect when that move happens.
