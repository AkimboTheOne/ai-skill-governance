# Doctrine Projection

## Learning

A skill should have one shared doctrine. Operational artifacts such as
`SKILL.md`, `AGENTS.md`, planner rules, runtime policy, activation policy, memory
policy, and review checklists are context-specific projections of that doctrine.

They may specialize how the doctrine applies in a given context, but they must not
introduce competing doctrine or require precedence rules to resolve doctrinal
conflict.

If artifacts appear to conflict, resolve the issue by restoring alignment with the
shared doctrine and narrowing the context-specific artifact.

## Evidence

This learning came from reviewing `ai-skill-governance` itself. Treating
`SKILL.md` and `AGENTS.md` as competing authorities created an unnecessary
precedence question. The better model is that `SKILL.md` governs skill use and
activation, while `AGENTS.md` governs agent operation and maintenance in the repo.
Both must remain doctrinally equivalent because both project the same shared
doctrine.

## Governance Notes

- Compatible with the required order: Question, Eliminate, Simplify, Accelerate,
  Automate.
- Reduces ambiguity without adding runtime behavior, hidden state, automation, or
  orchestration.
- Keeps doctrinal memory human-readable and versioned with the canonical skill.
