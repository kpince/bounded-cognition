---
name: sleep-cycle-consolidation
description: Use when running offline consolidation over sessions, feedback, failures, successes, or candidate notices to produce staged reviewable adaptations without auto-merging them.
version: 0.1.0
author: Bounded Cognition Project
license: MIT
metadata:
  hermes:
    tags: [sleep-cycle, consolidation, adaptation-ledger, adaptive-agents, governance]
    related_skills: [bounded-cognition, cognitive-lineage-governance]
---

# Sleep-Cycle Consolidation

## Overview

A sleep cycle is an offline consolidation pass. It reviews accumulated experience and proposes bounded candidate adaptations.

It does not change model weights. It does not mutate core behavior. It does not auto-merge skill edits. It stages reviewable candidates for human, operator, or expert review.

```text
review experience
  -> mine signals
  -> group patterns
  -> propose bounded candidates
  -> attach evidence and gates
  -> stage for review
```

## When to Use

Use this skill when:

- reviewing recent sessions for recurring failures or successes;
- converting user corrections into candidate procedure changes;
- mining candidate notices from child agents or profiles;
- preparing adaptation-ledger entries;
- producing review packets before patching skills;
- creating regression examples from accepted adaptations.

Do not use this skill to auto-patch, auto-merge, or convert weak one-off anecdotes into operational doctrine.

## Inputs

Possible inputs:

- session history;
- operator corrections;
- expert/domain feedback;
- repeated tool failures;
- repeated successful workflows;
- candidate cognitive PRs;
- prior accepted/rejected adaptations;
- existing regression examples.

## Required Output Statement

Every sleep report must include this statement:

```text
This report proposes candidate adaptations only. No operational skill, memory, doctrine, or code has been modified unless explicitly listed under Approved Changes.
```

## Candidate Format

Use this format for each proposed adaptation:

```text
CAND-YYYY-MM-DD-NN — Short title

Type: skill patch | procedure | distinction | regression example | upstream notice | rejection note
Status: proposed | accepted | rejected | superseded
Scope: agent | lineage | domain:<name> | project:<name> | profile:<name> | experimental
Source signals:
- ...

Proposal:
...

Rationale:
...

Risk:
...

Gate:
...

Regression example:
problem -> expected behavior after adaptation
```

## Procedure

1. Gather the bounded input set.
2. Mine signals: corrections, failures, successes, repeated patterns, validation moments, and rejected ideas.
3. Group signals by affected workflow, skill, project, profile, or lineage level.
4. Propose the smallest bounded candidate adaptation.
5. Assign evidence, risk, scope, and gate.
6. Add a regression example when behavior should change.
7. Mark all candidates `proposed` unless explicitly approved.
8. Do not apply changes unless separately instructed.

## Gates

Choose a gate that matches the domain:

- Human/operator gate for project or agent behavior.
- Expert gate when representing domain reality.
- Regression check for deterministic workflows.
- Eval prompt for behavioral expression.
- Mixed gate when both interpretation and deterministic checks matter.

## Common Pitfalls

1. **Summaries instead of candidates.** A sleep report must produce reviewable proposals, not just recap.
2. **Auto-merging.** Sleep proposes; review accepts or rejects.
3. **Oversized adaptations.** Split broad changes into small candidates.
4. **No rejected-hypothesis memory.** Rejections prevent repeated bad ideas.
5. **Weak evidence.** Mark low-confidence candidates as questions or experimental.
6. **Forgetting gates.** Every candidate needs a validation path.

## Verification Checklist

- [ ] Input scope is clear.
- [ ] Required no-auto-merge statement is present.
- [ ] Each candidate has type, status, scope, source signals, proposal, rationale, risk, gate, and regression example when relevant.
- [ ] No operational artifact was modified unless separately approved.
- [ ] Rejected or low-confidence ideas are preserved as such.
