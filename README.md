# ai-skill-governance

Foundation repository for AI skill governance, planning constraints, runtime policies, and cognitive governance rails.

---

## Purpose

This repository defines a documentation-first governance foundation for designing, building, reviewing, and evolving AI skills.

It exists to help agents and human operators:

- define skill boundaries,
- preserve architectural clarity,
- prevent unnecessary complexity,
- establish planning heuristics,
- constrain runtime behavior,
- evaluate automation readiness,
- and evolve skills without governance drift.

---

## What This Repository Is

This repository is:

- a skill governance foundation,
- a cognitive rail for agents,
- a source of planning and runtime constraints,
- a repository of reusable skill engineering artifacts,
- and a documentation-first operating model for skill evolution.

---

## What This Repository Is Not

This repository is not currently:

- a CLI,
- a runtime engine,
- an orchestration framework,
- a Python package,
- a code generator,
- a multi-agent system,
- or an autonomous execution platform.

Code may be introduced later only if the documentation-based operating model proves stable enough to justify automation.

---

## Core Doctrine

> Do not automate, distribute, abstract, optimize, or orchestrate something that has not first been questioned, eliminated, simplified, and understood.

Complexity is not value.

Complexity is operational cost unless continuously justified.

---

## Engineering Order

All design, planning, review, and evolution should follow this order:

1. Question
2. Eliminate
3. Simplify
4. Accelerate
5. Automate

Do not optimize before simplification.

Do not automate before stability.

---

## Intellectual Influences

This repository is inspired by several engineering and operational traditions:

- [Elon Musk's five-step engineering algorithm](https://insideevs.com/news/526954/elon-musk-5-steps-success/):
  question requirements, delete, simplify, accelerate, automate.
- [Toyota Production System](https://global.toyota/en/company/vision-and-philosophy/production-system/index.html):
  waste reduction, flow, jidoka, just-in-time, and kaizen.
- [Lean Thinking](https://www.lean.org/lexicon-terms/lean-thinking-and-practice/):
  value, value stream, flow, pull, and continuous improvement.
- [Theory of Constraints](https://www.tocinstitute.org/five-focusing-steps.html):
  focus improvement on the system constraint before optimizing locally.
- [Systems Thinking](https://donellameadows.org/archives/leverage-points-places-to-intervene-in-a-system/):
  preserve visibility into feedback loops, leverage points, and unintended
  consequences.

These influences are not treated as rigid doctrine. They inform the repository's
governance posture: question first, remove unnecessary complexity, simplify what
remains, accelerate only stable systems, and automate last.

---

## Repository Structure

Canonical structure:

```text
ai-skill-governance/
├── README.md
├── SKILL.md
├── FOUNDATION.md
├── AGENTS.md
├── skill-charter.md
│
├── governance/
│   ├── planner-rules.yaml
│   ├── runtime-policy.yaml
│   └── activation-policy.yaml
│
├── reviews/
│   └── checklist.md
│
├── skills/
│   └── templates/
│       └── skill-charter.template.md
│
├── memory/
│   └── README.md
│
└── references/
    └── README.md
```

The structure should remain small until additional artifacts justify their
existence.

Root-level duplicates such as `planner-rules.yaml`, `runtime-policy.yaml`, or
`checklist.md` are intentionally avoided. The canonical paths are the governed
subdirectories listed above.

---

## Artifact Families

| Artifact | Purpose |
|---|---|
| [SKILL.md](SKILL.md) | Defines this skill's operating identity, activation contract, and boundaries. |
| [FOUNDATION.md](FOUNDATION.md) | Defines reusable engineering doctrine. |
| [AGENTS.md](AGENTS.md) | Defines agent-facing operational constraints. |
| [skill-charter.md](skill-charter.md) | Defines the concrete charter for this repository's skill. |
| [governance/planner-rules.yaml](governance/planner-rules.yaml) | Defines planning heuristics and complexity governance. |
| [governance/runtime-policy.yaml](governance/runtime-policy.yaml) | Defines runtime execution boundaries. |
| [governance/activation-policy.yaml](governance/activation-policy.yaml) | Defines when and how governance activates. |
| [reviews/checklist.md](reviews/checklist.md) | Defines review criteria before implementation or automation. |
| [skills/templates/skill-charter.template.md](skills/templates/skill-charter.template.md) | Defines the standard charter for future skills. |
| [memory/README.md](memory/README.md) | Defines memory boundaries, precedence, and doctrinal promotion candidate handling. |
| [references/README.md](references/README.md) | Defines how stable references may be added without creating uncontrolled context. |

---

## Artifact Relationships

`SKILL.md` is the operational entrypoint for Codex. It should stay concise and
delegate detail to the canonical artifacts.

`FOUNDATION.md`, `AGENTS.md`, and `skill-charter.md` define identity and doctrine.

The `governance/` files define planner, runtime, and activation policy.

The `reviews/`, `skills/templates/`, `memory/`, and `references/` directories
support review, future skill creation, memory boundaries, precedence, doctrinal
promotion, and governed references.

---

## Evolution Policy

This repository should evolve in this order:

1. stabilize doctrine,
2. stabilize skill identity,
3. define agent constraints,
4. define planning rules,
5. define runtime policy,
6. define activation semantics,
7. define review process,
8. then evaluate whether automation is justified.

Premature code is architectural debt.

---

## Final Principle

> A skill should reduce operational complexity faster than it creates architectural complexity.
