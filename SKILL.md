# SKILL.md

# AI Skill Governance

## Purpose

This skill defines a cognitive governance rail for designing, building, reviewing, and evolving AI skills.

It helps agents and human operators:

- define skill boundaries,
- reject unnecessary complexity,
- apply planning discipline,
- preserve runtime governance,
- evaluate automation readiness,
- and evolve skills without architectural drift.

This skill is not intended to execute domain work directly.

It is intended to guide how skills should be reasoned about, constrained, reviewed, and improved.

---

## Core Identity

`ai-skill-governance` is a support skill for skill engineering.

It exists to assist agents in:

- defining new skills,
- reviewing existing skills,
- improving skill maturity,
- identifying architectural drift,
- evaluating runtime risk,
- and preserving human-governable AI systems.

It should function as:

- a cognitive rail,
- a planning constraint layer,
- a complexity governance reference,
- and an architectural review companion.

It should not become:

- a general-purpose orchestration engine,
- an autonomous agent runtime,
- a framework platform,
- a code generator by default,
- or a substitute for human architectural judgment.

---

## Core Doctrine

> Do not automate, distribute, abstract, optimize, or orchestrate something that has not first been questioned, reduced, simplified, and understood.

Complexity is not value.

Complexity is operational cost unless continuously justified.

---

## Mandatory Engineering Order

All skill work must follow this order:

1. Question
2. Eliminate
3. Simplify
4. Accelerate
5. Automate

Do not optimize before simplification.

Do not automate before stability.

Do not introduce sophistication without clear operational need.

---

## Activation Intent

This skill should activate when the user or agent is working on:

- defining a skill,
- reviewing a skill,
- improving a skill,
- creating a skill charter,
- designing agent instructions,
- designing runtime policies,
- designing planner rules,
- defining activation semantics,
- introducing automation,
- adding tools,
- adding memory,
- adding orchestration,
- evaluating RAG,
- evaluating multi-agent behavior,
- or changing skill architecture.

This skill should remain lightweight when the task is:

- simple content editing,
- formatting,
- minor wording improvement,
- or low-risk documentation cleanup.

---

## Primary Responsibilities

This skill is responsible for helping with:

### Skill Definition

- clarify purpose,
- define scope,
- identify non-goals,
- establish operating boundaries,
- define expected behavior,
- identify required references,
- and specify activation conditions.

### Skill Construction

- propose minimal repository structures,
- define canonical artifacts,
- separate doctrine from runtime policy,
- separate references from activators,
- avoid premature code,
- and preserve documentation-first evolution.

### Skill Review

- evaluate complexity,
- detect overengineering,
- identify missing governance,
- challenge vague requirements,
- expose hidden assumptions,
- and validate human auditability.

### Skill Improvement

- propose controlled evolution,
- identify maturity gaps,
- refine activation semantics,
- improve planner rules,
- improve runtime policies,
- and update supporting documentation consistently.

---

## Non-Goals

This skill does not directly own:

- domain-specific execution,
- business workflow automation,
- external platform integration,
- autonomous write operations,
- background execution,
- multi-agent orchestration,
- persistent hidden memory,
- or runtime enforcement implementation.

Those capabilities may be supported by other skills or tools, but this skill governs whether such additions are justified.

---

## Architectural Preferences

Prefer:

- markdown-first documentation,
- explicit contracts,
- local reasoning,
- human-readable memory,
- deterministic execution paths,
- bounded context loading,
- simple repository structures,
- and minimal tooling.

Avoid by default:

- premature `src/` directories,
- unnecessary CLI scaffolding,
- vector databases without retrieval need,
- RAG without evidence,
- multi-agent orchestration without necessity,
- recursive tool chains,
- hidden mutable state,
- and framework proliferation.

---

## Reference Model

This skill is expected to rely on these artifact families:

```text
ai-skill-governance/
├── README.md
├── SKILL.md
├── AGENTS.md
├── FOUNDATION.md
│
├── doctrine/
├── governance/
├── reviews/
├── skills/
├── memory/
└── references/
```

Each folder must justify its existence.

The repository should remain small until evolution demands otherwise.

---

## Cognitive Governance Rail

The cognitive governance rail is composed of:

- doctrine,
- planning heuristics,
- runtime constraints,
- activation policies,
- complexity budgets,
- review checklists,
- skill charters,
- and human governance principles.

The rail does not replace agent reasoning.

It conditions agent reasoning.

---

## Activation Layers

This skill should distinguish between:

### References

Stable knowledge used for context.

Examples:

- foundation principles,
- engineering doctrine,
- anti-patterns,
- architectural preferences.

### Activators

Rules that determine when governance should intervene.

Examples:

- user asks to add orchestration,
- user asks to create a new skill,
- user asks to introduce automation,
- user proposes distributed memory,
- user requests runtime behavior changes.

### Enforcement

Constraints that determine how strongly the skill should respond.

Examples:

- advisory,
- warning,
- require justification,
- require human confirmation,
- reject or defer.

---

## Runtime Philosophy

Runtime behavior should remain:

- explicit,
- bounded,
- inspectable,
- auditable,
- reversible where possible,
- and human-governable.

The skill should resist:

- uncontrolled autonomy,
- hidden state mutation,
- unbounded context growth,
- recursive execution,
- unnecessary tool chaining,
- and automation of unstable processes.

---

## Human Governance

Human operators must retain:

- visibility,
- override capability,
- execution awareness,
- architectural control,
- and final authority over destructive or persistent actions.

If humans cannot understand what changed, why it changed, and what risk was introduced, the skill has failed.

---

## Evolution Policy

This skill should evolve by:

1. strengthening clarity,
2. reducing ambiguity,
3. improving activation semantics,
4. refining governance artifacts,
5. documenting decisions,
6. and only later considering automation.

Do not add code until the documentation-based operating model is stable.

Do not add runtime behavior until activation and enforcement semantics are clear.

---

## Quality Bar

A good output from this skill should:

- reduce complexity,
- clarify boundaries,
- improve decision quality,
- expose tradeoffs,
- identify unjustified assumptions,
- preserve human governance,
- and produce artifacts that agents can actually use.

A bad output from this skill:

- adds ceremony,
- creates generic frameworks,
- hides complexity,
- overuses YAML,
- introduces runtime before doctrine,
- or makes the skill harder to govern than the skills it supports.

---

## Final Principle

> A skill should reduce operational complexity faster than it creates architectural complexity.

If it does not, it is no longer a skill.

It is infrastructure debt.
