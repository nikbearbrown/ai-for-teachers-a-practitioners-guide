# CAJAL Figure Intelligence — Chapter 13: Academic Integrity, Privacy, and Honest Use

**Source:** `chapters/13-academic-integrity-privacy-and-honest-use.md`
**Mode:** `/scan silent`
**Domain note:** AI+1 practitioner guide / K-12 and higher-ed teaching. Chapter argues detection is the right tool for the wrong job; design is the right tool for the right job. Four author-placed figures plus two reference tables.

---

## Density Recommendation

**4 figures, Argumentative density.** All four carry distinct argumentative load — detection-failure case, Bastani empirical pivot, five-question diagnostic, equity cross-tab. None is redundant.

---

## Zone Map

- **MC:** Detection's three independent failure modes. Bastani's same-model / opposite-outcome result. The five-question AI-survivability diagnostic. Equity-asymmetric AI adoption by demographic group.
- **VG:** Performance paradox curve shape (practice up, exam down). Decision-tree shape of the five questions converging on yes/no terminals.
- **PQ:** OpenAI classifier 26% accuracy (withdrawn). Liang >50% TOEFL misclassification. Vanderbilt 1% × 75,000 = 750 wrongly flagged. Bastani: GPT-Base +48% practice / −17 pp exam; GPT-Tutor +127% practice / =control on exam. Pew 2025: 26% overall, 31% Black/Hispanic, 22% White teen use.

---

## Figure 13.1 — Three Independent Failure Modes

**Priority: Critical.** Disqualifies detection in one image. The independence of the three failures is the key visual.

### Block 1 — Illustrae paste block

Three stacked horizontal rows, each row representing one independent failure mode. Row 1 (top): a Vermillion `#D55E00` filled rounded rectangle band representing *tools are unreliable* — with two small Vermillion filled circles inside it (one for Weber-Wulff 2023, one for the OpenAI 26% withdrawal). Row 2 (middle): an Orange `#E69F00` filled rounded rectangle band representing *errors are biased* — with two small Orange filled circles (one for Liang 2023, one for the TOEFL >50% misclassification anchor). Row 3 (bottom): a Reddish Purple `#CC79A7` filled rounded rectangle band representing *institutions are walking back* — with three small Reddish Purple filled circles representing the Vanderbilt arithmetic (1% × 75,000 = 750). Each row sits alone with no connecting arrows — independence is the visual claim. A thin Black `#000000` 1pt horizontal divider separates each row. A small Sky Blue `#56B4E9` filled square sits to the right of each row, identical in shape, denoting that each row alone is sufficient to disqualify detection. White background, flat vector, double-column 174mm preferred.

### Block 2 — Full SCOPE prompt

[S] Double-column 174mm preferred, vector, white background.
[C] Three independent failure modes, stacked. No arrows between rows — independence is the visual. Identical sufficiency-marker on the right of each row indicates any single row disqualifies detection.
[O] Three horizontal bands stacked vertically. Thin dividers between bands. Sufficiency-marker squares aligned on the right.
[P] Failure 1 (unreliable) Vermillion. Failure 2 (biased) Orange. Failure 3 (institutional retreat) Reddish Purple. Sufficiency markers Sky Blue. Dividers Black 1pt.
[E] No statistics rendered as text in image, no logos, no institution names, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, statistics, institution logos, university shields, vendor names, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 13.2 — The Bastani Result

**Priority: Critical.** The chapter's empirical anchor. The opposite-direction outcomes are what makes the design argument inevitable.

### Block 1 — Illustrae paste block

A grouped bar chart. X-axis: three condition groups arranged left to right — *Control* (no AI), *GPT Base*, *GPT Tutor*. For each condition, two vertical adjacent bars: a *practice performance* bar (Sky Blue `#56B4E9` filled rectangle) and an *unaided exam score* bar (Blue `#0072B2` filled rectangle). Y-axis: relative performance, with a Black `#000000` 1pt horizontal baseline at the control level. Bars rise above baseline (better) and drop below baseline (worse). Control: both bars at baseline height. GPT Base: practice bar rises ~48% above baseline; exam bar drops below baseline (the −17 pp loss, drawn in Vermillion `#D55E00` filled rectangle to signal the harm). GPT Tutor: practice bar rises ~127% above baseline (much taller than GPT Base practice); exam bar matches baseline (Blue, neutral). A small Bluish Green `#009E73` filled "OK" marker sits above the GPT-Tutor exam bar to denote no harm; a small Vermillion filled marker sits below the GPT-Base exam bar to denote the durable-learning harm. White background, flat vector, double-column 174mm preferred.

### Block 2 — Full SCOPE prompt

[S] Double-column 174mm preferred, vector, white background.
[C] Three conditions × two outcomes. Same model. Same students. Opposite durable-learning outcomes by condition. GPT-Base practice up + exam down; GPT-Tutor practice way up + exam level.
[O] Grouped bar chart. Three condition clusters. Two bars per cluster. Horizontal baseline at control. Below-baseline region used for the harm bar.
[P] Practice bars Sky Blue. Exam bars Blue (when at/above baseline) or Vermillion (when below baseline as harm). Baseline Black 1pt. Harm marker Vermillion. No-harm marker Bluish Green.
[E] No numeric labels rendered, no condition names rendered as text, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, numeric annotations, condition names, percentages, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 13.3 — The Five-Question Diagnostic

