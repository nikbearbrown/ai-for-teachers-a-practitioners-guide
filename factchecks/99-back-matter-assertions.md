# Assertions Report: 99-back-matter.md
**Date:** 2026-05-18
**Source file:** chapters/99-back-matter.md
**Assertions flagged:** 38
**Breakdown:** STAT: 6 | GUIDELINE: 3 | APPROVAL: 0 | EVIDENCE: 26 | SPECIALIST: 2 | CURRENT: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

### C1. Bastani et al. 2025 — TITLE INCOMPLETE (CONTRADICTED on title-string)
**Category:** EVIDENCE
**Type:** BASIC
**Location:** Notes §Preface n.1; References entry
**Asserted text:** "Generative AI can harm learning" (Bastani et al., PNAS 2025, DOI 10.1073/pnas.2422633122)
**Verification:** PNAS / PubMed / SSRN all list the published title as **"Generative AI *without guardrails* can harm learning: Evidence from high school mathematics."** The back-matter omits the "without guardrails" qualifier and the subtitle.
**Verdict:** CONTRADICTED — title is materially shortened. The "without guardrails" clause is load-bearing for the chapter's argument (it is *precisely* the point that guardrails matter). DOI is correct. Correction DOI 10.1073/pnas.2518204122 also confirmed. Author list confirmed (Bastani, Bastani, Sungu, Ge, Kabakcı, Mariman).
**Source:** https://www.pnas.org/doi/10.1073/pnas.2422633122

### C2. Henkel et al. 2024 — TITLE WRONG (CONTRADICTED)
**Category:** EVIDENCE
**Type:** BASIC
**Location:** Notes §Ch 5 n.14; References entry "Can large language models tutor at scale? *L@S 2024*. arXiv:2405.02985."
**Asserted text:** Title given as "Can large language models tutor at scale?"
**Verification:** arXiv:2405.02985 is in fact titled **"Can Large Language Models Make the Grade? An Empirical Study Evaluating LLMs Ability to Mark Short Answer Questions in K-12 Education"** by Owen Henkel et al. The paper is about LLM *marking* of short-answer questions, not tutoring. Whether it appeared in *L@S 2024* proceedings is also doubtful — arXiv lists it as a standalone preprint dated May 5, 2024.
**Verdict:** CONTRADICTED — title is wrong, topic is mischaracterized ("tutor at scale" vs "mark short answer questions"), venue ("*L@S 2024*") likely wrong. arXiv number correct.
**Source:** https://arxiv.org/abs/2405.02985

---

## Full Findings

### 1. Bastani et al. 2025 study details
**Category:** STAT | **Type:** EMPHATIC | **Location:** Notes §Preface n.1; Glossary "Bastani finding"
**Asserted text:** "~1,000 Turkish high schoolers… GPT Base outperformed control during practice (~48% gain) but lost ground on the unassisted exam (−17 percentage points). GPT Tutor outperformed during practice (~127% gain) and held its exam scores."
**Verification:** Sample size, country, study design, and the direction/magnitude of effects match the published abstract and summaries. The −17 figure is widely cited; the 48%/127% practice-gain figures match independent summaries.
**Verdict:** CONFIRMED (numeric specifics depend on reading; values match secondary summaries). The Glossary entry phrases the −17 as "17 percentage points lower" — consistent.
**Source:** https://www.pnas.org/doi/10.1073/pnas.2422633122

### 2. Walton/Gallup 2025 — date and n
**Category:** STAT | **Type:** BASIC | **Location:** Notes §Ch 1 n.2
**Asserted text:** "*Teaching for Tomorrow: 2025 Survey of K–12 Teachers* (June 18, 2025). n = 2,232 public-school teachers, RAND American Teacher Panel."
**Verification:** Gallup/Walton confirms n = 2,232; fieldwork March 18–April 11, 2025. The book attributes the panel to "RAND American Teacher Panel"; the Gallup methodology page describes the survey as conducted "by web" with a sample of 2,232 U.S. teachers — **the panel attribution to RAND is unverified**. Release date "June 18, 2025" plausible but not directly confirmed against publication date. The 5.9 hours/week figure is confirmed.
**Verdict:** PARTIAL / UNVERIFIED on panel-vendor attribution (RAND ATP); CONFIRMED on n=2,232 and 5.9 hours.
**Source:** https://www.gallup.com/analytics/659819/k-12-teacher-research.aspx

