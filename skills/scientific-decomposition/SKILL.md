---
name: scientific-decomposition
description: Decompose a scientific question into independently answerable research tasks in tasks.md. Use after question formulation, before specifying individual results, figures, or implementation work.
---

# Scientific decomposition

Decompose what must be learned, not the sequence of coding, plotting, or writing operations.

## Context

Read `question.md`, relevant `terminology.md`, and any existing `tasks.md` in the paper workspace. A supplied standalone question is sufficient for a provisional decomposition; label missing scope decisions. Clarify an ambiguous output destination before writing. Modify paper artifacts only, leaving the framework unchanged.

## Procedure

1. Identify the distinct aspects of the central question: phenomena, dependencies, comparisons, mechanisms, boundary conditions, and validation needs, as relevant.
2. Express each task as a specific scientific question or an action with an identifiable answer. Explain how its answer contributes to the central question.
3. Separate tasks whose answers require distinct reasoning, while avoiding artificial fragmentation of closely related questions. Identify scientific dependencies without prescribing implementation order.
4. Check that the set covers the stated scope and can be answered with plausible evidence. Keep figures, algorithms, and experiment parameters out unless essential to the scientific meaning.
5. Surface choices about breadth and feasibility to the researcher. Preserve optional, deferred, and excluded tasks with reasons rather than erasing them.

## Artifact and completion

Write `tasks.md` with stable IDs (`T01`, `T02`, …), each task's question, contribution to the main question, answer criterion or evidence needed at a high level, dependencies, and scope status. Reuse existing IDs; do not renumber survivors or reuse retired IDs. Record unresolved decisions separately.

Tasks are ready for `task-review` when each has a potentially identifiable answer and the set plausibly addresses the central question within the stated scope. This skill does not establish that sufficient results have been designed; that is checked later through result design and evidence mapping.
