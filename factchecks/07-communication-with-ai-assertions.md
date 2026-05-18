# Assertions Report: 07-communication-with-ai.md
**Date:** 2026-05-18
**Source file:** chapters/07-communication-with-ai.md
**Assertions flagged:** 21
**Breakdown:** STAT: 4 | GUIDELINE: 5 | APPROVAL: 3 | EVIDENCE: 5 | SPECIALIST: 2 | CURRENT: 2

**Verdict counts:** CONFIRMED: 16 | CONTRADICTED: 0 | UNVERIFIED: 4 | OUTDATED: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

No critical CONTRADICTED items in this chapter. The chapter is unusually well-cited; nearly all load-bearing claims trace cleanly to their primary sources. The only items that warrant reviewer attention are:

1. **The 600-comments / 72-to-16-hour arithmetic in §1** is already labeled by the chapter as *composite-illustrative* and *not measured for any specific teacher* (line 21). This is an honest disclosure; no fix needed, but reviewers should confirm the chapter's hedging holds across the case-study prose.
2. **The 50% / 2.5-hour weekly reduction** referenced in §1 is also pre-flagged in the chapter as not independently validated. This matches the brief's load-bearing-claim #7 and is appropriately scoped.
3. **The Tenzer 2024 defamation citation** verifies as a real article — but the chapter's framing ("publisher-liability principle ... extends, in the controlling reading") is stronger than the case law currently supports. The chapter does flag this as `[contested]` with "defamation case law for AI-drafted communications is actively developing." Reviewer should confirm the hedging is sufficient. See E5 below.

---

## Full Findings

### EVIDENCE category

