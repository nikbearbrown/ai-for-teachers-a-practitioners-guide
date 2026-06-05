# CAJAL Figure Intelligence — Chapter 9: Making Graphs and Data Visualizations with AI

**Source:** `chapters/09-making-graphs-and-data-visualizations-with-ai.md`
**Mode:** `/scan silent`
**Domain note:** AI+1 practitioner guide / K-12 and higher-ed teaching. Truncated-axis lies, Cairo's "compared with what?", Tufte's proportional ink, distribution-over-means for equity, the five-question audit. Bertin's retinal variables as ancestor framing. Four author-placed figures plus one reference table.

---

## Density Recommendation

**4 figures, Audit density.** All four earn their place. The chapter teaches a checklist and three of the four figures embody pieces of it.

---

## Zone Map

- **MC:** Truncated-axis distortion (same data, two charts, two stories). Distribution-over-means equity move (bar of means hides three different teaching situations). Five-question audit as operating procedure.
- **VG:** Cairo's four failure modes as a 2×2-like quadrant grid. Three distributions yielding the same mean (uniform, bimodal, long-tail). Sorted-vs-alphabetical bar arrangement.
- **PQ:** 83.5 percent overestimation under truncation (Yang 2021). Lie factor ~5.5 in the worked example. ~8 percent / ~0.5 percent color-blindness floor.

---

## Figure 9.1 — Truncated vs. Zero-Baseline Bar Chart

**Priority: Critical.** The chapter's single most important visual argument.

### Block 1 — Illustrae paste block

A two-panel side-by-side bar chart composition. Left panel: six vertical bars representing six teachers, with the y-axis starting around 68 (truncated). Bars vary dramatically in visible height — the leftmost bar much taller than the rightmost. All bars Sky Blue `#56B4E9` filled. Axis lines Black `#000000` 1pt. A small Vermillion `#D55E00` filled triangle floats near the y-axis origin marking the truncation. Right panel: the same six bars on a y-axis starting at zero (running 0-100). The bars now appear as nearly equal heights, clustered in a tight band near the top of the axis. Bars Sky Blue `#56B4E9` filled. A thin Bluish Green `#009E73` horizontal dashed line crosses the bars at the proficiency benchmark level. A small Bluish Green check shape floats beside the right panel marking the honest version. A vertical Black `#000000` 1pt separator divides the two panels. White background, flat vector, double-column 174mm preferred.

### Block 2 — Full SCOPE prompt

[S] Double-column 174mm preferred, vector, white background.
[C] Two panels showing the same six-bar dataset. Left has truncated y-axis exaggerating differences. Right has zero baseline showing tight clustering, with a benchmark reference line.
[O] Side-by-side panels. Truncation warning marker on left; pass check on right. Benchmark line on right panel.
[P] All bars Sky Blue (single color, no decorative variation). Axes Black 1pt. Truncation warning Vermillion. Benchmark line Bluish Green dashed. Pass check Bluish Green. Separator Black 1pt.
[E] No teacher names, no rendered numerals on axes, no rendered values on bars, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, teacher names, axis numerals, value labels on bars, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, multi-color bar palettes, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 9.2 — Cairo's Four Failure Modes

**Priority: Important.** Names the four "compared with what?" failures.

### Block 1 — Illustrae paste block

A 2×2 quadrant grid composition. Outer frame Black `#000000` 1pt. Each of four cells contains a small abstract chart icon. Top-left cell (absolute counts): two Sky Blue `#56B4E9` filled bars of different heights with a small Vermillion `#D55E00` question-mark blob beside them. Top-right cell (time series without baseline): a Blue `#0072B2` 1pt line rising upward, with a small Vermillion `#D55E00` dashed-outline rectangle floating behind it indicating missing prior-years context. Bottom-left cell (cross-sectional without controls): two Bluish Green `#009E73` filled circles of different sizes with a Vermillion 1pt arrow crossing between them and a small Vermillion warning triangle. Bottom-right cell (single-value claim): a single Orange `#E69F00` filled rectangle (one value) floating alone with a Vermillion question mark beside it. White background, flat vector, double-column 174mm preferred.

### Block 2 — Full SCOPE prompt

[S] Double-column 174mm preferred, vector, white background.
[C] Four-cell grid. Each cell holds an abstract chart icon with a Vermillion warning element indicating the missing reference.
[O] 2×2 grid. Outer frame and internal dividers as thin lines.
[P] Chart icons Sky Blue / Blue / Bluish Green / Orange to differentiate failure categories. Warning elements Vermillion. Frame and dividers Black 1pt.
[E] No cell labels, no failure-mode names, no rendered numerals, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, failure-mode names, axis numerals, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 9.3 — Three Distributions, Same Mean

