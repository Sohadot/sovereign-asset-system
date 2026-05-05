# Cloudflare Asset Operations Skill

## Purpose

This skill governs how an AI agent may assist with Cloudflare operations for sovereign-grade digital assets.

Cloudflare is treated as an edge-control layer.

It is not the source of truth for content.

It is not the primary build system.

It is not the strategic asset repository.

GitHub remains the canonical source of truth.

Cloudflare may be used for:

- DNS control
- nameserver delegation
- TLS / SSL configuration
- redirect rules
- security posture
- caching posture
- Cloudflare Pages deployment when connected to GitHub
- edge-level performance and protection

This skill exists to prevent unsafe, improvised, or account-wide Cloudflare changes.

---

## Core Principle

The agent may assist with Cloudflare management only under strict governance.

The agent must never treat Cloudflare as a place for random experimentation.

Every Cloudflare action must be tied to a specific asset, a specific zone, a specific purpose, and a reversible operational decision.

No broad account-level action may be taken unless explicitly authorized.

---

## Source of Truth Rule

GitHub remains the source of truth.

Cloudflare should reflect the governed repository state.

The agent must not create a Cloudflare configuration that contradicts:

- the asset dossier
- the site architecture
- the deployment workflow
- the canonical output root
- the sovereign asset methodology

Cloudflare is downstream of the repository.

It must not override the repository.

---

## Allowed Operations

The agent may assist with the following operations when explicitly requested:

### DNS

- review DNS records
- propose DNS records
- add or update DNS records when authorized
- identify conflicting records
- prepare zone onboarding instructions
- verify CNAME, A, AAAA, TXT, MX, and verification records

### TLS and Security

- recommend SSL/TLS posture
- check whether HTTPS is enforced
- propose redirect rules
- propose security headers where applicable
- review basic zone security posture

### Cloudflare Pages

- connect an asset to Cloudflare Pages when approved
- align deployment with GitHub repository source
- confirm production branch
- confirm build command
- confirm output directory
- avoid direct upload unless explicitly approved

### Redirects and Canonicals

- propose www to root redirects
- propose root to www redirects only if approved
- ensure canonical asset URL matches dossier and architecture
- avoid redirect chains

### Performance

- recommend cache behavior
- review static asset caching
- propose compression/performance settings
- avoid aggressive rules that break correctness

---

## Prohibited Operations

The agent must not:

- create or store Cloudflare API tokens in the repository
- expose secrets in code, markdown, logs, screenshots, or commits
- use global API keys
- make account-wide changes without explicit authorization
- change billing settings
- change ownership or account identity
- delete zones
- transfer domains
- change nameservers without explicit asset-level approval
- create experimental Workers, Pages projects, or routes outside the approved architecture
- make Cloudflare the source of content truth
- bypass GitHub as the canonical asset repository

---

## Permission Discipline

Use least privilege.

Prefer zone-scoped access where possible.

Do not request account-wide permissions unless the task truly requires them.

A Cloudflare token should be:

- purpose-specific
- time-bounded where possible
- limited to required zones
- limited to required permissions
- rotated or revoked when no longer needed

The agent must not ask for broader permissions merely for convenience.

---

## Recommended Token Classes

### DNS Management Token

Use only for DNS operations.

Typical purpose:

- add verification records
- configure CNAME/A/AAAA records
- update TXT records
- support asset onboarding

### Pages Deployment Token

Use only when direct API-based Pages deployment is explicitly approved.

Default preference remains GitHub integration.

### Read-Only Audit Token

Use for reviewing zone configuration without making changes.

This is preferred during audit phases.

---

## Operational Modes

### Audit Mode

The agent may inspect or reason about Cloudflare configuration and provide findings.

No changes are made.

### Proposal Mode

The agent may propose exact changes.

No changes are made until approved.

### Execution Mode

The agent may apply approved changes if the environment has the required permissions.

Execution must be limited to the approved asset and approved zone.

### Emergency Mode

Only use when explicitly declared by the owner.

Emergency mode must still avoid broad destructive actions.

---

## Cloudflare Pages Rule

If Cloudflare Pages is used, the preferred deployment model is:

GitHub repository → Cloudflare Pages Git integration → automatic deployment from approved branch.

The agent must confirm:

- repository
- production branch
- build command
- output directory
- environment variables
- custom domain
- deployment status

Do not use Direct Upload unless explicitly approved.

---

## DNS Onboarding Sequence

For a new asset, follow this sequence:

1. Confirm the asset domain.
2. Confirm registrar.
3. Confirm whether nameservers are delegated to Cloudflare.
4. If not delegated, prepare nameserver delegation instructions.
5. Add or verify required DNS records.
6. Verify HTTPS behavior.
7. Verify canonical root.
8. Confirm redirects.
9. Confirm final status in the asset dossier or onboarding note.

Do not skip delegation verification.

---

## Security Rules

The agent must never request or expose:

- Global API Key
- account password
- recovery codes
- unrestricted API token
- raw secrets in chat or files

Secrets must be stored only in approved secret stores, such as GitHub repository secrets or local environment variables, when explicitly required.

No secret belongs in the repository.

---

## Output Requirements

When performing Cloudflare work, the agent must produce:

- asset name
- domain
- Cloudflare zone
- operation type
- proposed change
- reason
- risk
- rollback plan
- approval status
- final state

For execution tasks, the agent must also report:

- what changed
- where it changed
- whether verification passed
- what remains unresolved

---

## Rollback Requirement

Every Cloudflare change must have a rollback plan.

The agent must not apply changes that cannot be clearly reversed unless explicitly approved.

Rollback examples:

- restore previous DNS record
- disable redirect rule
- revert SSL/TLS setting
- remove custom domain from Pages
- restore previous Pages production branch

---

## Final Rule

Cloudflare is an edge-governance layer.

It must strengthen the asset.

It must not create hidden complexity.

It must not weaken GitHub-first discipline.

It must never become an uncontrolled operational surface.
