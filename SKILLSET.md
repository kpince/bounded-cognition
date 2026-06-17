# Bounded Cognition Skill Set

This repository contains a Hermes skill set for bounded, reviewable, externalized cognition.

## Load order

1. `bounded-cognition` — always load first. It defines the frame and routes to the other skills.
2. `cognitive-lineage-governance` — load when reviewing a local adaptation, clone discovery, or proposed upstream contribution.
3. `sleep-cycle-consolidation` — load when mining experience into staged candidate adaptations.

## Operational contract

The skill set teaches agents to improve through externalized reviewable artifacts, not through unrestricted self-modification.

Allowed outputs:

- candidate skill patches
- cognitive PRs
- sleep-cycle reports
- regression examples
- rejection notes
- scope-labeled doctrine notes
- validation questions

Forbidden shortcuts:

- raw memory sync
- private transcript dumping
- automatic upstream merge
- broad doctrine from a single weak signal
- claiming model-weight or core-system adaptation

## Minimal workflow

```text
experience
  -> local adaptation
  -> candidate cognition
  -> reviewable artifact
  -> human/operator/expert gate
  -> accepted/rejected/experimental decision
  -> selective inheritance
```
