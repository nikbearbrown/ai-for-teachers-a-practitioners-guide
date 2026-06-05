# CAJAL Figure Intelligence — Chapter 11: Coding with AI: An Introduction

**Source:** `chapters/11-coding-with-ai-an-introduction.md`
**Mode:** `/scan silent`
**Domain note:** AI+1 practitioner guide / K-12 and higher-ed teaching. Chapter argues the bottleneck for teachers building tools with AI is specification, not syntax. Five author-placed figures across bottleneck shift, spec components, verification protocol, before/after specs, and Wing's computational thinking.

---

## Density Recommendation

**4 figures, Conceptual density.** Author placed 5 fig stubs; Figure 11.4 (before/after spec comparison) is best rendered as the chapter's existing block-quote text on the page and does not earn a separate diagram. The other four carry the conceptual load.

---

## Zone Map

- **MC:** The bottleneck shift (syntax → specification). The five-component spec as a single object. Verification of behavior in absence of code-readability.
- **VG:** The five-pass verification protocol as a sequenced checklist. Wing's computational-thinking moves mapped to a concrete teacher example.
- **PQ:** Peng 2023 (55.8% faster on specified tasks). Veracode 2025 (~45% OWASP flaw). arXiv 2025 (16–18% Python vuln). Three-bucket risk table (already rendered as Table 11.1).

---

## Figure 11.1 — The Bottleneck Shift

**Priority: Important.** Names the chapter's central reframe. Worth a clean two-state diagram.

### Block 1 — Illustrae paste block

A horizontal two-column composition. Left column labeled by post-typography "Pre-2022 world": a vertical stack of stages — *intent* (small Sky Blue `#56B4E9` filled square at top), *decomposition* (Sky Blue square), *abstraction* (Sky Blue square), then a Vermillion `#D55E00` filled rectangle representing the syntax/typing layer drawn much larger than the other stages — visibly the bottleneck, with a Black `#000000` 1pt arrow narrowing as it passes through. Output (small Bluish Green `#009E73` filled circle) at the bottom. Right column labeled "Post-2022 world": same stack of stages but the syntax rectangle is now small Orange `#E69F00` (delegated, no longer load-bearing) while the *intent/decomposition/abstraction* stages are drawn larger in Blue `#0072B2` filled rectangles. A Reddish Purple `#CC79A7` 1pt curved arrow loops from the top of the right column back into the human-judgment stages. White background, flat vector, single-column 89mm.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Two-column before/after of where the bottleneck sits in a teacher coding task. Syntax stage shrinks; specification stages enlarge.
[O] Side-by-side vertical stacks. Bottleneck stage visibly larger in the "before" column, visibly smaller in the "after" column.
[P] Specification stages Sky Blue (before) / Blue (after, enlarged). Syntax bottleneck Vermillion (before) / Orange (after, small). Output Bluish Green. Judgment loop Reddish Purple.
[E] No code snippets rendered, no specific language names, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, code snippets, language names, IDE screenshots, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 11.2 — Five-Component Specification

**Priority: Critical.** The chapter's load-bearing operational object. The five components must be visually individuated.

### Block 1 — Illustrae paste block

A pentagon composition. Five filled nodes arranged around a central labeled core. Top node: *intent* (Blue `#0072B2` filled circle). Upper right: *constraints* (Sky Blue `#56B4E9` filled circle). Lower right: *success criteria* (Bluish Green `#009E73` filled circle). Lower left: *exclusions* (Vermillion `#D55E00` filled circle). Upper left: *output format* (Orange `#E69F00` filled circle). Central node: a Reddish Purple `#CC79A7` filled rounded square representing the specification document itself. Each outer node connects to the central node with a Black `#000000` 1pt line. A faint Sky Blue `#56B4E9` 15% opacity ring encloses the whole pentagon, suggesting that all five components must be present together. White background, flat vector, single-column 89mm.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Five-component specification rendered as five nodes orbiting a central spec document. Each node distinct; missing any one degrades the spec.
[O] Pentagon arrangement. Central document node connected to all five outer nodes.
[P] Intent Blue. Constraints Sky Blue. Success criteria Bluish Green. Exclusions Vermillion. Output format Orange. Spec document Reddish Purple. Connector lines Black 1pt.
[E] No text rendered in image, no document mockup, no decorative ornament, no shadows, no drop shadows on nodes.

### Block 3 — Negative prompt

text labels, document mockups, code snippets, file icons, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 11.3 — Five-Pass Verification Protocol

**Priority: Critical.** The chapter's deployable instrument. Verification is what protects teachers.

### Block 1 — Illustrae paste block

