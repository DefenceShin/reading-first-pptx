---
name: reading-first-pptx
description: Use when Codex needs to create or remake a high-density, reading-oriented, analytical editable .pptx deck from notes, source documents, screenshots, tables, or existing slides, especially when the materials are incomplete but the result still needs clear logic, restrained design, and native PowerPoint editability.
---

# Reading-First PPTX

## Contract

- Output an editable native `.pptx` by default.
- Treat native PowerPoint editability as non-negotiable.
- If the brief is unclear, ask up to 3 targeted questions before building.
- Prefer outline first, then deck build, unless the input is already stable or the user explicitly wants direct generation.
- Keep one dominant conclusion per slide.
- Allow dense support layers on the same slide when they strengthen the same argument.
- Prefer clear logic and reading value over decorative spaciousness.
- Apply the project writing rules to outward-facing PPT copy when they exist.
- Use the `PowerPoint` skill for actual deck creation, editing, rendering, and verification when available.
- Reuse the skill resources as an operating system: select a layout, select components, apply style rules, then run quality gates.
- When the active PPT project folder provides `red.pptx` or `resources/red.pptx`, use it as the default template/style baseline. If it is unavailable, follow the normal baseline workflow or any reference/template the user explicitly provides. Do not require a template inside the skill directory.

## Workflow

### 1. Read inputs

Inputs:

- rough notes
- existing PPT/PPTX files
- spreadsheets or tables
- screenshots
- visual references, brand pages, design guides, or sample decks
- PDFs, Word files, markdown, or reports
- scattered facts from chat

Extract:

- source facts
- interpretation
- unfinished or implied logic
- reusable visual DNA when the user provides style references

If unclear, ask only for:

- audience or use scenario
- core message
- output scope or slide count expectation

Then restate the task in 2-4 lines.

### 2. Lock baseline

- In the active PPT project folder, use `red.pptx` or `resources/red.pptx` as the reference template for page size, layout behavior, report header rhythm, density, chart/table treatment, and red-anchor composition when either file exists. If neither exists, continue with the normal baseline workflow or the user's explicit reference/template.
- Keep the original color and typography system from `references/style-anchor.md` while using that template baseline.
- Do not ask the user to choose the default template/style unless the user explicitly asks for a different template, brand, website, screenshot, sample deck, or visual direction.
- Inspect any available master, theme, or prior deck before creating slide geometry.
- Keep the visual language native to PowerPoint: editable text boxes, tables, charts, shapes, lines, and grouped elements.
- Avoid rasterizing whole slides, embedding HTML screenshots as slide bodies, or using non-editable image composites unless the source itself is an image.
- If the user explicitly provides a non-default style target, translate it through `references/visual-style-transfer.md` before designing slides.

If the workspace also contains real internal report decks or prior business presentations, use them only to infer density expectations, grouping habits, and practical tolerance for single-slide information load. Do not depend on any one file as a required reference.

### 3. Plan the deck

- the deck objective
- target slide count
- one dominant conclusion for each slide
- which source materials support each slide
- which slides need charts, tables, comparison structures, frameworks, process visuals, or note blocks
- a layout choice for each slide from `references/slide-patterns.md`
- a component choice for each important content unit from `references/component-system.md`
- a page rhythm plan that alternates dense explanation, comparison, chart, and summary pages when the deck is long

If the content is structurally ambiguous, propose 2-3 narrative or page-structure directions inside the same visual language, recommend one, and explain the trade-off briefly. Do not turn this into a multi-style exercise.

If the source pack is large, mixed, or incomplete, stop here and confirm the outline before full deck production.

### 4. Run preflight before building

Before writing slides, read the relevant references:

- `references/style-anchor.md` for the fixed visual language.
- `references/content-rules.md` for density, inference, and wording boundaries.
- `references/slide-patterns.md` for page structure selection.
- `references/component-system.md` for reusable native PowerPoint building blocks.
- `references/visual-style-transfer.md` only when the user asks to match, imitate, absorb, or reference a non-default external visual style.
- `references/quality-gates.md` for preflight and final checks.

Preflight checks:

- Confirm output path and expected file name.
- Confirm page size, default template baseline, fonts, and color tokens. Prefer `red.pptx` or `resources/red.pptx` in the active PPT project folder when present; otherwise use the normal baseline workflow or the user's explicit reference/template, with `style-anchor.md` for colors/fonts.
- Confirm the visual target only when the user explicitly provides a non-default brand, website, screenshot, sample deck, or style direction.
- Confirm every planned slide has one conclusion, one structural core, and source support.
- Confirm tables/charts have enough room to stay readable.
- Confirm any screenshot or picture slide has image source files or an explicit placeholder plan.
- Confirm the deck does not depend on a non-editable full-slide image as the main deliverable.

### 5. Rewrite content

- rewrite titles into conclusion-style titles
- compress repetitive wording
- convert loose bullets into grouped evidence, comparison blocks, or structured notes
- add missing connective explanation where needed
- do not invent facts, dates, numbers, customers, citations, or unsupported conclusions

### 6. Compose the slide

1. conclusion-style title
2. structural core such as a chart, diagram, matrix, framework, map, or table
3. compact annotations, side notes, or comparison notes
4. short takeaway, implication, boundary, or highlight statement

Avoid slides that are only a title plus one oversized visual and a few labels.

Use native PowerPoint geometry deliberately:

- align to a small grid; keep margins consistent across the deck
- use local headers, chips, thin dividers, and annotation strips before large decorative panels
- use no more than 1-2 emphasis treatments on a slide
- keep titles, tables, labels, and callouts editable
- keep chart data editable when a chart is created from data
- group related shapes after alignment is stable, but avoid over-grouping text that users may need to edit

If page risk is high, preview 1-2 key slides before full deck production:

- one high-density body slide
- one chart or comparison slide if the deck depends on it

Use the preview step when structure risk, density risk, or visual risk is high. Do not skip straight to the full deck when one failed page would invalidate the whole direction.

### 7. Verify

Check the actual deck, not only the source content:

- the `.pptx` opens normally in PowerPoint when PowerPoint is available
- slides are readable at normal viewing size
- the main point is visible within a few seconds
- content is dense but not jammed
- source facts remain intact and unsupported conclusions were not introduced
- typography, color use, and title treatment follow the style rules
- any requested style imitation is visible through reusable design decisions, not copied artifacts
- the company template, page frame, and visual language were not drifted away from without instruction
- the deck does not drift into dashboard, poster, blueprint, or generic infographic aesthetics

Run a short self-critique before finishing:

- information completeness
- hierarchy clarity
- detail execution
- factual safety
- functional usefulness

Fix obvious problems before returning the deck.

If the deck was built or edited with scripts, open or render representative slides after generation. If PowerPoint automation is unavailable, inspect the package structure and use the strongest available fallback renderer from the `PowerPoint` skill.

## Output

- be an editable `.pptx`
- respect the company template when that template exists and the user has not asked to override it
- preserve or improve information density rather than emptying the page
- follow the extracted style language rather than clone a specific reference deck
- open cleanly in PowerPoint when PowerPoint is available

Keep the output as a true editable `.pptx` with editable text, shapes, and charts.

## References

- [style-anchor.md](./references/style-anchor.md)
- [content-rules.md](./references/content-rules.md)
- [slide-patterns.md](./references/slide-patterns.md)
- [component-system.md](./references/component-system.md)
- [visual-style-transfer.md](./references/visual-style-transfer.md)
- [quality-gates.md](./references/quality-gates.md)
