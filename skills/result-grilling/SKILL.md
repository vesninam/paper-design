---
name: result-grilling
description: Critically review a planned scientific result for interpretability, controls, metrics, alternative explanations, and sufficient evidence. Use to challenge results/RXX.md before experiments or mockup creation.
---

# Result grilling

Test whether the proposed evidence could support the intended inference, including when the experiment does not yield the preferred pattern.

## Context and interaction

Read the target result description, linked tasks, and central question; inspect any existing mockup as an illustration rather than evidence. For a standalone result, review against the supplied purpose and state missing context. Work in the paper workspace only; do not alter the framework or skill files.

Lead with the most consequential weakness. Ask a focused question, use the reply, and continue where uncertainty remains. Do not substitute an unsolicited redesign for discussion of a scientific choice.

## Challenges

- Does the proposed comparison actually answer its linked task aspects? Is a claimed mechanism identifiable from these observations?
- Are the varied factors, controls, baselines, and reference truth sufficient? Could nuisance variables or interactions explain the apparent effect?
- Do metrics preserve scientifically important distinctions? For example, detectability need not imply accurate morphology or position.
- Are uncertainty, replication, sensitivity, and validation appropriate to the inference? Are thresholds justified independently of the desired outcome?
- Would null, reversed, mixed, or low-precision outcomes be interpretable? Could the design distinguish them?
- Does the representation expose the necessary dimensions? Does a combined result integrate related evidence or hide unrelated questions?
- Do the proposed generalizations exceed the sampling, model assumptions, or available observations?

## Artifact and completion

Add a review section to the relevant `results/RXX.md`, recording concern, consequence for inference, proposed remedy, researcher decision, and unresolved status. Apply agreed revisions while preserving the result ID, planned status, and decision history. Keep unaccepted consequential changes as proposals.

Report whether the result is ready, ready with stated limitations, or blocked by specific decisions. Identify affected task, evidence, mockup, and paper-map links for follow-up. Readiness means the design can produce interpretable evidence, not that the hypothesis is true or the paper is publishable.
