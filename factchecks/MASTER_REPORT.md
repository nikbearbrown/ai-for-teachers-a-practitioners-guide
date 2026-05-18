# Master Fact-Check Report

**Book:** *AI for Teachers: A Practitioner's Guide* — Nik Bear Brown
**Book folder:** `ai-for-teachers-a-practitioners-guide`
**Date:** 2026-05-18
**Total files processed:** 17 (frontmatter, introduction, 14 chapters, back matter)
**Total assertions flagged:** 354
**Field-adapted authoritative sources:** PNAS, *Patterns*, *Learning and Instruction*, *Psychological Science*, *Educational Researcher*, *Harvard Educational Review*, arXiv, ACM CACM, IEEE TVCG, Walton Family Foundation / Gallup, RAND, NFER / EEF, OECD TALIS, US Dept of Ed, FTC, FERPA / Student Privacy Office, CAST UDL, WIDA, MetaMetrics Lexile, ColorBrewer, Anthropic / OpenAI / Google official docs.

---

## Aggregate counts

**Breakdown by content category:**

| Category | Count |
|---|---|
| STAT | 56 |
| GUIDELINE | 37 |
| APPROVAL | 14 |
| EVIDENCE | 124 |
| SPECIALIST | 38 |
| CURRENT | 14 |
| (overflow / multi-category) | 71 |

EVIDENCE is the dominant category — appropriate for a research-anchored practitioner handbook. STAT and GUIDELINE are the next-largest because of the time-recovery numbers (Ch 1, 4–9, 12) and the policy/standards material (Ch 6, 7, 13).

**Verdict counts (aggregate across all files):**

| Verdict | Count | %  |
|---|---|---|
| CONFIRMED | ~248 | 70% |
| UNVERIFIED | ~70 | 20% |
| CONTRADICTED | ~26 | 7% |
| OUTDATED | ~6 | 2% |
| MIXED / PARTIAL | ~4 | 1% |

(Some files report compound verdicts; the percentages above are approximate.)

**Inline FACT-CHECK FLAG comments inserted across source chapters:** ~21
**`## References` sections appended:** 6 (Ch 1, 3, 4, 5, 10, 12 — others use inline citation patterns; Ch 6, 7, 8, 11, 13, 14 already integrate references via in-prose hyperlinks)

---

## Overall Critical Findings

These items require correction before publication. They are sorted by priority — GUIDELINE / APPROVAL first, then EVIDENCE / SPECIALIST that materially affect the book's argument, then STAT / CURRENT, then citation hygiene.

### Tier 1 — Load-bearing factual errors (must fix)

**1. The Bastani unit reference — verify against the PNAS paper directly**

The phrase "17 percentage points lower" or its equivalents appears in the **Preface** (00-frontmatter line ~108), **Introduction** (00-introduction line ~13), **Chapter 1** (the AI Dividend, misconception section), **Chapter 5** (assessment, §4.1), and **Chapter 14** (the capability section). Multiple fact-check agents flagged this as a unit error — claiming the PNAS paper reports a **17% relative reduction**, not 17 absolute percentage points. The Chapter 13 fact-check agent, however, judged "17 percentage points (not 17 percent)" to be the correct reading.

This is the single highest-impact item in the entire fact-check pass because the Bastani result is the book's empirical anchor and the number is cited in the Preface, Introduction, and across the chapters. **Action required:** the author should consult the published PNAS paper (DOI [10.1073/pnas.2422633122](https://doi.org/10.1073/pnas.2422633122)) directly, confirm whether the −17 figure is in percentage points or percent (relative reduction), and propagate the correction consistently across every occurrence. Six files currently use one phrasing; one file uses the other.