**E1. Line 21, 87 — EdWeek 2025 IEP-AI adoption report and CDT 60% / 18-point figure**
- Claim: "A 2025 industry survey reported nearly 60% of special-education teachers used AI to develop an IEP or Section 504 plan during 2024–25, up 18 points from the previous year — 15% drafting in full, 31% identifying progress trends, 30% summarizing existing plans."
- Type: POSITIVE (precise numbers attached to a named outlet)
- **Verdict:** CONFIRMED (with one minor adjustment).
- **Finding:** The EdWeek piece reports the Center for Democracy and Technology (CDT) survey: 57% of special-education teachers used AI for IEPs or 504 plans in 2024–25 (up from 39% in 2023–24, an 18-point increase). The chapter rounds "57%" to "nearly 60%," which is fair. CDT's breakdown: 31% identify progress trends; 30% summarize IEPs/504s; 28% choose accommodations; 15% draft IEPs in full (up from 8%). All three sub-numbers the chapter cites match the source.
- Source: [EdWeek 2025](https://www.edweek.org/teaching-learning/teachers-are-using-ai-to-help-write-ieps-advocates-have-concerns/2025/10); [OPEN MINDS summary](https://openminds.com/market-intelligence/news/57-of-licensed-special-education-teachers-reported-using-ai-to-help-with-individual-education-plans-during-the-2024-2025-school-year/); [Disability Scoop coverage](https://www.disabilityscoop.com/2025/11/18/concerns-raised-as-teachers-increasingly-use-ai-to-write-ieps/31742/)
- Note: Minor possible refinement — replace "nearly 60%" with "57%" to be precise. The chapter's current phrasing is defensible but slightly inflates by ~3 pts.

**E2. Line 87 — K-12 Dive on advocate concerns**
- Claim: "Advocate concerns track the same fault line: AI-drafted plans built on thin student input may fail IDEA's individualization requirement."
- Type: POSITIVE (institutional/advocacy claim)
- **Verdict:** CONFIRMED. K-12 Dive's piece on heightened AI use in special education frames the same individualization-risk concern, attributing it to advocate sources.
- Source: [K-12 Dive 2025](https://www.k12dive.com/news/artificial-intelligence-special-education-Section-504-benefits-risks-privacy-IDEA-IEP/804535/)

**E3. Line 67 — Castro Ponce et al. 2022, Google Translate ~75% accuracy for Spanish ELL family communication**
- Claim: "A peer-reviewed evaluation of Google Translate for English-to-Spanish teacher-to-parent email communication with Latino ELL families rated translations at roughly 75% accuracy, with documented errors in literal translation, register, and punctuation — while overall meaning was usually preserved."
- Type: POSITIVE (precise stat with named source)
- **Verdict:** CONFIRMED. The study — Castro-Ponce et al., "Communicating with Parents of Latino English Language Learners: Is Google Translate an Accurate Option?," *Journal of Latinos and Education* 23(1), 2022 (online 2022, in print 2024) — does report ~75% accuracy, with documented errors in literal translation, inconsistent register/formality, and overuse of punctuation; evaluators noted strong overall meaning preservation. The chapter's characterization is faithful.
- Source: [Castro-Ponce et al. 2022, *Journal of Latinos and Education*](https://www.tandfonline.com/doi/abs/10.1080/15348431.2022.2104849); [ResearchGate](https://www.researchgate.net/publication/362270606_Communicating_with_Parents_of_Latino_English_Language_Learners_Is_Google_Translate_an_Accurate_Option)
- Note: The hyphenated form "Castro-Ponce" is the author's standard byline; the chapter prints "Castro Ponce" (no hyphen). Cosmetic.

**E4. Line 113, 334 — Mapp & Kuttner 2013 Dual Capacity-Building Framework (SEDL / US Dept of Ed)**
- Claim: "The U.S. Department of Education's Dual Capacity-Building Framework for Family–School Partnerships (Mapp & Kuttner 2013) treats family-school communication not as information transmission but as relationship infrastructure — trustful relationships are a process condition for effective partnership."
- Type: POSITIVE (named authority, named framing)
- **Verdict:** CONFIRMED. The framework was authored by Karen Mapp with support from Paul Kuttner and published in 2013 by SEDL in association with the US Department of Education. "Process conditions" — including trust — are explicit components of the framework. Version 2.0 was released in 2019; the chapter's invocation of the 2013 origin is correct.
- Source: [SEDL DualCapacityFramework PDF](https://sedl.org/pubs/framework/DualCapacityFramework.pdf); [ed.gov hosted PDF (cited in chapter)](https://www.ed.gov/media/document/41-dual-capacity-building-framework-family-school-partnerships-109231.pdf); [ERIC ED593896](https://eric.ed.gov/?id=ED593896)

**E5. Line 107, 192 — Tenzer 2024 publisher-liability argument extending to AI-drafted content**
- Claim: "The publisher-liability principle in U.S. defamation doctrine — the party who publishes a defamatory statement is the responsible party, regardless of who composed the underlying text — extends, in the controlling reading, to AI-drafted content the user signs and sends (Tenzer 2024)."
- Type: POSITIVE (named doctrine + named legal authority)
- **Verdict:** CONFIRMED that the article exists and that Tenzer argues this position. **UNVERIFIED-by-overstatement** that "the controlling reading" extends publisher liability to AI-drafted content the user signs. Tenzer's article ("Defamation in the Age of Artificial Intelligence," 80 *N.Y.U. Annual Survey of American Law* 135, 2024) discusses liability across stakeholders in AI generation/deployment but is academic legal commentary, not controlling precedent. The chapter does flag this with `[contested]` and notes that "defamation case law for AI-drafted communications is actively developing; specific outcomes in the school-records context are not yet settled."
- Source: [Tenzer 2024, NYU Annual Survey](https://annualsurveyofamericanlaw.org/wp-content/uploads/2024/09/02_NYS_80_2_Tenzer.pdf); [Pace Digital Commons](https://digitalcommons.pace.edu/lawfaculty/1280/); [SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4545070)
- Note: Reviewer may wish to soften "in the controlling reading" to "Tenzer argues" — the publisher-liability principle itself is settled common law, but its extension to AI-drafted content is the contestable point.

### GUIDELINE category

**G1. Line 113, 334 — Kraft & Rogers 2015 field experiment on teacher-to-parent communication**
- Claim: "Kraft & Rogers (2015) showed in a field experiment that brief positive teacher-to-parent messages produce measurable changes in student behavior."
- Type: POSITIVE (named study + empirical claim)
- **Verdict:** CONFIRMED (with one caveat).
- **Finding:** Kraft, M.A. & Rogers, T. (2015). "The Underutilized Potential of Teacher-to-Parent Communication: Evidence from a Field Experiment," *Economics of Education Review* 47, 49–63. The 5-week intervention used brief individualized weekly teacher-to-parent messages in a high school credit-recovery program; failure-to-earn-credit dropped from 15.8% to 9.3% (a 41% reduction), driven largely by reducing dropouts. **Important nuance:** the largest effects came from messages emphasizing what students could improve, not purely positive messages. The chapter's wording — "brief positive teacher-to-parent messages produce measurable changes in student behavior" — is accurate in direction but slightly oversimplified. Kraft & Rogers themselves note improvement-oriented messages outperformed purely positive ones.
- Source: [Kraft & Rogers 2015 (Harvard Scholar PDF, cited in chapter)](https://scholar.harvard.edu/files/todd_rogers/files/empirical_in_press.kraft_rogers.pdf); [Annenberg Brown](https://annenberg.brown.edu/publications/underutilized-potential-teacher-parent-communication-evidence-field-experiment); [ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S0272775715000497)
- Recommendation: Optional refinement — "brief individualized teacher-to-parent messages, especially those emphasizing areas to improve, produce measurable changes in student outcomes (dropout reduction in the original study)."

**G2. Line 115 — Hattie *Visible Learning* teacher-student-relationship effect, direction-only**
- Claim: "The teacher-student-family relationship is, in John Hattie's Visible Learning synthesis, among the higher-impact influences on student outcomes — direction well-supported across literatures, though specific effect-size magnitudes are methodologically contested."
- Type: BASIC (direction-only claim with `[contested]` flag on magnitude)
- **Verdict:** CONFIRMED. The chapter does not assert d=0.72; it asserts direction-with-contested-magnitude. The teacher-student-relationships influence in Hattie's published rankings is listed at d=0.72, placing it well above the 0.40 "hinge point." Critiques of Hattie's effect-size methodology (Wecker, Bernstein, Snook et al.) are well-documented; the chapter's hedging is appropriate.
- Source: [Visible Learning effect-size list (cited in chapter)](https://visible-learning.org/hattie-ranking-influences-effect-sizes-learning-achievement/)
- Note: The contestation note is fair and matches the brief's load-bearing-claim #4. No change needed.

**G3. Line 115 — Hamre & Pianta CLASS: emotional support, classroom organization, instructional support; stronger effects for higher-risk students**
- Claim: "The CLASS framework from Hamre and Pianta operationalizes relationship quality through emotional support, classroom organization, and instructional support, with stronger effects for higher-risk students (Pianta 2016)."
- Type: POSITIVE (named framework + 3 named domains + differential-effect claim)
- **Verdict:** CONFIRMED. The three CLASS domains (Emotional Support, Classroom Organization, Instructional Support) are correctly named. The "stronger effects for higher-risk students" claim is well-supported in the Hamre & Pianta literature (see *Building a Science of Classrooms*, FCD, and subsequent studies on at-risk subgroups). The 2016 Pianta citation ("Putting the Science of Classroom Interactions to Work for Children, Teachers, Schools, and the Field," *Policy Insights from the Behavioral and Brain Sciences*) supports the chapter's framing.
- Source: [Pianta 2016, *Policy Insights from BBS* (cited in chapter)](https://journals.sagepub.com/doi/abs/10.1177/2372732215622457); [Hamre & Pianta — Building a Science of Classrooms](https://www.fcd-us.org/wp-content/uploads/2016/04/BuildingAScienceOfClassroomsPiantaHamre.pdf); [APS CLASS Description PDF](https://aps2016.apsva.us/wp-content/uploads/2021/04/CLASS-Description.pdf)

**G4. Line 192 — NCPMI 2018 PBIS Behavior Incident Report: "objective, specific, observable" language**
- Claim: "The PBIS Behavior Incident Report protocol (NCPMI 2018) requires objective, specific, observable language."
- Type: POSITIVE (protocol claim attributed to a named center)
- **Verdict:** CONFIRMED. The NCPMI BIR v2 Training-Instructions-Definitions (October 2018) instructs that incident descriptions use objective, specific, observable terms. The chapter's invocation is faithful.
- Source: [NCPMI BIR v2 Training (cited in chapter)](https://cfrmorris.org/wp-content/uploads/2019/04/NCPMI_BIR_v2_Training-Instructions-Definitions_10-18.pdf); [NCPMI BIR Data-Based Decision-Making Guide](https://cfrmorris.org/wp-content/uploads/2019/04/NCPMI_BIR_v2_Guide_01-19_ADA.pdf); [NCPMI BIRS Overview](https://www.challengingbehavior.org/implementation/data-decision-making/birs/)

**G5. Line 57 — Mollick's "co-pilot" pattern from *Co-Intelligence* (2024)**
- Claim: "Register conversion is form-work. The model is good at form-work — what Ethan Mollick in *Co-Intelligence* (2024) calls the 'co-pilot' pattern."
- Type: BASIC (named work and named coinage)
- **Verdict:** CONFIRMED (with mild caveat). Mollick's *Co-Intelligence: Living and Working with AI* (Portfolio/Penguin, 2024) does present a typology of human-AI collaboration patterns that includes co-piloting as a core mode. "Co-pilot pattern" is closer to a paraphrase of Mollick's framing than an exact coinage from the book (Mollick discusses "AI as co-worker," "centaur" and "cyborg" workflows). The chapter's invocation is fair but reviewer may want to confirm exact phrasing if a quotation marks-style claim survives editing.

### APPROVAL / LEGAL category

**A1. Line 89 — FERPA (20 U.S.C. § 1232g) and education records**
- Claim: "The most concrete near-term constraint is FERPA (20 U.S.C. § 1232g), which treats records containing personally identifiable student information as education records. Pasting student names, IDs, behavioral specifics, or assessment data into a non-enterprise AI tool ... creates an education record outside school control and likely violates FERPA."
- Type: BASIC (statutory citation + applied principle)
- **Verdict:** CONFIRMED. The statutory cite is correct. The applied principle — that pasting PII into a consumer AI tool without a school-official agreement risks FERPA noncompliance — matches FPF 2024 guidance and current Department of Education student-privacy guidance. The chapter properly flags `[contested]` because specific FERPA application to AI tooling varies by state DPA implementation.
- Source: [Future of Privacy Forum 2024 (cited in chapter)](https://fpf.org/wp-content/uploads/2024/10/Ed_AI_legal_compliance.pdf_FInal_OCT24.pdf); [studentprivacy.ed.gov](https://studentprivacy.ed.gov/)

**A2. Line 77 — IDEA "meaningful native-language access" requirement; Section 504 "related expectations"**
- Claim: "The Individuals with Disabilities Education Act (IDEA) generally requires meaningful native-language access for parents in special-education communications; Section 504 carries related expectations."
- Type: BASIC (statutory principle, generalized)
- **Verdict:** CONFIRMED with one important nuance. IDEA explicitly requires that *notices* (prior written notice, procedural safeguards notice, evaluation/consent forms) be provided in the parent's native language unless clearly not feasible (34 CFR §300.503(c); §300.9). **However**, OSEP's 2016 guidance is explicit that IDEA does *not* require IEPs themselves to be translated; instead, districts must "take whatever action is necessary" to ensure the parent understands proceedings, including interpretation. Title VI and the EEOA add overlapping language-access duties. The chapter's "generally requires meaningful native-language access" is a fair umbrella summary; reviewer might consider tightening if precision matters in any subsequent passage.
- Source: [OSEP IEP Translation guidance, June 14, 2016](https://sites.ed.gov/idea/files/policy_speced_guid_idea_memosdcltrs_iep-translation-06-14-2016.pdf); [Center for Parent Information & Resources Q&A](https://www.parentcenterhub.org/qa2/)

**A3. Line 77 — "IDEA / Section 504 native-language standards as applied to machine translation are an active area without settled case law"**
- Type: BASIC (legal-status claim, hedged)
- **Verdict:** CONFIRMED. There is no settled federal case law applying IDEA/§504 native-language standards specifically to machine translation in K-12. State-level developments (e.g., Illinois 2023 amendments expanding translation accommodations) and OCR/OSEP technical assistance are the active sources. The chapter's hedge is appropriate.
- Source: [Franczek P.C. — Illinois 2023 amendments](https://www.specialedlawinsights.com/2023/05/new-amendments-to-illinois-special-education-regulations-increase-translation-accommodations-for-parents-and-guardians/)

### STAT category

**S1. Line 21 — "150 students across five sections ... 7 minutes each ... 18 hours per cycle ... 72 hours every year"**
- Type: POSITIVE (arithmetic in case study)
- **Verdict:** CONFIRMED-by-disclosure. The chapter explicitly labels this composite-illustrative and not measured for any specific teacher. The arithmetic checks: 150 × 7 min = 1,050 min = 17.5 h (rounded to 18); 4 cycles × 18 h = 72 h. The "five hours, not eighteen" reduction also arithmetic-checks: 150 × 90 sec ≈ 3.75 h, rounded up to "five hours." Internally consistent and properly framed as illustrative.

**S2. Line 21 — "50% / 2.5-hour weekly reduction projected by the book's overall time model"**
- Type: POSITIVE (book-level model claim)
- **Verdict:** UNVERIFIED (pre-flagged). The chapter explicitly states this "has not been independently validated in a teacher-week time-use study and is presented as an estimate, not a finding." This matches load-bearing-claim #7 in the brief. The chapter's hedging is sufficient.

**S3. Line 67 — "General estimates for high-resource European language pairs cluster in the 80–90% range on routine prose"**
- Type: POSITIVE (range estimate, MT accuracy)
- **Verdict:** UNVERIFIED-by-genericity. This is a generic MT-literature summary without a specific source citation. The 80–90% accuracy range for high-resource pairs on routine prose is consistent with the broad MT literature (BLEU and human-eval studies of Google Translate, DeepL, NMT systems on Spanish/French/German/Italian), but the chapter does not name a specific benchmark or paper. Acceptable as a generalization; reviewer may wish to add a single citation (e.g., a recent MT survey) to anchor the range.
- Recommendation: Optional citation — e.g., a recent WMT benchmark report or Hendy et al. 2023 GPT/MT comparison.

**S4. Line 332 — Misconception #2 repeats the 80–90% claim**
- Type: POSITIVE (range estimate, restated)
- **Verdict:** UNVERIFIED — same as S3. Consistent with the literature; no specific source.

### SPECIALIST category

**SP1. Line 69 — Low-resource language MT degradation (Karen, Burmese, Somali, Haitian Creole, indigenous)**
- Claim: "The picture changes substantially for low-resource languages — including languages widely spoken by U.S. immigrant families: Karen, Burmese, Somali, Haitian Creole, several indigenous languages. The model's fluency on a low-resource output is not evidence of its accuracy."
- Type: POSITIVE (specialist claim about a domain)
- **Verdict:** CONFIRMED-by-mechanism. The chapter flags this as `[contested]` and notes the absence of comprehensive education-specific MT benchmarks across these languages — appropriate hedging. The fluency/accuracy decoupling for low-resource MT is well-established in the MT literature (FLORES-200, NLLB-200 evaluations); systems trained on smaller parallel corpora produce more confidently-fluent-but-wrong output. The chapter's mechanism explanation ("a translation system is good at a language pair in proportion to how much parallel text was in its training data") is correct.

**SP2. Line 79 — Equity asymmetry: AI translation may "quietly widen" the access gap for low-resource languages**
- Claim: "A district that adopts AI translation without maintaining qualified human interpreters for low-resource languages has made the situation better for some families and worse for others."
- Type: POSITIVE (equity claim)
- **Verdict:** UNVERIFIED-by-empirics. The claim is a defensible mechanism story but the chapter does not cite a study documenting the widening gap. The §8 "Still puzzling" section explicitly names this as an open empirical question — "If AI translation continues to improve for high-resource languages while improving slowly for low-resource ones, does the gap ... widen or narrow over five years? Mechanism stories run both directions; the longitudinal study does not exist." The chapter is internally consistent — the body makes the mechanism claim, the puzzling section names it as unverified empirically.

### CURRENT category

**C1. Line 89 — "specific FERPA application to AI tooling varies by state DPA implementation"**
- Type: BASIC (regulatory-status claim, hedged)
- **Verdict:** CONFIRMED. Student Privacy Compass and FPF both document the patchwork of state Data Privacy Agreement (DPA) implementations layered onto FERPA. The chapter's `[contested]` flag is appropriate.
- Source: [studentprivacycompass.org](https://studentprivacycompass.org/); [FPF 2024](https://fpf.org/wp-content/uploads/2024/10/Ed_AI_legal_compliance.pdf_FInal_OCT24.pdf)

**C2. Line 374 — "Industry surveys exist; rigorous parent-side evaluation of AI-drafted versus teacher-drafted communications does not, as of early 2026"**
- Type: BASIC (literature-status claim)
- **Verdict:** CONFIRMED-by-absence. No rigorous randomized parent-perception study comparing AI-drafted vs. teacher-drafted communications has been published as of May 2026, to the best of available evidence. The §7 "What would change my mind" passage frames this correctly as an open empirical question.

---

## Unverified Assertions

| # | Line | Claim | Why unverified |
|---|------|-------|----------------|
| U1 | 21 | "50% / 2.5-hour weekly reduction" | Pre-flagged by chapter; matches book-level model estimate not yet validated. |
| U2 | 67, 332 | "80–90% range" for high-resource MT routine prose | Generic literature summary without anchored citation. |
| U3 | 79 | Equity-gap widening claim for low-resource MT | Mechanism story; chapter's own §8 names this as unsettled empirics. |
| U4 | 107 | Tenzer "controlling reading" framing | Article verified; "controlling reading" overstates the doctrinal status — chapter does flag with `[contested]`. |

---

## AI-Pass Flags

No fabricated citation flags detected. Every named source — Mapp & Kuttner, Kraft & Rogers, Castro-Ponce et al., Hattie, Pianta, NCPMI, Tenzer, EdWeek, K-12 Dive, FPF — resolves to a real, locatable primary document. URLs in the chapter appear to be accurate and stable. The chapter's `[contested]` and `[verify]` markings track the genuine empirical uncertainties — no over-confident gaps detected.

Cross-book Bastani check: no "17 percentage points" Bastani reference appears in this chapter. (Not flagged elsewhere in chapter 7.)

---

## Reliability Assessment

This is one of the cleaner chapters in the book for fact-checking. Every load-bearing source the brief asked to verify (Mapp & Kuttner, Kraft & Rogers, Castro-Ponce, Hattie direction-only, Pianta CLASS, EdWeek IEP survey, Tenzer, FERPA/IDEA principle-level statements) resolves to a real primary source and is faithfully characterized — with the chapter pre-flagging the items that genuinely warrant `[contested]` (Hattie magnitude, IDEA/§504-vs-MT case law, defamation case law for AI-drafted content, low-resource MT equity). The only edits worth considering are cosmetic: tighten "nearly 60%" to "57%" (E1); soften Tenzer's "controlling reading" to "Tenzer argues" (E5); optionally add a citation anchor to the 80–90% MT range claim (S3). The chapter's hedging discipline is consistently appropriate.
