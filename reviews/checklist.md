# Engineering Review Checklist

## Core Review Order

Always evaluate in this order:

1. Question
2. Eliminate
3. Simplify
4. Accelerate
5. Automate

Do not skip steps.

Do not optimize before simplification.

Do not automate before stability.

---

## 1. Requirement Validation

### Purpose

Validate whether the requirement should exist at all.

### Checklist

- [ ] Is the requirement solving a real problem?
- [ ] Is the requirement still relevant?
- [ ] Is there a clear owner?
- [ ] Is the operational value measurable?
- [ ] Can someone explain why this exists?
- [ ] Is this requirement inherited without validation?
- [ ] Is this architecture driven by real need instead of trend adoption?
- [ ] Is this introducing complexity for appearance rather than value?

### Reject If

- nobody can justify the requirement,
- the requirement exists only because it was always done this way,
- the requirement exists only to imitate another architecture,
- the requirement creates operational burden without measurable benefit.

---

## 2. Elimination Review

### Purpose

Remove unnecessary complexity before improving anything.

### Checklist

- [ ] Can this be removed entirely?
- [ ] Can this be merged into an existing capability?
- [ ] Can this reduce dependencies?
- [ ] Can this reduce orchestration?
- [ ] Can this reduce context expansion?
- [ ] Can this reduce moving parts?
- [ ] Can this reduce cognitive load?
- [ ] Is this duplicating an existing system or workflow?

### Reject If

- the solution adds layers without reducing operational cost,
- the solution increases dependency sprawl,
- the solution creates orchestration without necessity,
- the solution preserves obsolete complexity.

---

## 3. Simplification Review

### Purpose

Prefer explicit, understandable, maintainable systems.

### Checklist

- [ ] Is the behavior explicit?
- [ ] Can humans easily understand the workflow?
- [ ] Can humans audit the system?
- [ ] Is the state model understandable?
- [ ] Is the architecture understandable without diagrams?
- [ ] Is the system deterministic where possible?
- [ ] Is the solution simpler than the problem it solves?
- [ ] Are abstractions operationally justified?

### Prefer

- modular monoliths,
- local reasoning,
- markdown/plain text,
- explicit contracts,
- deterministic flows,
- human-readable memory.

### Reject If

- the architecture is harder to understand than the problem,
- the system depends on hidden behavior,
- the abstraction hides operational reality,
- the orchestration layer becomes the main complexity source.

---

## 4. Acceleration Review

### Purpose

Optimize only stable and validated systems.

### Checklist

- [ ] Is the workflow already stable?
- [ ] Are failure modes understood?
- [ ] Is ownership clear?
- [ ] Is the process operationally consistent?
- [ ] Is optimization targeting a real bottleneck?
- [ ] Is this reducing operational friction?
- [ ] Is this reducing feedback loop latency?
- [ ] Is this improving throughput without increasing chaos?

### Reject If

- optimization is targeting a workaround,
- acceleration hides instability,
- scaling happens before simplification,
- deployment speed exceeds operational understanding.

---

## 5. Automation Review

### Purpose

Automate only systems that are already operationally valid.

### Checklist

- [ ] Is the process stable?
- [ ] Are inputs well-defined?
- [ ] Are outputs verifiable?
- [ ] Is rollback possible?
- [ ] Is auditability preserved?
- [ ] Is human override available?
- [ ] Is automation bounded?
- [ ] Are side effects controlled?
- [ ] Does automation preserve operational clarity?

### Reject If

- automation hides broken process design,
- the workflow is ambiguous,
- rollback is impossible,
- ownership is unclear,
- automation amplifies operational confusion,
- AI is compensating for missing engineering discipline.

---

## AI-Specific Review

### Context Management

- [ ] Is context loading minimal and relevant?
- [ ] Is unnecessary memory avoided?
- [ ] Is context traceable and auditable?
- [ ] Is hallucination surface minimized?

### Tooling Review

- [ ] Is tool usage minimal and justified?
- [ ] Is tool chaining necessary?
- [ ] Are tool side effects explicit?
- [ ] Is recursive orchestration avoided?

### Memory Review

- [ ] Is memory human-readable?
- [ ] Is memory mutation explicit?
- [ ] Is memory scope bounded?
- [ ] Is persistent state operationally justified?
- [ ] Does repo-local memory take precedence over global user memory?
- [ ] Does canonical memory promotion require explicit human approval?
- [ ] Is local preference prevented from becoming general doctrine?

---

## Complexity Governance

### Final Questions

- [ ] Does this reduce or increase operational complexity?
- [ ] Does this reduce or increase cognitive load?
- [ ] Can humans still govern the system?
- [ ] Is the architecture maintainable under pressure?
- [ ] Is the complexity proportional to the problem?
- [ ] Is this reversible?
- [ ] Is this observable?
- [ ] Is this introducing sophistication without necessity?

---

## Final Principle

> Complexity must justify itself continuously.

The best architecture is not the most sophisticated.

It is the one that remains understandable, maintainable, governable, and operationally stable under real-world pressure.
