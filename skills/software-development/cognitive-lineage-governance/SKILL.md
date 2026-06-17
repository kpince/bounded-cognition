---
name: cognitive-lineage-governance
description: Use when a clone, profile, descendant, or agent reports a local discovery that may become upstream lineage material through a reviewed cognitive pull request.
version: 0.1.0
author: Bounded Cognition Project
license: MIT
metadata:
  hermes:
    tags: [lineage, cognitive-pr, governance, inheritance, adaptive-agents]
    related_skills: [bounded-cognition, sleep-cycle-consolidation]
---

# Cognitive Lineage Governance

## Overview

Cognitive lineage governance controls how local agent discoveries move upstream into reusable cognition.

Core rule:

```text
Do not synchronize cognition. Curate it through cognitive pull requests.
```

A child profile, clone, descendant, or local agent may adapt under pressure. That adaptation is not automatically true, safe, or general. It becomes lineage material only after it is distilled, redacted, scoped, reviewed, and accepted.

## When to Use

Use this skill when:

- an agent or profile has learned something locally;
- a clone wants to contribute a discovery upstream;
- a local workflow improvement may become reusable guidance;
- deciding whether to patch a skill, add an eval, add a doctrine note, or keep a discovery local;
- reviewing cognitive PRs;
- deciding who should inherit an accepted adaptation.

Do not use this skill to merge raw memory, raw session logs, private client context, or agent self-report without review.

## Cognitive PR Format

Convert proposed upstream contributions into this shape:

```text
Cognitive PR

Source agent/profile:
Source context/domain:
Proposed title:
Artifact type:
Proposed lineage update:
Evidence:
Fitness environment:
Observed pressure:
Resonance or validation signals:
Why this may be reusable:
What has been removed/redacted:
Risks and possible overfit:
Conflicts with existing doctrine:
Suggested scope:
Suggested target artifact:
Should descendants inherit by default?: yes / no / test first
Validation or expression eval needed?: yes / no / deferred, with why
Acceptance criteria:
Rejection criteria:
Reviewer decision needed:
```

## Scope Labels

Assign the narrowest truthful scope:

- `lineage-core` — broadly applicable across descendants.
- `agent-core` — reusable for agents in this family.
- `domain-seed/<domain>` — domain-scoped.
- `project/<name>` — project-scoped.
- `profile/<name>` — profile-scoped.
- `clone-local` — valid locally, not upstream.
- `experimental` — promising, not default inherited.
- `eval-only` — useful as a test, not doctrine.
- `reference-only` — background, not behavioral instruction.

If scope is unclear, choose narrower or experimental.

## Evidence Review

Strong evidence:

- human/operator/expert validation;
- repeated usefulness across contexts;
- correction that prevented a known failure;
- behavioral eval improvement;
- clearer objective inference;
- validated readback or resonance signal.

Weak evidence:

- agent self-report;
- a single anecdote;
- elegance or plausibility;
- local workaround for temporary state;
- private context that cannot be safely generalized.

## Review Decisions

Use these decisions:

- **Accept** — safe, useful, evidenced, scoped, and targeted.
- **Reject** — unsafe, false, overfit, already covered, or not useful enough.
- **Revise and resubmit** — promising but needs redaction, evidence, scope, or target refinement.
- **Keep local** — valid in the source environment but not lineage material.
- **Accept experimentally** — test under limited inheritance.
- **Eval only** — preserve as a behavioral check.
- **Reference only** — useful context, not operational doctrine.

## Inheritance Is Separate

After acceptance, ask:

```text
Who should inherit this, and when?
```

Acceptance preserves a reviewed artifact. It does not force all descendants to inherit it.

## Redaction Gate

Reject or return for revision if the candidate includes:

- secrets, keys, auth material, or credentials;
- raw private messages;
- raw client/customer/employee/financial/legal data;
- unapproved identifying details;
- raw transcripts or memory dumps;
- local paths or implementation accidents presented as doctrine.

## Common Pitfalls

1. **Merging before review.** Always create the cognitive PR first.
2. **Trusting the source clone.** Trust does not remove the need for evidence and scope.
3. **Universal inheritance by default.** Most adaptations should start narrow.
4. **Raw transcript dependence.** Distill the adaptation; do not move the life history.
5. **No eval for behavior change.** If behavior should change, add or defer an explicit eval.

## Verification Checklist

- [ ] Candidate is in cognitive PR format.
- [ ] Source, environment, and observed pressure are identified.
- [ ] Private/local material has been removed.
- [ ] Evidence and risk are listed.
- [ ] Scope is assigned.
- [ ] Acceptance and inheritance are treated separately.
- [ ] A reviewer decision is requested before operational changes.