### 3. NFER/EEF 2024 Teacher Choices Trial — n and effect
**Category:** STAT | **Type:** BASIC | **Location:** Notes §Ch 1 n.3
**Asserted text:** "n = 259 secondary science teachers in 68 English schools. ChatGPT plus a brief guide reduced lesson-preparation time by 31% in the standard condition."
**Verification:** NFER/EEF reports confirm 259 Year 7/8 science teachers, 68 schools, and the 31% lesson-planning time reduction (56.2 min vs 81.5 min/week). Title/publisher correct.
**Verdict:** CONFIRMED.
**Source:** https://www.nfer.ac.uk/publications/chatgpt-in-lesson-preparation-a-teacher-choices-trial/

### 4. OECD TALIS 2018 country hours
**Category:** STAT | **Type:** BASIC | **Location:** Notes §Ch 1 n.4
**Asserted text:** "Finland's lower-secondary teachers report 31.6 working hours per week. Australia's 2018 figure is 45 hours."
**Verification:** TALIS 2018 is widely reported with country averages roughly in these ranges; specific figures of 31.6 (Finland) and 45 (Australia) are consistent with secondary aggregators but the exact decimal for Finland should be confirmed against TALIS 2018 Vol I table.
**Verdict:** UNVERIFIED on exact decimals; directionally CONFIRMED.

### 5. Dell'Acqua et al. 2023 HBS Working Paper 24-013
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 2 n.5; References entry
**Verification:** Title "Navigating the Jagged Technological Frontier: Field Experimental Evidence…" and HBS Working Paper number 24-013 confirmed. Author list confirmed. The back-matter cites the paper as 2023 — HBS page lists Sept 2023.
**Verdict:** CONFIRMED.
**Source:** https://www.hbs.edu/faculty/Pages/item.aspx?num=64700

### 6. Shulman 1986 — *Educational Researcher*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 2 n.6; References entry; Glossary "PCK"
**Verification:** "Those Who Understand: Knowledge Growth in Teaching," *Educational Researcher* 15(2), 4–14 — confirmed.
**Verdict:** CONFIRMED.

### 7. Shulman 1987 — *Harvard Educational Review*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 2 n.6; References entry
**Verification:** "Knowledge and Teaching: Foundations of the New Reform," *Harvard Educational Review* 57(1), 1–22 — confirmed.
**Verdict:** CONFIRMED.

### 8. Hattie effect size critique citations (Bergeron & Rivard 2017; Wrigley 2018; Kraft 2020)
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 2 n.7; References entries
**Verification:** Bergeron & Rivard 2017 *McGill J. of Education* 52(1), 237–246 — confirmed standard cite. Wrigley 2018 *British Educational Research Journal* 44(3), 359–376 — confirmed. Kraft 2020 *Educational Researcher* 49(4), 241–253 — confirmed.
**Verdict:** CONFIRMED (all three).

### 9. Wei et al. 2022 — Chain-of-Thought
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 3 n.9; References entry
**Verification:** arXiv:2201.11903 confirmed. Title "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models" exact. Author list in references is incomplete — actual author order is Wei, Wang, Schuurmans, Bosma, **Ichter, Xia,** Chi, Le, Zhou. The back-matter omits Ichter and Xia.
**Verdict:** PARTIAL — citation correct on essentials; author list truncated/incomplete.
**Source:** https://arxiv.org/abs/2201.11903

### 10. Zheng et al. 2023 — Persona prompting
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 3 n.10; References entry
**Verification:** arXiv:2311.10054 confirmed. Title in the back-matter Notes section is given as "Helpful Assistant or Fruitful Facilitator? Investigating Personas in System Prompts" — this is **not the actual paper title**. The published v2/v3 title is "When 'A Helpful Assistant' Is Not Really Helpful: Personas in System Prompts Do Not Improve Performances of Large Language Models." References entry has the correct title. Author list per arXiv: Mingqian Zheng, Jiaxin Pei, Lajanugen Logeswaran, Moontae Lee, David Jurgens — references entry lists only "Zheng, Pei, Jurgens," omitting Logeswaran and Lee.
**Verdict:** CONTRADICTED on the Notes-section title string; PARTIAL on References author list.
**Source:** https://arxiv.org/abs/2311.10054

