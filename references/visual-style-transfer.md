# Visual Style Transfer

Use this only when the user explicitly provides a non-default visual reference and asks for a deck to match, imitate, absorb, borrow from, or feel like that style.

Default behavior: if the user does not provide a special visual target, use `resources/红色.pptx` as the template baseline and `style-anchor.md` as the color/font authority. If the relative template path is unavailable, use `D:\Skills Development\pptx\resources\红色.pptx`. Do not ask the user to choose a visual direction.

When this file is triggered, convert the external reference into editable PowerPoint rules instead of copying surfaces blindly.

## What To Extract

Extract the reference's visual DNA:

- **Mood**: restrained, editorial, technical, premium, playful, cinematic, institutional, product-led, etc.
- **Color roles**: background, text, structure, accent, warning, highlight, chart series, image treatment.
- **Typography voice**: serif/sans/mono balance, weight, casing, title scale, label style, number treatment.
- **Layout behavior**: margins, grid, asymmetry, density, reading path, title placement, footer behavior.
- **Component shapes**: chips, dividers, tables, cards, callouts, diagrams, image masks, chart frames.
- **Depth and material**: flat, paper-like, subtle shadow, glass, outline-only, layered panels, photographic.
- **Image language**: photo crop, illustration, abstract art, product screenshot, texture, icon style.
- **Motion or web cues**: translate only into static PPT equivalents such as rhythm, layering, or section contrast.

Do not merely name the source style. State the reusable choices that can be applied across slides.

## Translation Process

1. Identify which parts of the reference are essential and which are incidental.
2. Extract real evidence where possible:
   - for a website, inspect screenshots/CSS/brand pages when available
   - for a brand guide, capture actual colors, fonts, spacing, and component rules
   - for a sample deck, inspect its masters, layouts, typography, colors, and recurring objects
   - for a screenshot, infer only visible traits and label uncertain items as inferred
3. Write a compact style brief or design-spec before building when the external style materially changes the default.
4. Decide whether the target deck should fully adopt the reference, lightly borrow it, or blend it with the default `resources/红色.pptx` structure and `style-anchor.md` colors/fonts.
5. Convert web, poster, or image-model cues into native PowerPoint equivalents:
   - CSS spacing -> slide margins and grid
   - web cards -> editable panels, table regions, or grouped shape modules
   - page hero -> cover or section divider only
   - animation -> static sequencing, layering, or progressive page rhythm
   - brand accent -> controlled highlight, not blanket recoloring
6. Apply the style consistently across title, body, charts, tables, diagrams, and image assets.

## Native PPTX Boundary

- Keep titles, body text, labels, tables, charts, and diagrams editable.
- Use generated or sourced images as assets, not as a substitute for the slide structure.
- Leave safe zones for editable overlay text when using image backgrounds.
- Avoid baking full slide titles, body paragraphs, legends, tables, or dense annotations into images.
- If a reference is mainly a website or poster, adapt its hierarchy and visual grammar; do not recreate a literal webpage or poster inside PowerPoint.

## Style Brief Template

Use this compact brief when the user supplies a reference:

```text
Visual target:
- Mood:
- Color roles:
- Type behavior:
- Layout behavior:
- Components to reuse:
- Image/asset treatment:
- What to avoid:
- PPT translation:
- Evidence source:
- Uncertain/inferred items:
```

For a deck, also define:

```text
Deck application:
- Cover / opener:
- Section dividers:
- Dense analytical pages:
- Charts and tables:
- Diagrams and frameworks:
- Appendix pages:
```

## PPT Image Asset Rules

Use image assets for:

- cover art
- section divider backgrounds
- concept visualization
- comparison scene
- data-support backdrop
- closing poster
- source screenshot evidence

Do not use image assets for:

- editable body copy
- dense tables
- chart labels or legends
- process diagrams that should remain editable
- text-heavy explanation pages

When generating or selecting images:

- build from the slide thesis, not only from the deck topic
- keep one dominant subject or metaphor
- preserve 25-35% calmer space for editable text when overlay text is needed
- prepare left-safe, right-safe, or center-safe variants if final layout is uncertain
- keep meaning-critical content inside the central 80% width and height
- avoid generic stock scenes, off-style gradients, fake dashboards, and unreadable microtext

## Imitation Guardrails

- Imitate principles, not proprietary artifacts.
- Avoid copying logos, exact layouts, trademarked illustrations, or distinctive brand assets unless the user has provided and authorized them.
- If the user asks for a named brand style, use broad visual traits unless they provide owned brand materials.
- Preserve the user's content hierarchy over style mimicry.
- Do not let style imitation weaken factual accuracy, readability, or editability.

## Quality Check

Before finishing, check:

- Is the requested style visible in color roles, typography, layout, and components?
- Is the style applied across slide types instead of only on the cover?
- Are analytical pages still readable and dense enough?
- Are the main slide objects editable?
- Are image assets used only where they add value?
- Did the deck avoid literal copying of protected or source-specific assets?
