---
name: result-mockup
description: Create explicitly illustrative figures, tables, or diagrams from planned scientific result specifications. Use before experiments to test whether the intended evidence and representation are concrete and interpretable.
---

# Result mockup

Make the intended representation tangible before research execution. The mockup specifies the comparison and visual encoding; it supplies no scientific evidence.

## Context

Read the target `results/RXX.md`, relevant task links, and review decisions in the paper workspace. Clarify ambiguous destinations. Do not modify framework or skills. If consequential design choices are missing, ask about them or create a visibly provisional layout with those choices marked open.

## Construction

1. Identify the scientific comparison and map its dimensions to axes, panels, table columns, or diagram elements. Include units, conditions, legends, reference comparisons, and uncertainty encodings where relevant.
2. Prefer a blank or schematic layout when a hypothetical trend would prejudge the outcome. If synthetic values help test readability, make their illustrative origin explicit and include plausible alternative patterns when useful.
3. Label every generated visual or table **ILLUSTRATIVE MOCKUP — NOT EXPERIMENTAL DATA** in the artifact itself and its caption. Do not use significance markers, precise fitted values, or apparent empirical uncertainties without explaining their illustrative construction.
4. Use plotting tools for quantitative axes and reproducible scientific figures, structured Markdown or CSV for tables, and Mermaid or vector tools for logical schemes. Select the simplest representation that answers the design question.
5. Inspect the output for legibility and scientific ambiguity. Check whether omitted factors, overcrowded panels, unavailable measurements, or misleading encodings require a design revision. Record those findings rather than hiding them with polished graphics.

## Artifacts and completion

Save deliverables under `results/mockups/`, named with the result ID, such as `R01.svg`, `R01-table.md`, or `R01.mmd`. For programmatic plots, retain the generator and any synthetic inputs alongside the output, with a reproducible seed if randomness is used. Keep illustrative data separate from real data and never overwrite measured outputs.

Link the mockup and its construction notes from `results/RXX.md`. Record what real data must replace each illustrative element and any open design issues. Completion means the researcher can see what will be compared, how the result could be interpreted, and what evidence is still needed; the plotted pattern is not a promised outcome.
