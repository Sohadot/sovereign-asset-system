# Asset Intelligence Factory Plan — strongavatar.com

> Copy of `templates/asset-intelligence-factory-plan.md`, completed for this asset.
> This document is subordinate to the asset's thesis document.
> Governed by `docs/INTELLIGENCE_FACTORY_DOCTRINE.md`.

---

**Asset:** `strongavatar.com`
**Portfolio tier:** Tier 1
**Plan version:** 0.1
**Status:** Draft
**Governing document:** `ASSET_THESIS.md` (pending — Execution Sequence #1)

---

## 0. Orientation

The synthetic-avatar field is built almost entirely on one axis: realism.
Platforms compete on how convincingly an avatar looks, sounds, and moves
like a human. That axis is collapsing into commodity — realism is now
cheap, fast, and reproducible by every vendor.

The axis that is *not* commodity, and is becoming scarce, is **governance**:
whose likeness is this, by what consent, traceable to what origin,
disclosed where required, revocable by whom, and accountable to whom.

`strongavatar.com` exists to own that second axis. Its governing position:

> An avatar is not strong because it is realistic. It is strong because its
> identity, consent, provenance, disclosure, and rights are governed and
> verifiable. Strength is a governance property, not a rendering property.

This plan develops the asset to Category Intelligence Factory grade: it does
not publish articles about synthetic avatars — it takes an avatar deployment
as input and returns a governed classification of its strength.

---

## 1. Category Ownership

**Avatar integrity** — the governed evaluation of a synthetic avatar's or
digital likeness's identity strength: consent, provenance, disclosure,
scope, revocability, and accountability.

The asset owns the question *"is this avatar strong?"* and redefines the
answer away from realism and toward governance.

---

## 2. Category Language

The vocabulary the asset originates and intends others to adopt. Terms
marked **(O)** are original to the asset; **(F)** are inherited from the
field and given governed definition.

- **Avatar Strength (O)** — the governed measure of an avatar's identity
  integrity across consent, provenance, disclosure, scope, revocability,
  and attribution. The asset's headline term.
- **Weak Avatar (O)** — an avatar deployed without governed consent,
  provenance, or disclosure; realistic but ungoverned.
- **Likeness Provenance (O)** — the traceable chain from a source identity
  (real or synthetic) to the deployed avatar.
- **Consent Basis (O)** — the documented authority under which a likeness
  is used, including its scope and expiry.
- **Identity Drift (O)** — divergence between an avatar's deployed behavior
  or appearance and its authorized identity scope.
- **Impersonation Surface (O)** — the exploitable space that allows an
  avatar to be cloned or repurposed to impersonate a real person.
- **Disclosure Integrity (O)** — whether synthetic origin is communicated
  wherever a viewer would reasonably need to know.
- **Revocation Gap (O)** — the absence of a mechanism to withdraw consent
  or decommission a deployed avatar.
- **Avatar Trust Score (O)** — the composite governed score produced by the
  engine, derived deterministically from the protocol.
- **Likeness Rights Chain (F)** — chain-of-title for an identity used in a
  synthetic avatar; given explicit entry and documentation criteria here.
- **Content Credentials / Provenance Signal (F)** — provenance metadata
  (C2PA-aligned); positioned here as one governance component, not the whole.

The discipline rule: every term must be precise enough to resist casual
substitution and natural enough that a platform's own documentation could
adopt it without crediting the source. When that adoption happens, the
asset has won (see `BUYER_LOGIC_AND_VALUE_MAXIMIZATION.md`, signal 2).

---

## 3. Ontology

**Name:** Avatar Integrity Ontology.

**Scope:** Classifies the *weakness classes* of synthetic avatars and
digital likenesses (the failure side) and the *governance components* that
remediate them (the strength side). It does not classify avatar
*aesthetics, style, or rendering quality* — those are explicitly out of
scope, because the thesis rejects realism as the strength axis.

**Versioning rule:** Append-aware and versioned. Classes may be added with
a new minor version and a `DECISION_LOG.md` entry; existing class
definitions may be refined but not silently repurposed. Each class carries
a stable identifier.

### Top-level weakness classes (what is wrong)

| ID | Class | One-line definition |
|----|-------|---------------------|
| W-01 | Consent Absence | No documented authority for the likeness in use. |
| W-02 | Provenance Void | No traceable origin and no content credentials. |
| W-03 | Disclosure Failure | Synthetic nature concealed where disclosure is warranted. |
| W-04 | Identity Drift | Avatar acts or appears beyond its authorized scope. |
| W-05 | Impersonation Exposure | Avatar can be cloned or misused to impersonate a real person. |
| W-06 | Rights Ambiguity | Likeness rights chain is unclear, incomplete, or contested. |
| W-07 | Revocation Gap | No mechanism to withdraw consent or decommission the avatar. |
| W-08 | Context Collapse | Avatar reused outside its authorized context or audience. |
| W-09 | Attribution Loss | No durable binding of the avatar to an accountable owner. |
| W-10 | Robustness Weakness | Avatar is vulnerable to adversarial tampering or spoofing. |

### Governance components (what makes an avatar strong)

| ID | Component | Remediates |
|----|-----------|-----------|
| C-01 | Consent Infrastructure | W-01, W-06 |
| C-02 | Provenance & Content Credentials Layer | W-02, W-10 |
| C-03 | Disclosure Layer | W-03 |
| C-04 | Scope & Usage Binding | W-04, W-08 |
| C-05 | Anti-Impersonation Controls | W-05, W-10 |
| C-06 | Rights Chain Documentation | W-06 |
| C-07 | Revocation & Kill-Switch Mechanism | W-07 |
| C-08 | Attribution & Accountable-Owner Binding | W-09 |

**Entry criteria for a class:** a class enters the ontology only when it
names a distinct, observable failure or governance function that (a) is not
a subset of an existing class, (b) can be detected or confirmed through the
protocol's structured inputs, and (c) maps to at least one component or
weakness on the opposite table.

---

## 4. Standard

**Name:** Strong Avatar Standard.

**Property governed:** identity integrity — the trustworthiness and
accountability of a deployed avatar, independent of its realism.

**Headline criteria (strength bands):**

| Band | Criterion summary |
|------|-------------------|
| **Ungoverned** | One or more of consent, provenance, or disclosure is absent. The avatar is realistic but cannot be trusted or accounted for. |
| **Provisional** | Consent and provenance exist but are incomplete; scope, revocation, or attribution is unverified. |
| **Governed** | Consent, provenance, disclosure, scope-binding, and attribution are all documented and verifiable. |
| **Sovereign** | Governed, plus revocation mechanism, anti-impersonation controls, and an auditable rights chain — the avatar is defensible under scrutiny by a regulator, platform, or rights holder. |

The ontology says what the failures and components *are*. The standard says
what *good* is: a Strong Avatar is one that reaches the Governed band or
above. The standard is the published definition any practitioner can apply
without the author present.

---

## 5. Protocol

**Name:** Avatar Strength Assessment Protocol.

**Inputs:** structured answers describing a single avatar deployment —
consent documentation, source-identity origin, provenance signaling,
disclosure placement, authorized scope, revocation capability, and
accountable owner. No free text is scored; every input is a bounded choice.

**Steps:**
1. Capture deployment attributes through the bounded questionnaire.
2. Map each answer to weakness classes (W-01…W-10) using the published
   rule table.
3. Identify the dominant weakness class and any compounding classes.
4. Determine the strength band (Ungoverned → Sovereign) from the band
   criteria.
5. Return the band, the dominant weakness, and the remediating components
   (C-01…C-08).

**Reproducibility:** the mapping from inputs to band is a published rule
table with no scoring discretion. Two competent operators assessing the
same deployment must reach the same band and the same dominant weakness
class. Any input combination that does not resolve deterministically is a
protocol defect, not an operator judgment call.

---

## 6. Engine

**Name:** Avatar Strength Diagnostic.

- **Phase 1 form:** a fully static, client-side, rules-based questionnaire
  (the structural pattern proven on `funnelplugs.com/engine.html`). No
  server, no model inference, no randomness — outputs are deterministic
  consequences of the protocol rule table. Complies with the asset's
  static/security/runtime doctrine.
- **Input:** the bounded deployment attributes defined by the protocol.
- **Output:** Avatar Strength band + dominant weakness class + the ranked
  remediating components, plus a plain-language summary.
- **Output links:** every result links into the reference layer — the band
  links to the Strong Avatar Standard page, the dominant weakness links to
  its W-class page, and each remediating component links to its C-class
  page. An output that points nowhere is forbidden (it would produce
  opinion, not intelligence).
- **Deferred to later phases:** Avatar Trust Score API (JSON endpoint over
  the same rule table), a governed avatar/likeness vendor registry,
  longitudinal monitoring for Identity Drift, and embeddable assessment
  widgets. None of these may ship before structural integrity is validated.

The engine sells *depth*, never *conclusions*: the free assessment returns a
real, complete band. Paid layers extend the analysis; they do not unlock a
withheld verdict.

---

## 7. Respectable Income

Revenue is a consequence of authority, never a substitute for it
(`SOVEREIGN_ASSET_EXECUTION_ORDER.md`). No income layer activates before
structural integrity is validated (Execution Sequence). In phase order:

| Phase | Output | Sold to | Why it raises trust |
|-------|--------|---------|---------------------|
| 1 | Free Avatar Strength Assessment | Anyone | Builds authority and adoption of the language; the diagnosis is complete and honest. |
| 2 | Full Avatar Strength Report (paid brief) | Platforms, agencies, rights holders | Extends a real free verdict with remediation depth and rights-chain documentation guidance — a reference artifact a buyer would keep. |
| 2 | Synthetic Likeness Governance Brief | Enterprise legal / trust & safety teams | Reference-grade governance writing; positions the asset as the standard, not a vendor. |
| 3 | Avatar Trust Score API | Synthetic-media platforms | Lets platforms surface a governed score they did not have to define; deepens dependence on the standard. |
| 3 | Governed Avatar/Likeness Vendor Directory | Vendors seeking listing | Listing requires meeting documented entry criteria — gatekeeping authority, not pay-to-list. |
| 3 | Standard / taxonomy licensing | Platforms, standards bodies | Licensing the frame is the purest expression of category ownership. |

Forbidden, per `INTERFACE_GOVERNANCE.md` and the monetization gates:
sidebar/affiliate banners, urgency widgets, pop-up capture interrupting
doctrine, any monetization that converts the diagnostic into a lead-capture
trap. Revenue the buyer would have to remove on acquisition is not built.

---

## 8. Strategic Buyer

| Rank | Buyer category | Existing problem this asset answers |
|------|----------------|-------------------------------------|
| 1 | Synthetic-media / AI-avatar platforms (digital-human video, voice, avatar generation) | They compete on realism and have no owned, credible language for *trust*. As scrutiny rises, they need a governance frame — and would rather own the one being adopted than cite a competitor's. |
| 2 | Content provenance / authenticity ecosystem (provenance, content-credentials, verification vendors) | They have generic provenance infrastructure but no avatar-specific application layer — the ontology, standard, and scoring that turn provenance into an *avatar strength* verdict. |
| 3 | Likeness-rights & digital-double platforms, talent agencies, estates | They manage rights but lack a published standard for what a *well-governed* likeness deployment is. The Strong Avatar Standard is the instrument they can point to. |

Secondary: trust-and-safety / brand-safety vendors, identity-verification
firms, and standards or policy bodies that need a ready-made interpretive
frame.

Per `BUYER_LOGIC_AND_VALUE_MAXIMIZATION.md`: this is an acquisition target,
not a sale. The construction goal is an asset a strategic buyer recognizes
as something they would *need to build* if they did not acquire it — priced
from replacement cost, not a revenue multiple.

---

## 9. The Loss Question

**Why is not acquiring this asset a structural loss?**

Because the parts that create the position cannot be rebuilt quickly:

- **The name.** `strongavatar.com` states the category's strength axis in
  two words. A competitor entering later cannot acquire the name and must
  argue *around* it.
- **The language.** Once *Avatar Strength*, *Weak Avatar*, and *Avatar
  Trust Score* are adopted by platforms and press, the buyer who does not
  own the source must speak someone else's vocabulary about their own
  product.
- **The ontology and standard.** A versioned, governed classification of
  avatar weakness and a published strength standard take domain
  understanding and time to build at equivalent precision — not a tutorial.
- **Accumulated reference and link graph.** A maintained corpus of class
  pages with a clean, orphan-free internal link graph is the product of
  disciplined accumulation, not a sprint.
- **Governance record.** Version history, decision logs, and claim
  discipline are what make the asset *trusted* in an era when anyone can
  generate text. That record cannot be back-dated.
- **Agent-legibility footprint.** Stable canonical URLs, consistent
  identifiers, and structured summaries mean that when AI agents answer
  "what makes an avatar trustworthy?", the governed source wins. That
  distribution advantage compounds and cannot be retrofitted late.

A competitor could build *an* avatar-governance site. They could not build
*this* name, this adopted language, this accumulated and governed
reference, and this agent-legible position — without years and the risk
that the category has already been claimed.

---

## 10. Interface Embodiment

**The thesis to embody:** strength is governance, not realism.

**The one system that makes it felt:** an **Avatar Credential Panel**. When
a user enters an avatar's attributes, the interface does *not* render a
glossy face. It resolves the avatar into a structured, monospace governance
readout — consent, provenance, disclosure, scope, revocation, attribution —
each line resolving to a verified or missing state, terminating in a
strength band. The deliberate absence of a beautiful rendered face, in a
field obsessed with rendered faces, *is* the argument.

**Mandatory interface test (`INTERFACE_GOVERNANCE.md`):**
1. **Concept alignment** — the panel reinforces the governing thesis
   directly (governance made visible, realism withheld). Pass.
2. **Performance** — static, client-side, deterministic; state transitions
   only, `prefers-reduced-motion` respected; no rendering load. Pass.
3. **Coherence** — monospace identifiers, low-saturation institutional
   palette, dense parseable layout; all derivable from the design system.
   Pass.

Prohibited patterns (hero-over-stock-photo, chat widget, urgency timers,
testimonial carousels, interrupt pop-ups) are rejected unconditionally.

---

## 11. Execution Sequence

Dependency-ordered. Each entry is completable and verifiable; no entry
depends on an unapproved layer. This follows
`SOVEREIGN_ASSET_EXECUTION_ORDER.md` — no step is parallelized for speed.

1. **`ASSET_THESIS.md`** — the governing thesis as a distinct, contradictable
   position (Execution Order Step 1). This plan is subordinate to it.
2. **Avatar Integrity Ontology document** — formal class definitions, IDs,
   and entry criteria (W-01…W-10, C-01…C-08).
3. **Strong Avatar Standard document** — band criteria, published in full.
4. **Avatar Strength Assessment Protocol document** — the input set and the
   deterministic rule table.
5. **Design system** — token set, component grammar, the Avatar Credential
   Panel grammar; established before any page is built.
6. **Doctrine pages** — manifesto, protocol, standard (institutional weight).
7. **Reference layer** — 10 weakness-class pages + 8 component pages, each
   meeting entry criteria, cross-linked with no orphans.
8. **Engine** — static Avatar Strength Diagnostic; every output links into
   the class pages from step 7.
9. **Structural integrity validation** — ontology ↔ standard ↔ protocol ↔
   engine ↔ interface consistency review; all inconsistencies resolved
   before any public exposure.
10. **Distribution configuration** — canonical URLs, sitemap, JSON-LD,
    machine-readable summaries, agent-legibility checks.
11. **Publish and record initial position** — baseline for drift tracking.
12. **Monetization gate** — only after step 9 passes, activate Phase 1 free
    assessment; defer paid layers per Section 7.

---

**Decision log reference:** an entry is required in `DECISION_LOG.md` when
this plan is moved from Draft to Approved or versioned beyond 0.1.

*Plan maintained under Sovereign Asset System — portfolio/asset-dossiers/strongavatar.com/*