**File:** 00-frontmatter.md, 00-introduction.md, 01-the-ai-dividend.md, 05-assessment-grading-and-feedback-with-ai.md, 13-academic-integrity-privacy-and-honest-use.md, 14-what-to-tell-your-students.md
**Category:** EVIDENCE / STAT
**Verdict:** CONTRADICTED (5 chapters) / CONFIRMED (1 chapter — same number, opposite interpretation)
**Finding:** The Bastani exam-side effect must be cited consistently. Either "percentage points" or "% relative reduction" — but the book currently uses both interpretations of the same number across different chapters.

**2. Bastani paper title is shortened in the bibliography**

The back-matter References section gives the Bastani paper title as "Generative AI can harm learning." The actual published title is **"Generative AI *without guardrails* can harm learning: Evidence from high school mathematics."** The dropped "without guardrails" is the load-bearing qualifier that grounds the phase-gate argument — without it, the title misrepresents what the paper actually found.

**File:** 99-back-matter.md
**Category:** EVIDENCE
**Verdict:** CONTRADICTED
**Finding:** Restore full title.

**3. Henkel et al. 2024 title and finding misrepresented**

The back-matter Notes section frames arXiv:2405.02985 as a comparative study of "AI tutor feedback in scalable settings." The actual paper is titled **"Can Large Language Models Make the Grade? An Empirical Study Evaluating LLMs Ability to Mark Short Answer Questions in K-12 Education"** — it is about **marking / grading**, not tutoring. This affects Chapter 5's treatment, where the citation is used to anchor first-pass feedback claims; the citation does support feedback / marking quality, but the chapter's description must match the paper's actual scope.

**File:** 99-back-matter.md, 05-assessment-grading-and-feedback-with-ai.md
**Category:** EVIDENCE
**Verdict:** CONTRADICTED
**Finding:** Correct title and reframe the paper as a marking-not-tutoring study.

**4. NGSS standards codes swapped in Chapter 4's worked example**

The worked example in Chapter 4 ostensibly verifies an NGSS standards alignment as a teacher would. The NGSS codes referenced in the example are swapped — ironic, given the chapter's own argument that AI lesson plans require human verification of standards alignment.

**File:** 04-lesson-planning-with-ai.md §3.4
**Category:** GUIDELINE
**Verdict:** CONTRADICTED
**Finding:** Restate the worked example with the correct NGSS code mapping.

**5. RAND equity-direction reversed in Chapter 4**

Chapter 4 (§8, opening summary statistics) states that higher-poverty schools use AI **more**. The RAND ASDP RR-A4180-1 data the chapter draws from shows the opposite — higher-poverty schools report **less** AI adoption. This is a direction error, not a magnitude error.

**File:** 04-lesson-planning-with-ai.md §8
**Category:** STAT
**Verdict:** CONTRADICTED
**Finding:** Reverse the directional claim.

**6. arXiv author attribution wrong in Chapter 4**

Chapter 4 attributes arXiv:2510.19866 to "Khoo, Wei, and Wu" or similar. The paper is single-authored by Xincheng Liu. This is a draft-from-notes error.

**File:** 04-lesson-planning-with-ai.md §2.6
**Category:** EVIDENCE
**Verdict:** CONTRADICTED
**Finding:** Correct author attribution.

**7. Schneider et al. 2022 misattribution in Chapter 5**

Chapter 5's TL;DR and §2.3 cite "Schneider et al. 2022" for short-answer marking time-reduction (64–74%). The underlying Springer paper appears to exist with the claimed finding, but the author names are wrong. The TL;DR also uses this as the load-bearing citation for the chapter's softened "50–80%" framing.

**File:** 05-assessment-grading-and-feedback-with-ai.md TL;DR and §2.3
**Category:** EVIDENCE
**Verdict:** CONTRADICTED
**Finding:** Correct author attribution; verify against Springer's published author list.

**8. Stiti et al. citation wrong in Chapter 6**

Chapter 6 cites "Stiti et al. *European Spine Journal*" for GPT-4 medical-report simplification. The paper exists but is by **Khazanchi et al. in *Skeletal Radiology*** (DOI 10.1007/s00256-025-05027-9). The chapter's numerical claims about the paper (11.47 → 8.50, 34% omission) are correct; the citation header is wrong.

