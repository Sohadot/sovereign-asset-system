# Asset Intelligence Factory Plan — Template

> Copy into the asset repository as `ASSET_INTELLIGENCE_FACTORY_PLAN.md`.
> This document is subordinate to the asset's thesis document.
> Governed by `docs/INTELLIGENCE_FACTORY_DOCTRINE.md`.

---

**Asset:** `domain.tld`
**Portfolio tier:** Tier 1
**Plan version:** 0.1
**Status:** Draft / Approved
**Governing document:** `ASSET_THESIS.md`

---

## 1. Category Ownership

What category does this asset own? One sentence. If the category cannot be named in one sentence, the asset is not ready for factory development.

## 2. Category Language

The vocabulary the asset originates. List the core terms, each with a one-line definition. Mark which terms are original to the asset and which are inherited from the field.

## 3. Ontology

Name the ontology. Define its scope, its top-level classes, the entry criteria for a class, and the versioning rule. State what the ontology classifies: components, problems, failure modes, or entities.

## 4. Standard

Name the standard. State what property it governs (integrity, safety, completeness, trustworthiness). List its criteria at headline level.

## 5. Protocol

Name the assessment or diagnostic procedure. Describe inputs, steps, and the form of the result. The protocol must be reproducible: two competent operators applying it to the same input must reach the same classification.

## 6. Engine

Describe the operational surface that executes the protocol. State explicitly:

- Phase 1 form (must comply with the asset's security and runtime doctrine)
- What input it takes
- What output it returns
- Which ontology class pages each output links to
- What is deferred to later phases (API, scoring service, data products)

## 7. Respectable Income

List the permitted revenue outputs in phase order, mapped to the asset's monetization doctrine. For each: what is sold, to whom, and why it raises rather than lowers trust.

## 8. Strategic Buyer

List buyer categories. For the top three: what existing problem of theirs does this asset answer?

## 9. The Loss Question

Why is not acquiring this asset a structural loss? Answer in terms of what cannot be rebuilt quickly: name, language, ontology, accumulated reference, link graph, governance record, agent-legibility footprint.

## 10. Interface Embodiment

How does the interface embody the thesis? Name the one interaction or visual system that makes the thesis felt, and confirm it passes the mandatory interface test in `INTERFACE_GOVERNANCE.md`.

## 11. Execution Sequence

The ordered, finite list of next builds. Each entry must be completable and verifiable. No entry may depend on an unapproved layer.

---

**Decision log reference:** entry required in `DECISION_LOG.md` when this plan is approved or versioned.
