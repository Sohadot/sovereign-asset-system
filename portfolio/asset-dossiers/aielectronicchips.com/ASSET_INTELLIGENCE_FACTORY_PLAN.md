# Asset Intelligence Factory Plan — aielectronicchips.com

> Copy of `templates/asset-intelligence-factory-plan.md`, completed for this asset.
> This document is subordinate to the asset's own thesis document
> (`CATEGORY_THESIS.md` in the `aielectronicchips` repository).
> Governed by `docs/INTELLIGENCE_FACTORY_DOCTRINE.md`.
>
> **Repository:** `Sohadot/aielectronicchips` (separate repo; this dossier is the
> portfolio-level registration and cross-reference, not a duplicate of the
> asset's own governance files).

---

**Asset:** `aielectronicchips.com`
**Portfolio tier:** Tier 1 — Sovereign Build Candidate
**Plan version:** 1.0
**Status:** Active — Layers 1–5, 7, 8, 11 built; Layer 9 partially built; Layers 6 and 10 in progress
**Governing document:** `CATEGORY_THESIS.md` (asset repo)

---

## 0. Orientation

This dossier registers `aielectronicchips.com` inside the Sovereign Asset
System portfolio. The asset was developed directly against this system's
doctrine — `INTELLIGENCE_FACTORY_DOCTRINE.md`, `CATEGORY_ARTIFACT_STANDARD.md`,
`INTERFACE_GOVERNANCE.md`, `BUYER_LOGIC_AND_VALUE_MAXIMIZATION.md`, and
`SOVEREIGN_ASSET_EXECUTION_ORDER.md` — over eight governed sprints, each
recorded in `DECISION_LOG.md` in the asset's own repository. It is the most
structurally advanced Tier 1 candidate in the portfolio to date: it already
carries a governed ontology, a responsible-interpretation standard, a
dependency-mapping model, a source registry, a claim boundary matrix, and a
public reference surface of thirteen indexable routes — all built before any
monetization surface was introduced, in compliance with the Execution Order's
"Revenue as Consequence" doctrine.

What remains is the factory-defining step: the Engine (Layer 6) has a
published protocol and data model but no live operational surface yet, and
distribution (custom domain, GitHub Pages) is prepared but not switched on.
This dossier exists to make that gap explicit and trackable at the portfolio
level, and to set the execution sequence that closes it.

---

## 1. Category Ownership

**AI Chip Sovereignty Intelligence** — the disciplined study of who can
design, produce, access, power, deploy, and sustain the physical systems
required for AI compute.

The asset owns the question *"what determines who can actually operate AI
compute, and where is that ability exposed?"* — reframing AI infrastructure
away from chip news and product comparison and toward governed dependency
analysis.

---

## 2. Category Language

- **Compute Sovereignty (O)** — the practical ability to design, produce,
  access, power, deploy, and sustain AI compute, independent of ownership
  narrative or national branding.
- **Silicon Sovereignty Stack (O)** — the eight-layer ontology (Design,
  Fabrication, Packaging, Memory, Interconnect, Power/Thermal, Export-Control,
  Deployment) through which compute dependency is read.
- **Dependency Exposure (O)** — a layer-specific condition of reliance that
  can be described without collapsing into a single sovereignty score.
- **Exposure Types (O)** — concentration, access, capacity, technology,
  operational, and evidence exposure; the vocabulary for naming *why* a layer
  is exposed.
- **Dependency States (O)** — Direct, Layered, Constrained, Opaque, Not
  Assessable; the five non-numeric states used to describe a dependency
  relationship at any layer, defined in `CHIP_DEPENDENCY_MAP_MODEL.md`.
- **Chip Dependency Map (O)** — the governed diagnostic instrument (model
  published; engine pending) that reads a case against the ontology and
  standard and returns exposure types, dependency states, and confidence —
  never a score or ranking.
- **Evidence Posture (F)** — inherited concept, given governed levels (High /
  Medium / Low / Insufficient) under `COMPUTE_SOVEREIGNTY_STANDARD.md`.

Discipline rule: the asset explicitly refuses "Sovereignty Score,"
"ranking," or "maturity grade" as vocabulary — `CHIP_DEPENDENCY_MAP_MODEL.md`
names this exclusion directly. The category language is deliberately
score-resistant; that restraint is itself the differentiator against chip
media and vendor-funded index products, which compete on rankings.

---

## 3. Ontology

**Name:** Compute Sovereignty Ontology v1 (`COMPUTE_SOVEREIGNTY_ONTOLOGY.md`).

**Scope:** Eight dependency layers — Design, Fabrication, Packaging, Memory,
Interconnect, Power/Thermal, Export-Control, Deployment — each with a
governing question, a public reference route, and example dependency
signals. Six cross-layer exposure types classify *why* a dependency exists
independent of layer.

**Entry criteria:** A layer enters only if it names a distinct capability
required to operate AI compute at scale, maps to at least one public
reference route, and can carry a dependency record (`entity`, `layer`,
`dependency`, `criticality`, `substitutability`, `evidence`, `confidence`,
`as_of`).

**Versioning rule:** Versioned (currently v1.0.0), append-aware, governed by
`DECISION_LOG.md` ADR entries in the asset repository.

**Interpretation rule:** No layer is sovereign in isolation — control at one
layer does not offset exposure at another. This rule is the ontology's
structural defense against the single-score reduction that would otherwise
be commercially tempting.

---

## 4. Standard

**Name:** Compute Sovereignty Standard v1 (`COMPUTE_SOVEREIGNTY_STANDARD.md`,
model ID `AEC-CS-001`).

**Property governed:** responsible interpretation of layer exposure —
what may and may not be concluded from evidence about a given layer.

**Headline structure:** four non-numeric evidence posture levels (High /
Medium / Low / Insufficient) applied across eight standard dimensions
matching the ontology layers. The standard explicitly forbids assigning
sovereign status to any entity, country, or company.

---

## 5. Protocol

**Name:** Chip Dependency Map Model v1 (`CHIP_DEPENDENCY_MAP_MODEL.md`,
model ID `AEC-CDM-001`), backed by `DEPENDENCY_RECORD_SCHEMA.md` and
`CHIP_DEPENDENCY_MAP_PROTOCOL.md`.

**Inputs:** a bounded entity, decision, and time horizon; structured
dependency records citing the governed source registry
(`data/source-registry.json`).

**Steps:** map the case to one or more ontology layers → classify each
layer's dependency using one of five states (Direct, Layered, Constrained,
Opaque, Not Assessable) → attach an exposure type → attach evidence posture
and confidence under the Standard → preserve layer separation in the output.

