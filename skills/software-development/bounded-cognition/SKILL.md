---
name: bounded-cognition
description: Use when designing or operating adaptive AI agents that learn through bounded, reviewable, externalized cognitive artifacts rather than raw memory sync, model-weight claims, or unrestricted self-modification.
version: 0.1.0
author: Bounded Cognition Project
license: MIT
metadata:
  hermes:
    tags: [bounded-cognition, adaptive-agents, lineage, skills, governance]
    related_skills: [cognitive-lineage-governance, sleep-cycle-consolidation]
---

# Bounded Cognition

## Overview

Bounded cognition is a framework for safe long-term adaptation in AI agents.

The core idea is a middle layer: **bounded, reviewable, externalized cognition**. Instead of claiming the model changed, syncing raw memory, or letting an agent freely rewrite itself, the agent learns into external artifacts that can be inspected, tested, rejected, revised, and selectively inherited.

Externalized cognition can include:

- skills
- procedures
- doctrine notes
- cognitive pull requests
- sleep-cycle reports
- adaptation ledgers
- evaluation prompts
- regression examples
- rejection notes
- question patterns
- inheritance rules

The system improves by converting experience into reviewable artifacts.

```text
experience
  -> local adaptation
  -> candidate cognition
  -> reviewed artifact
  -> selective inheritance
```

## When to Use

Use this skill when:

- designing adaptive-agent workflows;
- reviewing whether a local agent discovery should become reusable guidance;
- introducing lineage, descendant, clone, or profile governance;
- preventing unsafe self-modification language;
- deciding how skills, memories, evals, ledgers, or procedures should evolve;
- preparing to use the `cognitive-lineage-governance` or `sleep-cycle-consolidation` skills.

Do not use this skill to justify automatic self-modification, raw transcript sync, private memory sharing, or unreviewed skill rewrites.

## Core Terms

### Bounded

Adaptations are scoped, named, and constrained. A local success does not automatically become global doctrine.

### Reviewable

Adaptations are visible to a human, operator, expert, or governance process. They can be accepted, rejected, revised, narrowed, tested, or kept local.

### Externalized

The cognition lives outside model weights in artifacts that can be versioned, inspected, linked, and evaluated.

### Cognition

The artifacts encode ways of interpreting, asking, distinguishing, suppressing, prioritizing, inheriting, and adapting. They are not merely config.

## Load Order

1. Load `bounded-cognition` first for the conceptual and safety frame.
2. Load `cognitive-lineage-governance` when a local discovery may move upstream.
3. Load `sleep-cycle-consolidation` when mining experience into candidate adaptations.

## Operating Loop

Use this loop for adaptive-agent learning:

1. Observe experience.
2. Identify a local adaptation, correction, repeated failure, repeated success, or operator signal.
3. Convert it into candidate cognition.
4. Choose the artifact type: cognitive PR, skill patch candidate, eval, regression example, rejection note, or doctrine note.
5. Assign evidence, risk, scope, and validation gate.
6. Stage for review.
7. Accept, reject, revise, keep local, or mark experimental.
8. Decide inheritance separately from acceptance.

## Safety Rules

- Do not claim model weights changed.
- Do not claim the core system mutated unless actual code/config changed and was verified.
- Do not auto-merge sleep-cycle output.
- Do not sync raw memories, transcripts, private messages, customer data, or secrets upstream.
- Do not treat agent self-report as sufficient evidence.
- Do not promote a local adaptation to general doctrine without scope and validation.
- Do not confuse accepted into lineage with inherited by all descendants.
- Preserve rejected candidates as negative signal.

## Artifact Types

Prefer reviewable artifacts:

- **Cognitive PR** — a proposed upstream cognitive update with source, evidence, scope, risk, and gate.
- **Skill patch candidate** — a bounded proposed edit to an existing skill.
- **Sleep-cycle report** — offline consolidation output containing staged candidates.
- **Regression example** — a problem and expected future behavior after an accepted adaptation.
- **Rejection note** — a candidate rejected with rationale, preserved to prevent repeated bad edits.
- **Doctrine note** — a stable principle or distinction, usually narrow and scoped.
- **Evaluation prompt** — a behavioral check that reveals whether an adaptation is expressed.

## Common Pitfalls

1. **Raw memory sync.** Memory is not lineage by default. Distill and redact before review.
2. **Auto-merging.** A candidate adaptation is not accepted until explicitly reviewed.
3. **Overgeneralizing.** Local pressure can produce local truth, not universal doctrine.
4. **Vague self-improvement claims.** Say which artifact changed, not that the agent magically improved.
5. **No rejection trail.** Rejected candidates are useful negative signal.
6. **Conflating acceptance and inheritance.** A lineage may preserve an insight without making every descendant inherit it.

## Verification Checklist

- [ ] Experience, local adaptation, candidate cognition, accepted artifact, and inherited behavior are distinguished.
- [ ] The proposed adaptation is externalized in a reviewable artifact.
- [ ] Scope, evidence, risk, and gate are stated.
- [ ] Private or local material is removed or explicitly approved.
- [ ] No model-weight or unrestricted self-modification claim is made.
- [ ] Acceptance and inheritance are handled as separate decisions.
