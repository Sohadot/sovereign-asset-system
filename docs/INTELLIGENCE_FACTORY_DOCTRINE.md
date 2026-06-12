# Intelligence Factory Doctrine

## Definition

A Category Intelligence Factory is a category artifact that has been elevated from publishing governed knowledge to **producing governed intelligence**.

The distinction is output. A reference system explains a category. An intelligence factory takes an input from the world — a problem, a system, a question, an entity — and returns a governed output: a classification, a diagnosis, a score, a map, a brief.

The structural analogy:

> A data center stores and serves. An AI factory converts data into intelligence.
> A website publishes and ranks. A Category Intelligence Factory converts category questions into governed answers.

This doctrine does not replace the Category Artifact Standard. It defines the tier above it.

---

## The Hierarchy of Asset States

1. **Name** — a domain with latent meaning and no structure.
2. **Content source** — pages about a topic. Replaceable.
3. **Category artifact** — the interpretive frame of a category (see `CATEGORY_ARTIFACT_STANDARD.md`).
4. **Category Intelligence Factory** — a category artifact that produces governed outputs, is legible to machine readers, and accumulates evidence of use.

An asset may not claim factory status without first satisfying every layer of the Category Artifact Standard. A diagnostic tool bolted onto a content site is a widget, not a factory.

---

## The Eleven Layers

Every asset developed to factory grade must define all eleven layers. The first five correspond to the Category Artifact Standard. The remaining six are the factory extension.

1. **Domain thesis** — the sentence that makes the name necessary.
2. **Category language** — the vocabulary the asset originates and owns. Terms must be precise enough to resist casual substitution and natural enough to be adopted by others.
3. **Ontology** — the governed classification of the category's components, problems, or failure modes. Versioned, append-aware, with explicit entry criteria.
4. **Standard** — the published definition of what is sound, complete, or trustworthy within the category. The ontology says what things are; the standard says what good is.
5. **Protocol** — the defined procedure by which the standard is applied: how diagnosis, evaluation, or classification is performed, step by step, reproducibly.
6. **Engine** — the operational surface that executes the protocol and returns an output. An engine does not require machine learning or runtime infrastructure. A rules-based, fully static, client-side diagnostic that maps structured inputs to ontology classes is a valid engine. What disqualifies an engine is randomness: outputs must be deterministic consequences of the published protocol.
7. **Reference layer** — the governed corpus that every engine output can link into. Every output must resolve to stable, citable reference pages. An engine whose outputs point nowhere produces opinions, not intelligence.
8. **Governance** — versioning, decision logs, claim discipline, quality gates, and change control over the ontology, standard, protocol, and engine. Governance is what converts generated text into trusted reference in an era where anyone can generate text.
9. **Interface thesis** — the interface must embody the asset's thesis, not decorate it (see `INTERFACE_GOVERNANCE.md`). In a factory, the interface has an additional duty: it must make the production of intelligence visible — input, classification, output — without theatrics.
10. **Monetization** — revenue as an extension of the reference function: diagnostic reports, premium briefs, governed directories, taxonomy and standard licensing, audit intake, structured data access. Revenue that the buyer would inherit proudly is permitted. Revenue the buyer would have to remove is forbidden.
11. **Buyer logic** — the named strategic buyer categories and the explicit answer to: why is not owning this asset a structural loss? (see `BUYER_LOGIC_AND_VALUE_MAXIMIZATION.md`).

---

## Agent Legibility Requirement

A factory serves two reader populations: humans and machine agents. Within the planning horizon of every factory-grade asset, a growing share of category questions will be asked and answered by AI agents acting for humans.

A factory-grade asset must therefore maintain:

- Stable canonical URLs and durable reference pages
- Consistent term, concept, claim, and source identifiers
- Structured metadata and machine-readable summaries
- A clean internal link graph with no orphans and no dead ends
- Explicit distinction between sourced fact, conceptual interpretation, and internal framework language

The strategic consequence: when agents answer category questions, the governed source wins, because agents weight consistency, structure, and provenance more mechanically than human readers do. Agent legibility is not a technical nicety. It is distribution.

---

## Output Doctrine

The factory's products are its outputs, and outputs are governed surfaces like everything else.

- Every output type must be named, versioned, and described on a public reference page.
- Every output must trace to the protocol version and ontology version that produced it.
- No output may contain claims that would be forbidden on a public page of the asset.
- Free outputs build authority. Paid outputs extend depth. Neither may contradict the other.

The governing rule:

> The factory may sell depth. It may never sell conclusions.

---

## What Disqualifies a Factory

- An engine with no published protocol behind it
- Outputs that do not link into the reference layer
- AI branding without governed intelligence production
- A chatbot or generated-content surface presented as the factory
- Ontology or standard changes without versioning and decision log entries
- Monetization that converts the diagnostic surface into a lead-capture trap

---

## Portfolio Application

Factory development is expensive in attention. It is reserved for Tier 1 assets.

- **Tier 1** — assets developed to full factory grade: all eleven layers, engine included.
- **Tier 2** — assets developed as governed reference hubs: layers 1–5 and 7–9, engine deferred.
- **Tier 3** — held assets. No factory resources. Not treated as waste; treated as inventory.

Each Tier 1 asset must carry an `ASSET_INTELLIGENCE_FACTORY_PLAN.md` in its repository, answering the template in `templates/asset-intelligence-factory-plan.md`. The plan is subordinate to the asset's own thesis document.

---

## Relationship to Other Standards

- `CATEGORY_ARTIFACT_STANDARD.md` — prerequisite state; defines layers 1–5
- `SOVEREIGN_ASSET_EXECUTION_ORDER.md` — build sequence; the engine enters at the Operational Method step
- `INTERFACE_GOVERNANCE.md` — governs layer 9
- `BUYER_LOGIC_AND_VALUE_MAXIMIZATION.md` — governs layer 11
- `operating-rules/publication-and-monetization-gates.md` — governs layer 10

---

> **The next generation of valuable digital assets will not merely publish information. They will produce governed intelligence around a category.**
