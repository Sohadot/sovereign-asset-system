# Asset Technical Manifest — FunnelPlugs.com

**Date:** 2026-06-01  
**Build State:** Phase 2 Complete  
**Manifest Purpose:** Technical verification document for buyer due diligence.

---

## Summary Statistics

| Metric | Value |
|--------|-------|
| Total published pages | 33 (+ 404.html) |
| Total word count (all pages) | ~99,000 words |
| Doctrine layer pages | 3 (Manifesto, Protocol, Standard) |
| Interactive tools | 1 (Revenue Leak Diagnostic Engine) |
| Taxonomy pages | 22 (10 leak classes + 10 plug classes + 2 indexes) |
| Concept / reference pages | 7 |
| Acquisition layer pages | 2 (strategic-value, structural-integrity-brief) |
| Pages with Article JSON-LD | 30 |
| Pages with FAQPage JSON-LD | 28 |
| Affiliate placement slots | 9 (3 pages × 3 slots each) |
| Email capture surfaces | 2 (engine.html post-completion gate, structural-integrity-brief.html) |

---

## Page-by-Page Inventory

### Core Doctrine (1,000–5,000+ words each)

| Page | Word Count | Schema Types | Primary Keyword Target |
|------|-----------|--------------|----------------------|
| manifesto.html | ~3,900 | Article, FAQPage | funnel integrity manifesto, structural revenue leakage |
| protocol.html | ~4,800 | Article, FAQPage | funnel failure diagnosis protocol, revenue leakage identification |
| standard.html | ~3,850 | Article, FAQPage | funnel integrity standard, commercial path completeness |
| ontology.html | ~5,700 | Article, FAQPage | plug ontology, funnel failure classification system |

### Interactive Tool

| Page | Word Count | Schema Type | Function |
|------|-----------|-------------|---------|
| engine.html | ~14,800 | WebApplication | 20-question diagnostic, email gate, GTM dataLayer events |

### Primary Navigation / Index Pages

| Page | Word Count | Schema Type | Function |
|------|-----------|-------------|---------|
| index.html | ~1,100 | WebSite, Organization, WebPage | Homepage / entry point |
| registry.html | ~970 | WebPage | Plug category registry (CAT-001/002/003) |
| reference.html | ~1,700 | CollectionPage | Full reference index with hasPart listing |

### Leak Class Pages (Structural Failure Taxonomy)

| Page | Word Count | Schema Types | Primary Leak Class |
|------|-----------|--------------|------------------|
| trust-collapse.html | ~2,350 | Article, FAQPage | Trust Collapse — decision boundary confidence failure |
| friction-overload.html | ~2,700 | Article, FAQPage | Friction Overload — motivation-resistance imbalance |
| flow-break.html | ~2,650 | Article, FAQPage | Flow Break — path architectural discontinuity |
| recovery-absence.html | ~2,760 | Article, FAQPage | Recovery Absence — no re-engagement architecture |
| structural-revenue-leakage.html | ~2,600 | Article, FAQPage | Structural Revenue Leakage — compound leakage classification |
| decision-ambiguity.html | ~2,140 | Article, FAQPage | Decision Ambiguity — commitment clarity failure |
| message-path-misalignment.html | ~2,315 | Article, FAQPage | Message-Path Misalignment — intent continuity failure |
| abandonment-recovery-logic.html | ~2,250 | Article, FAQPage | Abandonment Recovery Logic — re-engagement mechanics |
| decision-stage-integrity.html | ~2,425 | Article, FAQPage | Decision Stage Integrity — commitment architecture |
| diagnostic-signal-layers.html | ~2,295 | Article, FAQPage | Diagnostic Signal Layers — behavioral signal interpretation |

### Plug Class Pages (Structural Intervention Taxonomy)

| Page | Word Count | Schema Types | Primary Plug Class |
|------|-----------|--------------|------------------|
| trust-infrastructure.html | ~2,060 | Article, FAQPage | Trust Infrastructure (CAT-001) |
| recovery-systems-layer.html | ~2,160 | Article, FAQPage | Recovery Systems (CAT-003) |
| friction-reduction-layer.html | ~2,295 | Article, FAQPage | Friction Reduction (CAT-002) |
| alignment-reinforcement-layer.html | ~2,135 | Article, FAQPage | Alignment Reinforcement (CAT-002) |
| decision-guidance-layer.html | ~2,635 | Article, FAQPage | Decision Guidance (CAT-002 + CAT-001) |
| flow-continuity-layer.html | ~2,650 | Article, FAQPage | Flow Continuity (CAT-002) |
| intervention-architecture.html | ~2,485 | Article, FAQPage | Intervention Architecture — sequencing logic |
| leak-plug-mapping.html | ~2,545 | Article, FAQPage | Leak-Plug Correspondence Mapping |
| plug-class-prioritization.html | ~2,735 | Article, FAQPage | Priority Sequencing — plug class installation order |

