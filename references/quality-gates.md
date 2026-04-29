# Quality Gates

Use this file before and after building a deck. Treat P0 items as blockers.

## P0 Blockers

- The output is not an editable native `.pptx`.
- A slide is effectively a flattened screenshot or full-slide bitmap when editable structure was possible.
- The deck invents facts, dates, numbers, citations, customers, or conclusions.
- A slide lacks a dominant conclusion or the conclusion is hard to find.
- Charts or tables are unreadable at normal slide size.
- The deck ignores the available company template, page size, or frame without user instruction.
- The deck fails to use `resources/红色.pptx` or `D:\Skills Development\pptx\resources\红色.pptx` as the default structural/template baseline when no other visual target was provided.
- Text boxes overlap, clip, or overflow.
- The style drifts into dashboard, poster, blueprint, generic infographic, neon, or decorative template aesthetics.
- A requested visual style is copied as a non-editable surface instead of translated into reusable PPT rules.

## Preflight

Before generation:

- Identify source files and the role each source plays.
- Separate confirmed facts from interpretation and assumptions.
- Decide slide count and page rhythm.
- Assign one layout pattern to each slide.
- Assign major components to each slide.
- Confirm which slides need charts, tables, screenshots, or diagrams.
- Confirm fonts, color tokens, margins, title treatment, footer, and page size.
- Confirm `resources/红色.pptx` or `D:\Skills Development\pptx\resources\红色.pptx` is the structural baseline unless the user explicitly provided a different brand, website, screenshot, sample deck, or visual direction.
- Confirm the external visual-style source, intended imitation strength, and transferred traits only when such a source was explicitly provided.
- Confirm placeholder handling for missing images or incomplete data.

## Slide-Level Check

For each slide:

- Title states a conclusion or decision-relevant message.
- Body structure supports the title directly.
- Main point is visible within a few seconds.
- Density is high enough to be useful but not jammed.
- Labels, legends, captions, and source notes are readable.
- Emphasis is limited to the most important number, contrast, or risk.
- Support notes add meaning rather than restating the title.
- No unsupported causal or market claim was introduced.

## Deck-Level Check

- The deck has a clear narrative sequence.
- Page rhythm alternates analytical modes when the deck is long.
- Colors, fonts, margins, chips, dividers, and title treatment are consistent.
- Similar slide types use similar geometry.
- Any requested style target is visible across body slides, not only on cover or divider pages.
- Appendices are quieter than main argument slides.
- There is no accidental mix of unrelated visual styles.
- The final file opens and representative slides render correctly.

## Editing Check

- Important text remains editable.
- Tables and charts are editable when they were created from data.
- Shapes are grouped only where grouping helps later editing.
- Source images are embedded at sufficient resolution.
- Generated or sourced images leave safe space for editable overlay text when used as backgrounds.
- Speaker notes, hidden slides, or comments do not contain stale draft text unless intentionally preserved.

## Self-Critique

Before responding to the user, state whether you checked:

- factual safety
- hierarchy clarity
- layout execution
- editability
- file opening or rendering

Fix obvious issues before returning the deck.