### 11. Wiggins & McTighe 2005 — *Understanding by Design*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 4 n.12; References entry
**Verification:** Expanded 2nd ed. published 2005 by ASCD — confirmed.
**Verdict:** CONFIRMED.

### 12. Steiss et al. 2024 — *Learning and Instruction*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 5 n.13; References entry
**Verification:** Volume 91, article 101894, 2024; "Comparing the quality of human and ChatGPT feedback of students' writing" — confirmed exact. Full author list confirmed.
**Verdict:** CONFIRMED.
**Source:** https://www.sciencedirect.com/science/article/pii/S0959475224000215

### 13. CAST UDL Guidelines 3.0 (July 2024)
**Category:** GUIDELINE | **Type:** BASIC | **Location:** Notes §Ch 6 n.16
**Verification:** CAST published UDL Guidelines version 3.0 in 2024 — date and version match published statements.
**Verdict:** CONFIRMED.

### 14. WIDA ELD Standards Framework (2020)
**Category:** GUIDELINE | **Type:** BASIC | **Location:** Notes §Ch 6 n.17
**Verification:** WIDA released the "2020 Edition of the English Language Development Standards Framework" — date confirmed.
**Verdict:** CONFIRMED.

### 15. Mapp & Kuttner 2013
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 7 n.19; References entry
**Verification:** "Partners in Education: A Dual Capacity-Building Framework for Family-School Partnerships," SEDL/U.S. Dept. of Education, 2013 — confirmed. Authors and institutional attribution correct.
**Verdict:** CONFIRMED.

### 16. Castro Ponce — Google Translate accuracy
**Category:** STAT | **Type:** BASIC | **Location:** Notes §Ch 7 n.20
**Asserted text:** "(cited in pantry). Empirical evidence on Google Translate accuracy (~75% for Spanish-English in education contexts; much lower for low-resource languages)."
**Verification:** Citation is incomplete (no full reference in the bibliography). The ~75% figure is plausible but unsupported by the back-matter alone.
**Verdict:** UNVERIFIED.

### 17. Mayer (ed.) 2014/2021 — *Cambridge Handbook of Multimedia Learning*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 8 n.21; References entry
**Verification:** 2nd edition (2014) and 3rd edition (2021) of the *Cambridge Handbook of Multimedia Learning* — confirmed. CUP, ed. Mayer.
**Verdict:** CONFIRMED.

### 18. Moreno & Mayer 2002 — *J. Educational Psychology*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 8 n.22; References entry
**Verification:** "Verbal redundancy in multimedia learning: When reading helps listening," *JEP* 94(1), 156–163, 2002 — confirmed.
**Verdict:** CONFIRMED.

### 19. Alley 2013 / Alley et al. 2006
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 8 n.23; References entries
**Verification:** *The Craft of Scientific Presentations* (2nd ed., Springer, 2013) confirmed. Alley, Schreiber, Ramsdell, Muffo 2006 *Technical Communication* 53(2), 225–234 — confirmed.
**Verdict:** CONFIRMED.

### 20. Reynolds 2008 — *Presentation Zen*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 8 n.24; References entry; Glossary "Slideument"
**Verification:** *Presentation Zen* (New Riders, 2008) — confirmed.
**Verdict:** CONFIRMED.

### 21. Cairo 2016 — *The Truthful Art*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 9 n.25; References entry
**Verification:** *The Truthful Art: Data, Charts, and Maps for Communication*, New Riders, 2016 — confirmed.
**Verdict:** CONFIRMED.

### 22. Tufte 1983/2001 — *Visual Display*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 9 n.26; References entry
**Verification:** *The Visual Display of Quantitative Information*, 1st ed. 1983, 2nd ed. 2001, Graphics Press — confirmed.
**Verdict:** CONFIRMED.

### 23. Knaflic 2015 — *Storytelling with Data*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 9 n.27; References entry
**Verification:** Wiley, 2015 — confirmed.
**Verdict:** CONFIRMED.

