# Assertions Report: 13-academic-integrity-privacy-and-honest-use.md
**Date:** 2026-05-18
**Source file:** chapters/13-academic-integrity-privacy-and-honest-use.md
**Assertions flagged:** 26
**Breakdown:** STAT: 11 | GUIDELINE: 4 | APPROVAL: 3 | EVIDENCE: 5 | SPECIALIST: 1 | CURRENT: 2

---

## ⚠️ Critical — Requires Immediate Expert Review

### C1. Bastani 2025 "17 percentage points" framing — CONFIRMED but verify chapter is consistent
**Type:** STAT / EVIDENCE
**Verdict:** CONFIRMED
**Where:** Line 11 (objectives), Line 62 ("17 percentage points lower"), Line 69 (precision note), Line 71, Line 123, Line 280.
The chapter consistently uses "17 percentage points" (not "17%" or "17-point") for the unguarded-condition exam decrement, and explicitly flags the distinction in §3.1: "the harm is 17 percentage points, not 17 percent." Bastani et al. (2025, PNAS) report the unguarded GPT condition produced an absolute decrement of ~17 percentage points on the post-test relative to control. This is the most-load-bearing claim in the chapter and the chapter handles it carefully. **No CONTRADICTED finding.** Note: PNAS summaries sometimes describe the decrement as a "17% relative reduction" — the chapter's language matches the absolute-points reading consistent with the paper's design.
**Source:** [PNAS 122(26), Bastani et al. 2025](https://www.pnas.org/doi/10.1073/pnas.2422633122).

### C2. Weber-Wulff "twelve tools" — MINOR CONTRADICTION (chapter undercounts)
**Type:** EVIDENCE / STAT
**Verdict:** CONTRADICTED (mild)
**Where:** Line 85: "Weber-Wulff et al. (2023)... tested twelve detection tools across 54 cases (756 total tests, March–May 2023)..."
The paper tested **fourteen** detection systems total — twelve free "AI checkers" plus two subscription/commercial systems (Turnitin and PlagiarismCheck). The chapter's "twelve" is the free-tool subset, not the full count cited in the abstract and used in the load-bearing claim. The 54-case / 756-test arithmetic checks out (54 × 14 = 756, consistent with the full-tool count). The chapter likely should say "fourteen" or "twelve free plus two subscription." **Recommend changing to "fourteen" to match the paper's headline framing.**
**Source:** [Weber-Wulff et al. IJEI 2023](https://link.springer.com/article/10.1007/s40979-023-00146-z); [arXiv 2306.15666](https://arxiv.org/abs/2306.15666).

---

## Full Findings

### F1. Bastani 2025 — three-arm field experiment in Turkish high school
**Type:** EVIDENCE / STAT
**Verdict:** CONFIRMED
**Where:** Line 53.
"Turkish high school across grades 9–11, approximately 1,000 students, multi-week math curriculum, random assignment to one of three conditions" — matches the published PNAS report. Three conditions (no-AI control, GPT Base, GPT Tutor) confirmed. Authors listed correctly (Bastani, Bastani, Sungu, Ge, Kabakcı, Mariman). DOI 10.1073/pnas.2422633122 correct.
**Source:** [PNAS 122(26)](https://www.pnas.org/doi/10.1073/pnas.2422633122); [SSRN preprint](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4895486).

### F2. Bastani 2025 — 48% practice gain (GPT Base) and 127% practice gain (GPT Tutor)
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Lines 58–59, 71, 123.
Multiple independent summaries (Wharton Knowledge, Bloom AI, secondary write-ups) report these exact figures (48% / 127%) as the practice-condition gains over no-AI control. Consistent with paper.

### F3. Bastani 2025 — August 2025 correction is affiliation-only
**Type:** EVIDENCE
**Verdict:** CONFIRMED
**Where:** Line 53, Line 303.
The August 20, 2025 correction (DOI 10.1073/pnas.2518204122) updates the affiliation listing for Osbert Bastani (University of Pennsylvania, Dept of Computer and Information Science) — no change to substantive numbers or design. Chapter's "pantry cross-check" note is accurate.
**Source:** [PMC12403119 correction notice](https://pmc.ncbi.nlm.nih.gov/articles/PMC12403119/).

### F4. Liang 2023 — Cell Press *Patterns* journal, seven GPT detectors
**Type:** EVIDENCE
**Verdict:** CONFIRMED
**Where:** Line 87.
Liang, Yuksekgonul, Mao, Wu, Zou (2023), *Patterns* 4(7), 100779. DOI 10.1016/j.patter.2023.100779. Seven GPT detectors evaluated. All correct.

### F5. Liang 2023 — ">50% TOEFL essays misclassified as AI-generated"
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Line 87, Line 222, Line 271.
Paper reports an average false-positive rate of **61.3%** across the seven detectors on 91 TOEFL essays. The chapter's "more than 50%" is a defensibly conservative restatement. (Some popular summaries say "up to 76%" — referring to the worst-performing single detector. The chapter's "more than 50%" matches the average. Recommend leaving as is.)

### F6. Liang 2023 — near-perfect accuracy on 8th-grade essays
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Line 87.
Paper reports detectors classified U.S. 8th-grade essays "near perfectly" (very low false-positive rate). Confirmed.

### F7. Liang 2023 — perplexity mechanism explanation
**Type:** SPECIALIST
**Verdict:** CONFIRMED
**Where:** Lines 89–90.
Mechanism description (detectors flag low-perplexity text; LLMs produce low-perplexity by construction; non-native writers also produce predictable text) matches the paper's hypothesis and supporting analysis.

### F8. OpenAI AI Text Classifier — launched Jan 31, 2023, withdrawn July 20, 2023
**Type:** CURRENT / APPROVAL
**Verdict:** CONFIRMED
**Where:** Line 85.
Both dates confirmed. The classifier was launched January 31, 2023 and withdrawn around July 20, 2023 (some sources say July 25; OpenAI's own blog updated July 20).

### F9. OpenAI classifier accuracy figures — 26% true-positive, ~9% false-positive
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Line 85, Line 222.
OpenAI publicly stated the classifier had **26% sensitivity** (correctly identified AI-written text 26% of the time) and **91% specificity** (correctly identified human-written text 91% of the time — implying ~9% false-positive on human text). Both figures confirmed via multiple independent reports and OpenAI's own announcement.

### F10. Vanderbilt — disabled Turnitin AI detector August 16, 2023
**Type:** CURRENT / APPROVAL
**Verdict:** CONFIRMED
**Where:** Line 93, Line 222.
Date confirmed via Vanderbilt Brightspace announcement (August 16, 2023). URL correct.

### F11. Vanderbilt arithmetic — 75,000 papers / 2022 / 1% / 750 students
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Line 93, Line 222.
Vanderbilt's published statement explicitly states: "We submitted 75,000 papers in 2022... a 1% false positive rate... approximately 750 student papers." Arithmetic verbatim.

### F12. Louise Stivers — UC Davis political science major, Turnitin flagged
**Type:** EVIDENCE / CURRENT
**Verdict:** CONFIRMED
**Where:** Line 95.
Confirmed via Rolling Stone (June 2023). She is a political science major at UC Davis; her Supreme Court case brief was flagged by Turnitin as partially AI-generated; she was referred to the Office of Student Support and Judicial Affairs and eventually cleared.

### F13. William Quarterman — UC Davis history major, GPTZero, failing grade
**Type:** EVIDENCE / CURRENT
**Verdict:** CONFIRMED
**Where:** Line 95.
Confirmed via multiple sources including USA Today and Washington Post reporting. Quarterman, history major at UC Davis, had a midterm flagged by GPTZero; received a failing grade and was referred; case dropped March 24 (2023). Demonstrated GPTZero's unreliability by showing it flagged MLK's "I Have a Dream" as AI-written.

### F14. FERPA citation — 20 U.S.C. § 1232g
**Type:** GUIDELINE
**Verdict:** CONFIRMED
**Where:** Line 131.
Statutory citation correct.

### F15. FERPA school-official exception — 34 CFR § 99.31(a)(1)(i)(B)
**Type:** GUIDELINE
**Verdict:** CONFIRMED
**Where:** Line 135.
Regulatory citation correct; characterization of the "direct control" requirement for external vendors is accurate to the regulation text.

### F16. COPPA citation — 15 U.S.C. § 6501–6506
**Type:** GUIDELINE
**Verdict:** CONFIRMED
**Where:** Line 139.
Statutory citation correct (COPPA spans 15 U.S.C. §§ 6501–6506).

### F17. COPPA Final Rule — finalized April 2025, effective June 23, 2025
**Type:** CURRENT / GUIDELINE
**Verdict:** CONFIRMED
**Where:** Line 139.
The FTC published the final amendments in the Federal Register on April 22, 2025, with an effective date of June 23, 2025. The FTC's initial announcement of the finalized rule was January 16, 2025 (under Chair Khan), but the official Federal Register publication date is April 22, 2025. Chapter's "April 2025" matches publication; "June 23, 2025" effective date correct.
**Source:** [Federal Register 90 FR 16936](https://www.federalregister.gov/documents/2025/04/22/2025-05904/childrens-online-privacy-protection-rule).

### F18. COPPA Final Rule — algorithm-training data retention restriction
**Type:** GUIDELINE
**Verdict:** CONFIRMED
**Where:** Line 139.
Confirmed: the final rule explicitly addresses children's personal information used for algorithm training, requiring that operators may not retain such information indefinitely even when claimed as necessary for algorithm improvement. Chapter's characterization is accurate.

### F19. US DOE OET 2023 report — "Artificial Intelligence and the Future of Teaching and Learning," May 2023
**Type:** GUIDELINE / APPROVAL
**Verdict:** CONFIRMED
**Where:** Line 137.
Report exists, was published May 2023 by the Office of Educational Technology, contains the "human-in-the-loop" framing. URL ed.gov/sites/ed/files/documents/ai-report/ai-report.pdf is correct.

### F20. DOE 2025 FERPA FAQ update / 2026 AI-specific FERPA publication
**Type:** GUIDELINE / CURRENT
**Verdict:** UNVERIFIED
**Where:** Line 137.
"The Department's 2025 FERPA FAQ refresh updated 37 questions, and a 2026 AI-specific FERPA publication is in preparation [verify on publication]" — the chapter already flags this as [verify on publication]. I cannot independently confirm the "37 questions" figure or the 2026 publication. Recommend leaving the inline [verify] flag.

### F21. Pew Research January 2025 — 26% of US teens use ChatGPT for schoolwork, doubled from 13%
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Line 145, Line 226.
Pew Research short-read published January 15, 2025. 26% in 2024 survey, up from 13% in 2023. Survey of 1,391 U.S. teens ages 13–17, conducted Sept 18 – Oct 10, 2024.

### F22. Pew January 2025 — racial cross-tabs (Black/Hispanic 31%, White 22%)
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Line 145, Line 226.
Pew explicitly reports Black teens 31%, Hispanic teens 31%, White teens 22% for ChatGPT-for-schoolwork. Confirmed.

### F23. Pew January 2025 — income cross-tabs (higher-income use higher than lower-income)
**Type:** STAT
**Verdict:** PARTIALLY CONFIRMED / IMPRECISE
**Where:** Line 145, Line 226.
The chapter says "higher-income families show higher rates than lower-income families." Pew data shows higher-income teens are more *aware* of ChatGPT (84% vs 67%) and more likely to *use* it overall (62% vs 52%), but the January 2025 Pew short-read on schoolwork use does not break out schoolwork-specific use by income as cleanly as it does race. The directional claim is supported but the specific framing risks slight overstatement. **Recommend the chapter add a note that income shapes ChatGPT awareness/access more than schoolwork-specific use in the Pew Jan 2025 break-out.** Mild flag — directional claim stands.

### F24. Pew January 2025 — acceptance norms (54% research, 29% math, 18% essays)
**Type:** STAT
**Verdict:** CONFIRMED
**Where:** Line 145.
Pew confirms 54% (research), 29% (math), 18% (essays) as the acceptance figures from the same survey.

### F25. TeachAI policy tracker — at least 28 US states had K-12 AI guidance by April 2025
**Type:** GUIDELINE / STAT
**Verdict:** CONFIRMED
**Where:** Line 141.
TeachAI policy tracker and Education Commission of the States reporting both indicate that by April 2025 at least 28 U.S. states had published K-12 AI guidance. (By late 2025, the count rose further.) URL teachai.org/policy-tracker correct.

### F26. Bjork & Bjork 1992 — storage strength vs retrieval strength framework
**Type:** EVIDENCE
**Verdict:** CONFIRMED
**Where:** Line 75.
Robert and Elizabeth Bjork's "new theory of disuse" distinguishing storage strength from retrieval strength is from Bjork, R. A., & Bjork, E. L. (1992). The chapter places this correctly as the cognitive-psychology backbone for the performance paradox. Note: chapter cites "Appendix G" — that appendix's existence and content is not verified here.

---

## Unverified Assertions

- **U1.** "DOE 2025 FERPA FAQ refresh updated 37 questions" (Line 137). Already flagged with [verify on publication] in the chapter — leave as is.
- **U2.** "A 2026 AI-specific FERPA publication is in preparation" (Line 137). Already flagged [verify].
- **U3.** "Medhavy GLP framework formalizes seven of these signals" (Line 115). Cannot independently verify the existence or content of the "Medhavy GLP framework." Recommend Nik verify or remove the reference.
- **U4.** Opening case (§2) is composite-illustrative and explicitly labeled as such — not a fact-check target. The 23% referral rate / four-week appeals window are illustrative figures, not factual claims about a real institution. The labeling at Line 29 is appropriate.
- **U5.** "Vanderbilt has had an honor code since 1875" (Line 230). Plausible and historically reasonable; not independently verified here. Recommend low-priority verification.
- **U6.** "Frictional appendix" reference (Line 212) — internal cross-reference, not externally verifiable.
- **U7.** "Appendix C" (the checklist), "Appendix G" (Bjork framework) — internal cross-references, not externally verifiable.
- **U8.** "The Trust Teacher framing applied to phone-ban policies" (Line 147) — internal cross-reference to another chapter, not verified here.

---

## AI-Pass Flags

- **AI-P1.** Line 53 mentions "pantry cross-check" — this is an internal workshop term (pantry = research notes), not a public source. Reader-facing phrasing might read awkward; consider rephrasing for the published edition.
- **AI-P2.** Line 85: chapter says "twelve detection tools" for Weber-Wulff. The paper tested fourteen total (twelve free + two subscription). See C2. **Recommend edit.**
- **AI-P3.** Line 145: the income-cross-tab framing could be tightened — Pew's January 2025 short-read foregrounds race/ethnicity and grade level more cleanly than income for schoolwork-specific use. See F23.
- **AI-P4.** Line 115: "Medhavy GLP framework" — unverified term. Nik should confirm or remove.
- **AI-P5.** Line 222 references "a wave of other universities have followed since" — directionally accurate (multiple universities have publicly distanced themselves from Turnitin AI detection or moved to design-first approaches), but no specific list cited. Defensible as a summary statement.
- **AI-P6.** The "Stivers, Quarterman" pair are real, well-documented cases — the URLs cited (Rolling Stone, NMLLP, NBC News) check out.
- **AI-P7.** Chapter handles the "17 percentage points vs 17 percent" distinction explicitly (Line 69) — exemplary precision; no action needed.

---

## Reliability Assessment

This chapter is **unusually high-quality** on factual fidelity for the load-bearing material. The Bastani 2025 treatment is rigorous, including the explicit "percentage points, not percent" precision move (Line 69), correct identification of the August 2025 correction as affiliation-only, and honest acknowledgment that this is one study. The Liang 2023, Weber-Wulff 2023, OpenAI withdrawal, and Vanderbilt arithmetic all verify cleanly. Two minor issues warrant edits: (a) Weber-Wulff tested **fourteen** detection tools (12 free + 2 subscription), not twelve as the chapter states — the paper's headline number is 14, and the 756-test arithmetic in the chapter actually requires 14 tools (54 × 14 = 756); (b) the Pew income cross-tab framing on Line 145 is directionally correct but somewhat imprecise about what the January 2025 short-read actually broke out for schoolwork use specifically. Recommend Nik review C2 (Weber-Wulff "twelve" → "fourteen") before publication. Everything else stands.
