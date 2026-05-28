# AI Skill Governance

## Description

Governance skill for designing, reviewing, and evolving AI skills, planner rules,
runtime policies, activation semantics, and automation readiness.

This skill keeps skill work stable, controllable, repeatable, auditable, and
human-governable. It is a governance layer, not a runtime engine.

---

## Core Doctrine

> Do not automate, distribute, abstract, optimize, or orchestrate something that has
> not first been questioned, eliminated, simplified, and understood.

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

---

## Normative Language

- `must` defines a hard constraint.
- `should` defines default behavior unless a documented exception applies.
- `may` defines optional behavior.

When a requirement conflicts with a default, the hard constraint wins.

---

## When to Use

Use this skill before implementation planning when a request involves:

- creating, modifying, or reviewing a skill,
- changing `SKILL.md` or `AGENTS.md`,
- designing planner rules,
- designing runtime policies,
- defining activation conditions,
- changing memory strategy,
- adding tools,
- introducing automation,
- introducing orchestration,
- evaluating RAG,
- evaluating vector databases,
- evaluating multi-agent behavior,
- or expanding architecture.

Keep this skill lightweight for formatting, typo fixes, minor wording updates, and
low-risk documentation cleanup that does not change behavior, activation, runtime
policy, memory, tooling, automation, or architecture.

---

## Activation

This skill activates as a planning and governance constraint before execution.

It should influence reasoning before implementation details are chosen. Its role is
to question necessity, reduce complexity, preserve auditability, and prevent
premature automation.

---

## Automatic Activation Conditions

Activate automatically when work touches:

- `SKILL.md`,
- `AGENTS.md`,
- `planner-rules.yaml`,
- `runtime-policy.yaml`,
- `activation-policy.yaml`,
- skill charters,
- review checklists,
- memory policy,
- tool policy,
- orchestration,
- automation,
- RAG,
- vector databases,
- multi-agent systems,
- recursive agent behavior,
- background execution,
- hidden persistent state,
- or runtime side effects.

---

## Keyword Activation

Concrete trigger terms include:

- `skill`,
- `SKILL.md`,
- `AGENTS.md`,
- `planner rules`,
- `runtime policy`,
- `activation`,
- `activation conditions`,
- `automation`,
- `orchestration`,
- `multi-agent`,
- `RAG`,
- `retrieval`,
- `vector database`,
- `memory`,
- `persistent memory`,
- `background agent`,
- `recursive agent`,
- `tool chain`,
- `governance`,
- `auditability`,
- `human override`,
- and `runtime`.

Keyword activation must consider context. Do not overactivate on incidental mentions
that do not affect skill design, architecture, runtime behavior, memory, tools, or
automation.

---

## Behavioral Activation

Activate when a request would:

- increase architectural scope,
- add a new moving part,
- add or expand tool usage,
- introduce hidden or persistent state,
- reduce human inspectability,
- automate an unstable process,
- add recursive or autonomous behavior,
- increase context loading,
- or make system behavior harder to audit.

---

## Blocking Activation

Move from advisory guidance to restrictive or blocking guidance when a request
proposes:

- destructive or irreversible side effects,
- hidden persistent state,
- autonomous background execution,
- recursive orchestration,
- tool chains without clear terminal conditions,
- RAG without demonstrated retrieval need,
- vector databases without demonstrated retrieval need,
- multi-agent orchestration without operational necessity,
- framework proliferation,
- or automation before process stability.

Blocking guidance must require explicit justification, human review, or deferral
before implementation.

---

## Suppression Conditions

Suppress governance intervention, or keep it lightweight, when the work is limited
to:

- spelling fixes,
- formatting changes,
- simple wording improvements,
- non-behavioral documentation cleanup,
- renaming for clarity without semantic change,
- or reviewing content without changing architecture, activation, runtime behavior,
  memory, tooling, or automation.

Suppression does not apply when a small-looking change alters operational behavior,
activation semantics, runtime boundaries, or human governance.

---

## Activation Priority

