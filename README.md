# Bounded Cognition

A skill set and research framework for bounded, reviewable, externalized cognition in adaptive AI agents.

This repository packages the framework as a usable Hermes skill set. It is also the home for the paper, examples, templates, and diagrams that explain the architecture.

## Core claim

Long-lived AI agents can adapt safely by learning into external artifacts — skills, ledgers, cognitive pull requests, sleep-cycle reports, evaluation prompts, procedures, and reviewed doctrine — instead of relying only on raw memory, model retraining, or unrestricted self-modification.

This is not an autonomous self-modification framework. It is a governance and artifact protocol for safe adaptation.

## What this gives a Hermes agent

Load these skills when you want an agent to:

- reason about bounded, reviewable, externalized cognition;
- review a local adaptation before promoting it into reusable doctrine;
- prepare cognitive pull requests from child profiles, clones, or other agents;
- run sleep-cycle consolidation without auto-merging outputs;
- distinguish experience, local adaptation, candidate cognition, accepted artifacts, and inherited behavior;
- preserve provenance, redaction, scope, and human/operator review gates.

## Install

### Option 1: add this repository as a skill tap

```bash
hermes skills tap add https://github.com/kpince/bounded-cognition
hermes skills install bounded-cognition
```

If your Hermes version expects a specific skill identifier from the tap, browse/search after adding the tap:

```bash
hermes skills browse
hermes skills search bounded-cognition
```

### Option 2: install individual skills directly

```bash
hermes skills install https://raw.githubusercontent.com/kpince/bounded-cognition/main/skills/software-development/bounded-cognition/SKILL.md
hermes skills install https://raw.githubusercontent.com/kpince/bounded-cognition/main/skills/software-development/cognitive-lineage-governance/SKILL.md
hermes skills install https://raw.githubusercontent.com/kpince/bounded-cognition/main/skills/software-development/sleep-cycle-consolidation/SKILL.md
```

## First use

In a Hermes session:

```text
/skill bounded-cognition
```

Then ask one of:

```text
Use the bounded-cognition skill set to review this candidate adaptation.
```

```text
Run a sleep-cycle consolidation pass over these notes and stage candidate adaptations only.
```

```text
Turn this local agent discovery into a cognitive PR without syncing raw memory upstream.
```

## Skill set

### `bounded-cognition`

The umbrella entrypoint. Defines the framework, safety rules, artifact types, and load order.

### `cognitive-lineage-governance`

Use when a child profile, clone, descendant, or agent has learned something locally and wants to send it upstream as a reviewable candidate.

### `sleep-cycle-consolidation`

Use when running offline consolidation over sessions, failures, successes, corrections, or candidate notices. Produces staged proposals, not automatic operational changes.

## Repository structure

```text
skills/                  Hermes-installable skills
paper/                   paper seed, abstract, outline
examples/                worked examples and sample artifacts
templates/               reusable cognitive PR and sleep-cycle templates
diagrams/                mermaid diagrams
```

## Safety principles

- Do not claim model weights changed.
- Do not claim Hermes core behavior mutated.
- Do not auto-merge sleep-cycle outputs.
- Do not synchronize raw memory upstream.
- Do not absorb private/client data into lineage artifacts.
- Do not universalize local adaptations without evidence, scope, and review.
- Distinguish accepted artifacts from inherited behavior.
- Preserve rejected candidates as negative signal.

## Paper

Working title:

> Bounded, Reviewable, Externalized Cognition: A Lineage Framework for Adaptive AI Agents Without Unrestricted Self-Modification

See `paper/abstract.md` and `paper/outline.md`.
