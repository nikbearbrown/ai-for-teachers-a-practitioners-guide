# CAJAL Figure Intelligence — Chapter 3: Prompting That Works

**Source:** `chapters/03-prompting-that-works.md`
**Mode:** `/scan silent`
**Domain note:** AI+1 practitioner guide / K-12 and higher-ed teaching. Chapter argues: the prompt is not a query, it is the entire specification of what gets built. Introduces the four-component template (ROLE / CONTEXT / TASK / CONSTRAINTS) and the diagnostic prompting loop. Names the "feeling-prompt trap" (warm/engaging/rigorous). Three author-placed figures, three tables.

---

## Density Recommendation

**3 figures, Concept-anchor density.** Three earn their place: (1) pointer-vs-specification contrast establishing the structural why; (2) the four-component template card as a memorable reference; (3) the diagnostic prompting loop showing how rounds converge. Tables (feelings-vs-operations, platform-comparison) stay as typography reference. Author-placed figure count matches.

---

## Zone Map

- **MC:** A generative prompt is the entire specification, not a pointer; the model has no context the prompt does not supply. The four components do distinct structural work. The loop diagnoses what the prompt forgot.
- **VG:** Search pipeline vs generative pipeline (two-panel contrast). The four-component card stacked vertically with structural-work callouts. The three-round loop as left-to-right flow.
- **PQ:** Six sentences vs one sentence (Teacher A/B). 30–40 prompts before reflex. Three rounds, seven minutes (worked photosynthesis example). Five to fifteen prompts per starter library category.

---

## Figure 3.1 — Pointer vs Specification

**Priority: Critical.** The structural reason prompting is different from searching. Must contrast the two pipelines visually so the asymmetry is felt, not just read.

### Block 1 — Illustrae paste block

A two-panel side-by-side composition, single-column 89mm. Left panel ("search engine pipeline"): three stacked horizontal nodes connected by Black `#000000` 1pt arrows pointing right — a small Sky Blue `#56B4E9` filled rounded rectangle (input query), a Sky Blue `#56B4E9` filled cylinder shape (index), and a stack of three small Bluish Green `#009E73` filled rectangles representing pre-existing documents. The arrow from index to documents is labeled "retrieval" post-typography. Right panel ("generative model pipeline"): three nodes — an Orange `#E69F00` filled rounded rectangle (prompt tokens), a Blue `#0072B2` filled rounded rectangle (probability distribution), and a horizontal stream of small Orange `#E69F00` filled circles emerging token-by-token. The arrow from prompt to distribution is labeled "conditioning" post-typography. A thin vertical Black `#000000` 1pt line separates the two panels. White background, flat vector.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Two-panel pipeline contrast. Search: query → index → pre-existing documents (retrieval). Generative: prompt → probability distribution → token-by-token output (conditioning).
[O] Two vertical panels separated by a thin line. Each panel runs left-to-right with three nodes.
[P] Search inputs/index Sky Blue; documents Bluish Green. Generative prompt/tokens Orange; distribution Blue. Arrows Black 1pt. Panel divider Black 1pt.
[E] No specific UI screenshots, no brand logos, no product names rendered as graphics, no decorative ornament, no shadows.

### Block 3 — Negative prompt

UI screenshots, search-engine logos, chatbot avatars, product brand names rendered as graphics, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 3.2 — The Four-Component Template Card

**Priority: Critical.** The chapter's central artifact. Must read as a reference card the teacher could mentally recall.

### Block 1 — Illustrae paste block

A stacked card composition, single-column 89mm. A tall rounded-rectangle "card" outlined Black `#000000` 1pt with white fill, oriented portrait, occupying the left two-thirds of the space. Inside the card, four horizontal stripes of equal height, each with a small filled circle on the left margin acting as the row marker — Sky Blue `#56B4E9` for ROLE (top), Bluish Green `#009E73` for CONTEXT (second), Orange `#E69F00` for TASK (third), Vermillion `#D55E00` for CONSTRAINTS (bottom). Each stripe has a horizontal line trailing right from its circle, Black `#000000` 0.5pt, representing the slot-to-fill. To the right of the card, four small Black `#000000` 0.75pt callout brackets (one per stripe) pointing left at each row, each ending in a small Orange `#E69F00` filled diamond marker — placeholders for the structural-work labels added post-typography. White background, flat vector.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Vertical reference card with four equal-height rows (ROLE / CONTEXT / TASK / CONSTRAINTS), each with a colored marker circle and a slot line. Callout brackets on the right side point to each row.
[O] Card occupies left two-thirds. Callout brackets along right edge.
[P] Card outline Black 1pt, white fill. Row markers: ROLE Sky Blue, CONTEXT Bluish Green, TASK Orange, CONSTRAINTS Vermillion. Slot lines Black 0.5pt. Callouts Black 0.75pt with Orange diamond endpoints.
[E] No actual prompt text rendered as image content, no example sentences, no decorative ornament, no shadows.

