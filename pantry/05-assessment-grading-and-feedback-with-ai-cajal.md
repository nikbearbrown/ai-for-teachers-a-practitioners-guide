# CAJAL Figure Intelligence — Chapter 5: Assessment, Grading, and Feedback with AI

**Source:** `chapters/05-assessment-grading-and-feedback-with-ai.md`
**Mode:** `/scan silent`
**Domain note:** AI+1 practitioner guide / K-12 and higher-ed teaching. Chapter pulls "grading" apart into four sub-tasks (first-pass scoring / feedback drafting / response grouping / final grade decision). Reports Steiss 2024 (criteria-alignment match, accuracy/prioritization/clarity/tone lose) and Henkel 2024 (QWK ~0.70 vs human ~0.75 inter-rater). Frames the rubric as a measuring instrument requiring calibration. Predicts a feedback-level Bastani parallel (prose-only, not yet measured). Names the four conditions where the workflow stops helping. Six author-placed figures.

---

## Density Recommendation

**4 figures, Concept-anchor density.** Four earn their place: (1) the four-sub-tasks-of-grading taxonomy, (2) the Steiss criteria comparison (1 win, 4 losses), (3) the Bastani parallel bars (control / GPT Base / GPT Tutor with practice/exam pairs), (4) the formative-to-summative gate-slide. The calibration-with/without-rerun timeline (5.3) and the "workflow earns its savings" figure (5.5) are softer; drop or fold into prose. Six figures is over-budget for a chapter built mostly on prose-driven argument.

---

## Zone Map

- **MC:** Grading is four sub-tasks, not one — AI is capable on three with appropriate gates, irreducible-teacher on the fourth. Rubric calibration is a measuring-instrument operation. The Bastani parallel predicts a feedback-level learning loss without review (prediction, not measured). The gate slides toward more human involvement as stakes rise.
- **VG:** Four-row sub-task taxonomy with capability/gate encoding. Steiss criteria comparison (alignment vs accuracy/prioritization/clarity/tone). Bastani three-condition grouped bars (practice / unaided exam). Formative-to-summative continuum with sliding gate marker.
- **PQ:** QWK ~0.70 (AI vs human) vs ~0.75 (human vs human). 50–80% time savings band (range, vendor-upper to peer-reviewed-lower). 80 min on 110 responses (worked example) vs 4 hours without AI. 80% kept / 15% edited / 5% overridden. ±0.5 calibration tolerance on five samples. 48% / 127% practice gains; -17% exam decrement (Bastani).

---

## Figure 5.1 — Four Sub-Tasks of Grading

**Priority: Critical.** The chapter's foundational disaggregation. Must show four rows with capability-encoding consistent with the book's execution/judgment canon.

### Block 1 — Illustrae paste block

A vertical four-row stack composition, single-column 89mm. Four horizontal stripes of equal height. Top three stripes (sub-tasks 1, 2, 3 — AI-capable with appropriate review): each tinted Bluish Green `#009E73` 15% opacity background. Bottom stripe (sub-task 4 — final grade decision, teacher-irreducible): tinted Vermillion `#D55E00` 15% opacity background. On the left margin of each stripe, a small filled circle marker — Bluish Green `#009E73` for the top three, Vermillion `#D55E00` for the bottom. To the right of each top-three marker, a small Orange `#E69F00` filled square indicates the required review gate (delegate-with-review). The bottom stripe has no Orange gate marker — instead it has a small Black `#000000` 1pt closed-circle "lock" symbol indicating the irreducible human boundary. White background, flat vector. Stripes separated by thin Black `#000000` 0.5pt horizontal lines.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Four-row stack of grading sub-tasks. Top three rows AI-capable with review gates. Bottom row teacher-irreducible (locked).
[O] Vertical stack, four equal-height rows. Left-margin markers + gate/lock indicators.
[P] Top three rows Bluish Green 15% with Bluish Green markers and Orange gate squares. Bottom row Vermillion 15% with Vermillion marker and Black lock. Row dividers Black 0.5pt.
[E] No sub-task names rendered as image content, no example student work, no rubric text, no decorative ornament, no shadows.

### Block 3 — Negative prompt

