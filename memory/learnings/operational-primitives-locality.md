# Operational Primitives Locality

## Learning

Operational primitives that define a skill's mechanical behavior should remain
inside that skill's `SKILL.md` unless there is a concrete external reuse case or
a separate maintenance boundary that justifies extraction.

This keeps doctrine and behavior aligned, avoids a second authority layer, and
reduces drift between the skill's stated rules and its actual execution model.

## Evidence

This learning came from shaping `ai-skill-governance` itself. A separate artifact
for the 10 operational actions was unnecessary once the actions were expressed as
internal doctrine with fixed execution shape.

## Governance Notes

- Compatible with the required order: Question, Eliminate, Simplify, Accelerate,
  Automate.
- Reduces duplication without adding runtime behavior, hidden state, or
  orchestration.
- Applies only when the goal is reusable operational behavior, not documentation
  cataloging.