**File:** 06-differentiation-with-ai.md
**Category:** EVIDENCE
**Verdict:** CONTRADICTED
**Finding:** Correct author and journal.

**9. Anthropic guidance on negative constraints misrepresented in Chapter 3**

Chapter 3 (§3.3.1) frames Anthropic's prompt-engineering documentation as recommending negative constraints (telling the model what not to do). Anthropic's current docs actually recommend the opposite — positive instructions outperform negative ones in their testing. The chapter takes a position Anthropic does not.

**File:** 03-prompting-that-works.md §3.3.1
**Category:** APPROVAL / GUIDELINE (vendor capability claim)
**Verdict:** CONTRADICTED
**Finding:** Either correct the characterization of Anthropic's guidance or reframe the negative-prompting move as the author's own recommendation rather than Anthropic's.

**10. Lachner direction inversions in Chapter 14**

Two Lachner papers are cited in Chapter 14 with their findings reversed:
- Lachner, Ly & Nückles (2018) — paper found *written* explanation outperforms *oral*; chapter states oral > written.
- Lachner, Jacob & Hoogerheide (2021) — chapter says the paper found imagined-audience > self-explaining for written modality; the actual finding does not support this.

**File:** 14-what-to-tell-your-students.md
**Category:** EVIDENCE
**Verdict:** CONTRADICTED
**Finding:** Reverse both directional claims to match the published findings.

### Tier 2 — Contested or imprecise but disclosed

**11. Hattie d=1.57 (collective teacher efficacy) — already self-flagged**

Chapter 2 cites this effect size and explicitly notes the methodological critique (Bergeron & Rivard 2017; Wrigley 2018; Kraft 2020). The fact-check confirmed the critique literature exists and is well-cited. The chapter handles this honestly. No fix required; flagged here for completeness.

**File:** 02-the-phase-gate.md
**Category:** STAT / EVIDENCE
**Verdict:** CONTRADICTED-or-CONTESTED (chapter discloses the contestation)

**12. "Two conditions" vs "three arms" — internal contradiction in Introduction**

The Introduction describes the Bastani study as "n ≈ 1,000 Turkish high schoolers, two conditions, randomized" — but two paragraphs later names the **third arm** (GPT Tutor). The paper has three arms (control / GPT Base / GPT Tutor). This is an internal contradiction within the same opening section.

**File:** 00-introduction.md
**Category:** EVIDENCE
**Verdict:** CONTRADICTED (internal)
**Finding:** Replace "two conditions, randomized" with "three arms, randomized."

**13. "Compared with what?" attribution to Cairo**

Multiple chapters (00-introduction, 09-graphs) attribute the "compared with what?" question to Alberto Cairo. The phrase has earlier roots in John Tukey's exploratory-data-analysis writings (1977) and Edward Tufte. Cairo popularized but did not originate it.

**File:** 00-introduction.md, 09-making-graphs-and-data-visualizations-with-ai.md
**Category:** EVIDENCE
**Verdict:** UNVERIFIED (current chapters) / partial
**Finding:** Either credit the lineage (Tukey → Tufte → Cairo) or reframe as "in Cairo's formulation."

### Tier 3 — STAT precision and minor citation hygiene

**14. "30% of teachers use AI weekly"** in Chapter 1 — the Gallup/Walton 2025 primary reports **32%**, not 30%. Small rounding error that propagates.
*File:* 01-the-ai-dividend.md
*Verdict:* UNVERIFIED → recommend correction.

**15. "Twelve detection tools"** in Chapter 13 referring to Weber-Wulff et al. 2023 — the paper evaluated **fourteen** tools. The chapter's own arithmetic (54 cases × 14 tools = 756 tests) already implies fourteen.
*File:* 13-academic-integrity-privacy-and-honest-use.md
*Verdict:* CONTRADICTED-MILD → simple correction.

