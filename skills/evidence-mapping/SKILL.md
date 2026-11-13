---
name: evidence-mapping
description: Build and review evidence.md linking scientific tasks and conditional claims to required evidence and planned results. Use to detect coverage gaps, weak inferences, redundancy, and intentional exclusions in a research design.
---

# Evidence mapping

Check scientific sufficiency, not merely whether every task ID appears somewhere. A planned result link identifies a route to evidence, not evidence already obtained.

## Context

Read `question.md`, `tasks.md`, all relevant `results/RXX.md`, and existing `evidence.md` in the paper workspace. Use actual artifact IDs rather than IDs copied from framework examples. Clarify the workspace before writing if ambiguous. Do not alter the framework or skill files.

## Mapping and review

1. For each task, state the question, possible or conditional claim, and evidence needed to support it within scope.
2. Link the result IDs that supply that evidence and explain their roles. Preserve many-to-many relationships; distinguish complementary evidence from repeated measures of the same thing.
3. Compare the requirement with the actual result specification: controls, metrics, uncertainty, validation, and generalization limits. An illustrative mockup does not satisfy any empirical requirement.
4. Identify missing evidence, partial coverage, unsupported claims, redundant results, and coherent opportunities to combine evidence. Keep a gap visible rather than inventing a result or silently weakening a task.
5. Retain intentionally excluded and deferred tasks with reasons and the consequences for the central answer. Propose any necessary narrowing to the researcher; do not silently assume it is accepted.

## Artifact and completion

Write `evidence.md` with a matrix such as:

| Task | Scientific question / conditional claim | Required evidence | Result IDs and roles | Coverage | Evidence state | Limitations / decision |
| --- | --- | --- | --- | --- | --- | --- |

Use coverage values such as `covered by plan`, `partial`, `missing`, `intentionally excluded`, and `deferred`. Keep evidence state separate, normally `planned` in Phase A; only mark evidence as obtained or evaluated when real artifacts support that state. Preserve existing execution evidence if present.

Add a short gap and decision register, plus any results with no clear contribution. Verify all linked task and result IDs exist and that mapped aspects match the descriptions. Completion means essential tasks have sufficient planned evidence and all remaining exclusions or gaps are explicit, with no stronger conclusion implied than the design permits.