### Concept / Reference Pages

| Page | Word Count | Schema Types | Topic |
|------|-----------|--------------|------|
| commercial-path-continuity.html | ~2,575 | Article, FAQPage | Path completeness model |
| canonical-url-governance.html | ~2,215 | Article, FAQPage | URL authority governance |
| dimensional-weakness-mapping.html | ~2,405 | Article, FAQPage | Cross-dimensional failure analysis |
| integrity-band-interpretation.html | ~2,600 | Article, FAQPage | Engine scoring band definitions |

### Acquisition Layer

| Page | Word Count | Schema Types | Function |
|------|-----------|--------------|---------|
| strategic-value.html | ~2,810 | WebPage | Primary buyer-facing acquisition page |
| structural-integrity-brief.html | ~2,850 | Article, FAQPage | Email-gated reference brief (lead capture) |

---

## Technical Infrastructure

| Component | Status | Detail |
|-----------|--------|--------|
| Canonical URLs | ✅ Active | All 33 pages have canonical `<link>` tags |
| Sitemap | ✅ Active | sitemap.xml with priority weights (1.0–0.6) and lastmod dates |
| robots.txt | ✅ Active | Standard allow-all with sitemap reference |
| Google Tag Manager | ✅ Active | GTM-56J99S4F on all pages |
| GTM dataLayer events | ✅ Active | `engine_email_capture` + `brief_email_capture` events |
| Structured data | ✅ Active | Article, FAQPage, WebSite, Organization, WebPage, WebApplication, CollectionPage |
| JSON-LD | ✅ Active | @graph structure on homepage; single-type on content pages |
| GitHub Pages | ✅ Deployed | Primary deployment platform |
| Cloudflare | ✅ Active | DNS and CDN governance layer |

---

## Content Quality Verification

All 33 pages meet or exceed the following criteria:
- ✅ Minimum 900 words of reference content (excluding nav/header/footer/script)
- ✅ Unique title tag targeting distinct keyword cluster per page
- ✅ Unique meta description per page
- ✅ Unique meta keywords per page (no shared generic tag sets)
- ✅ JSON-LD structured data (Article and/or FAQPage on content pages)
- ✅ og:type = "article" on content pages (changed from "website" on all leaf pages)
- ✅ Internal links to related pages (minimum 2 per page)
- ✅ Strategic value link in site footer (all 33 pages)

---

## Lead Capture Infrastructure

| Surface | Gate Type | GTM Event | Audience Signal |
|---------|----------|-----------|----------------|
| engine.html | Post-completion (20 questions required to reach gate) | `engine_email_capture` with integrity_band + primary_leak | High intent — actively diagnosing structural funnel failure |
| structural-integrity-brief.html | Bottom-of-page (full content visible, gate on delivery) | `brief_email_capture` with source | Mid intent — seeking reference and audit tools |

---

## Affiliate Placement Structure (Pending Activation)

| Page | Slot ID | Tool Category | Activation Status |
|------|---------|--------------|------------------|
| friction-overload.html | friction-diagnostic-tools | Session recording tools | PENDING — agreement required |
| friction-overload.html | friction-diagnostic-tools | Form analytics | PENDING — agreement required |
| friction-overload.html | friction-diagnostic-tools | Step-funnel measurement | PENDING — agreement required |
| trust-collapse.html | trust-evidence-platforms | Review aggregation | PENDING — agreement required |
| trust-collapse.html | trust-evidence-platforms | Case study / outcome documentation | PENDING — agreement required |
| trust-collapse.html | trust-evidence-platforms | Guarantee / risk reversal frameworks | PENDING — agreement required |
| recovery-absence.html | recovery-automation-platforms | Behavioral trigger email | PENDING — agreement required |
| recovery-absence.html | recovery-automation-platforms | Exit-based paid retargeting | PENDING — agreement required |
| recovery-absence.html | recovery-automation-platforms | CRM / multi-touch orchestration | PENDING — agreement required |

---

*Manifest maintained under Sovereign Asset System — portfolio/asset-dossiers/funnelplugs.com/*