**Priority: Critical.** The deployable instrument of the chapter. Five-stage decision tree that converts a "no" to a "yes" via redesign.

### Block 1 — Illustrae paste block

A vertical decision-tree composition. Five sequential diamond nodes stacked top to bottom, each rendered as a Sky Blue `#56B4E9` filled diamond representing one diagnostic question — *defense in conversation*, *novel application beyond training cutoff*, *process trail required*, *real-time unassisted performance*, *would good artifact alone reveal learning*. From each diamond, a Bluish Green `#009E73` 1pt arrow exits to the right and continues downward to the next diamond (the "yes" branch). From each diamond, a Vermillion `#D55E00` 1pt arrow exits to the left and terminates at a small Vermillion filled rectangle representing the redesign-target outcome. All five "yes" arrows ultimately converge at the bottom on a single Blue `#0072B2` filled larger circle representing the AI-survivable terminal. A small Orange `#E69F00` filled square sits beside each Vermillion redesign target labeled (post-typography) as "smallest move that converts no → yes." White background, flat vector, single-column 89mm.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Five sequential yes/no diagnostic questions. Yes-branches descend through all five and converge at AI-survivable terminal. Each no-branch points at a redesign-target with a "smallest move" annotation.
[O] Vertical decision-tree cascade. Yes-arrows on the right (downward). No-arrows on the left (to redesign targets). Single convergence point at the bottom.
[P] Question diamonds Sky Blue. Yes-arrows Bluish Green. No-arrows Vermillion. Redesign targets Vermillion. Convergence terminal Blue. Smallest-move callouts Orange.
[E] No text inside diamonds, no question text rendered, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, question text, callout text, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 13.4 — Teen ChatGPT-for-Schoolwork Use by Group

**Priority: Important.** The equity finding must be visible because it inverts the intuition behind bans.

### Block 1 — Illustrae paste block

A horizontal bar chart. Y-axis: demographic group rows arranged top to bottom — *Black teens*, *Hispanic teens*, *White teens*, *Overall teens*, *Higher-income families*, *Lower-income families*. X-axis: percentage of teens reporting AI-for-schoolwork use, 0–35%. Each bar is a Sky Blue `#56B4E9` filled rectangle, except the *Overall teens* bar which is highlighted in Vermillion `#D55E00` filled (the headline figure the chapter argues against using as a basis for blanket policy). A Black `#000000` 1pt vertical zero-baseline runs at the left. Black 1pt tick marks at 0, 10, 20, 30 along the x-axis. A faint Orange `#E69F00` 15% opacity horizontal band shades the rows where the bar exceeds the overall average — visually grouping Black and Hispanic teens above the average. A small Bluish Green `#009E73` filled square sits to the right of each demographic row as a row-identifier swatch. White background, flat vector, single-column 89mm.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Horizontal bar chart of teen AI-for-schoolwork rates by demographic group. The overall-teens bar uses the chapter's accent color to mark the figure that bans and requirements both reference. Above-average rows shaded to make the cross-tab visible.
[O] Horizontal bars. Y-axis demographic groups. X-axis percentage 0–35. Zero baseline on the left. Above-average band shading.
[P] Demographic bars Sky Blue. Overall-teens accent bar Vermillion. Above-average band Orange 15%. Row swatches Bluish Green. Axes Black 1pt.
[E] No percentage labels rendered as text, no group names rendered, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, percentage numbers, group names, demographic labels, source citations, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## What CAJAL Declines to Architect

- **Table 13.1 (research-paper redesign before/after).** Typography reference table.
- **Table 13.2 (routine vs. stop-and-check privacy operations).** Typography reference table.
- **The policy paragraph block.** Belongs as block-quoted prose, not a figure.
- **The before/after assignment prompts.** Belong as side-by-side prose blocks, not as a figure.
- **Wayback Machine portrait (Plato).** AI-generated portrait, handled outside CAJAL pipeline.

---

## Video Candidate Pass

**FIGURE 13.1 (three failure modes):** STATIC SUFFICIENT.
**FIGURE 13.2 (Bastani result):** **MILD VIDEO CANDIDATE.** A two-stage reveal — practice bars first, then exam bars — could dramatize the reversal. Optional. Static comparison reads as well in print.
**FIGURE 13.3 (five-question diagnostic):** STATIC SUFFICIENT.
**FIGURE 13.4 (Pew demographic bars):** STATIC SUFFICIENT.

**Video candidates identified: 1 mild.** Not recommended as priority. The chapter's deliverables are policy paragraphs and assignment redesigns — printable diagnostics serve the teacher better than animated ones.

---

## Split-point note

Chapter cross-references Ch 12 (workflow.md as documented record of AI use) and the Bastani study which also appears in Ch 14. The Bastani bar chart in Fig 13.2 and the Bastani three-group chart in Ch 14 Fig 14.2 should be visually distinct but palette-consistent — both depict the same study at different argumentative purposes. Use identical condition colors across the two figures so readers recognize the same data.
