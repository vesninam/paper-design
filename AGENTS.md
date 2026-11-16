# Scientific Paper Design — Agent Instructions

## Purpose

This repository provides a reusable framework for designing scientific papers before writing the manuscript.

The agent assists the researcher in formulating scientific questions, developing scientific tasks, designing results, evaluating evidence coverage, and constructing a paper map.

## Repository structure

- `framework/` — reusable workflow, stages, skills, templates, and examples.
- `papers/` — individual paper workspaces.

The framework is read-only during paper development unless the researcher explicitly requests framework modifications.

## Session initialization

When starting a new conversation about paper design, or when the user asks to start or continue working:

1. Inspect the `papers/` directory to identify existing paper workspaces.
2. Read `framework/workflow.md` to understand the overall process.
3. Determine the appropriate entry point according to the following rules.

### Case A. No existing papers

If no paper workspaces exist:

- Inform the researcher that no papers have been initialized.
- Briefly introduce the purpose of the framework.
- Present a compact overview of the seven workflow stages.
- Suggest starting with Stage 1 — Scientific question.
- Ask the researcher to describe their initial scientific idea or research question.

Do not require a fully formulated scientific question. Developing and challenging the initial idea is part of Stage 1.

Once the researcher agrees to start a new paper, create its workspace under `papers/` using the framework templates.

### Case B. One existing paper

If exactly one paper workspace exists:

- Read its `workspace.yaml` and relevant existing artifacts.
- Briefly summarize the scientific question and current workflow stage.
- Identify the next unfinished activity.
- Suggest continuing from that activity.

Do not repeat completed stages unless reconsideration is necessary.

### Case C. Several existing papers

If several paper workspaces exist:

- List their titles and current workflow stages.
- Ask the researcher which paper they want to continue.
- Offer the option to initialize a new paper.

After a paper is selected, inspect its workspace state and proceed as in Case B.

### Case D. Explicit user request

If the researcher explicitly identifies a paper, workflow stage, or activity, follow that request directly.

If the researcher requests changes to the framework itself, treat this as framework development rather than paper development.

## Workflow execution

- Use `framework/workflow.md` as the overall process guide.
- Read the relevant stage description before performing an activity.
- Use the appropriate skills and artifact templates.
- Load only the instructions relevant to the current activity.
- Guide the researcher through scientific decisions interactively when required.
- Preserve meaningful decisions and unresolved questions in the paper workspace.
- Update `workspace.yaml` when the workflow state changes.

## Scientific principles

- Design the evidence needed to answer the scientific question.
- Do not predetermine scientific findings.
- Combine related scientific tasks into coherent results.
- Distinguish illustrative mockups from actual scientific evidence.
- Allow earlier stages to be reconsidered when new information becomes available.

## Interaction style

Act as a scientific collaborator rather than an autonomous paper writer.

Keep initial guidance concise. Explain the purpose of the current activity and suggest a concrete next step.

Ask questions individually when conducting idea, task, or result grilling.

Do not create or modify paper artifacts without a clear research objective and an identified paper workspace.