A vertical numbered cascade. Five sequential horizontal bands, each containing one filled circle node on the left and a thin connecting Black `#000000` 1pt arrow descending to the next band. Band 1: *spec pass* (Blue `#0072B2` filled circle) — node has three small Sky Blue `#56B4E9` filled squares to its right representing three hand-computed test inputs. Band 2: *edge pass* (Sky Blue filled circle) — node has small Vermillion `#D55E00` filled triangles to its right representing edge cases. Band 3: *wrong-input pass* (Bluish Green `#009E73` filled circle) — node has a small Vermillion filled "X" symbol to its right representing intentional failure. Band 4: *privacy pass* (Reddish Purple `#CC79A7` filled circle) — node has a small Orange `#E69F00` filled circle representing a network query. Band 5: *sentinel pass* (Orange filled circle) — node has a single small Blue filled diamond to its right representing the sentinel row. A faint Black `#000000` 1pt vertical timeline runs down the left side. White background, flat vector, single-column 89mm.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Five sequential verification passes a teacher runs against AI-generated code. Spec → edge → wrong-input → privacy → sentinel. Behavior tested, not code read.
[O] Vertical top-to-bottom numbered cascade. One row per pass. Visual indicator of what each pass inspects.
[P] Spec pass Blue. Edge pass Sky Blue. Wrong-input pass Bluish Green. Privacy pass Reddish Purple. Sentinel pass Orange. Connector arrows Black 1pt. Edge cases Vermillion.
[E] No code snippets rendered, no terminal mockups, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, code snippets, terminal output, error messages, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 11.5 — Wing's Computational Thinking Moves on Ms. R's Spec

**Priority: Important.** Closes the chapter by linking Wing 2006 to a specific teacher case. The map clarifies what survives the syntactic layer.

### Block 1 — Illustrae paste block

A two-column mapping diagram. Left column lists five filled nodes, each a Wing computational-thinking move (each rendered as a small Blue `#0072B2` filled circle): *abstraction*, *decomposition*, *anticipating failure modes*, *naming boundaries*, *parameterization*. Right column lists five filled nodes representing concrete moves in Ms. R's polynomial specification (each rendered as a Bluish Green `#009E73` filled circle): *parameterized polynomial form*, *rendering / interaction / calculation split*, *edge case (a=0)*, *no-internet runtime constraint*, *input ranges and step sizes*. Each left node connects to its corresponding right node via a Black `#000000` 1pt line. A small Reddish Purple `#CC79A7` filled square sits at the bottom center labeled (post-typography) as the specification document — the place where all five moves converge. Sky Blue `#56B4E9` 15% opacity background tints the left column lightly to mark it as the conceptual register. White background, flat vector, single-column 89mm.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Two-column map. Wing's computational-thinking moves on the left correspond one-to-one with concrete moves in Ms. R's polynomial spec on the right. Specification document at bottom center as convergence point.
[O] Side-by-side columns. Diagonal connector lines between matching nodes. Convergence node at bottom.
[P] Wing moves Blue. Ms. R's spec moves Bluish Green. Spec document Reddish Purple. Connectors Black 1pt. Left column background Sky Blue 15%.
[E] No text rendered, no equations, no graph of the cubic, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, equations, function plots, screenshots, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## What CAJAL Declines to Architect

- **Figure 11.4 — before/after specification comparison.** The chapter already renders both specs as block-quoted plain text. Rendering them again as a "figure" would be a typographic table at best, a screenshot at worst. Drop the figure; keep the prose block. The contrast is carried by the typography.
- **Table 11.1 (risk classification).** Typography reference table. Keep as table; do not graph.
- **The polynomial demo screenshot.** Not in the chapter as a figure and would be an applied-screenshot artifact (CAJAL drops screenshots).
- **Wayback Machine portrait (Grace Hopper).** AI-generated portrait, handled outside CAJAL pipeline.

---

## Video Candidate Pass

**FIGURE 11.1 (bottleneck shift):** STATIC SUFFICIENT.
**FIGURE 11.2 (five-component spec):** STATIC SUFFICIENT.
**FIGURE 11.3 (five-pass verification protocol):** **MILD VIDEO CANDIDATE.** Sequential-procedure criterion met. A short animation walking the five passes in order, with a simulated input flowing through each, could compress a 30-minute first-time experience into a 60-second mental rehearsal. Optional, not load-bearing.
**FIGURE 11.5 (Wing → Ms. R mapping):** STATIC SUFFICIENT.

**Video candidates identified: 1 mild.** Not recommended as priority. The chapter's argument is best served by static diagrams that a teacher can post next to their laptop.

---

## Split-point note

Chapter cross-references Ch 02 (phase gates), Ch 03 (template pattern), Ch 13 (FERPA + integrity), and Ch 12 (workflow.md). The five-component spec node in Fig 11.2 should visually echo any "template pattern" diagram from Ch 03 if such exists; coordinate palette and node shape across chapters so the same conceptual object reads as the same object.
