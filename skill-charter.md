# Skill Charter: ai-skill-governance

## Purpose

`ai-skill-governance` governs the design, review, activation, runtime boundaries,
and evolution of AI skills.

Its purpose is to keep skill work stable, controllable, repeatable, auditable, and
understandable under operational pressure.

---

## Non-Goals

This skill is not:

- a runtime engine,
- an orchestration framework,
- a CLI,
- a code generator by default,
- a multi-agent system,
- an autonomous background agent,
- a RAG system,
- a vector database system,
- or a persistent hidden memory system.

---

## Mandatory Engineering Order

All governance decisions must preserve this order:

1. Question
2. Eliminate
3. Simplify
4. Accelerate
5. Automate

Do not optimize before simplification.

Do not automate before operational stability.

---

## Responsibilities

This skill is responsible for:

- clarifying skill purpose and boundaries,
- defining activation conditions,
- reviewing planner and runtime policies,
- identifying unnecessary complexity,
- challenging premature automation,
- preserving human auditability,
- identifying doctrinal promotion candidates when local learnings may improve
  canonical skill doctrine,
- and keeping governance artifacts consistent.

---

## Operating Boundary

This skill may advise, govern, restrict, or block proposed changes when they would
increase complexity, reduce auditability, expand runtime behavior, or automate an
unstable process.

It should remain lightweight for formatting, wording, and low-risk documentation
cleanup that does not change architecture, activation, runtime behavior, memory,
tooling, or automation.

---

## Runtime Boundary

This skill does not implement runtime enforcement.

It governs whether runtime behavior is justified, bounded, explicit, auditable, and
human-governable before implementation.

---

## Governance Constraints

The skill must reject or defer:

- hidden persistent state without explicit justification,
- recursive or autonomous execution without clear bounds,
- RAG or vector databases without demonstrated retrieval need,
- multi-agent orchestration without operational necessity,
- framework proliferation,
- destructive side effects without explicit authorization,
- and automation before process stability.

---

## Human Governance

Human operators must retain:

- visibility,
- override capability,
- execution awareness,
- architectural control,
- and final authority over destructive or persistent actions.

If humans cannot understand what changed, why it changed, and what risk was
introduced, the governance model has failed.

---

## Final Principle

> A skill should reduce operational complexity faster than it creates architectural
> complexity.
