# Assets Layer

## Purpose

This directory defines how individual assets are structured inside the Sovereign Asset System.

It is the execution layer.

---

## Core Principle

Only serious assets enter this layer.

Not every domain belongs here.

---

## Directory Pattern

assets/
  <domain-normalized>/
    domain-dossier.md
    site/

Example:

assets/
  evergreenprotocol-com/
    domain-dossier.md
    site/

---

## Naming Rules

- lowercase only
- replace "." with "-"
- no variations

Correct:
evergreenprotocol-com

---

## Required Files

### domain-dossier.md

The core operating document.

### site/

The public build root.

---

## Canonical Output Rule

Each asset must have one clear site root:

assets/<domain>/site/

Do not create multiple outputs.

---

## Entry Conditions

Asset must have:

- portfolio entry
- strategic assessment
- dossier

---

## Allowed Asset Types

- category anchors
- sovereign builds
- high-value assets

---

## Not Allowed

- weak domains
- speculative inventory
- unused assets

---

## Build Discipline

Allowed:
- dossier
- site structure

Avoid:
- random files
- drafts
- duplicates

---

## Relationship to System

- contexts → logic
- skills → execution
- templates → structure
- rules → control
- assets → implementation

---

## Final Rule

If an asset enters this layer:

it must be treated seriously.

This is not storage.

This is execution.