sub-task names rendered as graphics, sample student work, rubric text, screenshots, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 5.2 — Steiss Five-Criteria Comparison

**Priority: Critical.** The chapter's empirical anchor on AI feedback capability. Must render the 1-of-5 outcome — alignment wins, the four properties that make feedback educational lose.

### Block 1 — Illustrae paste block

A horizontal grouped-bar composition, single-column 89mm. Five criterion groups along the x-axis (post-typography labels: alignment, accuracy, prioritization, clarity, tone). Each group has two adjacent bars: left bar (ChatGPT) and right bar (teacher). The first group (alignment): ChatGPT bar is slightly taller than the teacher bar — both colored Sky Blue `#56B4E9` (ChatGPT) and Blue `#0072B2` (teacher). Groups 2–5: ChatGPT bars visibly shorter than teacher bars (teacher wins). A faint Vermillion `#D55E00` 15% opacity vertical band covers groups 2–5 indicating "the four properties where AI loses." A faint Bluish Green `#009E73` 15% opacity vertical band covers group 1 indicating "the one property AI matches/exceeds." Axis Black `#000000` 1pt. No numeric values rendered. White background, flat vector.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Five grouped-bar criteria. Group 1 (alignment): ChatGPT matches/exceeds teacher. Groups 2–5: teacher wins. Background bands distinguish the one win-zone from the four loss-zones.
[O] X-axis: five criterion groups. Y-axis: rated quality. Two bars per group.
[P] ChatGPT bars Sky Blue. Teacher bars Blue. Win-zone band Bluish Green 15%. Loss-zone band Vermillion 15%. Axes Black 1pt.
[E] No numeric axis values rendered as image content, no specific scores, no decorative ornament, no shadows.

### Block 3 — Negative prompt

numeric axis values, criterion names rendered as graphics, chart titles, gibberish letters, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 5.3 — Bastani Parallel at the Feedback Level

**Priority: Important.** Reactivates Chapter 2's Bastani figure at the grading-and-feedback altitude. Must label the prediction explicitly (not yet measured at the feedback level).

### Block 1 — Illustrae paste block

A grouped-bar chart, single-column 89mm. Three condition groups along the x-axis (post-typography: Control, GPT Base, GPT Tutor). Each group has two adjacent bars: practice (Sky Blue `#56B4E9` filled) and unaided exam (Blue `#0072B2` filled). The GPT Base group has the practice bar taller than control but the exam bar visibly shorter than control — the prediction-of-interest. The GPT Tutor group has the practice bar tallest in the chart and the exam bar near the control baseline. A faint Black `#000000` 0.5pt dashed horizontal line marks the control-exam baseline across the chart. A small Orange `#E69F00` filled diamond marker hovers above the GPT Base exam bar with a thin Black `#000000` 0.75pt connector — placeholder for the "prediction, not measured" annotation post-typography. White background, flat vector.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Grouped bar chart with three conditions and two metrics per condition (practice / unaided exam). The GPT Base exam bar drops below the control exam baseline. The GPT Tutor practice bar is the tallest. A diamond marker flags the predicted (not measured) bar.
[O] X-axis: three conditions. Y-axis: performance. Two adjacent bars per group. Baseline dashed line. Prediction marker on GPT Base exam.
[P] Practice bars Sky Blue. Exam bars Blue. Baseline Black 0.5pt dashed. Prediction marker Orange with Black 0.75pt connector. Axes Black 1pt.
[E] No numeric axis labels rendered, no specific percentage values rendered, no decorative ornament, no shadows.

### Block 3 — Negative prompt

numeric axis labels, percentage values rendered as graphics, condition names rendered as graphics, chart titles, gibberish letters, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## Figure 5.4 — Formative-to-Summative Gate Slide

**Priority: Important.** The gate placement principle. Must render a continuum with a movable gate that visibly shifts position with the stakes axis.

### Block 1 — Illustrae paste block

