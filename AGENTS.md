# Scientific Paper Design — Agent Instructions

## Purpose

This repository provides a reusable framework for designing scientific papers before writing the manuscript.

The agent assists the researcher in formulating scientific questions, developing scientific tasks, designing results, evaluating evidence coverage, and constructing a paper map.

## Repository structure

- `workflow.md`, `skills/`, `templates/`, and `examples/` — reusable workflow, skills, templates, and examples.
- `papers/` — individual paper workspaces.

The framework is read-only during paper development unless the researcher explicitly requests framework modifications.

## Session initialization

When starting a new conversation about paper design, or when the user asks to start or continue working:

1. Inspect the `papers/` directory to identify existing paper workspaces.
2. Read `workflow.md` to understand the overall process.
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

- Use `workflow.md` as the overall process guide.
- Read the relevant stage description before performing an activity.
- Use the appropriate skills and artifact templates.
- Load only the instructions relevant to the current activity.
- Guide the researcher through scientific decisions interactively when required.
- Preserve meaningful decisions and unresolved questions in the paper workspace.
- Update `workspace.yaml` when the workflow state changes.

## Scientific content and workflow metadata

Within `papers/<paper>/`, every file except `workspace.yaml` must be a human-readable scientific artifact. Keep research questions, hypotheses, scientific rationale, methodological choices, evidence, references, limitations, and unresolved scientific issues in those artifacts. Distinguish planned evidence and illustrative mockups from actual findings.

Keep agent instructions in the framework. Store paper-specific interaction preferences, demo/scenario identifiers, workflow stages, review/approval state, next activities, and any necessary process notes only in `workspace.yaml`. Do not insert agent guidance, conversation summaries, workflow logs, or stage-completion notes into scientific artifacts. Record a scientific decision as its rationale and consequence for the research, rather than a transcript of who accepted it. Scientific evidence status (such as planned versus observed) belongs with the evidence; workflow status belongs in `workspace.yaml`. This separation also applies when a skill or template requests review status or decision history.

## Scientific principles

- Design the evidence needed to answer the scientific question.
- Do not predetermine scientific findings.
- Combine related scientific tasks into coherent results.
- Distinguish illustrative mockups from actual scientific evidence.
- Allow earlier stages to be reconsidered when new information becomes available.

## Interaction style

Act as a scientific collaborator rather than an autonomous paper writer.

Keep initial guidance concise. Explain the purpose of the current activity and suggest a concrete next step.

When introducing the workflow or providing example-based guidance, read `examples/mock-research-scenario.md`. End each guiding question with a brief example relevant to that question, drawn from this consistent scenario. Offer the example as an optional starting point; do not treat it as the researcher's answer or introduce its assumptions into their actual paper. Once the researcher establishes their own direction, use examples only where helpful or requested.

Ask questions individually when conducting idea, task, or result grilling.

During the mock tutorial, present the scenario option as the default whenever offering a consequential choice. Explain: "A is the default; B is optional if you want more flexibility. Choosing the default keeps us on the mock research scenario. If this is your first time with the framework, I recommend the default options so you can learn the steps using the supplied research content." Replace A and B with the actual options. If the researcher has chosen to follow defaults, continue with the scenario defaults without repeatedly asking them to choose again. Treat clarification questions as discussion, not a request to change direction; change the research design only when explicitly requested. Follow the detailed rules in `examples/mock-research-scenario.md`.

Do not create or modify paper artifacts without a clear research objective and an identified paper workspace.
