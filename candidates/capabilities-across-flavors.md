# Cross-flavor capabilities — product, capability and mechanism

**Status:** candidate conceptual distinction (2026-10-14), not an adopted PResolver product architecture.

## Observation motivating the proposal

VSlices has a concrete operational product, **Tooling**. TDidacta has **Platform**. Their domain-facing responsibilities are different, but both may need to transform governed semantic inputs into examinable realizations or presentations.

The specific initiating example was **documentary continuity**: a Docs Standard semantic structure with relationships may be interpreted or expressed through Framework-level representations, then rendered or realized through a domain-dependent mechanism. Whether Framework must be an intermediate stage in either flavor is **not established**.

The similarity suggests investigating a cross-flavor **capability** rather than asserting that either flavor should be renamed to a common Tooling/Platform product.

## Candidate distinctions

- **Product:** a responsibility-bearing conceptual boundary with its own authority and evolution.
- **Capability:** an ability to accomplish a bounded outcome under stated inputs, constraints and examinable guarantees. It may be contributed by several products rather than exclusively owned by one.
- **Mechanism:** a way of realizing or supporting that capability in a particular setting; multiple mechanisms may exist.
- **Surface:** a domain-appropriate encounter, interface or operational presentation through which the capability is used or observed.

These are working terms. Their independence and relationship to existing PResolver/VSlices/TDidacta terms remain to be tested.

## Candidate example: semantic projection

A deliberately incomplete sketch:

```text
source meaning / documentary relations
  -> admitted interpretation or representation (possibly Framework)
  -> capability: project while conserving material semantic distinctions
       -> VSlices: Tooling mechanisms and output surfaces
       -> TDidacta: Platform mechanisms and pedagogical surfaces
  -> evidence of what was preserved, changed, unsupported or lost
```

This **does not** assert an obligatory Docs Standard -> Framework -> Tooling/Platform pipeline. Some targets may legitimately bypass an intermediate model or involve other owners. Nor does one shared capability absorb all domain-specific responsibilities of either product.

### Responsibility questions

1. **Docs Standard:** Which documentary identities, questions, relations and guarantees are authoritative in the relevant flavor?
2. **Framework:** Which, if any, target-independent operational representations are justified for this transformation?
3. **Projection capability:** What is the minimal independently meaningful contract: admitted source, target context, preservation obligations, unknowns and observable results?
4. **Tooling / Platform:** Which mechanisms realize that contract without redefining the source meaning?
5. **Consumer / actor:** Who is authorized to assert that a resulting projection is adequate for the domain?

## Competing explanations

- A genuinely common capability exists at PResolver level.
- The products share only superficial terminology; their preservation criteria differ materially.
- A narrower reusable relation exists (for example, reconstruction, admissibility or provenance) without a universal projection capability.
- The capability exists, but belongs to a composition of responsibilities rather than a single base product.
- Some mechanisms are domain-specific and do not warrant extraction.

A flavor is not obliged to reproduce Method, Design, Docs Standard and Framework simply because those names recur in the family.

## Minimal test strategy

Start with one narrowly scoped documentary relation or intended transformation in each flavor. Define each case's source authority, required distinctions, admissible change, evidence and failure conditions **before** abstracting. Test each locally; then compare the contracts without using shared names as proof. Only then test chained/composed projections, including cases where local success fails globally. Seek at least one hostile counterexample.

If a reusable contract survives, consider candidate promotion into PResolver while preserving ownership of flavor-specific definitions and realizations. If it does not, preserve the contrast rather than manufacture uniformity.

## Research and ownership boundaries

- [VSlices Suite](https://github.com/the-alive-lab/vslices) is canonical for VSlices conceptual identity and product boundaries.
- [VSlices Tooling](https://github.com/the-alive-lab/vslices/blob/main/products/tooling/README.md) owns its specific operational meaning.
- [TDidacta](https://github.com/the-alive-lab/tdidacta) and [TDidacta Platform](https://github.com/tdidacta/platform) own their respective semantics and realizations.
- [XFR-STU-001 supervised case S](https://github.com/vslices/research-space/blob/main/lines/cross-flavor-resolution/studies/stu-001-transferencia-tdidacta/12-caso-s-supervisado-presolver-kcollectiva.md) governs its own transfer study; this note does **not** claim to execute or supersede that study.
- [PResolver historical project definition](https://github.com/vslices/ideas/blob/main/proyectos/p-resolver/README.md) remains the current conceptual starting authority until explicit adoption.

## Open decision

Should PResolver **own a catalog of capabilities**, **provide a process to discover and test generalizable capabilities**, or do both under distinct responsibilities?

Do not settle that question by defining PResolver as an 'extractor' only because cross-flavor comparison first exposed the opportunity.