**Priority: Critical.** The equity move. Must show that three distinct distributions reduce to the same bar.

### Block 1 — Illustrae paste block

A three-panel horizontal composition. Top row across all three panels: a single Sky Blue `#56B4E9` filled bar of identical height in each panel (representing the same mean = 72). A thin Black `#000000` 1pt horizontal divider runs beneath the bars. Below the divider, each panel shows a different distribution drawn as a strip-plot of small Bluish Green `#009E73` filled dots: Panel 1 (uniform near mean): dots clustered tightly around the center. Panel 2 (bimodal): two clusters of dots, one on the low side, one on the high side. Panel 3 (long-tail): a dense cluster on the high side, with a small group of dots far on the low side circled by a thin Vermillion `#D55E00` 1pt dashed outline (highlighting the underserved students). A thin Black 1pt vertical line separates each panel. White background, flat vector, double-column 174mm preferred.

### Block 2 — Full SCOPE prompt

[S] Double-column 174mm preferred, vector, white background.
[C] Three panels. Top half: identical Sky Blue bars (mean). Bottom half: three distinct distributions as strip-plots of dots. Long-tail outliers in panel 3 marked with a Vermillion dashed outline.
[O] Three panels horizontally. Two-zone vertical division within each panel. Separators between panels.
[P] Mean bars Sky Blue. Distribution dots Bluish Green. Outlier highlight Vermillion dashed outline. Dividers Black 1pt.
[E] No axis numerals, no panel labels, no rendered values, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, panel names, axis numerals, value labels, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 9.4 — Five-Question Audit Checklist Card

**Priority: Important.** The operational artifact teachers carry into the chart-review moment.

### Block 1 — Illustrae paste block

A printable card composition. A single Sky Blue `#56B4E9` outlined (no fill) large rectangle with rounded corners as Black `#000000` 1pt outline. Inside, five small horizontal Sky Blue `#56B4E9` filled bands stacked vertically. Beside each band on the left, a small numbered Blue `#0072B2` filled circle (positions 1-5, no rendered numerals). On the right of each band, a small Bluish Green `#009E73` filled check shape (pass state). Below the five bands, a single Orange `#E69F00` filled band representing the AI-conditional sixth question (does the chart match the data), with a small Vermillion `#D55E00` filled warning triangle beside it. White background, flat vector, single-column 89mm.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Card with five numbered question-bands plus one AI-conditional sixth band. Position markers and check shapes per row.
[O] Vertical stack inside a rounded card outline. Position markers left; checks right.
[P] Card outline Black 1pt. Question bands Sky Blue. Position markers Blue. Check shapes Bluish Green. Sixth band Orange. AI-conditional warning Vermillion triangle.
[E] No question text rendered, no rendered numerals, no decorative ornament, no shadows.

### Block 3 — Negative prompt

text labels, question text, rendered numerals, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## What CAJAL Declines to Architect

- **Table 9.1 (five functional chart categories).** Typography reference table.
- **The six-teacher data table in the worked example.** Typography table.
- **Jacques Bertin portrait.** AI Wayback Machine image; not chapter content.
- **Screenshots of AI chart tools, Excel, or spreadsheet interfaces.** None appear; CAJAL would decline regardless.

---

## Video Candidate Pass

**FIGURE 9.1 (Truncated vs. zero baseline):** **STRONG VIDEO CANDIDATE.** A morph from the truncated panel to the zero-baseline panel — same bars sliding into clustered band as the y-axis extends down — would dramatize how the lie is the default and what changes when it is corrected. The mechanism-as-learning-target criterion is met.
**FIGURE 9.2 (Four failure modes):** STATIC SUFFICIENT.
**FIGURE 9.3 (Three distributions, same mean):** **MILD VIDEO CANDIDATE.** A reveal animation — bars first, then dots filling in below each panel — would make the "the mean conceals" claim viscerally clear.
**FIGURE 9.4 (Audit card):** STATIC SUFFICIENT — printable artifact.

**Video candidates identified: 1 strong + 1 mild.** Recommended: **Fig 9.1 (axis truncation morph).** This is the chapter's most teachable moment and the dynamic transition is exactly the cognition the figure is asking the reader to perform.

---

## Split-point note

Chapter cross-references Ch 08 (Cleveland-McGill encoding rank shared with slides), Ch 13 (equity — distribution-over-means is the bridge), and the Bertin framing. Keep Sky-Blue=data, Vermillion=warning, Bluish-Green=preserved/honest convention consistent so readers carry the semantics from Ch 06 onward.