### Block 3 — Negative prompt

example prompt text rendered as graphics, sample sentences, screenshots, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 3.3 — The Three-Round Diagnostic Prompting Loop

**Priority: Critical.** The skill the chapter is teaching. Must render the loop as iteration over a probability space, not as trial-and-error.

### Block 1 — Illustrae paste block

A horizontal three-node flow composition, single-column 89mm or double-column 174mm. Three nodes left-to-right, each a rounded rectangle. Round 1 (left): smallest, Sky Blue `#56B4E9` filled — the one-line vague prompt. Round 2 (middle): medium, Blue `#0072B2` filled — the four-component prompt. Round 3 (right): largest, Bluish Green `#009E73` filled — the gap-closing follow-up. Between Round 1 and Round 2, a thick Black `#000000` 1.5pt arrow with a small Orange `#E69F00` filled triangular kink at its midpoint labeled "diagnostic observation" post-typography. Same arrow style between Round 2 and Round 3. Below each node, a horizontal probability-space band: at Round 1, a wide Sky Blue `#56B4E9` 15% opacity rectangle; at Round 2, a narrower Blue `#0072B2` 15% opacity rectangle; at Round 3, a narrow Bluish Green `#009E73` 15% opacity rectangle — visually narrowing as the loop runs. White background, flat vector.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm or double-column 174mm, vector, white background.
[C] Three rounds of the prompting loop with the probability space narrowing as the rounds progress. Diagnostic observations between rounds drive the convergence.
[O] Horizontal left-to-right: Round 1 → Round 2 → Round 3. Probability bands beneath each node visualize the narrowing space.
[P] Round 1 Sky Blue, Round 2 Blue, Round 3 Bluish Green. Probability bands match round colors at 15% opacity, narrowing right. Arrows Black 1.5pt with Orange diamond kinks.
[E] No specific prompt text rendered as graphics, no example outputs, no decorative ornament, no shadows.

### Block 3 — Negative prompt

prompt text rendered as graphics, example outputs, lesson plan content, brand names, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## What CAJAL Declines to Architect

- **Table 3.1 (Teacher A vs Teacher B spec components).** Typography reference table — keep as table; the prose worked example carries the move.
- **Table 3.2 (feelings vs operations).** Typography reference table — keep as table.
- **Table 3.4 (platform comparison: NotebookLM / Claude / ChatGPT / Gemini).** Typography reference table; do not redraw as a figure.
- **The photosynthesis worked example.** Prose worked example — does not benefit from a figure beyond the loop visualization in Fig 3.3.
- **The four-line ROLE/CONTEXT/TASK/CONSTRAINTS code-block.** Typography artifact rendered in monospace within prose; not a figure.
- **Charlotte Mason portrait.** AI Wayback Machine asset; separate portrait pipeline.
- **Screenshots of ChatGPT / Claude / Gemini / NotebookLM UIs.** Out of scope by CAJAL discipline.

---

## Video Candidate Pass

**FIGURE 3.1 (pointer vs specification):** STATIC SUFFICIENT. A two-panel contrast.
**FIGURE 3.2 (four-component card):** STATIC SUFFICIENT. Reference card.
**FIGURE 3.3 (three-round loop):** **MILD VIDEO CANDIDATE.** A short animation showing the probability space narrowing across rounds could dramatize the diagnostic-not-guessing claim. In print, static suffices.

**Video candidates identified: 1 mild.** Recommended for digital edition.

---

## Split-point note

The four-component canon (ROLE / CONTEXT / TASK / CONSTRAINTS color assignments — Sky Blue / Bluish Green / Orange / Vermillion) should be reused if downstream chapters break down specific prompt components. Chapter 4 (lesson planning), Chapter 5 (calibration prompts), Chapter 7 (parent communication) all reactivate this template; keep the color-to-component canon consistent across them so the reader recognizes the same four slots.