### 24. Cleveland & McGill 1984 — *JASA*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 9 n.28; References entry
**Verification:** *JASA* 79(387), 531–554, Sept 1984; "Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods" — confirmed.
**Verdict:** CONFIRMED.

### 25. Holder & Xiong 2023 — *IEEE TVCG*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 9 n.29; References entry
**Asserted text:** "Holder, M., & Xiong, C. (2023). Dispersion vs disparity… *IEEE Transactions on Visualization and Computer Graphics*."
**Verification:** Paper exists and is correctly titled. **First-author first initial is wrong**: it is **Eli Holder** (initial "E."), not "M." The paper was peer-reviewed at IEEE VIS 2022 and appears in TVCG (the journal that publishes the VIS proceedings); 2023 year for the TVCG journal volume is plausible.
**Verdict:** CONTRADICTED on author initial (M. → E.); CONFIRMED on title/venue/topic.
**Source:** https://ieeexplore.ieee.org/abstract/document/9913065

### 26. Liang et al. 2023 — *Patterns*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 10 n.30; References entry
**Verification:** "GPT detectors are biased against non-native English writers," *Patterns* 4(7), 100779, 2023; DOI 10.1016/j.patter.2023.100779 — confirmed. Author list confirmed (Liang, Yuksekgonul, Mao, Wu, Zou).
**Verdict:** CONFIRMED.
**Source:** https://www.cell.com/patterns/fulltext/S2666-3899(23)00130-7

### 27. Flower & Hayes 1981
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 10 n.31; References entry
**Verification:** "A Cognitive Process Theory of Writing," *College Composition and Communication* 32(4), 365–387, Dec 1981 — confirmed.
**Verdict:** CONFIRMED.

### 28. Kosmyna et al. 2025 — MIT Media Lab preprint
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 10 n.32; References entry
**Verification:** "Your Brain on ChatGPT: Accumulation of cognitive debt when using an AI assistant for essay writing tasks" — confirmed (note: arXiv title pluralizes "tasks"; back-matter uses singular "task" — minor discrepancy). arXiv:2506.08872, MIT Media Lab project page. The chapter's own footnote text already flags "verify before final" — appropriate caution.
**Verdict:** CONFIRMED (with minor singular/plural variance in title rendering).
**Source:** https://arxiv.org/abs/2506.08872

### 29. Peng et al. 2023 — GitHub Copilot
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 11 n.33; References entry
**Verification:** arXiv:2302.06590; Peng, Kalliamvakou, Cihon, Demirer; "The Impact of AI on Developer Productivity: Evidence from GitHub Copilot" — confirmed. Back-matter caveat about "measures time-to-complete only" is consistent with the paper.
**Verdict:** CONFIRMED.

### 30. Wing 2006 — *CACM*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 11 n.34; References entry
**Verification:** "Computational Thinking," *Communications of the ACM* 49(3), 33–35, March 2006 — confirmed.
**Verdict:** CONFIRMED.

### 31. RAND ASDP RR-A956-31 — "68% have received no formal AI training"
**Category:** STAT | **Type:** EMPHATIC | **Location:** Notes §Ch 12 n.35; References entry
**Asserted text:** "Teacher training data — the source for the '68% have received no formal AI training' framing. Verify wording."
**Verification:** RAND's ASDP educator AI survey series exists; "RR-A956-31" appears in RAND's report numbering scheme but the specific 68% figure is not directly confirmable here. The chapter's own note flags "Verify wording" — appropriate.
**Verdict:** UNVERIFIED on specific 68% figure / specific report number.

### 32. Davenport & Prusak 1998 — *Working Knowledge*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 12 n.36; References entry
**Verification:** *Working Knowledge: How Organizations Manage What They Know*, HBS Press, 1998 — confirmed.
**Verdict:** CONFIRMED.

### 33. Wood & Neal 2007 — *Psychological Review*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 12 n.37; References entry
**Verification:** "A new look at habits and the habit-goal interface," *Psychological Review* 114(4), 843–863, 2007 — confirmed.
**Verdict:** CONFIRMED.

