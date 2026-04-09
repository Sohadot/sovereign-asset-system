# Naming Conventions

## Purpose

This document defines the official naming rules for files, folders, assets, statuses, and working documents inside the Sovereign Asset System.

Its purpose is not cosmetic.

Its purpose is structural discipline.

A repository that grows without naming discipline becomes harder to search, harder to govern, harder to scale, and easier to corrupt through inconsistency.

This system is designed for long-horizon, high-trust, sovereign-grade work.

Naming must reflect that standard.

## Core Principle

Names must be:

- clear
- stable
- searchable
- scalable
- structurally consistent
- free of unnecessary variation

Naming is part of operating quality.

A weak naming system creates silent disorder.

A strong naming system reduces friction, ambiguity, and drift.

## Repository-Wide Naming Rules

Apply these rules across the entire repository unless a section below defines a tighter standard.

### Rule 1: Use Lowercase for Files and Folders

All repository file names and folder names must use lowercase only.

Correct:

- `portfolio-context.md`
- `buyer-fit-analysis`
- `domain-dossier.md`

Incorrect:

- `Portfolio-Context.md`
- `BuyerFitAnalysis`
- `Domain_Dossier.md`

### Rule 2: Use Hyphens, Not Spaces

Use hyphens to separate words in folder names and file names.

Correct:

- `strategic-narrative-design`
- `buyer-engagement-posture`
- `portfolio-priority-framework.md`

Incorrect:

- `strategic narrative design`
- `buyer_engagement_posture`
- `portfolioPriorityFramework.md`

### Rule 3: Avoid Underscores in Canonical File and Folder Names

Underscores create inconsistency and should be avoided for canonical repository objects.

Use underscores only when an external system forces them.

### Rule 4: Avoid Abbreviations Unless They Are Widely Standardized

Prefer full, legible names over compressed forms.

Correct:

- `buyer-fit-analysis`
- `executive-pitchwriting`

Avoid:

- `buyer-fit`
- `exec-pitch`
- `narr-design`

The repository should remain readable without institutional memory.

### Rule 5: One Canonical Name Per Concept

Do not create multiple variants for the same conceptual object.

Choose one canonical form and keep it stable.

Correct:

- always use `buyer-brief.md`

Incorrect:

- `buyer-brief.md`
- `buyerbrief.md`
- `brief-for-buyer.md`
- `buyer-sheet.md`

### Rule 6: Prefer Functional Names Over Decorative Names

Names should reflect role, not style.

Correct:

- `portfolio-taxonomy.md`
- `strategic-asset-one-pager.md`

Avoid decorative ambiguity such as:

- `master-map.md`
- `gold-layer.md`
- `signal-core.md`

unless the file is explicitly conceptual and doctrine-approved.

## Folder Naming Rules

### Top-Level Folders

Top-level folders must use explicit functional names.

Approved pattern:

- `contexts`
- `skills`
- `templates`
- `operating-rules`

Avoid vague or future-confusing folder names such as:

- `stuff`
- `resources`
- `misc`
- `working`
- `temp`
- `notes`

### Skill Folders

Each skill must live in its own folder named exactly after the skill.

The folder name must match the `name:` field in the skill frontmatter.

Correct:

- `skills/domain-strategic-assessment/`
- `skills/strategic-narrative-design/`

Inside each skill folder, the file name must be:

- `SKILL.md`

Correct pattern:

    skills/domain-strategic-assessment/
      SKILL.md

Do not rename `SKILL.md` per skill.

### Template Files

Template files should live directly under `templates/` unless a future subdivision becomes necessary.

Use descriptive functional names ending in `.md`.

Correct:

- `domain-dossier.md`
- `buyer-brief.md`
- `outreach-sequence.md`
- `strategic-asset-one-pager.md`

### Context Files

Context files should live under `contexts/` and be named by concept.

Correct:

- `digital-sovereignty-doctrine.md`
- `portfolio-context.md`
- `portfolio-taxonomy.md`
- `portfolio-priority-framework.md`

