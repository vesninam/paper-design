---
name: paper-mapping
description: Represent the scientific argument as canonical paper-map.yaml and a derived Mermaid graph. Use after evidence mapping to expose dependencies, synthesis, and unsupported steps from the research question to conditional conclusions.
---

# Paper mapping

Represent scientific logic, not figure numbering, manuscript sections, or execution order. YAML is canonical; Mermaid is a visualization derived from it.

## Context

Read the question, tasks, result descriptions, and evidence matrix in the paper workspace. If coverage is unresolved, retain the gaps visibly. Clarify ambiguous destinations before writing; do not modify the framework or skills. Inspect an existing map's schema and preserve it when adequate rather than forcing migration.

## Construct the argument

Identify the question, relevant result nodes, intermediate synthesis or claims, and scoped conclusion. Preserve existing task and result IDs. Distinguish a real scientific dependency from shared subject matter or a convenient presentation sequence. Label edges with the logical relationship and explain what information they carry.

Do not assume a favorable result. Express claims and conclusions conditionally until supported by actual evidence. Show branches that provide complementary evidence and where they must be combined. Flag circular reasoning, unsupported generalization, and missing premises instead of drawing an apparently complete path.

## Canonical representation

If no schema exists, use a compact structure of this form, adapted to the actual project:

```yaml
version: 1
stage: research-design
nodes:
  - id: Q
    type: question
    label: Central scientific question
    artifact: question.md
    status: formulated
  - id: R01
    type: result
    label: Planned comparison
    artifact: results/R01.md
    task_ids: [T01]
    status: planned
  - id: C01
    type: conclusion
    label: Scoped answer conditional on the evidence
    status: conditional
edges:
  - from: Q
    to: R01
    relation: motivates
    rationale: This comparison addresses a necessary aspect of the question.
  - from: R01
    to: C01
    relation: may-support
    rationale: The answer depends on the measured comparison and its uncertainty.
open_issues: []
```

The example is structural, not a default scientific argument. Add synthesis nodes and unresolved issues where the real reasoning requires them. If the logical graph contains a cycle, distinguish an iterative research feedback loop from a circular evidential argument.

## Artifacts and validation

Write `paper-map.yaml`, then derive `paper-map.mmd` using stable node IDs and quoted, escaped labels. Encode edge relationships and planned or conditional status in visible labels; include open gaps rather than relying only on color. Regenerate Mermaid after YAML changes rather than editing the two independently.

Parse YAML when tools are available. Check unique node IDs, existing edge endpoints, valid artifact paths and task IDs, and agreement between the YAML nodes and edges and the Mermaid graph. Render Mermaid if a renderer is available; otherwise state that rendering was not checked.

Completion means the logical path to a scoped answer is explicit, with unsupported steps recorded. It does not certify that the planned evidence will support the intended conclusion.
