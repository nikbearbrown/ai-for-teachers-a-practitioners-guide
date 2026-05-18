# Assertions Report: 05-assessment-grading-and-feedback-with-ai.md
**Date:** 2026-05-18
**Source file:** chapters/05-assessment-grading-and-feedback-with-ai.md
**Assertions flagged:** 24
**Breakdown:** STAT: 8 | GUIDELINE: 2 | APPROVAL: 0 | EVIDENCE: 9 | SPECIALIST: 2 | CURRENT: 3

---

## ⚠️ Critical — Requires Immediate Expert Review

### C1. Bastani 2025 — "17 percentage points lower" (CONTRADICTED — unit error)
- **Type:** STAT / EMPHATIC
- **Location:** §4.1, "The GPT Base students scored 17 percentage points *lower* than the control."
- **Verdict:** CONTRADICTED.
- **Finding:** The published Bastani et al. PNAS paper reports a **17% relative reduction** in exam scores for the GPT Base group vs. control on the closed-book post-test — NOT 17 percentage points. The distinction matters: "17% lower than the control mean" is a relative effect; "17 percentage points lower" implies an absolute gap on a 0–100 scale and overstates the magnitude. Multiple authoritative summaries (Wharton Knowledge, PubMed abstract, the paper itself) describe this as "17% lower" or a "17% reduction."
- **Recommended fix:** Replace "17 percentage points *lower*" with "17% lower" (or "a 17% relative reduction").
- **Source:** [Bastani et al. 2025, PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122); [Correction DOI](https://www.pnas.org/doi/10.1073/pnas.2518204122).

### C2. "Schneider et al. 2022" attribution (CONTRADICTED — authorship error)
- **Type:** EVIDENCE / BASIC
- **Locations:** TL;DR (line 3); §2.3 (line 65).
- **Verdict:** CONTRADICTED.
- **Finding:** The DOI cited (10.1007/s40593-022-00322-1) resolves to "Reducing Workload in Short Answer Grading Using Machine Learning" by **Rebecka Weegar and Peter Idestam-Almquist**, published online 2022 / in print 2023 in the *International Journal of Artificial Intelligence in Education* (Springer). There is no "Schneider et al. 2022" at this DOI. The chapter consistently misattributes authorship.
- **Recommended fix:** Replace all instances of "Schneider et al. 2022" with "Weegar & Idestam-Almquist 2022" (or 2023, matching print year). The 64–74% reduction range comes from their results; the underlying paper supports the citation, only the author names are wrong.
- **Source:** [Weegar & Idestam-Almquist 2022, IJAIED](https://link.springer.com/article/10.1007/s40593-022-00322-1).

### C3. arXiv 2602.23580 — date/availability mismatch (UNVERIFIED at time of writing)
- **Type:** EVIDENCE
- **Location:** §3.3, the bracketed `[verify…]` note: "the citation in the research notes pointed to a paper I cannot fully confirm at this writing."
- **Verdict:** UNVERIFIED in the chapter as drafted, but the paper does exist. It is "BRIDGE the Gap: Mitigating Bias Amplification in Automated Scoring of English Language Learners via Inter-group Data Augmentation" (Wang et al.). arXiv lists the submission date as February 2026 — i.e., after the chapter's stated writing window for some earlier drafts. The bias-amplification finding it documents IS in the published preprint.
- **Recommended fix:** The chapter already brackets a verify-flag; if Nik wants to include this paper, swap the inline citation to arXiv 2602.23580 and remove the disclaimer, or keep the disclaimer if Nik prefers to wait for peer review.
- **Source:** [arXiv:2602.23580](https://arxiv.org/abs/2602.23580).

---

## Full Findings

### 1. TL;DR — "50–80% range for time saved"
- **Type:** STAT / BASIC
- **Verdict:** CONFIRMED (with caveats). The 64–74% peer-reviewed anchor is correct (Weegar & Idestam-Almquist, see C2). Vendor and individual-teacher claims cluster higher (75–85%). The 50–80% framing is a reasonable synthesis. Author attribution must be fixed (see C2).
- **Source:** [Weegar & Idestam-Almquist 2022](https://link.springer.com/article/10.1007/s40593-022-00322-1).

### 2. TL;DR — Gallup-Walton "5.9-hour weekly AI dividend"
- **Type:** STAT
- **Verdict:** CONFIRMED. Gallup-Walton 2025 report states teachers using AI weekly save an average of 5.9 hours per week. Sample: 2,232 U.S. K-12 public teachers (March 18 – April 11, 2025).
- **Source:** [Walton Family Foundation / Gallup 2025](https://www.waltonfamilyfoundation.org/the-ai-dividend-new-survey-shows-ai-is-helping-teachers-reclaim-valuable-time).

### 3. §2.2 — Steiss et al. 2024 finding
- **Type:** EVIDENCE / BASIC
- **Verdict:** CONFIRMED. Article DOI 10.1016/j.learninstruc.2024.101894, *Learning and Instruction* vol. 91, article 101894. Authors: Steiss, Tate, Graham, et al. The five-criterion comparison and the finding (ChatGPT matches on criteria-based; humans win on accuracy, prioritization, clarity, supportive tone) match the paper.
- **Source:** [Steiss et al. 2024, ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0959475224000215).

### 4. §2.2 — Henkel et al. 2024 (arXiv 2405.02985)
- **Type:** EVIDENCE / STAT
- **Verdict:** CONFIRMED. Title: "Can Large Language Models Make the Grade? An Empirical Study Evaluating LLMs Ability to Mark Short Answer Questions in K-12 Education." Authors: Henkel, Boxer, Hills, Roberts. Carousel platform, K-12 science/history, ages 5–16, GPT-4 few-shot kappa ~0.70 vs. human-human ~0.75. All confirmed.
- **Source:** [Henkel et al. 2024, arXiv](https://arxiv.org/abs/2405.02985).

### 5. §2.2 — Hewlett ASAP-AES 2012 Kaggle competition
- **Type:** EVIDENCE / BASIC
- **Verdict:** CONFIRMED. Hewlett Foundation sponsored the Automated Student Assessment Prize on Kaggle in 2012; $100K prize pool; quadratic-weighted kappa as agreement metric.
- **Source:** [Kaggle ASAP-AES](https://www.kaggle.com/competitions/asap-aes); [Hewlett Foundation announcement](https://hewlett.org/newsroom/hewlett-foundation-sponsors-prize-to-improve-automated-scoring-of-student-essays/).

### 6. §2.2 — Attali & Burstein 2007 ETS e-rater
- **Type:** EVIDENCE / BASIC
- **Verdict:** CONFIRMED. "Construct Validity of e-rater® in Scoring TOEFL® Essays," ETS Research Report 2007. Reports human-machine correlation approximating inter-human-rater correlation on TOEFL essays.
- **Caveat:** The chapter's ERIC URL (EJ843852) points to a 2006 piece in *Journal of Technology, Learning, and Assessment* (vol. 4 no. 3), which is a different (slightly earlier) Attali & Burstein paper on e-rater V.2. Both papers exist; if Nik wants the 2007 TOEFL-specific paper, the canonical citation is the ETS Research Report Series (DOI 10.1002/j.2333-8504.2007.tb02063.x). The current ERIC link supports the broader e-rater claim but is for the 2006 paper.
- **Recommended fix:** Either change year to 2006 to match the ERIC URL, or update URL to the Wiley ETS Research Report.
- **Sources:** [Attali & Burstein 2007 ETS RR](https://onlinelibrary.wiley.com/doi/abs/10.1002/j.2333-8504.2007.tb02063.x); [Attali & Burstein 2006 JTLA](https://files.eric.ed.gov/fulltext/EJ843852.pdf).

### 7. §2.3 — EssayGrader "80%" vendor claim
- **Type:** CURRENT / EMPHATIC
- **Verdict:** UNVERIFIED. The chapter cites no link for the EssayGrader claim. As a vendor marketing figure it is a reasonable to flag for editorial review; not a finding.
- **Recommended fix:** Either add an inline citation to the vendor page or rephrase as "vendor pages report figures up to 85%."

### 8. §2.4 — EU AI Act Annex III point 3 classification
- **Type:** GUIDELINE / BASIC
- **Verdict:** CONFIRMED. The EU AI Act (Regulation 2024/1689), Annex III point 3, classifies AI systems for educational and vocational training as high-risk — including (3.b) systems used "to evaluate learning outcomes." Documentation, oversight, transparency requirements apply.
- **Caveat:** The chapter URL (`artificialintelligenceact.eu/the-act/`) is an unofficial mirror; the official text is on EUR-Lex. Either link is acceptable but EUR-Lex is more authoritative for a high-stakes regulatory citation.
- **Source:** [EUR-Lex Regulation 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj); current mirror: [artificialintelligenceact.eu](https://artificialintelligenceact.eu/the-act/).

### 9. §2.4 — "teacher of record" U.S. statutes
- **Type:** GUIDELINE
- **Verdict:** UNVERIFIED but defensible. The chapter says "teacher of record" statutes "vary by state but generally locate summative grade authority with the licensed educator." This is broadly consistent with state education codes (e.g., Texas Education Code Chapter 21; Florida statutes assigning final grade authority to instructors of record). The chapter does not cite specific statutes — appropriate for a textbook-level claim but should be flagged for review by an education-law specialist if exactness matters.
- **Recommended fix:** Add a representative state citation or soften ("in U.S. K-12 and higher-ed practice, the licensed educator is generally treated as the assessor of record").

### 10. §3.1 — Landis & Koch 1977 κ thresholds
- **Type:** STAT / EVIDENCE
- **Verdict:** CONFIRMED. "The Measurement of Observer Agreement for Categorical Data," *Biometrics* 33: 159–174 (1977). Canonical thresholds: 0.61–0.80 substantial; 0.81–1.00 almost perfect. Chapter restatement is accurate.
- **Source:** [Landis & Koch 1977, JSTOR](https://www.jstor.org/stable/2529310).

### 11. §3.1 — Krippendorff's α ≥ 0.80 cutoff
- **Type:** STAT
- **Verdict:** CONFIRMED. Krippendorff's conventional rule of thumb is α ≥ 0.80 for usable data; α ≥ 0.667 for tentative conclusions. Widely cited (Krippendorff, *Content Analysis*, 2004; 2018 edition).
- **Recommended fix:** Consider adding an inline link to Krippendorff source if the claim is load-bearing.

### 12. §4.1 — "about a thousand Turkish high school students"
- **Type:** STAT / BASIC
- **Verdict:** CONFIRMED. The PNAS paper states "nearly 1,000" high school students in Turkey.
- **Source:** [Bastani et al. 2025, PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122).

### 13. §4.1 — "GPT Base condition outscored the no-AI control by 48%" during practice
- **Type:** STAT / EMPHATIC
- **Verdict:** CONFIRMED. Wharton/PNAS abstract: 48% performance improvement during practice for GPT Base, 127% for GPT Tutor. Chapter cites only the GPT Base 48%.
- **Source:** [Bastani et al. 2025, PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122).

### 14. §4.1 — "GPT Tutor … closed most but not all of that gap"
- **Type:** STAT
- **Verdict:** CONFIRMED with nuance. The PNAS paper shows GPT Tutor closed most of the post-test gap relative to GPT Base; in some specifications, GPT Tutor students performed statistically indistinguishably from control on the closed-book exam. "Most but not all" is a defensible reading; some summaries describe it as "no statistically significant difference." Either framing is supportable.
- **Source:** [Bastani et al. 2025, PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122).

### 15. §7.2 — Steiss reiteration
- **Type:** EVIDENCE
- **Verdict:** CONFIRMED. Same paper as §2.2.

### 16. §7.4 — ELL/ESL bias claim (high-proficiency essays underscored)
- **Type:** EVIDENCE / SPECIALIST
- **Verdict:** CONFIRMED (mixed literature; chapter handles it carefully). Multiple papers document that AES systems and human raters both underscore high-proficiency ELL essays relative to native-speaker essays of equivalent rated quality. One recent quantification: a 10.3% under-scoring gap (cited in arXiv 2601.16724). The chapter's framing — "sometimes reproduces and sometimes amplifies" — is consistent with the active literature.
- **Sources:** [arXiv 2505.10643](https://arxiv.org/abs/2505.10643); [arXiv 2602.23580 BRIDGE](https://arxiv.org/abs/2602.23580); [Loukina et al., automated scoring fairness literature].

### 17. §3.3 — Loukina ETS Research Reports link
- **Type:** EVIDENCE / SPECIALIST
- **Verdict:** UNVERIFIED. The ERIC URL provided (`EJ1233920`) is referenced as "Loukina et al. on bias in automated scoring, ETS Research Reports." The ID format is ERIC; the connection to a specific Loukina ETS paper should be re-verified. The body of Loukina work on fairness in AES is real and authoritative (Loukina, Madnani, Zechner — multiple ETS publications between 2017 and 2022), but the specific ERIC ID needs confirmation.
- **Recommended fix:** Verify the ERIC ID resolves to the intended Loukina paper, or substitute a confirmed citation (e.g., Loukina et al. 2019 ACL paper "The many dimensions of algorithmic fairness in educational applications").

### 18. §1 — "90-to-22-hour arithmetic"
- **Type:** STAT / I-LANGUAGE (composite/illustrative)
- **Verdict:** CONFIRMED as labeled. The chapter explicitly flags this as composite-illustrative. Acceptable under the workshop's hard rule #1 because it is named as a constructed case.

### 19. §1 — "Professor Daniels"
- **Type:** BASIC / I-LANGUAGE (composite)
- **Verdict:** CONFIRMED as labeled (composite character).

### 20. §5 — Worked example numbers (110 responses, 80 minutes, 5% override rate)
- **Type:** STAT
- **Verdict:** CONFIRMED as labeled — chapter says "Numbers are illustrative; the prompt structure is the real artifact." Acceptable under the workshop's transparency norms.

### 21. §7.3 — "calibration drift across model versions"
- **Type:** CURRENT
- **Verdict:** UNVERIFIED. The claim that the same prompt may score differently on GPT-4 vs GPT-4o is plausible and matches anecdotal practitioner reports, but is not anchored to a published study in the chapter. Chapter labels it as "a real hazard" — flag for "no peer-reviewed RCT" status.
- **Recommended fix:** Either add a citation (e.g., a model-eval consistency paper) or soften phrasing to acknowledge it as practitioner observation.

### 22. §7.1 — "no license, no employer, and no relationship with the student"
- **Type:** GUIDELINE / EMPHATIC
- **Verdict:** CONFIRMED as a normative statement; no factual claim under test.

### 23. §10 — "No standard exists for re-calibrating prompts when underlying models update"
- **Type:** CURRENT
- **Verdict:** UNVERIFIED but reasonable. As of the chapter's writing date there is no widely-adopted industry standard for prompt-version calibration drift detection; chapter handles this honestly under "Still puzzling."

### 24. §4.2 — "no such trial has been published" (for AI feedback with/without teacher review RCT)
- **Type:** CURRENT / EMPHATIC
- **Verdict:** CONFIRMED to best knowledge as of May 2026. No peer-reviewed three-arm RCT comparing teacher-written / AI-with-teacher-review / AI-no-review feedback on student learning outcomes has been published. Chapter handles uncertainty appropriately.

---

## Unverified Assertions

- EssayGrader vendor "80%" claim (no link in chapter).
- Specific Loukina ERIC ID resolution.
- "Calibration drift across model versions" (practitioner-known, not peer-reviewed).
- The "teacher of record" statutory framing (no state code cited).

---

## AI-Pass Flags

None of the assertions trigger a generic-AI-generated voice flag. The chapter consistently uses first-person reasoning, hedges, and labels composite material. Three specific verb choices ("The data shows" was used once in the original chapter draft) — but the chapter mostly avoids the forbidden phrase list from CLAUDE.md §6.

---

## Reliability Assessment

The chapter is **substantially reliable** but has **two unit/attribution errors that should be fixed before publication**: the "17 percentage points" unit error on Bastani (this is a meaningful overstatement of effect size and the most important fix in the chapter) and the "Schneider et al. 2022" misattribution (the underlying Springer paper is real but the author names are wrong). Beyond those, the chapter's handling of effect sizes, uncertainty, and the ELL bias literature is unusually careful; most other flagged items are minor.

---

*Generated 2026-05-18.*
