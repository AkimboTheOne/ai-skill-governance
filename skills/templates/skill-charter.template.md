# Skill Charter Template

## Purpose

This document defines the operational identity,
architectural boundaries,
behavioral constraints,
and governance expectations of a skill.

A skill must remain:

- understandable,
- bounded,
- maintainable,
- composable,
- and operationally governable.

---

# Skill Identity

## Skill Name

`<skill-name>`

---

## Primary Purpose

Describe the single operational capability this skill exists to provide.

The purpose must be:

- explicit,
- bounded,
- operationally meaningful.

Avoid vague goals.

A skill should solve a focused problem.

It should not become a generalized platform.

---

## Non-Goals

Explicitly define what the skill does NOT do.

Examples:

- orchestration engine,
- autonomous runtime,
- workflow platform,
- distributed infrastructure,
- generic code generation,
- persistent hidden memory.

If boundaries are unclear, scope drift becomes inevitable.

---

# Operational Scope

## Responsibilities

List responsibilities directly owned by the skill.

Responsibilities should be:

- measurable,
- operationally clear,
- explicit.

Prefer concrete operational capabilities over abstract intentions.

---

## Out of Scope

List intentionally excluded responsibilities.

Anything not explicitly included should default to out of scope.

---

# Engineering Constraints

## Mandatory Engineering Order

The skill must always operate in this order:

1. Question
2. Eliminate
3. Simplify
4. Accelerate
5. Automate

Do not optimize before simplification.

Do not automate before operational stability.

---

## Complexity Constraints

The skill should prefer:

- explicit behavior,
- deterministic workflows,
- human-readable memory,
- bounded context,
- simple interfaces,
- direct operations.

Avoid:

- hidden state,
- recursive orchestration,
- unnecessary abstractions,
- premature distribution,
- orchestration-heavy architecture.

---

## Architectural Defaults

### Prefer

- markdown/plain text,
- filesystem-readable structures,
- modular monolith patterns,
- explicit contracts,
- deterministic execution,
- local reasoning.

### Require Explicit Justification

- vector databases,
- RAG pipelines,
- multi-agent systems,
- distributed memory,
- asynchronous orchestration,
- background autonomous behavior,
- hidden persistent state.

---

# Runtime Boundaries

## Execution Model

Define whether the skill is:

- assistive,
- advisory,
- deterministic,
- read-only,
- write-enabled,
- interactive,
- bounded,
- autonomous.

Execution behavior must remain explicit.

---

## Write Constraints

If write operations exist:

- require explicit intent,
- require bounded targets,
- require auditability,
- require reversibility where possible.

The skill must not mutate hidden state silently.

---

## Memory Constraints

Memory should remain:

- inspectable,
- editable,
- auditable,
- operationally understandable.

Avoid uncontrolled memory growth.

Prefer local, human-readable memory.

---

# Human Governance

Human operators must retain:

- visibility,
- override capability,
- execution awareness,
- architectural control.

If humans cannot understand what the skill is doing and why, governance has failed.

---

# Tooling Policy

## Tool Usage Principles

The skill should:

- minimize unnecessary tooling,
- avoid recursive tool chains,
- prefer deterministic operations,
- minimize orchestration complexity.

Tool usage must remain:

- bounded,
- explainable,
- operationally justified.

---

# Planning Constraints

Before introducing new capability, ask:

- Does this solve a real problem?
- Can this be simplified?
- Can this be merged into existing behavior?
- Does this increase cognitive load?
- Is the complexity proportional to the problem?
- Can humans still reason about the system?
- Is this introducing sophistication without necessity?

---

# Failure Philosophy

The skill should fail:

- explicitly,
- predictably,
- observably,
- recoverably.

Avoid:

- silent degradation,
- hidden retries,
- concealed orchestration,
- opaque runtime behavior.

Operational clarity is more important than artificial smoothness.

---

# Observability Principles

The skill should preserve:

- execution visibility,
- operational traceability,
- explainable behavior,
- deterministic reasoning where possible.

A human operator should understand:

- what happened,
- why it happened,
- and what changed.

---

# Complexity Governance

The objective is not minimalism.

The objective is controlled complexity.

Sophistication without operational value is architectural debt.

---

# Final Principle

> A skill should reduce operational complexity faster than it creates architectural complexity.
