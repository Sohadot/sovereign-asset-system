# Cloudflare Dashboard Operator Skill

## Purpose

This skill governs how an AI agent may assist with Cloudflare configuration through the Cloudflare dashboard only.

This skill does not permit Cloudflare API usage.

The agent may operate through the visual dashboard interface when an authorized user is logged in and has explicitly approved the task.

Cloudflare is treated as an edge-governance layer.

GitHub remains the source of truth.

---

## Core Rule

The agent may work inside Cloudflare only through the dashboard UI.

The agent must not request, create, store, or use:

- Cloudflare API tokens
- Global API keys
- account passwords
- recovery codes
- unrestricted credentials
- secret keys

No Cloudflare secret belongs in the repository.

No Cloudflare secret belongs in chat.

No Cloudflare secret belongs in markdown files.

---

## Operating Model

The approved operating model is:

1. The owner logs in to Cloudflare manually.
2. The agent receives a specific asset-level task.
3. The agent navigates the Cloudflare dashboard interface.
4. The agent proposes the exact change before applying it.
5. The owner approves sensitive changes.
6. The agent applies the approved change through the dashboard.
7. The agent verifies the visible result.
8. The change is documented in the repository when relevant.

The agent must not act silently.

---

## Allowed Dashboard Operations

The agent may assist with:

### DNS

- inspect DNS records
- add DNS records
- edit DNS records
- remove DNS records only with explicit approval
- configure CNAME, A, AAAA, TXT, MX records
- verify DNS conflicts
- document DNS decisions

### Nameserver Delegation

- identify Cloudflare nameservers
- guide registrar-side delegation
- verify delegation status
- document delegation state

The agent must not change registrar settings unless explicitly authorized and technically able through the registrar dashboard.

### TLS / HTTPS

- review SSL/TLS mode
- enable HTTPS-related dashboard settings when approved
- verify HTTPS behavior
- document TLS posture

### Redirects

- configure root / www redirect logic when approved
- prevent redirect chains
- prevent redirect loops
- preserve canonical domain identity

### Cloudflare Pages

- create or configure a Pages project through the dashboard
- connect the approved GitHub repository
- set the production branch
- set the build command
- set the output directory
- attach the custom domain
- verify deployment status

The preferred Pages model is GitHub integration, not direct upload.

### Caching and Security

- review cache settings
- configure basic caching rules when approved
- review security posture
- configure basic security settings when approved

---

## Prohibited Operations

The agent must not:

- use Cloudflare API
- create API tokens
- ask for API tokens
- store secrets
- change billing settings
- change account ownership
- remove users
- delete zones without explicit owner command
- transfer domains
- make broad account-wide changes
- create undocumented Workers or Pages projects
- create hidden routes
- bypass GitHub as source of truth
- publish from an unapproved folder

---

## Approval Levels

### Low-Risk Actions

Examples:

- reviewing settings
- identifying DNS records
- checking deployment state
- preparing a change plan

Allowed without special approval.

### Medium-Risk Actions

Examples:

- adding DNS records
- changing CNAME records
- setting Pages output directory
- adjusting redirects
- changing cache behavior

Require explicit approval before execution.

### High-Risk Actions

Examples:

- deleting records
- changing nameservers
- changing SSL/TLS mode
- deleting Pages projects
- deleting zones
- changing account security
- changing billing

Require explicit owner approval and should be handled slowly.

---

## Required Pre-Execution Statement

Before making any medium-risk or high-risk change, the agent must state:

- asset name
- domain
- Cloudflare area
- current setting
- proposed setting
- reason
- risk
- rollback plan

The agent may proceed only after approval.

---

## Source of Truth Rule

Cloudflare must reflect the governed repository architecture.

For static sites, the preferred deployment model is:

GitHub main branch → Cloudflare Pages Git integration → approved custom domain.

Cloudflare must not become the place where content is authored.

Cloudflare must not create an alternate source of truth.

---

## Verification Rule

After each executed change, the agent must verify:

- what changed
- whether the dashboard shows the expected state
- whether the domain behavior matches the intended result
- whether any unresolved warning remains

If verification is incomplete, the agent must say so clearly.

---

## Documentation Rule

Relevant Cloudflare changes should be documented in the asset record.

For asset-specific Cloudflare onboarding, use:

templates/cloudflare-asset-onboarding.md

or the asset-specific file:

assets/<domain-normalized>/cloudflare-onboarding.md

---

## Final Rule

The agent may operate inside Cloudflare only as a dashboard assistant.

No API.

No tokens.

No hidden automation.

No uncontrolled account-wide action.

Cloudflare must support the sovereign asset architecture, not replace it.

---

## Mandatory Operating Clause

Use Cloudflare dashboard operation only.

Do not use Cloudflare API.

Do not request or create API tokens.

The owner will log in manually and approve sensitive dashboard actions before execution.

The agent may assist only through Cloudflare dashboard-guided operation under owner supervision.

No Cloudflare credentials, passwords, API tokens, global API keys, recovery codes, or secrets may be requested, stored, copied, exposed, or committed.

GitHub remains the source of truth.

Cloudflare is only an edge-governance layer for DNS, TLS, redirects, security posture, caching, custom domains, and Cloudflare Pages configuration when approved.
