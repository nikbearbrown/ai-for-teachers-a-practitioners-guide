# Assertions Report: 04-lesson-planning-with-ai.md
**Date:** 2026-05-18
**Source file:** chapters/04-lesson-planning-with-ai.md
**Assertions flagged:** 19
**Breakdown:** STAT: 7 | GUIDELINE: 3 | APPROVAL: 1 | EVIDENCE: 4 | SPECIALIST: 3 | CURRENT: 1

---

## Critical — Requires Immediate Expert Review

### C1. NGSS standard codes are swapped — CONTRADICTED
**Location:** Section 3.4 (line 206)
**Type:** SPECIALIST / GUIDELINE
**Claim:** Chapter says: *"she opens NGSS HS-LS1-7 in another tab, reads the actual standard text ('Use a model to illustrate how photosynthesis transforms light energy into stored chemical energy' — and the related HS-LS1-5 on cellular respiration)"*
**Verdict:** **CONTRADICTED.** The codes are reversed. **HS-LS1-7** is the cellular respiration standard: *"Use a model to illustrate that cellular respiration is a chemical process whereby the bonds of food molecules and oxygen molecules are broken and the bonds in new compounds are formed resulting in a net transfer of energy."* **HS-LS1-5** is the photosynthesis standard: *"Use a model to illustrate how photosynthesis transforms light energy into stored chemical energy."*
**Source:** [NGSS HS-LS1-7](https://www.nextgenscience.org/pe/hs-ls1-7-molecules-organisms-structures-and-processes) ; [HS-LS1-7 Evidence Statements (NGSS)](https://www.nextgenscience.org/sites/default/files/HS-LS1-7_Evidence%20Statements%20Jan%202015.pdf)
**Impact:** This is a worked example explicitly about cellular respiration. The chapter quotes the photosynthesis standard's text under the wrong code in the very sentence demonstrating the verification discipline. The error undermines the section's pedagogical move (verify the standard text matches the assessment). Must be corrected before publication.

---

## Full Findings

### F1. NFER/EEF trial — 31% time reduction headline — CONFIRMED
**Location:** TL;DR (line 3); Section 2.1 (line 55); Section 3.5 (line 210)
**Type:** STAT / EVIDENCE
**Claim:** *"31% reduction in lesson preparation time"* / *"56.2 minutes per week ... compared with 81.5 minutes per week ... a 25.3-minute weekly saving, or 31%."*
**Verdict:** **CONFIRMED.** NFER evaluation report: ChatGPT group spent 56.2 min/week vs. 81.5 min/week in comparison group, average saving 25.3 min/week. Reported as "lesson and resource preparation time ... was 69% of the time spent by the non-GenAI group in weeks six to ten of the trial."
**Source:** [NFER/EEF Evaluation Report (2024)](https://d2tic4wvo1iusb.cloudfront.net/production/documents/projects/chatgpt_in_lesson_planning_-_evaluation_report.pdf?v=1736353004) ; [EEF news summary](https://educationendowmentfoundation.org.uk/news/teachers-using-chatgpt-alongside-a-guide-to-support-them-to-use-it-effectively-can-cut-lesson-planning-time-by-over-30-per-cent)
**Note:** The 31% / 69% figure is specifically the weeks 6-10 comparison; chapter does not specify the window but the headline is the figure EEF leads with.

### F2. NFER/EEF trial — n=259, 68 schools, KS3 science teachers, summer 2024 — CONFIRMED
**Location:** Section 2.1 (line 55)
**Type:** STAT / EVIDENCE
**Claim:** *"a cluster-randomised RCT across 68 English secondary schools and 259 Key Stage 3 science teachers"*
**Verdict:** **CONFIRMED.** 259 Year 7 and Year 8 science teachers from 68 schools; school-randomised controlled trial; ten-week implementation in the summer term 2024.
**Source:** [NFER publication page](https://www.nfer.ac.uk/publications/chatgpt-in-lesson-preparation-a-teacher-choices-trial/) ; [EEF project page](https://educationendowmentfoundation.org.uk/projects-and-evaluation/projects/choices-in-edtech-using-generative-ai-chatgpt-for-ks3-science-lesson-preparation-2024-teacher-choices-trial)

### F3. NFER/EEF — blind expert panel of five science teachers scoring thirty resources — UNVERIFIED
**Location:** Section 2.1 (line 55)
**Type:** STAT / EVIDENCE
**Claim:** *"A blind expert panel of five science teachers scored thirty resources — fifteen treatment, fifteen control — on clarity, engagement, age-appropriateness, and scientific accuracy."*
**Verdict:** **UNVERIFIED — partial.** The expert-panel review and "no statistically significant difference" finding are confirmed by NFER/EEF. The specific numbers (five panelists, thirty resources, 15+15) were not retrievable from the search summaries; chapter's exact figures could not be independently confirmed against the published Appendix without direct PDF inspection. Flag for direct verification of Appendix in the NFER report.

### F4. NFER/EEF — "no statistically significant difference" on quality — CONFIRMED
**Location:** Section 2.1 (line 55)
**Type:** EVIDENCE
**Claim:** *"They found no statistically significant difference on any dimension."*
**Verdict:** **CONFIRMED.** EEF: "Quality did not appear to be affected based on an expert panel reviewing the quality of lesson resources, without knowing which had been produced using ChatGPT."
**Source:** [NFER publication page](https://www.nfer.ac.uk/publications/chatgpt-in-lesson-preparation-a-teacher-choices-trial/)

### F5. Shulman 1986 citation — CONFIRMED
**Location:** Section 2.2 (line 61)
**Type:** SPECIALIST / EVIDENCE
**Claim:** *"Lee Shulman, in his 1986 Educational Researcher article 'Those Who Understand: Knowledge Growth in Teaching'"*
**Verdict:** **CONFIRMED.** Shulman, L. S. (1986). Those who understand: Knowledge growth in teaching. *Educational Researcher*, 15(2), 4-14.
**Source:** [Sage journals (AERA)](https://journals.sagepub.com/doi/10.3102/0013189X015002004) ; [ERIC record EJ330821](https://eric.ed.gov/?id=EJ330821)
**Note:** Chapter cites journal/year/issue correctly. Pagination (4-14) not stated in chapter but matches if added.

### F6. Shulman 1987 citation — CONFIRMED with minor pagination note
**Location:** Section 2.2 (line 61)
**Type:** SPECIALIST / EVIDENCE
**Claim:** *"His 1987 Harvard Educational Review paper, 'Knowledge and Teaching: Foundations of the New Reform,' developed the construct into a model of pedagogical reasoning."*
**Verdict:** **CONFIRMED.** Shulman, L. (1987). Knowledge and Teaching: Foundations of the New Reform. *Harvard Educational Review*, 57(1), 1-22 (some sources list 1-23). Chapter's characterization of the paper as developing the pedagogical-reasoning model is faithful.
**Source:** [ERIC record EJ351846](https://eric.ed.gov/?id=EJ351846)

### F7. PCK characterization — CONFIRMED (faithful)
**Location:** Section 2.2 (lines 63-74)
**Type:** SPECIALIST
**Claim:** The chapter's plain-English unpacking of PCK as the blend a teacher acquires by teaching a particular thing to particular students over time, with the misconception / analogy / sequencing dimensions.
**Verdict:** **CONFIRMED.** This is a faithful, slightly informal restatement of Shulman's PCK construct — "ways of representing and formulating the subject that make it comprehensible to others" plus knowledge of what makes specific topics easy or difficult, including students' preconceptions and misconceptions. The chapter's four-question operationalization is a teaching gloss, not a direct quote, and is consistent with how PCK is discussed in the literature.

### F8. Wiggins & McTighe 2005 — CONFIRMED
**Location:** Section 2.4 (line 88)
**Type:** SPECIALIST / EVIDENCE
**Claim:** *"Grant Wiggins and Jay McTighe's Understanding by Design (ASCD, 2nd ed. 2005)"* and three-stage backward design (1. Identify desired results; 2. Determine acceptable evidence; 3. Plan learning experiences).
**Verdict:** **CONFIRMED.** Wiggins, G., & McTighe, J. (2005). *Understanding by Design* (2nd ed.). ASCD (Alexandria, VA). The three-stage backward design framework is correctly characterized.
**Source:** [ASCD — Understanding by Design, Expanded 2nd Edition](https://www.ascd.org/books/understanding-by-design-expanded-2nd-edition?variant=103055)

### F9. Khoo, Wei, and Wu 2025 preprint — CONTRADICTED (author attribution)
**Location:** Section 2.6 (line 113); Section 5.2 (line 341); Section 8 (line 427)
**Type:** EVIDENCE / SPECIALIST
**Claim:** *"A 2025 preprint by Khoo, Wei, and Wu evaluated AI-generated lesson plans across models and prompt frameworks in high-school physics"* (arXiv 2510.19866)
**Verdict:** **CONTRADICTED.** The arXiv paper 2510.19866 exists and matches the chapter's description of the methodology (five LLMs — GPT-5, Claude Sonnet 4.5, Gemini 2.5 Flash, DeepSeek V3.2, Grok 4 — and three prompt frameworks TAG/RACE/COSTAR; topic: The Electromagnetic Spectrum). However the author is **Xincheng Liu**, not "Khoo, Wei, and Wu." The author attribution must be corrected. The chapter already carries [verify] markers on this citation — verdict resolves to: author list wrong, finding ("prompt framework dominates over model size") substantively confirmed.
**Source:** [arXiv 2510.19866 abstract](https://arxiv.org/abs/2510.19866)
**Title:** "An Evaluation of the Pedagogical Soundness and Usability of AI-Generated Lesson Plans Across Different Models and Prompt Frameworks in High-School Physics."

### F10. The "35% with templates" sub-condition figure — UNVERIFIED
**Location:** Section 2.1 (line 57)
**Type:** STAT / EVIDENCE
**Claim:** Chapter already flags [verify] for *"TIKTOC-cited '35% with templates' condition"* and notes the confirmable headline is 31% for the ChatGPT-plus-guide arm.
**Verdict:** **UNVERIFIED.** The NFER/EEF Teacher Choices Trial reports a single intervention arm (ChatGPT + structured guide) vs. comparison. There is no separately published sub-condition for a "templates" arm in the headline reporting. The 35% figure does not surface in the search-confirmed NFER materials. Recommend dropping the figure or sourcing it precisely.

### F11. Walton/Gallup 2025 "Teaching for Tomorrow" — six-weeks-per-year — CONFIRMED
**Location:** Section 8 (line 421)
**Type:** STAT / EVIDENCE
**Claim:** *"The Walton/Gallup self-reports ... measure teacher-reported hours."*
**Verdict:** **CONFIRMED.** Walton Family Foundation / Gallup, "Teaching for Tomorrow: Unlocking Six Weeks a Year With AI" (2025). Weekly AI users save an average of 5.9 hours/week (~6 weeks/year). Survey: n=2,232 U.S. K-12 public school teachers; fielded March 18 – April 11, 2025.
**Source:** [Gallup, May 2025](https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx) ; [Walton Family Foundation report PDF](https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf)

### F12. RAND 2025 — higher-poverty schools use AI for lesson planning more — CONTRADICTED
**Location:** Section 8 (line 423)
**Type:** STAT / EVIDENCE
**Claim:** *"RAND finds that higher-poverty schools use AI for lesson plan generation more, and receive less AI training to evaluate the output ([RAND 2025, RR-A134-25]; [RAND 2025, RR-A4180-1])."*
**Verdict:** **CONTRADICTED — direction reversed.** RAND RR-A134-25 (Diliberti et al., 2025) reports the opposite direction on usage: "Teachers and principals in higher-poverty schools were **less likely** to report using AI tools than those in lower-poverty schools, and principals in high-poverty schools reported providing guidance for use of AI less often than their counterparts in lower-poverty schools."
**Source:** [RAND RR-A134-25 — Uneven Adoption of AI Tools (2025)](https://www.rand.org/pubs/research_reports/RRA134-25.html) ; [ERIC ED672957](https://eric.ed.gov/?id=ED672957)
**Impact:** The chapter's equity-gap argument needs revision. The direction of the gap (less use, less guidance in higher-poverty schools) still supports the chapter's broader point about equity, but the specific claim "higher-poverty schools use AI for lesson plan generation more" is contradicted. The sentence after it ("receive less AI training to evaluate the output") is supported by RAND.

### F13. Ten-week summer trial framing — CONFIRMED
**Location:** Section 3.5 (line 210); Section 8 (line 425)
**Type:** EVIDENCE
**Claim:** *"the NFER trial ran ten weeks in summer"*
**Verdict:** **CONFIRMED.** The implementation lasted ten weeks in the summer term 2024.
**Source:** [NFER publication page](https://www.nfer.ac.uk/publications/chatgpt-in-lesson-preparation-a-teacher-choices-trial/)

### F14. NFER trial — quality did not differ on blind review — CONFIRMED (restatement)
**Location:** TL;DR (line 3); Section 3.6 (line 214)
**Type:** EVIDENCE / APPROVAL
**Claim:** *"no observed loss of resource quality on blind expert review"* and *"The trial measured teacher time and resource quality. It did not measure student learning outcomes."*
**Verdict:** **CONFIRMED.** Both the quality finding and the explicit boundary (no student-outcome measurement) match the published evaluation.
**Source:** [EEF news summary](https://educationendowmentfoundation.org.uk/news/teachers-using-chatgpt-alongside-a-guide-to-support-them-to-use-it-effectively-can-cut-lesson-planning-time-by-over-30-per-cent)

### F15. NGSS HS-LS1-7 description in TASK prompt — CONFIRMED (with caveat from C1)
**Location:** Section 3.2 (line 161), Section 3.3 (line 189)
**Type:** GUIDELINE
**Claim:** The chapter directs an AI prompt to target "NGSS HS-LS1-7" for a cellular respiration unit.
**Verdict:** **CONFIRMED appropriate code for cellular respiration.** HS-LS1-7 is the correct standard for cellular respiration. (This makes the swap in §3.4 — flagged at C1 above — internally inconsistent within the chapter itself.)
**Source:** [NGSS HS-LS1-7](https://www.nextgenscience.org/pe/hs-ls1-7-molecules-organisms-structures-and-processes)

### F16. "Cleanest single piece of evidence in the field" — APPROVAL / I-LANGUAGE
**Location:** Section 2.1 (line 57)
**Type:** APPROVAL
**Claim:** *"This is, to my reading, the cleanest single piece of evidence in the field."*
**Verdict:** **UNVERIFIED — judgment call.** Labeled "to my reading" so claim is I-language, not assertion of fact. The NFER/EEF trial is widely considered the most methodologically rigorous published RCT on AI in lesson preparation as of mid-2026, but no formal landscape comparison appears in the chapter. Acceptable as I-language; no change required.

### F17. PCK has been "measured for decades" — CURRENT / EVIDENCE
**Location:** Section 8 (line 421)
**Type:** EVIDENCE / CURRENT
**Claim:** *"a finding (PCK matters) that has been measured for decades"*
**Verdict:** **CONFIRMED.** Shulman's PCK construct (1986/87) plus four decades of subsequent research on PCK's relationship to student outcomes broadly support this framing. The link from PCK to student learning has substantial empirical support, though magnitudes vary by subject and methodology — the chapter's general claim is defensible.

### F18. "Most rigorous published trial to date" framing — APPROVAL / EMPHATIC
**Location:** TL;DR (line 3)
**Type:** APPROVAL / EMPHATIC
**Claim:** *"the most rigorous published trial to date — the NFER/EEF 'ChatGPT in Lesson Preparation' RCT"*
**Verdict:** **CONFIRMED — defensible as of writing.** No competing pre-registered, school-randomised RCT on AI in lesson preparation with comparable scale has been published as of May 2026 to displace this claim. Re-verify near publication date; the EEF has a follow-on Oak National Academy AI lesson-planning trial announced/in-flight.
**Source:** [EEF news — new trial on Oak AI lesson planning](https://educationendowmentfoundation.org.uk/news/new-trial-ai-powered-lesson-planning)

### F19. The Day 1 prompt's NGSS framing as "draft pending teacher verification" — GUIDELINE
**Location:** Section 3.2 / Section 4.1 templates
**Type:** GUIDELINE
**Claim:** Standards alignment from AI should be treated as draft pending verification.
**Verdict:** **CONFIRMED (good practice).** Consistent with Khoo/Liu (arXiv 2510.19866) finding that even strong prompt frameworks do not eliminate residual standards alignment errors; standards-citation accuracy is the highest-stakes place for confidently-wrong AI output. Chapter's guideline aligns with the evidence.

---

## Unverified Assertions

- **F3** — Specific panel size (n=5) and sample size (30 resources / 15+15) for the blind expert quality review. Confirm against the NFER/EEF report Appendix directly.
- **F10** — The "35% with templates" sub-condition figure. Already flagged inline by author. Recommend removing if not located.
- **F16** — "Cleanest single piece of evidence" — judgment call, labeled as I-language; leave as is.

---

## AI-Pass Flags

The following are not strict factual errors but warrant a copy-edit / source pass before publication:

1. **C1 — NGSS code swap (line 206):** Highest-priority correction. Swap "HS-LS1-7" and "HS-LS1-5" in the standard-text quote in §3.4. The sentence should read: "she opens NGSS HS-LS1-7 in another tab, reads the actual standard text ('Use a model to illustrate that cellular respiration is a chemical process whereby the bonds of food molecules and oxygen molecules are broken and the bonds in new compounds are formed resulting in a net transfer of energy' — and the related HS-LS1-5 on photosynthesis), and confirms..."

2. **F9 — Author attribution for arXiv 2510.19866:** "Khoo, Wei, and Wu" should be **Xincheng Liu** (single author). Update all three citations in §2.6, §5.2, §8. Title is also worth verifying inline — full title is "An Evaluation of the Pedagogical Soundness and Usability of AI-Generated Lesson Plans Across Different Models and Prompt Frameworks in High-School Physics."

3. **F12 — RAND equity claim direction:** The sentence in §8 reading "higher-poverty schools use AI for lesson plan generation more" reverses the RAND finding. Recommend rewriting to: "RAND finds that higher-poverty schools use AI tools *less* than lower-poverty schools and their principals provide guidance for AI use *less often* — meaning the teachers most likely to benefit from a structural-draft dividend, and most likely to need training to evaluate it, are precisely the ones least likely to receive either." This preserves the equity concern and matches the source.

4. **F10 — The "35% with templates" figure (line 57):** Already flagged inline. Remove if not sourceable in NFER report.

5. **F1 — Time-window precision:** Consider noting that the 31% headline corresponds to weeks 6-10 of the trial (the steady-state period after teachers had a chance to adapt to the workflow), not the full ten-week average from week one. Not strictly an error but a useful precision.

---

## Reliability Assessment

The chapter is largely well-sourced and the headline empirical claims (NFER/EEF 31%, n=259, 68 schools; Walton/Gallup six weeks; Shulman PCK; Wiggins & McTighe backward design) all hold up. The chapter's intellectual honesty about the time-vs-learning gap is exemplary. However, two errors of substance must be corrected before publication: the swapped NGSS codes in the worked example (C1) and the wrong author attribution for arXiv 2510.19866 (F9). One claim about RAND's equity finding is directionally reversed (F12) and should be rewritten. Overall reliability: high on framework / canon citations; moderate on specifics, with three concrete fixes needed.