High priority applies to hidden state, autonomous execution, background execution,
recursive orchestration, RAG, vector databases, multi-agent behavior, destructive
side effects, runtime side effects, and automation proposals.

Medium priority applies to new skills, skill upgrades, planner rule changes, runtime
policy changes, memory strategy, tool expansion, and architecture refactoring.

Low priority applies to formatting, wording, and low-risk documentation cleanup.

High priority maps to restrictive guidance and may become blocking when unsafe
automation, hidden state, irreversible side effects, or unbounded orchestration are
proposed. Medium priority maps to governing guidance. Low priority maps to advisory
guidance or suppression.

---

## Output Modes

### Advisory

Use for low-risk work. Identify tradeoffs, suggest simplification, and avoid
unnecessary ceremony.

### Governing

Use for normal skill design and review. Apply the mandatory engineering order,
validate boundaries, and preserve the canonical artifacts.

### Restrictive

Use when complexity, scope, or runtime risk is increasing. Require justification,
recommend scope reduction, and prefer simpler alternatives.

### Blocking

Use when the request would introduce unsafe automation, hidden state, irreversible
side effects, recursive orchestration, or unbounded complexity without explicit
authorization and operational justification.

---

## Responsibilities

This skill is responsible for:

- clarifying skill purpose and boundaries,
- defining activation conditions,
- reviewing planner and runtime policies,
- identifying unnecessary complexity,
- challenging premature automation,
- preserving human auditability,
- recommending simpler alternatives,
- and keeping governance artifacts consistent.

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
- runtime enforcement implementation,
- RAG infrastructure,
- vector database infrastructure,
- or framework platforms.

Those capabilities may be supported by other skills or tools, but this skill governs
whether such additions are justified.

---

## Hard Constraints

- Preserve the mandatory order: Question, Eliminate, Simplify, Accelerate,
  Automate.
- Do not automate unstable or unclear workflows.
- Do not optimize before simplification.
- Do not introduce hidden persistent state.
- Do not introduce RAG, vector databases, recursive agents, multi-agent
  orchestration, or framework-heavy systems without explicit operational
  justification.
- Preserve human visibility, auditability, reversibility, and override capability.
- Keep state, policies, and memory human-readable unless a stronger operational need
  is documented.

---

## Runtime Governance

Runtime behavior must remain:

- explicit,
- bounded,
- inspectable,
- auditable,
- reversible when the action can be reversed or explicitly confirmable when it
  cannot,
- and human-governable.

This skill does not implement runtime enforcement. It governs whether proposed
runtime behavior is justified, bounded, and understandable before implementation.

---

## Canonical Artifacts

This skill relies on these canonical artifacts:

- [README.md](README.md) for repository orientation,
- [FOUNDATION.md](FOUNDATION.md) for reusable engineering doctrine,
- [AGENTS.md](AGENTS.md) for agent-facing operational constraints,
- [skill-charter.md](skill-charter.md) for this skill's concrete charter,
- [governance/planner-rules.yaml](governance/planner-rules.yaml) for planning
  heuristics,
- [governance/runtime-policy.yaml](governance/runtime-policy.yaml) for runtime
  boundaries,
- [governance/activation-policy.yaml](governance/activation-policy.yaml) for
  activation policy,
- [reviews/checklist.md](reviews/checklist.md) for review criteria,
- [skills/templates/skill-charter.template.md](skills/templates/skill-charter.template.md)
  for future skill charters,
- [memory/README.md](memory/README.md) for memory boundaries,
- and [references/README.md](references/README.md) for governed reference material.

Root-level duplicates of governed policies should not be created.

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

A good output from this skill should reduce complexity, clarify boundaries, improve
decision quality, expose unjustified assumptions, and preserve human governance.

A bad output adds ceremony, creates generic frameworks, hides complexity, overuses
YAML, introduces runtime before doctrine, or makes the skill harder to govern than
the skills it supports.

---

## Final Principle

> A skill should reduce operational complexity faster than it creates architectural
> complexity.