### 34. Weber-Wulff et al. 2023 — *Int. J. Educational Integrity*
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 13 n.38; References entry
**Verification:** "Testing of detection tools for AI-generated text," *International Journal for Educational Integrity* 19, article 26, 2023 — confirmed. **The back-matter says "Evaluation of 14 AI text detection tools" — the published paper actually tested 14 detection tools (12 publicly available + 2 commercial)**, consistent.
**Verdict:** CONFIRMED.
**Source:** https://link.springer.com/article/10.1007/s40979-023-00146-z

### 35. OpenAI 2023 — AI Text Classifier withdrawal
**Category:** CURRENT | **Type:** BASIC | **Location:** Notes §Ch 13 n.39; References entry
**Asserted text:** "Public withdrawal of the AI Text Classifier, July 2023."
**Verification:** OpenAI announced withdrawal of the AI Text Classifier on July 20, 2023 — confirmed.
**Verdict:** CONFIRMED.

### 36. FTC 2025 COPPA Final Rule
**Category:** GUIDELINE | **Type:** BASIC | **Location:** Notes §Ch 13 n.40; References entry
**Verification:** FTC issued amendments to the COPPA Rule in early 2025 — directionally confirmed; the back-matter cites at the principle level only ("defer specifics to district counsel") which is appropriate.
**Verdict:** CONFIRMED.

### 37. Bjork & Bjork 1992 / 2011
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 14 n.41; References entries; Glossary "Storage strength vs retrieval strength"
**Verification:** 1992 chapter in Healy, Kosslyn, & Shiffrin (Eds.), *From Learning Processes to Cognitive Processes*, Vol. 2, pp. 35–67, Erlbaum — confirmed (back-matter has details correct). 2011 chapter in Gernsbacher et al. (Eds.), *Psychology and the Real World*, Worth Publishers — confirmed. Back-matter says "and the desirable-difficulties framework" referring to the 2011 chapter (full title: "Making things hard on yourself, but in a good way: Creating desirable difficulties to enhance learning") — consistent.
**Verdict:** CONFIRMED.

### 38. Roediger & Karpicke 2006 — both papers
**Category:** EVIDENCE | **Type:** BASIC | **Location:** Notes §Ch 14 n.42; References entries
**Verification:**
- "Test-enhanced learning: Taking memory tests improves long-term retention," *Psychological Science* 17(3), 249–255, 2006 — confirmed.
- "The power of testing memory: Basic research and implications for educational practice," *Perspectives on Psychological Science* 1(3), 181–210, 2006 — confirmed.
**Verdict:** CONFIRMED (both).

---

## Glossary consistency check

- **Ad hoc AI use, Systematic AI use, Capability-building vs capability-borrowing, Fluency trap, Frictional framework, GLP, Jagged technological frontier, Lexile framework, PCK, Phase gate, Performance paradox, Process documentation, Prompt library, Redundancy Principle, Rubric calibration gate, Slideument, Storage vs retrieval strength, Task taxonomy, Worked example** — definitions consistent with how the terms are used in the chapters (no contradictions detected).
- **Bastani finding** entry: "48% higher on practice and 17 percentage points lower on the unassisted exam" — this collapses a percentage gain (48%) with a percentage-point loss (17 pp) using language consistent with the Notes section. Internally consistent; phrasing could be clearer for novice readers, but no factual error.
- **Cognitive offloading — "Risko & Gilbert (2016)"** — Risko & Gilbert published a 2016 paper "Cognitive offloading" in *Trends in Cognitive Sciences*; reference is plausible but **not in the bibliography**. UNVERIFIED-as-bibliography-omission.
- **Compared with what? — "Cairo's (2016)"** — matches bibliography Cairo 2016 *The Truthful Art*.

---

## Sanskrit etymology

### मेधावी (Medhavi) — Sanskrit verification
**Category:** SPECIALIST | **Type:** BASIC | **Location:** "A note on the index" §
**Asserted text:** "from Sanskrit मेधावी, 'intelligent' or 'intellectually brilliant'"
**Verification:** Sanskrit dictionaries (wisdomlib, sanskritdictionary.org) give Medhāvī / Medhāvin meanings of "intelligent, wise, learned, possessed of mental power, intellectually brilliant." Devanagari spelling मेधावी is correct (medhāvī, m.; medhāvinī, f.).
**Verdict:** CONFIRMED.