**Result form:** a layered, non-numeric exposure read-out with sources,
confidence, and explicit unknowns — never a single score.

**Reproducibility:** the model is fully deterministic and rules-based by
design (`CHIP_DEPENDENCY_MAP_MODEL.md` "What the Model Does Not Do" bars any
scoring, ranking, or maturity-grade output), so two operators applying it to
the same sourced case should reach the same layered classification. This has
been specified but not yet tested against independent operators — see
Execution Sequence item 1.

---

## 6. Engine

**Status: specified, not yet operational.** This is the asset's single
largest gap against factory grade.

- **Phase 1 form:** a fully static, client-side, rules-based form-to-output
  tool is the correct Phase 1 shape under `INTELLIGENCE_FACTORY_DOCTRINE.md`
  ("a rules-based, fully static, client-side diagnostic... is a valid
  engine"). No backend, no LLM, no chatbot — the doctrine and the asset's own
  `INTERFACE_THESIS.md` both prohibit dressing this up as an AI feature.
- **Input:** a small structured form matching `DEPENDENCY_RECORD_SCHEMA.md`
  (entity type, layer(s) in question, known dependencies, available
  evidence).
- **Output:** dependency layers touched, exposure type(s), dependency
  state(s), confidence level, and a suggested brief type — exactly the
  "First Tool Boundary" already specified in the asset's own
  `ASSET_INTELLIGENCE_FACTORY_PLAN.md` and `data/chip-dependency-model.json`.
- **Reference linkage:** every output must resolve to the matching ontology
  layer page (`/design-fabrication-packaging/`, `/hbm-memory/`, etc.) and to
  `/methodology/` for confidence interpretation — the model and route map
  already exist to support this.
- **Deferred to later phases:** scored API access, structured data product,
  entity-specific published dependency maps (explicitly deferred by
  `CHIP_DEPENDENCY_MAP_MODEL.md` itself, "not... in Sprint 8").

Until the engine ships, `/chip-dependency-map/` is a reference page about a
future tool, not a factory output. That is an honest and doctrine-compliant
Sprint 8 state, but it is the next required build to cross from Category
Artifact into Category Intelligence Factory.

---

## 7. Respectable Income

Per `MONETIZATION_BOUNDARY.md` in the asset repository, in phase order:

1. **Compute Sovereignty Briefs** — paid, concise, decision-oriented
   assessments for a named entity/decision/time horizon. Sellable today via
   qualified inquiry even before the engine ships, since the Asset
   Intelligence Factory production pipeline (source → claim → ontology
   mapping → confidence review → bounded artifact) is already defined.
2. **Chip Dependency Audits** — scoped reviews of an organization or sector,
   sold to advisory firms, investors, and infrastructure buyers who need a
   defensible written exposure read rather than a public score.
3. **Premium Reference Dossiers** — deep single-layer artifacts (e.g. an HBM
   supply dossier), extending the free reference layer without contradicting
   it.
4. **Ontology / Standard licensing** — once adoption signals exist (see
   Layer 11 loss question), licensing the Compute Sovereignty Ontology and
   Standard vocabulary to advisory or research firms.
5. **Governed API access** — deferred until engine output volume and
   maintenance process are proven; explicitly gated in
   `MONETIZATION_BOUNDARY.md` ("Release Gate").

Each of these is revenue the buyer would inherit proudly: none require
removing a feature or retracting a claim before a strategic acquirer could
put its name behind the asset. Currently, only the qualified-inquiry mailto
pathway on `/strategic-availability/` is live; briefs 1–2 above are sellable
now without further engineering and are the fastest respectable-income path
while the engine is built.

---

## 8. Strategic Buyer

Per `BUYER_LOGIC.md` in the asset repository:

1. **Semiconductor / supply-chain intelligence and advisory firms** — this
   asset answers their recurring client question ("where is our AI compute
   exposed?") with a governed vocabulary and method they do not currently
   own; acquiring it buys a category vocabulary, not just traffic.
2. **Cloud, data-center, and compute operators** — need a neutral, non-vendor
   framework to brief their own executives and boards on infrastructure
   dependency without relying on a competitor's or supplier's narrative.
3. **Sovereign funds, institutional investors, and policy/geopolitical
   research organizations** — need citable, evidence-bounded language for AI
   infrastructure exposure that does not carry the liability of an
   unsupported ranking; the Claim Boundary Matrix and Source Policy are
   exactly the underwriting an institutional buyer would otherwise have to
   build itself.

---

## 9. The Loss Question

Not acquiring this asset means leaving unclaimed:

- **The name and the category sentence.** "AI chips are the physical
  substrate of compute sovereignty" is a specific, ownable thesis distinct
  from generic "AI chip news" framing — a competitor would have to
  out-position it, not just out-spend it.
- **The vocabulary.** Terms like Compute Sovereignty, Silicon Sovereignty
  Stack, and Dependency Exposure are original to this asset. If a rival
  publishes first with a competing vocabulary and it gets cited, this asset's
  language advantage is permanently reduced.
- **The governed accumulation.** Eight sprints of ADR-logged decisions, a
  claim boundary matrix, a twenty-record source registry, and a coherence
  audit are not reproducible quickly — they represent restraint (what was
  deliberately *not* published) as much as content, and restraint cannot be
  bought after the fact once a competitor has already published loosely.
- **The agent-legibility footprint.** Canonical URLs, single-h1 pages,
  consistent ontology-layer routing, and a clean internal link graph across
  thirteen indexable routes are already in place — exactly what
  `INTELLIGENCE_FACTORY_DOCTRINE.md` identifies as what wins when AI agents
  answer category questions on a buyer's behalf.

---

## 10. Interface Embodiment

`INTERFACE_THESIS.md` names the interaction: the **Silicon Sovereignty
Stack** ordered list (visible on the home page as an eight-item layer
sequence with governing questions) is the one visual system that makes the
thesis felt — dependency as a stacked, layered structure, not a flat topic
list or a gamified score dial. Deep black/graphite/silicon-gray with copper
traces for dependency and reserved electric blue for active evidence gives
every color a defined analytical function, and the explicit prohibited-
patterns list (no neon, no sci-fi dashboard, no arbitrary scores, no hidden
confidence) matches `INTERFACE_GOVERNANCE.md` directly.

Current build (`index.html`, `assets/css/main.css`) implements this without
external JS, frameworks, or CDN dependencies — a legitimate, accessible,
fast, agent-legible baseline. It has not yet been tested against the
mandatory interface test questions in `INTERFACE_GOVERNANCE.md` in a formal
review pass (see Execution Sequence item 4); no 3D/WebGL is used, which is
consistent with the doctrine's default toward restraint given the analytical
register of this category.

---

## 11. Execution Sequence

1. **Engine v1 build.** Ship the static, client-side Chip Dependency Map
   form-to-output tool at `/chip-dependency-map/`, conformant to
   `CHIP_DEPENDENCY_MAP_MODEL.md` and linking every output to its ontology
   layer page. This is the single highest-leverage build — it converts the
   asset from Category Artifact to Category Intelligence Factory.
2. **Go live.** Enable GitHub Pages on the asset repository, point
   `aielectronicchips.com` DNS at it, and complete the manual items in
   `PUBLIC_LAUNCH_READINESS_CHECKLIST.md`. No SEO, traffic, or income is
   possible before this step; it is a prerequisite, not an enhancement.
3. **Respectable income activation.** Turn the qualified-inquiry mailto
   pathway into a real intake: a structured brief-request form (still no
   checkout, per `MONETIZATION_BOUNDARY.md`) that captures entity, decision,
   time horizon, and layer scope, and a defined delivery process for
   Compute Sovereignty Briefs and Chip Dependency Audits (Layer 7, items
   1–2), so the asset earns before the engine or acquisition step.
4. **Interface governance review.** Run the current build against the
   mandatory interface test in `INTERFACE_GOVERNANCE.md` and record the
   result in `DECISION_LOG.md`.
5. **Adoption monitoring.** Establish the position-monitoring process from
   `SOVEREIGN_ASSET_EXECUTION_ORDER.md` Step 12 — track whether "Compute
   Sovereignty" or "Silicon Sovereignty Stack" language is picked up
   elsewhere, as the leading indicator for Layer 9's loss-question strength.

---

**Decision log reference:** entry required in this repository's own
decision-tracking layer when this plan is approved or versioned. The
asset's own `DECISION_LOG.md` (in `Sohadot/aielectronicchips`) remains the
authoritative record of ontology, standard, and model versioning decisions;
this dossier tracks the portfolio-level registration and tier only.