A horizontal continuum composition, single-column 89mm. A long horizontal Black `#000000` 1pt baseline with two endpoint markers — left endpoint labeled "formative" (post-typography), right endpoint labeled "summative." A gradient ramp underneath the baseline transitions from Bluish Green `#009E73` 25% opacity on the left to Vermillion `#D55E00` 25% opacity on the right — encoding low-stakes-to-high-stakes. Three vertical gate markers along the baseline: a Bluish Green `#009E73` 1.5pt vertical line at the left third (light review gate position), an Orange `#E69F00` 2pt vertical line at the middle (medium review), and a Vermillion `#D55E00` 2.5pt vertical line at the right third (full teacher review). Above each gate marker, a small filled circle in the same color indicating gate position. A thin horizontal Black `#000000` 0.75pt arrow runs above the entire continuum left-to-right with a small Orange `#E69F00` filled diamond at its midpoint indicating "gate slides as stakes rise." White background, flat vector.

### Block 2 — Full SCOPE prompt

[S] Single-column 89mm, vector, white background.
[C] Horizontal continuum from formative (left) to summative (right). Stakes gradient underneath. Three gate markers along the baseline at progressively higher stakes positions. A directional arrow above marks the gate-slide trajectory.
[O] Horizontal baseline. Stakes gradient underneath. Three gate verticals at left third, middle, right third. Slide arrow above.
[P] Baseline and slide arrow Black 1pt and 0.75pt. Stakes gradient: Bluish Green 25% left → Vermillion 25% right. Gate markers progressively: Bluish Green / Orange / Vermillion. Slide arrow midpoint diamond Orange.
[E] No axis labels rendered as image content, no example assessment names, no decorative ornament, no shadows.

### Block 3 — Negative prompt

axis labels rendered as graphics, assessment names, gradebook screenshots, gibberish letters, titles, captions, decorative ornament, photographic elements, realistic 3D textures, drop shadows, gradient fills, gradient backgrounds, hand-drawn styles, sketch lines, decorative borders, colorful backgrounds, visual clutter, fuzzy borders, watermarks, red-green color combinations, rainbow color scales, 3D perspective distortion

---

## What CAJAL Declines to Architect

- **Figure 5.3 (two-column timeline "without the re-run" vs "with").** Best as a sentence or brief table in prose; the calibration-drift narrative carries itself.
- **Figure 5.5 ("When the calibration workflow earns its time savings").** Vague title; argument is conditional ("if these four conditions hold"). Better as the four-condition list in prose. Drop.
- **The unnumbered calibration time/savings comparison.** Drop; prose carries it.
- **LMS gradebook / dashboard screenshots.** Out of scope by CAJAL discipline.
- **Anonymized student essay excerpts.** Student work samples — out of scope.
- **Rubric text printouts.** Typography artifact; do not redraw.
- **κ / QWK formula renderings.** Typography artifact; equation in prose.
- **Edward Thorndike portrait.** AI Wayback Machine asset; separate portrait pipeline.
- **EU AI Act Annex III citation graphic.** Reference, not a figure.

---

## Video Candidate Pass

**FIGURE 5.1 (four sub-tasks):** STATIC SUFFICIENT.
**FIGURE 5.2 (Steiss criteria comparison):** STATIC SUFFICIENT.
**FIGURE 5.3 (Bastani parallel):** STATIC SUFFICIENT. Same as Chapter 2's Bastani bars — style consistently.
**FIGURE 5.4 (formative-summative slide):** **MILD VIDEO CANDIDATE.** A digital edition could let the reader drag the gate along the continuum to see the stakes/review trade-off. In print, static suffices.

**Video candidates identified: 1 mild.** Recommended for digital edition.

---

## Split-point note

Three canons must hold consistent with prior chapters. (1) The four-sub-task taxonomy (Fig 5.1) inherits the Bluish Green / Orange / Vermillion encoding from Chapter 1's three-zone taxonomy and Chapter 4's two-layer split — keep colors aligned. (2) The Bastani bars (Fig 5.3) should be visually parallel to Chapter 2's Fig 2.4 (same bar coloring, same condition ordering, same baseline-dashed-line convention) so the reader recognizes "same finding, different altitude." (3) The formative-to-summative gate (Fig 5.4) reactivates Chapter 2's gate language — the Vermillion vertical bar at the summative end should match the Vermillion of Chapter 2's red-tier gate cluster, signaling "permanent, high-stakes." Chapter 6 (differentiation) and Chapter 7 (parent communication) will likely reactivate the gate canon — lock it here so downstream rendering is consistent.
