# Cloudflare Asset Onboarding

## Purpose

This template governs how a digital asset is onboarded into Cloudflare.

It should be completed before or during Cloudflare setup for any sovereign-grade asset.

Cloudflare onboarding is not only technical.

It is part of asset governance.

---

## Asset Identity

- **Asset Name:** <asset name>
- **Domain:** <domain>
- **Repository:** <repository path or URL>
- **Canonical Site Root:** <path>
- **Date Opened:** <YYYY-MM-DD>
- **Operator:** <name or role>
- **Status:** <planned / in-progress / active / paused / retired>

---

## Strategic Context

### Asset Role

Describe the role of the asset.

Examples:

- sovereign-grade reference asset
- structured reference build
- category anchor
- commercial landing layer
- multilingual authority asset

### Cloudflare Role

Explain why Cloudflare is being used.

Choose all that apply:

- DNS
- TLS / HTTPS
- custom domain
- Cloudflare Pages
- redirects
- caching
- security posture
- performance
- edge governance

---

## Source of Truth

- **Canonical Repository:** <repo>
- **Canonical Branch:** main
- **Canonical Site Root:** <path>
- **Deployment Model:** <GitHub integration / GitHub Actions / manual pending / other>

### Source-of-Truth Confirmation

Confirm:

- [ ] GitHub remains the source of truth
- [ ] Cloudflare does not contain uncontrolled source content
- [ ] deployment path matches repository architecture
- [ ] no parallel output root is being introduced

---

## Cloudflare Zone

- **Cloudflare Account:** <account name or ID reference>
- **Zone Name:** <domain>
- **Zone ID:** <zone id or pending>
- **Nameservers Delegated:** <yes / no / pending>
- **Registrar:** <registrar>
- **Delegation Date:** <YYYY-MM-DD or pending>

### Nameserver Notes

Record nameserver delegation notes here.

---

## DNS Records

| Type | Name | Value | Proxied | TTL | Purpose | Status |
|---|---|---|---|---|---|---|
| A / CNAME / TXT | <name> | <value> | <yes/no> | <ttl> | <purpose> | <planned/active> |

### DNS Notes

Add any DNS-specific notes here.

---

## Cloudflare Pages

Complete only if Cloudflare Pages is used.

- **Pages Project Name:** <name>
- **Connected Repository:** <repo>
- **Production Branch:** main
- **Build Command:** <command or none>
- **Output Directory:** <directory>
- **Custom Domain:** <domain>
- **Preview Deployments:** <enabled / disabled / pending>

### Pages Notes

Record Pages-specific decisions here.

---

## TLS / HTTPS

- **SSL/TLS Mode:** <mode>
- **Always Use HTTPS:** <yes / no / pending>
- **Automatic HTTPS Rewrites:** <yes / no / pending>
- **HSTS:** <yes / no / pending / not used>

### TLS Notes

Record TLS decisions and risks here.

---

## Redirects and Canonicals

- **Canonical Host:** <root / www / subdomain>
- **www Behavior:** <redirect to root / root to www / no redirect / pending>
- **HTTP Behavior:** <redirect to HTTPS / pending>
- **Trailing Slash Policy:** <slash / no slash / system default>

### Redirect Rules

| Rule | From | To | Purpose | Status |
|---|---|---|---|---|
| <rule name> | <from> | <to> | <purpose> | <planned/active> |

---

## Security Posture

- **WAF / Security Rules:** <none / planned / active>
- **Bot Protection:** <none / planned / active>
- **Rate Limiting:** <none / planned / active>
- **Access Rules:** <none / planned / active>

### Security Notes

Record security posture here.

---

## Caching and Performance

- **Static Asset Caching:** <default / custom / pending>
- **HTML Caching:** <default / custom / pending>
- **Compression:** <enabled / pending>
- **Image Optimization:** <none / planned / active>

### Caching Notes

Record cache decisions here.

---

## API Token Requirements

Complete only if API access is required.

### Token Purpose

Describe why a token is required.

### Required Scope

Choose the narrowest required scope:

- read-only audit
- DNS edit for specific zone
- Pages edit
- zone settings edit
- other

### Security Confirmation

- [ ] no global API key is used
- [ ] no token is committed to the repository
- [ ] token is stored only in an approved secret store
- [ ] token permissions are limited to the minimum needed
- [ ] token can be revoked when no longer needed

---

## Deployment Verification

Verify after setup:

- [ ] domain resolves
- [ ] HTTPS works
- [ ] canonical host works
- [ ] redirects work
- [ ] deployment source is correct
- [ ] latest GitHub commit is reflected
- [ ] no unintended Cloudflare behavior detected

---

## Rollback Plan

Describe how to reverse the Cloudflare setup if needed.

Include:

- DNS rollback
- Pages rollback
- redirect rollback
- TLS rollback
- cache rollback

---

## Current Decision

### Onboarding Verdict

Choose one:

- not ready
- ready for DNS setup
- ready for Pages setup
- ready for deployment verification
- active and verified
- paused pending correction

### Immediate Next Action

Write one action only.

### Rationale

Explain why this is the correct next action.

---

## Change Log

Use this format:

- **Date:** <YYYY-MM-DD>
- **Change Type:** <DNS / TLS / Pages / Redirect / Security / Cache / Token / Verification>
- **Summary:** <what changed>
- **Reason:** <why it changed>
- **Rollback:** <how to reverse if needed>

---

## Notes

Use this section only for disciplined Cloudflare onboarding notes.

Do not store secrets here.