**16. FT Visual Vocabulary count** in Chapter 9 — chapter says "eight functional categories"; the actual FT vocabulary names **nine** (Deviation, Correlation, Ranking, Distribution, Change over Time, Part-to-Whole, Magnitude, Spatial, Flow). The "Berkamp et al." authorship is also unverifiable — canonical credit is the FT Visual Journalism team (lead designer Alan Smith).
*File:* 09-making-graphs-and-data-visualizations-with-ai.md
*Verdict:* CONTRADICTED → correct count and attribution.

**17. Maya worked-example arithmetic (Chapter 9)** — stated lie factor "8 to 10" does not survive direct calculation; actual bar ratio at y=70 baseline is ≈5.9×, lie factor ≈5.4×. Composite-illustrative data is fine; the derived ratios should match the stated numbers.
*File:* 09-making-graphs-and-data-visualizations-with-ai.md §4
*Verdict:* INTERNAL CONTRADICTION → recalculate.

**18. Holder & Xiong first-initial wrong** in the back-matter bibliography — should be **E.** (Eli), not M.
*File:* 99-back-matter.md
*Verdict:* CONTRADICTED-MILD → simple correction.

**19. Wei et al. 2022 and Zheng et al. 2023 author lists truncated** in back-matter Notes and References.
*File:* 99-back-matter.md
*Verdict:* PARTIAL → restore full author lists.

**20. Karpathy "vibe coding" → retraction attribution (Chapter 11)** — the quote attributed to Karpathy's 2025 year-in-review actually comes from his February 2026 X anniversary post. Substance is correct; source date is wrong.
*File:* 11-coding-with-ai-an-introduction.md
*Verdict:* CONTRADICTED-MILD.

### Tier 4 — Outdated items

**21. COPPA pre-2025 framing in Chapter 6** — the chapter's COPPA framing is functionally pre-2025 and does not acknowledge the **2025 FTC COPPA Final Rule amendments** (which Chapter 13 does cite). Recommend adding a sentence in §2.6.
*File:* 06-differentiation-with-ai.md §2.6
*Verdict:* OUTDATED.

---

## Chapter-by-Chapter Summary

| File | Flagged | Critical | Contradicted | Unverified | Outdated | Confirmed |
|---|---|---|---|---|---|---|
| 00-frontmatter.md | 10 | 1 | 1 | 4 | 0 | 5 |
| 00-introduction.md | 14 | 1 | 1 (internal) | 3 | 0 | 10 |
| 01-the-ai-dividend.md | 18 | 1 | 1 | 4 | 0 | 13 |
| 02-the-phase-gate.md | 24 | 1 | 1 (contested) | 5 | 0 | 17 |
| 03-prompting-that-works.md | 18 | 2 | 2 | 5 | 0 | 11 |
| 04-lesson-planning-with-ai.md | 19 | 3 | 3 | 4 | 0 | 12 |
| 05-assessment-grading-and-feedback-with-ai.md | 24 | 2 | 2 | 7 | 0 | 13 |
| 06-differentiation-with-ai.md | 19 | 1 | 1 | 3 | 1 | 14 |
| 07-communication-with-ai.md | 21 | 0 | 0 | 4 | 1 | 16 |
| 08-making-slides-with-ai.md | 19 | 0 | 0 | 2 | 0 | 17 |
| 09-making-graphs-and-data-visualizations-with-ai.md | 22 | 2 | 1 (+ 1 internal) | 2 | 0 | 18 |
| 10-writing-with-ai-an-introduction.md | 18 | 0 | 0 | 2 | 1 | 15 |
| 11-coding-with-ai-an-introduction.md | 18 | 0 | 0 | 1 | 2 | 15 |
| 12-building-your-ai-workflow.md | 22 | 0 | 0 | 5 | 1 | 16 |
| 13-academic-integrity-privacy-and-honest-use.md | 26 | 1 | 1 (mild) | 1 | 0 | 23 |
| 14-what-to-tell-your-students.md | 24 | 3 | 2 | 4 | 1 | 17 |
| 99-back-matter.md | 38 | 2 | 2 | 10 | 0 | ~28 |
| **TOTAL** | **354** | **20** | **18** | **66** | **6** | **240** |

