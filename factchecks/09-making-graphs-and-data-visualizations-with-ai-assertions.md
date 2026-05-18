# Assertions Report: 09-making-graphs-and-data-visualizations-with-ai.md
**Date:** 2026-05-18
**Source file:** chapters/09-making-graphs-and-data-visualizations-with-ai.md
**Assertions flagged:** 22
**Breakdown:** STAT: 3 | GUIDELINE: 4 | APPROVAL: 0 | EVIDENCE: 11 | SPECIALIST: 3 | CURRENT: 1

**Verdict counts:** CONFIRMED: 18 | CONTRADICTED: 1 | UNVERIFIED: 2 | OUTDATED: 0 | MIXED: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

### 1. "compared with what?" attribution to Cairo (MIXED / attribution chain)
**Line 84** — "Alberto Cairo… names the single most useful diagnostic for chart honesty: *compared with what?*"
- **Category:** EVIDENCE
- **Type:** POSITIVE (named attribution)
- **Verdict:** MIXED. Cairo uses "compared with what?" as a load-bearing diagnostic in both *The Truthful Art* (2016) and *How Charts Lie* (2019). However, the phrase has earlier roots: Edward Tufte uses "At the heart of quantitative reasoning is a single question: Compared to what?" as a foundational framing across his work (esp. *Visual Explanations*, 1997), and the question is commonly traced through Tukey-era statistical thinking. Calling Cairo the originator overstates; he is the popularizer most associated with applying it specifically to chart honesty audit.
- **Recommendation:** Soften the attribution chain to "Cairo's load-bearing diagnostic, sharpening a question Tufte had named earlier" or similar. The chapter's reflexive-commitment standard (CLAUDE.md §4) calls for honest attribution chains; current phrasing reads as if Cairo coined it.
- **Source:** [Tufte — Advice for effective analytical reasoning](https://www.edwardtufte.com/notebook/advice-for-effective-analytical-reasoning/); Cairo, *The Truthful Art* (New Riders 2016); Cairo, *How Charts Lie* (W. W. Norton 2019).

### 2. FT Visual Vocabulary "eight functional categories" count (CONTRADICTED, minor)
**Line 53** — "the Financial Times' open-source Visual Vocabulary (Berkamp et al., FT Interactive) name eight functional categories of chart question."
- **Category:** EVIDENCE
- **Type:** POSITIVE (specific count)
- **Verdict:** CONTRADICTED (factual). The FT Visual Vocabulary names **nine** categories: Deviation, Correlation, Ranking, Distribution, Change over Time, Part-to-Whole, Magnitude, Spatial, and Flow. "Eight" is one short. Also: the lead designer credit is typically "Alan Smith / FT Visual Journalism Team" — the "Berkamp et al." attribution is unconfirmed; the canonical citation is to the FT Chart Doctor / FT Visual Journalism team rather than a named "Berkamp."
- **Recommendation:** Change to "nine functional categories" and re-cite as "Financial Times Visual Journalism Team, *Visual Vocabulary*" or remove the specific authorial attribution.
- **Source:** [FT chart-doctor/visual-vocabulary repo](https://github.com/Financial-Times/chart-doctor/tree/main/visual-vocabulary)

---

## Full Findings

### EVIDENCE category

**E1. Line 53 — Andy Kirk, *Data Visualisation: A Handbook for Data Driven Design* (SAGE, 2nd ed. 2019)**
- Type: BASIC (citation metadata)
- **Verdict:** CONFIRMED. SAGE Publications, 2nd edition published 2019, ISBN 9781526468925.
- Source: [SAGE/Amazon listing](https://www.amazon.com/Data-Visualisation-Handbook-Driven-Design/dp/1526468921)

**E2. Lines 74, 84 — Cole Nussbaumer Knaflic, *Storytelling with Data* (Wiley, 2015), Chapter 2 "Choosing an Effective Visual"**
- Type: BASIC (citation metadata + chapter title)
- **Verdict:** CONFIRMED. Wiley, 2015. Chapter 2 is titled "Choosing an Effective Visual." Knaflic's guidance — name the audience, identify the single takeaway, then pick the form — is accurate to her Chapters 1–2.
- Source: [Wiley Online Library](https://onlinelibrary.wiley.com/doi/10.1002/9781119055259.ch2); [Wiley book page](https://www.wiley.com/en-us/Storytelling+with+Data:+A+Data+Visualization+Guide+for+Business+Professionals-p-9781119002253)

**E3. Line 74 — Stephen Few, *Show Me the Numbers* (Analytics Press, 2nd ed. 2012)**
- Type: BASIC (citation metadata)
- **Verdict:** CONFIRMED. Analytics Press, 2nd edition published June 2012, 371 pages.
- Source: [Analytics Press](https://www.analyticspress.com/smtn.php)

**E4. Line 84 — Alberto Cairo, *The Truthful Art* (New Riders, 2016)**
- Type: BASIC (citation metadata)
- **Verdict:** CONFIRMED. New Riders (Pearson imprint), 2016, ISBN 9780321934079, 400 pages.
- Source: [Pearson product page](https://www.pearson.com/en-us/subject-catalog/p/the-truthful-art-data-charts-and-maps-for-communication/P200000008947/9780133440539)

**E5. Line 84 — Alberto Cairo, *How Charts Lie* (W. W. Norton, 2019)**
- Type: BASIC (citation metadata)
- **Verdict:** CONFIRMED. W. W. Norton, October 2019, ISBN 9781324001560.
- Source: [Norton catalog](https://wwnorton.com/books/9781324001560)

**E6. Line 99 — Edward Tufte, *The Visual Display of Quantitative Information* (Graphics Press, 1st ed. 1983; 2nd ed. 2001), Chapter 2 "Graphical Integrity"**
- Type: BASIC (citation metadata + chapter content)
- **Verdict:** CONFIRMED. Graphics Press, 1st ed. 1983; 2nd ed. 2001. The "Graphical Integrity" chapter (Ch. 2) introduces the Lie Factor and the principle that visual magnitude should be proportional to data magnitude (the precursor of the proportional-ink articulation later).
- Source: [Edward Tufte Wikipedia](https://en.wikipedia.org/wiki/Edward_Tufte); [Tufte's principles overview](https://thedoublethink.com/tuftes-principles-for-visualizing-quantitative-information/)

**E7. Line 101 — Tufte's textbook lie factor of 14.8: "53% numerical change displayed as a 783% visual change"**
- Type: POSITIVE (precise numbers)
- **Verdict:** CONFIRMED. The example is the 1978 NYT fuel-economy standards chart: data change 18→27.5 mpg = 53%; visual length change 0.6"→5.3" = 783%; lie factor = 14.8. Tufte's range "1.0 ± 0.05" (the chapter says "0.95 to 1.05") is correct.
- Source: [InfoVis Wiki — Lie Factor](https://infovis-wiki.net/wiki/Lie_Factor); [datavis.ca Gallery — Lie Factor](https://www.datavis.ca/gallery/lie-factor.php); [Tufte notebook](https://www.edwardtufte.com/notebook/computing-lie-factor-by-dividing-percentages/)

**E8. Line 105 — Anshul Pandey et al., "How Deceptive Are Deceptive Visualizations?" CHI 2015**
- Type: BASIC (citation + finding)
- **Verdict:** CONFIRMED. Pandey, Rall, Satterthwaite, Nov, and Bertini, CHI 2015 (Seoul, April 18–23). The paper documents large viewer-misperception effects from common distortion techniques including y-axis truncation. Chapter framing is accurate.
- Source: [ACM DL](https://dl.acm.org/doi/10.1145/2702123.2702608); [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2566968)

**E9. Line 105 — "Yang and colleagues (2021)… in some conditions 83.5% of participants overestimated the data effect when the y-axis was truncated"**
- Type: POSITIVE (precise percentage)
- **Verdict:** CONFIRMED. Yang, Vosgerau & Loewenstein (2021), "Truncating Bar Graphs Persistently Misleads Viewers," *Journal of Applied Research in Memory and Cognition* (Elsevier). Across five studies, ~83.5% of participants showed the truncation effect, persisting even after explicit instruction.
- Source: [ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S2211368120300978)
- Note: The chapter cites "Yang and colleagues (2021)" without giving the journal or co-authors. Reviewer may wish to add a more complete citation given the load-bearing 83.5% number.

**E10. Line 105 — Correll, Bertini, Franconeri, "Truncating the Y-Axis: Threat or Menace?" CHI 2020, arXiv:1907.02035**
- Type: BASIC (citation metadata + finding)
- **Verdict:** CONFIRMED. CHI 2020 Honorable Mention paper. arXiv ID 1907.02035 (July 2019; updated January 2020). The finding — truncation effect is persistent even when explicitly labeled — is correctly stated.
- Source: [arXiv:1907.02035](https://arxiv.org/abs/1907.02035); [Correll Medium](https://mcorrell.medium.com/truncating-the-y-axis-threat-or-menace-d0bce66d4d08)

**E11. Lines 125, 269 — Holder & Xiong, "Dispersion vs. Disparity" — arXiv:2208.04440, 2022; published *IEEE TVCG* 2023**
- Type: POSITIVE (citation metadata + load-bearing finding)
- **Verdict:** CONFIRMED. Eli Holder & Cindy Xiong (now Cindy Xiong Bearfield), arXiv 2208.04440 (Aug 2022); IEEE TVCG publication 2022/2023 (IEEE Xplore document 9913065). The finding — bar charts of means encourage stronger essentialist / "deficit thinking" inferences than variance-revealing alternatives — is accurate to the paper. The paper ran four experiments (not "a series" indeterminate); chapter framing is broadly faithful.
- Source: [arXiv:2208.04440](https://arxiv.org/abs/2208.04440); [IEEE Xplore 9913065](https://ieeexplore.ieee.org/document/9913065/)

**E12. Lines 135–137 — Cleveland & McGill (1984), *JASA* 79(387), 531–554; perception hierarchy**
- Type: POSITIVE (citation + ordered ranking)
- **Verdict:** CONFIRMED. William Cleveland and Robert McGill, "Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods," *JASA* Vol. 79, No. 387 (September 1984), pp. 531–554. The hierarchy as stated in the chapter (position on common scale > position on non-aligned scales > length > angle > area > volume > color luminance > color hue) is the canonical reading. (Minor: Cleveland & McGill's original list orders the perceptual *elementary tasks* slightly differently; "shading/color saturation" appears as the last task. The chapter's collapse into "color luminance > color hue" is a faithful pedagogical simplification.)
- Source: [JASA paper PDF](http://euclid.psych.yorku.ca/www/psy6135/papers/ClevelandMcGill1984.pdf)

**E13. Line 143 — Harrower & Brewer, "ColorBrewer.org: An Online Tool for Selecting Colour Schemes for Maps," *The Cartographic Journal* 40(1), 2003**
- Type: BASIC (citation metadata)
- **Verdict:** CONFIRMED. *The Cartographic Journal*, Vol. 40, No. 1 (2003), pp. 27–37. DOI 10.1179/000870403235002042.
- Source: [Taylor & Francis Online](https://www.tandfonline.com/doi/abs/10.1179/000870403235002042); [colorbrewer2.org](https://colorbrewer2.org)

### SPECIALIST category

**S1. Lines 103, 107 — "AI tools — Excel's default behavior, ChatGPT's matplotlib output, Claude's Artifact charts, Julius.ai — almost all auto-fit the y-axis to the data range by default"**
- Type: POSITIVE (capability/defect claim across named tools)
- **Verdict:** CONFIRMED (with nuance). matplotlib's default `autoscale` behavior fits axes to data range; Excel auto-fits the y-axis to data range by default for bar charts (a documented and widely critiqued behavior); ChatGPT Code Interpreter output inherits matplotlib defaults; Claude Artifacts using D3/Recharts also auto-fit by default unless prompted otherwise. Julius.ai behavior is broadly the same as matplotlib-based pipelines. The claim is correct as a class statement about default behavior.
- Note: Excel does *sometimes* default to zero baseline for bar charts when the data range starts near zero; the auto-truncation is most aggressive when all values are far from zero. Chapter framing remains defensible as a general claim about tool defaults.

**S2. Line 109 — "Tufte holds that line charts can start anywhere because they encode shape, not magnitude. Stephen Few argues line charts with non-zero baselines are nearly as dishonest as truncated bars when the visual is meant to communicate magnitude rather than trend shape."**
- Type: POSITIVE (named disagreement)
- **Verdict:** CONFIRMED. Tufte's line-chart position is articulated in *Visual Display* and in his online forum responses (line graphs encode change, not absolute magnitude). Few's position is explicit in *Show Me the Numbers* and in his Perceptual Edge newsletters: when magnitude is the message, zero baseline is required for lines as well as bars. The disagreement is real and frequently rehearsed in the visualization community.
- Note: Cairo's "split the difference" framing in the chapter is a fair summary of his treatment in *The Truthful Art* and *How Charts Lie*, though not a verbatim Cairo quote.

**S3. Line 277 — "8% of male readers and 0.5% of female readers with color-vision deficiency"**
- Type: STAT (specific percentages, embedded inside a misconception correction)
- **Verdict:** CONFIRMED. These figures (≈8% of males, ≈0.5% of females of Northern European descent with red-green color-vision deficiency) are the canonical numbers in the colorblindness literature and accurately reported.
- Source: NIH / National Eye Institute population estimates; consistent with WCAG and ColorBrewer documentation.

### GUIDELINE category

**G1. Line 8 (TL;DR) and §5 — The "five-question chart checklist" anchored to Cairo and Tufte**
- Type: GUIDELINE (proposed practice)
- **Verdict:** UNVERIFIED-by-design. The five-question framing is the chapter's *own synthesis*. It is not attributed to an external guideline body (e.g., ASA, NCES, IES). The chapter's loadbearing claim ("anchored to Cairo's 'compared with what?' and Tufte's proportional ink") is sound; the checklist itself is a Nik Bear Brown synthesis and is accurately presented as such. Reviewer should ensure the chapter does not at any point imply external endorsement.

**G2. Line 41 — "five-question audit, anchored in three names that matter — Cairo, Tufte, Knaflic"**
- Type: GUIDELINE
- **Verdict:** CONFIRMED as a defensible canonical triad in the field. These are the three names a teacher-audience text would most reasonably anchor on for chart honesty practice.

**G3. Lines 47–63 — "Five functional categories most useful for teacher data — comparison, change over time, distribution, relationship, part-to-whole"**
- Type: GUIDELINE (taxonomy claim)
- **Verdict:** CONFIRMED. This 5-category collapse from the FT Visual Vocabulary's nine is a standard pedagogical simplification (also used by Few, Knaflic, and Kirk in different orderings). The chapter explicitly notes the FT names eight (see E2 — should be nine) and that the chapter uses five "for teacher data," which is fair scoping.

**G4. Line 149 — "ColorBrewer's *Set2* for categorical and *YlOrRd* or *Blues* for sequential, in colorblind-safe variants where available"**
- Type: GUIDELINE (named palette recommendation)
- **Verdict:** CONFIRMED. Set2, YlOrRd, and Blues are all canonical ColorBrewer palettes. Set2 is categorical and largely colorblind-safe; YlOrRd is sequential (note: ColorBrewer's documentation flags YlOrRd as *not* fully colorblind-safe for some pairs — *Blues* and *YlGnBu* are safer choices). The chapter's "in colorblind-safe variants where available" hedge is responsible.

### STAT category

**T1. Line 165 — "The 2025 FACTS benchmark on grounded reasoning reports hallucination rates of 3–10% on frontier models depending on task and reasoning mode [verify exact figure]"**
- Type: POSITIVE (precise range, named benchmark)
- **Verdict:** CONFIRMED with caveat. Google DeepMind's FACTS Grounding benchmark (and the FACTS v2 expansion published December 2025) reports hallucination/grounding-error rates broadly in the 3–10%+ band for current frontier models, with reasoning modes consistently performing *worse* (some exceeding 10% — Grok-4-fast-reasoning reaches ~20%; GPT-5, Claude Sonnet 4.5, Grok-4, Gemini-3-Pro all exceed 10% on grounded summarization). The chapter's "3–10%" is a reasonable summary but understates the high end on reasoning-mode evaluations.
- Recommendation: Revise to "3–10% on the easier grounded tasks; over 10% on grounded summarization for reasoning-mode evaluations." The `[verify exact figure]` marker is already present — keep it until citation is added.
- Source: FACTS Grounding benchmark (Google DeepMind, Dec 2024 launch; v2 Dec 2025); industry roundups cited in research notes.

**T2. Line 198 — Maya's worked example: "Adams's bar is more than 8× longer than Sandoval's at this scale. The data difference is 6.8 points out of 100 — about 9%. Lie factor is roughly 8 to 10"**
- Type: STAT (lie factor calculation on illustrative data)
- **Verdict:** CONFIRMED as a plausible illustrative calculation. With y-axis at 70: Adams 78.2 → bar length 8.2; Sandoval 71.4 → bar length 1.4. Ratio = 8.2/1.4 ≈ 5.9× (not strictly "more than 8×"; closer to 6×). True data ratio 78.2/71.4 ≈ 1.10. Lie factor ≈ 5.9 (visual ratio) / 1.10 (data ratio) ≈ 5.4× — so the chapter's "8 to 10" lie factor is overstated by roughly a factor of two when computed strictly. (Tufte's own formula uses % effect change, not raw ratios; the chapter mixes framings.)
- Note: This is composite-illustrative data (chapter notes this on line 184), so factual accuracy isn't the issue — internal arithmetic consistency is. Reviewer may want to either tighten the numbers or relabel as "the visual gap looks roughly 5–10× the data gap" without committing to a specific lie factor.

**T3. Lines 393, 436 — Julius.ai cited with "*TechCrunch*, July 2025 [verify exact date]" and "Evaluating Graphical Perception with Multimodal LLMs, arXiv:2504.04221, 2025"**
- Type: CURRENT (recent citations)
- **Verdict:** CONFIRMED. TechCrunch published "AI data analyst startup Julius nabs $10M seed round" on **July 28, 2025**. The arXiv paper 2504.04221 ("Evaluating 'Graphical Perception' with Multimodal LLMs," Nguyen, Maeda, Geshvadi, Haehn) was posted April 5, 2025. Both citations are accurate.
- Recommendation: Drop the `[verify exact date]` flag — date is July 28, 2025.
- Source: [TechCrunch July 28 2025](https://techcrunch.com/2025/07/28/ai-data-analyst-startup-julius-nabs-10m-seed-round/); [arXiv:2504.04221](https://arxiv.org/abs/2504.04221)

### CURRENT category

**C1. Line 393 — "ChatGPT Advanced Data Analysis (OpenAI)… Claude Artifacts (Anthropic)… Julius.ai"**
- Type: CURRENT (product naming as of writing)
- **Verdict:** CONFIRMED. All three are current product names as of mid-2026. The chapter's own caveat — "tools change quarterly" — is appropriate. Note: OpenAI's product has been variously branded "Code Interpreter," "Advanced Data Analysis," and now (2025+) is generally surfaced as a tool inside ChatGPT rather than a named product mode; "Advanced Data Analysis" is recognizable and defensible.

---

## Unverified Assertions

**U1. Line 53 — "Berkamp et al., FT Interactive"**
- The FT Visual Vocabulary is the product of the FT Visual Journalism team; the lead designer most frequently credited is Alan Smith. "Berkamp" as a named author does not appear in any verifiable source for this artifact. UNVERIFIED — likely incorrect attribution.

**U2. Line 245 — "841 students in the dataset"**
- Sum of Maya's six teachers' n values (142+138+145+140+139+137) = **841**. Arithmetic checks. CONFIRMED internally.

---

## AI-Pass Flags

The chapter is internally consistent in voice and method. Two patterns to watch:

1. **"Author/originator" attributions that compress history.** Cairo did not coin "compared with what?" — he sharpened a phrasing with deeper roots in Tufte and statistical practice. The chapter's framing (Critical Issue 1) treats Cairo as origin. This is consistent with the workshop's reflexive-commitment standard (CLAUDE.md §4) only if amended.

2. **Composite-illustrative numbers with derived "lie factors."** The Maya worked example states a lie factor "8 to 10" that does not survive direct arithmetic on the stated numbers. Composite data is fine; arithmetic-on-composite-data needs to remain internally consistent or be expressed as a range rather than a derived ratio.

---

## Reliability Assessment

This is one of the strongest-sourced chapters in the book. The four load-bearing primary citations — Cairo, Tufte, Cleveland & McGill, Holder & Xiong — are all verified accurate in author, title, year, journal/publisher, and substantive finding. The CHI 2015 (Pandey), CHI 2020 (Correll), and arXiv:2504.04221 (Nguyen) references all check out cleanly. The main fixes needed are (a) softening the "Cairo coined 'compared with what?'" framing to acknowledge Tufte's earlier articulation, (b) correcting "eight" to "nine" categories for the FT Visual Vocabulary and dropping the unverifiable "Berkamp et al." attribution, (c) tightening the Maya worked-example arithmetic so the stated lie factor matches the stated bar ratios, and (d) updating the Julius.ai TechCrunch citation to "July 28, 2025." None of these defeats the chapter's argument; all of them tighten its scholarship.
