# Style Anchor

## Tone

Default template baseline: use `red.pptx` or `resources/red.pptx` from the active PPT project folder for layout behavior, page rhythm, information density, header treatment, chart/table styling, and red-anchor composition when either file exists. If neither exists, continue with the normal baseline workflow. Keep the color and typography tokens below as the default visual system.

- restrained
- premium
- analytical
- editorial
- logic-first
- explanation-driven
- professional
- document-like
- McKinsey-style consulting report on the default/red-template path

It should not feel like a dashboard, poster, blueprint, engineering drawing, or audience-specific campaign deck.

## Core Traits

- light title area
- dense structured middle body
- restrained footer area
- white or near-white canvas
- red-and-navy consulting rhythm with a white report-like base
- thin top header line or compact header system on most body pages
- compact page chrome with tight top rule, small section marker, and restrained page/source notes
- modular chips and local headers instead of heavy full-page bars
- line-based organization, thin dividers, and subtle grouping
- one clear focal conclusion with supporting analytical layers around it
- clear hierarchy without visual drama

## Main Title

- keep the slide main title as plain bold text
- keep it directly on white or very light neutral background
- an optional thin divider line below the title is allowed
- do not force a navy title bar behind the main title
- do not convert the title into a full-width colored bar for visual impact

## Color System

- Navy `#263F6A`
- Crimson/Red `#AF0837`

These are the default production colors. Do not replace them with colors extracted from `resources/红色.pptx` or another reference unless the user explicitly asks for a different brand or palette.

Use navy mainly for:

- module labels
- section chips
- local category headers
- compact subhead blocks
- comparison tags

Use red mainly for:

- key numbers
- highlights
- emphasis tags
- risk levels
- important keywords
- contrast points
- focal circles, arcs, arrows, or one dominant directional anchor

Keep the background white or very light neutral. Do not introduce additional dominant colors unless the user explicitly asks for them.

When borrowing consulting-deck conventions on the default/red-template path from external references such as `seulee26/mckinsey-pptx`, preserve this palette. Translate their blue-heavy or full-navy treatments into the local navy/red system instead of copying their colors. If the user provides another explicit style reference, follow that reference through `visual-style-transfer.md` instead of imposing this consulting influence.

## Typography

- Chinese text: `汉仪中宋简`
- English titles: `corpoA`
- English body text: `corpoS`
- Mixed-language text boxes: keep Chinese on `汉仪中宋简`, English titles on `corpoA`, and English body on `corpoS`; do not collapse the whole box into one font.

These are the default production fonts. Do not replace them with fonts observed in `resources/红色.pptx` or another reference unless the user explicitly asks for a different brand or typography system.

## Layout

- keep the top area visually light
- use the report-like header rhythm from `resources/红色.pptx`: thin top rule, compact metadata, and restrained page marks when useful
- let the middle body carry most of the information density
- prefer asymmetrical editorial layouts
- use one dominant analysis zone plus one or more support zones when possible
- use line-based structure, subtle borders, dashed separators, and compact chips to organize content
- avoid relying on large heavy cards as the default layout language
- prefer embedded analytical zones over many large standalone cards
- avoid equal-width multi-column layouts unless direct comparison is the real point
- favor editable consulting-style structures: charts with interpretation, dense tables, KPI modules, risk matrices, process flows, maps, and logical architecture diagrams
- choose a recognizable page type before drawing: executive summary, issue tree, comparison matrix, prioritization map, chart with takeaway pane, roadmap, process plan, assessment table, or dense appendix
- make chart and table slides feel intentionally composed: chart/table first, interpretation block beside or below it, source/method note in the footer zone
- use tight margins and disciplined body regions rather than oversized whitespace; consulting polish comes from alignment and compression, not emptiness
- use red as a concentrated visual anchor on one major region of a slide; do not flood the whole page with red
- use navy to carry structure in headers, table bands, diagram nodes, labels, and chart framing
- use light gray fields to support tables and modules without becoming visually dominant
- if no other reference is provided and `red.pptx` or `resources/red.pptx` is available in the active PPT project folder, make body pages feel structurally close to that template: dense, modular, editable, chart/table heavy, and consulting-report oriented
- if no other reference is provided, or if the active baseline is `red.pptx` / `resources/red.pptx`, make body pages feel structurally close to a McKinsey-style working deck: conclusion title, compact page chrome, one main analytical structure, explicit interpretation, and minimal ornament

## Density

- maximize useful analytical payload within readable limits
- dense is good when hierarchy remains clear
- if space remains, add one more useful analytical layer before enlarging graphics
- the slide should read as one integrated argument, not several detached mini-pages
- do not split content across slides if it can remain readable and logically integrated on one page
- reduce graphic scale before reducing useful analytical content

## Structure

1. conclusion-style title
2. structural core such as chart, diagram, matrix, framework, map, or table
3. compact annotations, side notes, or comparison notes
4. short takeaway, implication, highlight, or boundary statement

Avoid slides that contain only a title, one large diagram, and a few labels.

## Text

- use compact paragraphs, short bullet clusters, concise notes, and claim-plus-evidence phrasing
- keep wording neutral and analytical
- explain the issue before suggesting who should act
- avoid audience-specific framing unless explicitly requested
- avoid inflated, generic, or AI-sounding wording

When several points follow the same logic, shorten them into parallel lead phrases with brief supporting detail instead of repeating full sentences.

## Graphics

- charts and diagrams must do analytical work, not decorative work
- prefer matrices, trade-off maps, ranked bars, comparison tables, maps, timelines, structured diagrams, and risk matrices when they help explain logic
- the graphic should carry part of the reasoning, not merely illustrate a topic
- use strong data labels and concise interpretation blocks on chart pages
- use large numbers, arrows, circles, or red markers only when they improve scanning hierarchy
- keep diagrams editable with shapes, lines, text, and native charts wherever possible

When comparing three or more items on the same logic, prefer structured comparison formats over several large text-heavy cards.

For technical structures such as architectures, frameworks, maturity models, operating models, or risk types, add at least one of:

- business meaning
- enterprise relevance
- implementation condition
- limitation
- trade-off
- risk note
- decision implication
- management impact

Do not stop at concept display.

## Emphasis

Emphasize only one or two elements per slide. Priority order:

1. main conclusion
2. key number, contrast, or analytical distinction
3. takeaway or highlight label

Do not overuse red text, bold text, chips, or icons at the same time.

## Review

- visual decisions should reinforce the central argument
- hierarchy should be understandable within a few seconds
- details such as alignment, spacing, and emphasis should feel deliberate
- decoration should never outrun explanation

## Negative Constraints

Do not produce:

- dashboard style
- infographic poster style
- blueprint aesthetics
- engineering manual aesthetics
- grid paper or drafting paper backgrounds
- measurement overlays
- framing ticks
- technical drawing borders
- coordinate lines
- oversized decorative icons
- heavy gray panel overuse
- 3D rendering
- neon or cyber style
- clutter
- weak alignment
