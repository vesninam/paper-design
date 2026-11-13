---
name: result-design
description: Design coherent planned scientific results and their evidence specifications in results/RXX.md. Use to compose reviewed research tasks into interpretable results before conducting experiments.
---

# Result design

Compose a compact scientific argument from the tasks. A planned result is an evidence specification, not an obtained finding or a prediction that must come true.

## Context

Read the question, reviewed tasks, terminology, and existing result descriptions in the paper workspace. For a standalone experiment, use its supplied question and constraints and state any missing context. Clarify the destination before writing if ambiguous; do not edit the framework or skills.

Read [references/result-questions.md](references/result-questions.md) when developing or substantially revising a result. Use its questions selectively and interactively, rather than asking the researcher to fill out the entire reference at once.

## Procedure

1. Group related task aspects into coherent contributions. The relationship is many-to-many: one result can address several tasks, and a task may need complementary results. Do not impose one figure per task or merge unrelated evidence to reduce result count.
2. Propose the result's scientific purpose and the task aspects it integrates. Establish what comparison or evidence would discriminate among meaningful answers before choosing the visual form.
3. Guide the researcher through consequential choices point by point: varied factors, controlled conditions, data or simulations, baselines, metrics, uncertainty, validation, and sufficient evidence. Mark unresolved choices; do not invent answers to complete the template.
4. Specify alternative interpretations, including null, contradictory, and inconclusive outcomes. Separate data-quality or precision criteria from a preferred scientific outcome; justify thresholds rather than choosing them to produce a desired conclusion.
5. Choose figures, tables, or other representations that expose the comparison. Identify dependencies, feasibility limits, and evidence that a mockup cannot supply.

## Artifact and completion

Create or update `results/R01.md`, `results/R02.md`, etc., retaining existing IDs and links. Each description should contain:

- ID, title, and status (`draft` or `planned`; never mark unobserved evidence as obtained).
- Scientific purpose, linked task IDs, and how their aspects form one contribution.
- Evidence and experiment design, data requirements, factors, controls, baselines, and dependencies.
- Measurements, uncertainty and robustness checks, sufficient-evidence criteria, and limitations.
- Intended representation and interpretation of alternative outcomes.
- Open decisions, review history, and mockup links when available.

For the result set, check essential task coverage and paper-scale coherence. A result is ready for review and mockup when its purpose, evidence requirements, and interpretation are explicit. Use `result-grilling` to challenge the specification and `result-mockup` to make its representation concrete, if available; neither produces actual evidence.
