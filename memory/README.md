# Operational Memory Model

## Purpose

This folder defines how governance memory should be handled for this skill.

The skill must distinguish between:

1. **skill memory** — permanent memory about the governance skill itself,
2. **installation memory** — local memory created when the skill is applied in a specific user, project, repo, organization, or agent environment,
3. **global user memory** — user-level preferences or context that are not specific to a single repository.

Mixing these memory types creates governance drift.

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

### Global User Memory

Global user memory belongs to the user's Codex environment, not to this repository
or to a consuming repository.

It records broad user preferences and context that are not specific to one repo,
organization, or governed skill instance.

Global user memory is fallback context.

It must not override local installation memory for the active repository.

---

## Default Rule

> The canonical skill repository stores reusable governance knowledge.
>
> The installation stores local operational history.
>
> Global user memory stores general preferences only when no repo-local memory
> provides a more specific decision.

---

## Memory Precedence

When applying this skill inside a repository, memory must be read in this order:

1. **Repo-local installation memory** in `.ai-skill-governance/`
2. **Global user memory** in the user's Codex environment
3. **Canonical skill memory** in `memory/`

Repo-local installation memory has priority for decisions about the active
repository.

Global user memory may inform defaults, but it must not override explicit
repo-local decisions.

Canonical skill memory governs reusable doctrine. It must not store repo-specific
preferences, user-specific preferences, organization-confidential decisions, or
local exceptions.

---

## Reserved Repository Memory Structure

The canonical skill repository may use this structure when real, reusable skill
memory exists:

```text
memory/
├── README.md
├── decisions/
├── learnings/
├── rejected-patterns/
├── evolution/
└── installation-template/
```

These directories are reserved extension points, not required empty folders.
Do not create them until there is auditable content that justifies their
existence.

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

## Doctrinal Promotion Candidate

The skill should recommend promotion when it detects a new doctrine that is:

- reusable across installations,
- compatible with the core doctrine,
- useful for future skill governance,
- supported by concrete context or repeated use,
- not confidential,
- not user-specific,
- and not merely a local project preference.

This is controlled self-management, not automatic mutation.

When recommending promotion, the skill should provide:

- the proposed doctrine,
- evidence or context that motivated it,
- compatibility with the core doctrine,
- risks or tradeoffs,
- the suggested canonical destination,
- and draft text that a human can review.

The draft must not be applied to canonical memory without explicit human approval.

Reject promotion when the candidate:

- contradicts the order `Question -> Eliminate -> Simplify -> Accelerate -> Automate`,
- introduces hidden or opaque memory,
- promotes automation before process stability,
- expands runtime behavior without governance,
- adds unjustified complexity,
- or converts local preference into general doctrine.

---

## Anti-Patterns

Avoid:

- storing user context inside canonical skill memory,
- storing organization decisions inside the reusable skill,
- treating installation exceptions as doctrine,
- allowing local drift to rewrite global principles,
- allowing global user memory to override repo-local decisions,
- writing promotion candidates directly into canonical memory without review,
- hiding governance memory in opaque runtime state.

---

## Final Principle

> Skill memory governs the product.
>
> Installation memory governs the local application of the product.