---

## About the Author — AI-Pass items verified

### Northeastern / Anthropic partnership (ENGR 0201 AI Fluency)
**Category:** SPECIALIST | **Type:** EMPHATIC
**Verdict:** AI-PASS (autobiographical; author asserts personal/professional facts).

### Humanitarians AI 501(c)(3), 2019
**Verdict:** AI-PASS (autobiographical; nonprofit status verifiable via IRS EO database but treated as author-asserted bio).

### Publication list — Avasthi, Lu, Brown 2021 (*Nature Methods*); Issak, Kakkar, Goetz, Brown, Harteveld 2023 (*ICLR*); Gultepe, Valluru, Brown, Sridhar 2026 (*Nano Today*); Balaji, Brown 2026 (*TechRxiv*)
**Verdict:** AI-PASS — autobiographical citation of author's own publications. Dates 2026 are future/in-press relative to today (2026-05-18) and plausible. Not independently verified here; flagged only because two are 2026 in-press (consistent with workshop date).

### UCLA Ph.D. / NSF IGERT Bioinformatics Fellow / DNAX Research / Cetus / Harvard Medical postdoc / UC Santa Cruz BA / Northeastern MBA / Master's IDDV
**Verdict:** AI-PASS (autobiographical).

---

## Unverified Assertions

| # | Item | Note |
|---|------|------|
| U1 | TALIS 2018 Finland 31.6 hrs / Australia 45 hrs | Direction CONFIRMED; exact decimals require TALIS Volume I table check. |
| U2 | Walton/Gallup panel attributed to "RAND American Teacher Panel" | Gallup methodology page describes web survey n=2,232 but does not visibly attribute to RAND ATP — verify. |
| U3 | Castro Ponce (cited in pantry) — Google Translate ~75% Spanish-English | No full citation in bibliography; pantry-only reference. |
| U4 | RAND ASDP RR-A956-31, 68% no formal AI training | Chapter's own note flags "Verify wording." |
| U5 | Risko & Gilbert (2016) cognitive offloading | Cited only in Glossary; not in bibliography. |
| U6 | UNESCO 2024 *AI Competency Framework for Students* | Existence plausible (UNESCO released both student and teacher AI competency frameworks in 2024); not independently confirmed here. |
| U7 | AI4K12 "Five Big Ideas in AI for K–12" | AI4K12 initiative real; "Five Big Ideas" is canonical framing — directionally CONFIRMED but not verified to a specific document URL here. |
| U8 | MetaMetrics Lexile Framework caveat | The substantive claim (GPT manipulates inputs reliably, conceptual content unreliably) is the chapter's own framing, not a cited empirical finding. |
| U9 | Mollick 2024 *Co-Intelligence* (Portfolio) | Publisher and year plausible; not independently verified here. |
| U10 | Henkel et al. 2024 venue "*L@S 2024*" | arXiv lists as preprint only; L@S 2024 publication unverified. See Critical C2. |

---

## AI-Pass Flags

- Acknowledgments (entire section) — personal-debt prose; not fact-checked per instructions.
- About the Author — autobiographical claims (degrees, employment, affiliations, fun facts) treated as author-asserted.
- "What this book is" / framing statements throughout the back-matter — interpretive, not factual.
- Glossary entries that paraphrase the book's own conceptual moves (Frictional framework, AI-survivable assignment, Phase gate, Capability-building vs capability-borrowing) — these are book-internal definitions, not external claims.

---

## Reliability assessment

The back-matter bibliography is generally reliable: ~85% of verified entries are CONFIRMED with exact title/year/venue/page match. Two CONTRADICTED items need correction before publication — the Bastani title is missing the load-bearing "without guardrails" qualifier, and the Henkel et al. citation has the wrong paper title and likely wrong venue (it is about *marking* short answers, not *tutoring*). Minor issues include the Holder & Xiong first-initial error (M. → E.), the Zheng et al. Notes-section title string (which differs from the actual paper title), and truncated author lists on Wei et al. and Zheng et al. The Sanskrit etymology is correct. Glossary definitions are internally consistent with chapter usage.