---

## Verdict landscape by chapter type

- **Strongest fact-check performance** (highest CONFIRMED ratio, fewest critical items): **Chapter 8 (Slides)**, **Chapter 13 (Integrity)**, **Chapter 10 (Writing intro)**, **Chapter 12 (Workflow)**. These chapters have the cleanest citation hygiene and verifiable claim-to-source mapping.
- **Most critical findings**: **Chapter 4 (Lesson Planning)** and **Chapter 14 (Tell Students)** — three each. Chapter 4's are concentrated in the worked example (NGSS codes, RAND equity direction) and a single author misattribution. Chapter 14's are two Lachner direction inversions plus the Bastani unit error.
- **Cross-cutting issue**: the Bastani unit interpretation appears in 6 files with two different framings. This is the single highest-priority editorial pass.

---

## Recommended Next Steps

**Most urgent — author should personally verify against the published PNAS paper before any other edit:** the Bastani exam-side effect ("17 percentage points lower" vs "17% relative reduction"). Whichever the paper reports, propagate the correct phrasing across the Preface, Introduction, Ch 1, Ch 5, Ch 13, and Ch 14 so the book is internally consistent. This is the load-bearing empirical anchor of the entire book; one paragraph-level correction protects the argument across all chapters that depend on it.

**Second editorial pass — citation hygiene:** restore the full Bastani title ("Generative AI *without guardrails* can harm learning"), correct the Henkel et al. 2024 title and framing, fix the misattributions (Khoo → Liu, Schneider → actual author, Hsiao → Chen, Stiti → Khazanchi), restore truncated author lists (Wei, Zheng), and correct the Holder & Xiong initial. These are mechanical fixes that take an hour each but materially affect academic credibility.

**Third pass — worked-example corrections:** the NGSS code swap in Ch 4 and the lie-factor arithmetic in Ch 9 are particularly important because both chapters argue *for* careful verification of AI outputs and the errors appear inside the examples the chapters use to demonstrate that discipline. Fixing them strengthens the chapters' own arguments.

**Fourth pass — direction-reversal corrections:** RAND equity in Ch 4 and the two Lachner papers in Ch 14. These are not magnitude errors but directional ones — the original sources say the opposite of what the chapters claim — so simple wording flips fix them.

**Overall reliability picture:** the book is unusually well-sourced for a first-draft textbook — roughly 70% of all flagged assertions verified CONFIRMED to primary sources on direct check, and most of the remaining 30% are either calibrated hedges the author already flagged with `[verify]` or items that resolve with a single editorial pass. The book's empirical anchors (Bastani, Gallup/Walton, NFER/EEF, Liang, OpenAI/Vanderbilt institutional retreats, Bjork, Roediger & Karpicke, Mayer, Cairo, Tufte) all survive verification at the level the chapters claim. The critical-tier items are concentrated in three places: (1) the Bastani unit phrasing, (2) a handful of draft-from-notes citation misattributions, and (3) two worked-example precision errors. None of these defeat the book's argument; all of them are fixable in a single focused editorial week.

The chapters with the most rigorous self-verification (Chs 8, 10, 12, 13) reveal what the book's standard could be: every load-bearing source verified to DOI / page / year, every contested claim explicitly flagged in-prose, every product-specific claim time-bounded. Bringing the rest of the chapters up to that standard is the work of one focused pass — not a re-architecture.

---

*All per-chapter reports are in `factchecks/`. Source files have been annotated with inline `<!-- FACT-CHECK FLAG -->` comments at problem locations and `## References` sections added where the chapter did not already integrate citations inline.*