### Operating Rules Files

Operating-rules files should live under `operating-rules/` and be named according to governance function.

Correct:

- `naming-conventions.md`
- `workflow.md`
- `quality-standard.md`

## File Naming Rules

### Markdown Files

All canonical markdown files must follow:

- lowercase
- hyphen-separated
- no spaces
- no trailing version number in file name
- no date in canonical file name unless the file is inherently date-based

Correct:

- `buyer-brief.md`
- `portfolio-context.md`

Incorrect:

- `Buyer Brief.md`
- `buyer_brief_v2.md`
- `portfolio-context-final.md`

### No “final”, “new”, “updated”, or “latest” in Canonical Names

Canonical files must not rely on unstable suffixes.

Avoid:

- `buyer-brief-final.md`
- `buyer-brief-new.md`
- `buyer-brief-latest.md`
- `portfolio-context-updated.md`

If content changes, update the file itself. Do not clone the identity.

### Versioning Belongs Inside the File, Not in the File Name

If versioning is needed, place it in frontmatter, metadata, or commit history.

Do not place version numbers in canonical file names unless there is a deliberate archived-version system.

Avoid:

- `domain-dossier-v3.md`
- `narrative-framework-v2.md`

## Asset Naming Rules

These rules apply when creating internal working files or folders for specific domains or assets.

### Domain-Based Asset Files

When a file or folder is tied to a specific domain, preserve the domain clearly in the name, but normalize it for file-system safety if needed.

Preferred approach for structured asset folders:

    assets/
      example-domain-com/
      category-asset-com/
      geographic-asset-com/

This keeps domain identity explicit while remaining stable in file paths.

### Replace Dots with Hyphens in File-System Representations

For folder names based on domains, replace `.` with `-`.

Correct:

- `example-domain-com`
- `geographic-asset-com`

Avoid:

- `example-domain.com`
- `geographic-asset.com`

This improves path stability and reduces tooling friction.

### Preserve the Domain in Human-Facing Headings

Inside the document, use the real domain form.

Examples:

- `ExampleDomain.com`
- `GeographicAsset.com`

File-system naming and presentation naming are not always identical.

## Status Naming Rules

Statuses must use fixed vocabulary.

Do not improvise status labels casually.

### Approved Asset Statuses

Use one of the following canonical forms for broad asset state:

- `raw-holding`
- `assessed`
- `positioned`
- `narratively-defined`
- `structurally-planned`
- `built`
- `commercially-prepared`
- `revenue-enabled`
- `actively-marketed`
- `acquisition-ready`

When displayed inside prose, these may appear in readable form:

- Raw Holding
- Assessed
- Positioned
- Narratively Defined
- Structurally Planned
- Built
- Commercially Prepared
- Revenue-Enabled
- Actively Marketed
- Acquisition-Ready

### Approved Priority Tier Names

Use these exact canonical forms:

- `tier-1`
- `tier-2`
- `tier-3`
- `tier-4`
- `tier-5`
- `tier-6`

Readable forms may appear in prose:

- Tier 1 — Sovereign Build Candidates
- Tier 2 — Strategic Positioning Candidates
- Tier 3 — Targeted Sale Candidates
- Tier 4 — Yield Support Candidates
- Tier 5 — Dormant Strategic Holds
- Tier 6 — Exploratory / Reassessment Pool

### Approved Development Depth Labels

Use these exact canonical forms in structured fields:

- `dormant-hold`
- `light-positioning`
- `strategic-landing-layer`
- `structured-reference-build`
- `sovereign-grade-build`

### Approved Commercialization Orientation Labels

Use these exact canonical forms:

- `sale-first`
- `value-build-first`
- `hold-and-develop`
- `reference-and-wait`
- `selective-buyer-outreach`
- `yield-supporting`
- `partnership-oriented`
- `internal-portfolio-anchor`

### Approved Revenue Tolerance Labels

Use these exact canonical forms:

- `no-active-monetization`
- `minimal-tolerable-monetization`
- `selective-strategic-monetization`
- `healthy-support-monetization`
- `core-revenue-compatible`

