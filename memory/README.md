# Operational Memory Model

## Purpose

This folder defines how governance memory should be handled for this skill.

The skill must distinguish between:

1. **skill memory** — permanent memory about the governance skill itself,
2. **installation memory** — local memory created when the skill is applied in a specific user, project, repo, organization, or agent environment.

Mixing these two memory types creates governance drift.

---

## Memory Boundary

### Skill Memory

Skill memory belongs to this repository.

It records:

- doctrine evolution,
- governance decisions,
- rejected architectural patterns,
- maturity changes,
- review learnings,
- activation policy changes,
- runtime policy changes,
- and lessons that should apply to all installations of the skill.

Skill memory is product memory.

It should be versioned with the skill.

---

### Installation Memory

Installation memory belongs to the consuming environment.

It records:

- project-specific decisions,
- user-specific preferences,
- local constraints,
- local exceptions,
- reviewed skill instances,
- repo-specific governance outcomes,
- organization-specific risk posture,
- and contextual tradeoffs.

Installation memory is operational context.

It should not be written back into the canonical skill repository unless it becomes a generalized learning.

---

## Default Rule

> The canonical skill repository stores reusable governance knowledge.
>
> The installation stores local operational history.

---

## Repository Memory Structure

```text
memory/
├── README.md
├── decisions/
├── learnings/
├── rejected-patterns/
├── evolution/
└── installation-template/
```

---

## Installation Memory Structure

A consuming repo may create:

```text
.ai-skill-governance/
├── decisions/
├── reviews/
├── exceptions/
├── maturity/
└── context.md
```

This local memory belongs to the installation.

It should be human-readable, auditable, and removable without breaking the canonical skill.

---

## Promotion Rule

A local installation learning may be promoted into canonical skill memory only if it is:

- reusable across installations,
- not tied to private context,
- not user-specific,
- not organization-confidential,
- and aligned with the core doctrine.

Promotion should be explicit.

Do not silently absorb local context into the skill.

---

## Anti-Patterns

Avoid:

- storing user context inside canonical skill memory,
- storing organization decisions inside the reusable skill,
- treating installation exceptions as doctrine,
- allowing local drift to rewrite global principles,
- hiding governance memory in opaque runtime state.

---

## Final Principle

> Skill memory governs the product.
>
> Installation memory governs the local application of the product.
