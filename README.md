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

> Do not automate, distribute, abstract, optimize, or orchestrate something that has not first been questioned, reduced, simplified, and understood.

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

## Repository Structure

Target structure:

```text
ai-skill-governance/
├── README.md
├── SKILL.md
├── FOUNDATION.md
├── AGENTS.md
│
├── doctrine/
│   └── engineering-bedrock.md
│
├── governance/
│   ├── planner-rules.yaml
│   ├── runtime-policy.yaml
│   ├── activation-policy.yaml
│   └── complexity-budget.yaml
│
├── reviews/
│   └── checklist.md
│
├── skills/
│   └── templates/
│       └── skill-charter.template.md
│
├── memory/
│   └── decisions/
│
└── references/
    └── musk-engineering-rules.md
```

The structure should remain small until additional artifacts justify their existence.

---

## Artifact Families

| Artifact | Purpose |
|---|---|
| `SKILL.md` | Defines this skill's operating identity and boundaries. |
| `FOUNDATION.md` | Defines reusable engineering doctrine. |
| `AGENTS.md` | Defines agent-facing operational constraints. |
| `governance/planner-rules.yaml` | Defines planning heuristics and complexity governance. |
| `governance/runtime-policy.yaml` | Defines runtime execution boundaries. |
| `governance/activation-policy.yaml` | Defines when and how governance activates. |
| `reviews/checklist.md` | Defines review criteria before implementation or automation. |
| `skills/templates/skill-charter.template.md` | Defines the standard charter for future skills. |

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