Do not invent variants unless the taxonomy evolves formally.

## Heading Naming Rules

Section headings inside templates and core documents should be:

- explicit
- role-based
- stable
- not overly clever

Correct:

- `## Strategic Thesis`
- `## Buyer Logic`
- `## Narrative Constraints`
- `## Immediate Next Action`

Avoid headings such as:

- `## The Big Why`
- `## Hidden Power`
- `## What This Really Means`
- `## Final Thoughts`

These are too unstable for a system repository.

## Document Title Rules

Human-facing markdown document titles may use title case.

Examples:

- `# Domain Dossier`
- `# Buyer Brief`
- `# Strategic Asset One-Pager`

The file name remains lowercase hyphenated, but the title inside the file should be clean and readable.

## Asset-Specific Working File Rules

If future asset-specific folders are added, prefer a stable structure such as:

    assets/
      example-domain-com/
        domain-dossier.md
        buyer-brief.md
        strategic-asset-one-pager.md
        notes.md

Within each asset folder:

- keep file names functional
- keep them identical across assets
- do not create custom naming patterns per asset unless necessary

This preserves cross-asset consistency.

## Date Naming Rules

Dates should use ISO format:

- `YYYY-MM-DD`

Correct:

- `2026-04-09`

Incorrect:

- `09-04-2026`
- `April-9-2026`
- `4-9-26`

If a date is needed in update logs or archival records, use ISO format only.

## Archive Naming Rules

If archived versions are ever necessary, place them in an `archive/` structure rather than corrupting canonical names.

Example:

    archive/
      2026-04-09-domain-dossier-legacy.md

Canonical current files must remain clean.

Archive naming may include dates because archival identity is historical, not canonical.

## Reserved Words to Avoid

Avoid using the following as canonical file or folder names unless their use is explicitly justified:

- `misc`
- `temp`
- `draft`
- `new`
- `old`
- `final`
- `latest`
- `backup`
- `random`
- `test`
- `ideas`

These words weaken structure and create ambiguity.

If something is temporary, it should usually not be promoted into the core repository structure.

## Renaming Discipline

Do not rename canonical files casually.

A canonical rename is justified only when:

- the original name is structurally wrong
- the conceptual scope has clearly changed
- the new name improves legibility without creating confusion

Renaming for taste alone is discouraged.

Each rename creates history friction and weakens search continuity.

## Change Control Rule

Before introducing a new naming pattern, ask:

1. Does this pattern already exist in the repository?
2. Is the new name clearer than the old one?
3. Is the naming logic scalable across many assets?
4. Will the name still make sense six months from now?
5. Does the name describe role rather than mood?

If the answer is no, do not introduce the new pattern.

## Examples of Good Naming

### Good File Names

- `portfolio-taxonomy.md`
- `portfolio-priority-framework.md`
- `domain-dossier.md`
- `buyer-brief.md`
- `strategic-asset-one-pager.md`
- `naming-conventions.md`

### Good Folder Names

- `skills/domain-strategic-assessment/`
- `skills/buyer-fit-analysis/`
- `skills/premium-asset-negotiation/`
- `operating-rules/`

### Good Asset Folder Names

- `example-domain-com`
- `category-asset-com`
- `geographic-asset-com`

## Examples of Bad Naming

### Bad File Names

- `Buyer Brief Final.md`
- `new_domain_notes.md`
- `pitch-v2-final-final.md`
- `random-ideas.md`
- `asset-master-sheet.md`

### Bad Folder Names

- `stuff/`
- `notes/`
- `temp-assets/`
- `future/`
- `misc-files/`

### Bad Asset Names

- `example domain`
- `domain-project-final`
- `asset-folder-v2`
- `super-domain-folder`

## Final Rule

If a name creates ambiguity, it is weak.

If a name cannot scale, it is weak.

If a name depends on memory rather than clarity, it is weak.

The correct naming system is one that makes the repository easier to govern as it grows.

Naming is not decoration.

Naming is governance.
