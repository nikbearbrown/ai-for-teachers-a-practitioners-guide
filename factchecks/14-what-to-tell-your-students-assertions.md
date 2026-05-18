# Assertions Report: 14-what-to-tell-your-students.md
**Date:** 2026-05-18
**Source file:** chapters/14-what-to-tell-your-students.md
**Assertions flagged:** 24
**Breakdown:** STAT: 1 | GUIDELINE: 3 | APPROVAL: 0 | EVIDENCE: 14 | SPECIALIST: 4 | CURRENT: 2

**Verdict counts:** CONFIRMED: 17 | CONTRADICTED: 2 | UNVERIFIED: 4 | OUTDATED: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

Two assertions require attention before the chapter is shown to readers.

**C1. Line 78 — "a roughly 17 percentage point exam drop" (Bastani 2025).** The unit is wrong. Across the published paper, the SRI seminar, Knowledge@Wharton coverage, and every secondary summary, the figure is consistently reported as a **17% *relative reduction*** in unassisted exam scores for the GPT Base group (i.e., the GPT Base group scored 17% *lower than* the no-AI control on a relative basis), not "17 percentage points." The chapter hedges with `[verify]` and warns the teacher to verify the figure against the paper before quoting it to a class — that warning is genuinely protective — but the wording itself still asserts the wrong unit. The hedge is not a correction; the wrong number is in the prose and will be quoted out of context. **Recommend changing "a roughly 17 percentage point exam drop" → "a roughly 17% *relative* exam-score reduction"** (and keeping the `[verify]` flag). This is the same unit-error pattern flagged across earlier chapters in this book — the only chapter that gets it right is Ch. 10, which avoids the magnitude entirely.

**C2. Line 122 — Lachner et al., 2020, *Learning and Instruction* — "explaining to an *imagined* audience outperforms explaining to oneself."** The paper the chapter cites (Lachner, Jacob, & Hoogerheide, *Learning and Instruction*, vol. 74, article 101438, published 2021 with online DOI year 2020 — citation year is borderline) titled "Learning by writing explanations: Is explaining to a fictitious student more effective than self-explaining?" reports across its experiments that **fictitious-audience writing did NOT significantly outperform self-explaining on most learning outcomes**, and in one configuration the self-directed condition outperformed the other-directed condition. The chapter's claim that this paper shows imagined-audience > self-explaining inverts what the paper found. The fictitious-audience effect in the broader literature (Hoogerheide and others) holds more reliably for *video* or *oral* explanations than for *written* ones, which is exactly what the cited Lachner/Jacob/Hoogerheide paper concludes. **Recommend either dropping this citation, replacing it with a citation that supports the claim (e.g., Hoogerheide's earlier video-explaining work), or rewriting the claim to track what the paper actually found** (writing modality complicates the social-presence effect).

A third issue (C3, below) is not "critical" but is the chapter's own flagged hedge becoming a real problem: the McMurtrie citation has no specific title or URL, and the brief itself flagged the title as not located. It should be downgraded to "Beth McMurtrie's reporting in *The Chronicle of Higher Education*'s 'Teaching' newsletter" with no implied specific piece — or removed.

---

## Full Findings

### EVIDENCE category

**E1. Line 70 — Bastani et al. (2025), *PNAS*, ~1,000 Turkish high-school students, three groups (no-AI / unconstrained GPT-4 / tutor-prompted GPT-4), math.**
- Claim: "A research team led by Hamsa Bastani at Wharton ran a randomized experiment with about a thousand high school students in Turkey, studying mathematics ([Bastani et al., 2025, *PNAS*]). Three groups. Group 1 practiced with pencil, paper, and textbook. Group 2 practiced with unconstrained access to GPT-4. Group 3 practiced with a version of GPT-4 that had been wrapped in a pedagogically designed prompt — it was instructed to act like a tutor, to ask questions rather than supply answers, to give hints rather than solutions."
- Category: EVIDENCE
- Type: POSITIVE (precise authority, sample, design)
- **Verdict:** CONFIRMED
- **Finding:** Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö., & Mariman, R. (2025). "Generative AI without guardrails can harm learning: Evidence from high school mathematics." *PNAS*, 122. DOI [10.1073/pnas.2422633122](https://www.pnas.org/doi/10.1073/pnas.2422633122). Sample: ~1,000 Turkish high-school math students. Three randomized arms (control / GPT Base / GPT Tutor) match the chapter's description. Tutor prompt designed to give hints, not answers. Mechanism summary is faithful.
- Source: [PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122); [PubMed 40560616](https://pubmed.ncbi.nlm.nih.gov/40560616/); [SSRN 4895486](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4895486)

**E2. Line 72 — "During practice, the unconstrained-AI group dramatically outperformed the no-AI group… accuracy on practice problems jumped substantially."**
- Category: EVIDENCE
- Type: POSITIVE (direction-only)
- **Verdict:** CONFIRMED
- **Finding:** Paper reports GPT Base scored 48% higher than control on practice problems (Bastani et al. 2025). Direction matches. The chapter wisely stays directional in this sentence rather than naming "48%."
- Source: [Knowledge@Wharton coverage](https://knowledge.wharton.upenn.edu/article/without-guardrails-generative-ai-can-harm-education/); [PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122)

**E3. Line 74 — "the unconstrained-AI group scored *worse* than the no-AI group by a substantial margin" on the unassisted exam.**
- Category: EVIDENCE
- Type: POSITIVE (direction-only)
- **Verdict:** CONFIRMED
- **Finding:** GPT Base group performed 17% lower (relative) than control on the unassisted exam. Direction matches; magnitude reserved for separate flag.
- Source: [PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122)

**E4. Line 78 — "a roughly 48% practice gain and a roughly 17 percentage point exam drop in the unconstrained condition."** ⚠️ CRITICAL
- Category: EVIDENCE / STAT
- Type: POSITIVE (precise magnitude) with `[verify]` hedge
- **Verdict:** CONTRADICTED (unit error)
- **Finding:** The 48% practice gain is correctly stated as a relative figure. The "17 percentage point exam drop" is a unit error — the paper and all primary coverage report this as a **17% relative reduction** in unassisted exam scores, not 17 percentage points. The chapter's `[verify]` flag and warning to teachers ("verify them against the published paper directly") is laudable but does not correct the on-page wording. **Required fix:** change "17 percentage point exam drop" to "17% relative exam-score reduction" (or remove the magnitude entirely, as Ch. 10 does).
- Source: [PNAS](https://www.pnas.org/doi/10.1073/pnas.2422633122); [Knowledge@Wharton](https://knowledge.wharton.upenn.edu/article/without-guardrails-generative-ai-can-harm-education/)

**E5. Line 76 — "The tutor-prompted group… Their exam scores were comparable to — and in some specifications, slightly above — the no-AI control."**
- Category: EVIDENCE
- Type: POSITIVE
- **Verdict:** CONFIRMED
- **Finding:** Paper reports GPT Tutor group exam performance "no worse than" control — direction matches. "Slightly above" in some specifications is also consistent with the Knowledge@Wharton summary and the supplementary materials.
- Source: [Knowledge@Wharton](https://knowledge.wharton.upenn.edu/article/without-guardrails-generative-ai-can-harm-education/)

**E6. Line 86 — Bjork & Bjork (1992) "A New Theory of Disuse"; Bjork & Bjork (2011) framework review.**
- Claim: "[Robert Bjork and Elizabeth Bjork] proposed that human memory has two distinct parameters that the introspective system cannot distinguish. They called them *storage strength* and *retrieval strength* ([Bjork & Bjork, 1992; framework reviewed in Bjork & Bjork, 2011])."
- Category: EVIDENCE
- Type: POSITIVE (canonical citation, mechanism summary)
- **Verdict:** CONFIRMED
- **Finding:** Bjork, R. A., & Bjork, E. L. (1992). "A new theory of disuse and an old theory of stimulus fluctuation." In Healy, Kosslyn, & Shiffrin (Eds.), *From Learning Processes to Cognitive Processes: Essays in Honor of William K. Estes* (Vol. 2, pp. 35–67). The framework summary (storage vs. retrieval strength, introspectively indistinguishable, storage strength does not decay) is faithful. Bjork, E. L., & Bjork, R. A. (2011). "Making Things Hard on Yourself, but in a Good Way: Creating Desirable Difficulties to Enhance Learning." In Gernsbacher et al. (Eds.), *Psychology and the Real World* (pp. 56–64). Worth Publishers. UNH PDF link in the chapter resolves.
- Source: [Bjork Lab PDF of 2011 chapter](https://bjorklab.psych.ucla.edu/wp-content/uploads/sites/13/2016/04/EBjork_RBjork_2011.pdf); [UNH PDF (chapter link)](https://www.unh.edu/teaching-learning-resource-hub/sites/default/files/media/2023-06/itow-introducing-desirable-difficulties-into-practice-and-instruction-bjork-and-bjork.pdf)

**E7. Line 92 — "They called these *desirable difficulties* — counterintuitive on purpose."**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (mechanism naming)
- **Verdict:** CONFIRMED
- **Finding:** The term "desirable difficulties" originates with R. A. Bjork (1994) and is developed across Bjork & Bjork 1992/2011. The chapter's list (spaced practice, interleaving, retrieval before re-reading, generation, productive struggle) maps directly to the standard inventory in Bjork & Bjork 2011.
- Source: [Bjork Lab](https://bjorklab.psych.ucla.edu/research/)

**E8. Line 94 — "the *direction* of the desirable-difficulties effect… is one of the most robust findings in modern learning science, with thirty-plus years of converging evidence."**
- Category: EVIDENCE / I-LANGUAGE
- Type: EMPHATIC + I-LANGUAGE (calibrated)
- **Verdict:** CONFIRMED (well-calibrated)
- **Finding:** The direction-only claim with explicit refusal to cite specific effect sizes ("I do not cite specific effect sizes from any single experiment as if they generalize") is exactly the right epistemic move. The direction is supported by Bjork & Bjork 2011, Roediger & Karpicke 2006, and multiple meta-analyses since.

**E9. Line 106 — Roediger & Karpicke (2006), *Psychological Science*, re-reading vs. testing, 5-minute vs. one-week retention reversal.**
- Claim: "Henry Roediger and Jeffrey Karpicke ran what is now the canonical study in 2006 ([Roediger & Karpicke, 2006, *Psychological Science*]). Students read a passage. One group then re-read it three more times. Another group read it once and took recall tests. Five minutes after the session, the re-readers outperformed the testers… A week later, the result reversed and the gap widened."
- Category: EVIDENCE
- Type: POSITIVE (canonical citation + design summary)
- **Verdict:** CONFIRMED
- **Finding:** Roediger, H. L., & Karpicke, J. D. (2006). "Test-enhanced learning: Taking memory tests improves long-term retention." *Psychological Science*, 17(3), 249–255. DOI [10.1111/j.1467-9280.2006.01693.x](https://doi.org/10.1111/j.1467-9280.2006.01693.x). Design summary is faithful: prose passages, three re-readings vs. one read plus tests, 5-minute vs. delayed criterion. Crossover at delay is the paper's headline finding. PubMed 16507066 link resolves.
- Source: [Sage](https://journals.sagepub.com/doi/10.1111/j.1467-9280.2006.01693.x); [PubMed 16507066](https://pubmed.ncbi.nlm.nih.gov/16507066/)

**E10. Line 106 — Roediger & Karpicke (2006), *Perspectives on Psychological Science*, "The Power of Testing Memory" review.**
- Category: EVIDENCE
- Type: POSITIVE
- **Verdict:** CONFIRMED
- **Finding:** Roediger, H. L., & Karpicke, J. D. (2006). "The Power of Testing Memory: Basic Research and Implications for Educational Practice." *Perspectives on Psychological Science*, 1(3), 181–210. DOI [10.1111/j.1745-6916.2006.00012.x](https://doi.org/10.1111/j.1745-6916.2006.00012.x). The chapter's framing ("the integrative review… that put the finding in front of educators") is faithful — this paper is widely treated as the educational-implications companion to the empirical paper above.
- Source: [Sage](https://journals.sagepub.com/doi/abs/10.1111/j.1745-6916.2006.00012.x); [WUSTL PDF](http://psychnet.wustl.edu/memory/wp-content/uploads/2018/04/Roediger-Karpicke-2006_PPS.pdf)

**E11. Line 110 — Karpicke & Blunt (2011), *Science*, retrieval practice beats concept mapping even on concept-map tests.**
- Claim: "Karpicke and Blunt later showed that this effect is large enough to beat elaborative study methods — including concept mapping… the retrieval-practice group outscored the concept-mapping group even on tasks that required the student to draw a concept map ([Karpicke & Blunt, 2011, *Science*])."
- Category: EVIDENCE
- Type: POSITIVE (precise authority, specific finding)
- **Verdict:** CONFIRMED
- **Finding:** Karpicke, J. D., & Blunt, J. R. (2011). "Retrieval Practice Produces More Learning than Elaborative Studying with Concept Mapping." *Science*, 331(6018), 772–775. DOI [10.1126/science.1199327](https://www.science.org/doi/10.1126/science.1199327). The "even on concept-mapping outcomes" finding is in the paper — retrieval-practice group outperformed concept-mapping group on a range of test types, including concept-map outcomes. Direction and specifics are faithful.
- Source: [Science](https://www.science.org/doi/10.1126/science.1199327); [Purdue Learning Lab PDF](https://learninglab.psych.purdue.edu/downloads/2011/2011_Karpicke_Blunt_Science.pdf)

**E12. Line 122 — Fiorella & Mayer (2016), *Educational Psychology Review*, eight generative-learning strategies.**
- Claim: "Fiorella and Mayer's review of generative learning collects the eight strategies that share this property: explaining, summarizing, mapping, drawing, imagining, self-testing, self-explaining, teaching ([Fiorella & Mayer, 2016, *Educational Psychology Review*])."
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (canonical citation, specific list)
- **Verdict:** CONFIRMED (minor list discrepancy)
- **Finding:** Fiorella, L., & Mayer, R. E. (2016). "Eight Ways to Promote Generative Learning." *Educational Psychology Review*, 28(4), 717–741. DOI [10.1007/s10648-015-9348-9](https://link.springer.com/article/10.1007/s10648-015-9348-9). The official eight are: **summarizing, mapping, drawing, imagining, self-testing, self-explaining, teaching, and enacting**. The chapter's list substitutes "explaining" (as a first item) for "enacting" (omitted) — minor list error. The chapter has 8 items but item 1 ("explaining") is not on the canonical list and "enacting" is missing. **Recommend correcting the list** to match the paper.
- Source: [Springer](https://link.springer.com/article/10.1007/s10648-015-9348-9); [ERIC EJ1120458](https://eric.ed.gov/?id=EJ1120458)

**E13. Line 122 — Lachner, Ly, & Nückles (2018), *Journal of Experimental Education*, oral vs. written explanation.**
- Claim: "oral explanation outperforms written explanation on conceptual transfer measures ([Lachner, Ly, & Nückles, 2018, *Journal of Experimental Education*])."
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (specific direction, specific outcome)
- **Verdict:** CONTRADICTED (direction inverted)
- **Finding:** Lachner, A., Ly, K.-T., & Nückles, M. (2018). "Providing Written or Oral Explanations? Differential Effects of the Modality of Explaining on Students' Conceptual Learning and Transfer." *Journal of Experimental Education*, 86(3), 344–361. DOI [10.1080/00220973.2017.1363691](https://www.tandfonline.com/doi/full/10.1080/00220973.2017.1363691). The paper's central finding is actually the **opposite** of what the chapter claims: "providing written explanations was more effective than providing oral explanations in supporting students to organize the content of the explanations, and the higher levels of organization yielded higher levels of students' conceptual knowledge." Written > oral, not oral > written. **Required fix:** either invert the direction in the chapter prose, or replace the citation with one that supports the chapter's claim (and check whether the chapter wants to make a transfer-vs.-organization distinction that this paper supports).
- Source: [Taylor & Francis](https://www.tandfonline.com/doi/full/10.1080/00220973.2017.1363691); [ERIC EJ1177046](https://eric.ed.gov/?id=EJ1177046); [Semantic Scholar](https://www.semanticscholar.org/paper/Providing-Written-or-Oral-Explanations-Differential-Lachner-Ly/e01a354482486c7f0c37a895c8e92a0e9ea15c96)

**E14. Line 122 — "Lachner et al., 2020, *Learning and Instruction*" — fictitious audience > self-explaining.** ⚠️ CRITICAL
- Claim: "Lachner and colleagues have shown that explaining to an *imagined* audience outperforms explaining to oneself ([Lachner et al., 2020, *Learning and Instruction*])."
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (specific authority + specific direction)
- **Verdict:** CONTRADICTED (finding-direction error)
- **Finding:** Lachner, A., Jacob, L., & Hoogerheide, V. (2021). "Learning by writing explanations: Is explaining to a fictitious student more effective than self-explaining?" *Learning and Instruction*, 74, Article 101438. DOI [10.1016/j.learninstruc.2020.101438](https://doi.org/10.1016/j.learninstruc.2020.101438). The paper's actual finding across two experiments is that fictitious-audience writing did **not** reliably outperform self-explaining; in one configuration, self-explaining outperformed the other-directed condition. The fictitious-audience effect from earlier literature (Hoogerheide and colleagues) is more robust for *video/oral* explanations than for *written* ones — which is what this paper's discussion explicitly says. **The chapter has the citation's direction inverted.** Also: year listed as 2020 but the volume is 2021 (DOI year is 2020 because of online-first publication) — borderline. **Required fix:** either drop this citation or rewrite the claim. Cleanest replacement is Hoogerheide, Loyens, & van Gog (2014) or similar for the video-explaining-to-fictitious-audience effect, which the literature supports.
- Source: [ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S0959475220307337); [Semantic Scholar](https://www.semanticscholar.org/paper/Learning-by-Writing-Explanations:-Is-Explaining-to-Lachner-Jacob/91e5210e2de57bbead4b33cb5923b1e0cdfdc798)

### SPECIALIST category

**S1. Line 138 — "what cognitive scientists call *prediction error* — the moment when what you expected does not match what you encountered, which is the signal that initiates the neurological cascade the Preface described."**
- Category: SPECIALIST
- Type: POSITIVE (mechanism naming)
- **Verdict:** CONFIRMED (in the sense intended)
- **Finding:** Prediction-error signaling (associated with dopaminergic learning circuits, Schultz et al. 1997 and subsequent literature) is a standard mechanism in computational learning theory and the predictive-processing tradition. The phrase "the neurological cascade the Preface described" is internal to the book; verification of the Preface's framing is outside this fact-check. The general construct is well-established.

**S2. Line 140 — Ericsson, Krampe, & Tesch-Römer (1993), *Psychological Review*, four conditions of deliberate practice.**
- Claim: "Anders Ericsson's framework for how expertise is built names four conditions: a specific well-defined goal, full concentration, immediate feedback, and operating at the edge of current competence ([Ericsson, Krampe, & Tesch-Römer, 1993, *Psychological Review*])."
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (canonical citation, specific list)
- **Verdict:** CONFIRMED
- **Finding:** Ericsson, K. A., Krampe, R. Th., & Tesch-Römer, C. (1993). "The Role of Deliberate Practice in the Acquisition of Expert Performance." *Psychological Review*, 100(3), 363–406. PsycNet record matches the chapter's URL. The four conditions named in the chapter map to Ericsson's standard formulation. Note: the chapter's list slightly compresses Ericsson's full statement (which also emphasizes that the practice is effortful and not inherently enjoyable), but the chapter's summary is faithful for pedagogical purposes.
- Source: [PsycNet](https://psycnet.apa.org/record/1993-40718-001); [PMC6731745 (revisit)](https://pmc.ncbi.nlm.nih.gov/articles/PMC6731745/)

**S3. Line 140 — "the '10,000-hour rule' popularization of this work was Gladwell's, not Ericsson's, and the strong version has been substantially complicated by subsequent meta-analyses ([Macnamara, Hambrick, & Oswald, 2014, *Psychological Science*])."**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (precise authority + correct attribution of popularization)
- **Verdict:** CONFIRMED
- **Finding:** Macnamara, B. N., Hambrick, D. Z., & Oswald, F. L. (2014). "Deliberate Practice and Performance in Music, Games, Sports, Education, and Professions: A Meta-Analysis." *Psychological Science*, 25(8), 1608–1618. DOI [10.1177/0956797614535810](https://journals.sagepub.com/doi/10.1177/0956797614535810). The meta-analysis found deliberate practice explains 26% of variance in games, 21% music, 18% sports, 4% education, <1% professions — substantively complicating the strong-form view. "Gladwell, not Ericsson" is correct: Ericsson never proposed a 10,000-hour rule; Gladwell coined that framing in *Outliers* (2008). Ericsson himself pushed back on Gladwell's framing repeatedly.
- Source: [Sage](https://journals.sagepub.com/doi/10.1177/0956797614535810); [PubMed 24986855](https://pubmed.ncbi.nlm.nih.gov/24986855/); [Gwern PDF](https://gwern.net/doc/psychology/2014-macnamara.pdf)

**S4. Line 140 — "edge-of-competence principle: practice that operates at the level where you fail just often enough to learn from the failure produces more growth than practice in the comfort zone."**
- Category: SPECIALIST
- Type: POSITIVE (mechanism summary)
- **Verdict:** CONFIRMED
- **Finding:** The edge-of-competence framing is consistent with Ericsson's "operating just beyond current competence" formulation and with Vygotsky's zone of proximal development. The "fail just often enough" framing is also consistent with the desirable-difficulties literature. Standard learning-science synthesis.

### GUIDELINE category

**G1. Line 165 — UNESCO 2024 *AI Competency Framework for Students*.**
- Claim: "[UNESCO, 2024] AI Competency Framework for Students"
- Category: GUIDELINE
- Type: POSITIVE (precise authority + year + title)
- **Verdict:** CONFIRMED
- **Finding:** UNESCO published the *AI Competency Framework for Students* (and a companion *AI Competency Framework for Teachers*) in September 2024. The framework defines 12 competencies across four dimensions (Human-centred mindset, Ethics of AI, AI techniques and applications, AI system design) at three progression levels (Understand, Apply, Create). Chapter's framing as "names what students should understand but provide thin empirical evidence about which instructional methods actually produce understanding" is fair — the document is a competency framework, not an instructional-methods evaluation. Chapter URL [unesco.org/en/digital-education/ai-future-learning](https://www.unesco.org/en/digital-education/ai-future-learning) is a landing page; canonical landing is [unesco.org/en/articles/ai-competency-framework-students](https://www.unesco.org/en/articles/ai-competency-framework-students).
- Source: [UNESCO AICFS](https://www.unesco.org/en/articles/ai-competency-framework-students); [UNESCO draft framework PDF](https://www.unesco.org/sites/default/files/medias/fichiers/2024/04/UNESCO-Draft-AI-competency-frameworks-for-teachers-and-school-students.pdf)

**G2. Line 167 — AI4K12 "Five Big Ideas" framework, K–2 grade-band guidelines.**
- Claim: "AI4K12's 'Five Big Ideas' framework has K–2 grade-band guidelines for naming what AI is and is not."
- Category: GUIDELINE
- Type: POSITIVE
- **Verdict:** CONFIRMED
- **Finding:** AI4K12 is a joint AAAI/CSTA initiative led by David Touretzky and colleagues. Its "Five Big Ideas in AI" are: (1) Perception, (2) Representation & Reasoning, (3) Learning, (4) Natural Interaction, (5) Societal Impact. Grade bands are K–2, 3–5, 6–8, 9–12. The chapter's claim that K–2 guidelines name "what AI is and is not" is faithful to the AI4K12 K–2 progression chart.
- Source: [AI4K12](https://ai4k12.org/); [Big Ideas Poster](https://ai4k12.org/resources/big-ideas-poster/)

**G3. Line 165 — "Treat them as informed defaults, not as findings." (calibrating the K–8 deployment recommendations)**
- Category: GUIDELINE / I-LANGUAGE
- Type: I-LANGUAGE (calibrated epistemic move)
- **Verdict:** CONFIRMED (well-calibrated)
- **Finding:** The chapter's explicit acknowledgement that K–8 recommendations are extrapolated from older-student research and "informed defaults, not as findings" is exactly the right epistemic posture. No correction needed.

### CURRENT category

**C-CUR1. Line 171 — Beth McMurtrie *Chronicle of Higher Education* "Teaching" newsletter; "many high schoolers already self-organize into 'use AI for the boring parts, do the hard parts yourself' patterns."** ⚠️ CRITICAL (downgrade)
- Category: CURRENT / SPECIALIST
- Type: POSITIVE (precise authority + specific empirical claim)
- **Verdict:** UNVERIFIED
- **Finding:** McMurtrie's "Teaching" newsletter at the Chronicle does cover students' AI use extensively in 2025–2026 (issues on July 24, 2025 "Why students are using AI"; March 27, 2025 "How students think about AI"; April 16, 2026 "The students who won't use AI"). However, I could not locate a specific piece with the title "What Should Students Know About AI?" (the brief flagged this title as not located, and I confirm). I also could not verify that any specific McMurtrie piece "documents" the exact pattern the chapter paraphrases ("use AI for the boring parts, do the hard parts yourself"). The Chronicle has covered related framings (the "AI sandwich" piece from March 19, 2026 is the closest match) but the chapter's paraphrase appears to be inferential, not quoted. **Recommend** rewriting as either: (a) a direct quote from a specific issue with URL, or (b) a softer attribution — "Beth McMurtrie's reporting in the Chronicle… has documented that some high schoolers describe self-organizing this way" — and drop the implicit claim of a named piece. The chapter's wording in fact does not invoke a title, only the newsletter, so this is more "specific claim without specific source" than fabricated citation. Still: the claim is empirical and needs anchoring.
- Source: [McMurtrie author page](https://www.chronicle.com/author/beth-mcmurtrie); [Teaching newsletter index](https://www.chronicle.com/newsletter/teaching); [7/24/2025 issue](https://www.chronicle.com/newsletter/teaching/2025-07-24); [3/27/2025 issue](https://www.chronicle.com/newsletter/teaching/2025-03-27)

**C-CUR2. Line 353 — "[verify whether any 2025–2026 replication studies have addressed grade 3–5 specifically]"**
- Category: CURRENT / I-LANGUAGE
- Type: I-LANGUAGE (explicit verify flag)
- **Verdict:** UNVERIFIED (consistent with the chapter's own flag)
- **Finding:** As of May 2026, I find no published large-N RCT of Bastani-style design in grades 3–5. UNESCO 2024 and AI4K12 are still the dominant frameworks; empirical work at grades 3–5 remains thin. The chapter's `[verify]` flag is well-placed and need not be removed; the chapter should retain its honest "still puzzling" framing.

### STAT category

**ST1. Line 285 — "AI removes the struggle, so it removes the learning."**
- Category: STAT / SPECIALIST
- Type: EMPHATIC (general principle stated as crisp slogan)
- **Verdict:** CONFIRMED (in the directional sense, for the population studied by Bastani)
- **Finding:** This is a rhetorical compression of the Bastani 2025 finding for the unconstrained-AI condition combined with the Bjork desirable-difficulties direction. Both anchor literatures support the direction. The sentence is a slogan, not a measurable claim, so it is fine as long as the surrounding text continues to acknowledge that the *tutor-prompted* condition does not remove the learning. The chapter does so.

---

## Unverified Assertions

- **U1 (Line 171):** McMurtrie's Chronicle paraphrase — see C-CUR1. The brief explicitly flagged this and asked for confirmation or downgrade. **Downgrade.**
- **U2 (Line 122, embedded):** Lachner et al. 2020 *Learning and Instruction* citation has a borderline year issue (volume year 2021, DOI year 2020) and a finding-direction error (see E14). Listed as CONTRADICTED above, but the date issue alone would be UNVERIFIED.
- **U3 (Line 353):** Author's own explicit `[verify]` on grade 3–5 replication studies. Confirmed as still unverified as of May 2026 — keep flag.
- **U4 (Line 78):** Author's own `[verify]` on the 17 percentage-point/relative-reduction figure. The author flagged this themselves; the unit error remains and needs correction (see E4).

---

## AI-Pass Flags

The chapter is in the top tier of fact-handling within this book. The author's epistemic honesty — explicit `[verify]` tags at exactly the right points (lines 78 and 353), refusal to cite effect sizes from individual experiments as if they generalize (line 94), the section calibrating the K–8 deployment as "informed defaults, not as findings" (line 165) — is unusually disciplined. Every cognitive-science citation resolves to a real paper at the named journal in the named year (or within 1 year, see Lachner 2020/2021 issue).

That said, three distinct on-page errors require correction before publication:

1. **Unit error on Bastani magnitude.** "17 percentage point" should be "17% relative reduction." (Line 78, see E4 / C1.)
2. **Direction-inversion on Lachner, Ly, & Nückles 2018.** Paper found written > oral, not oral > written. (Line 122, see E13.)
3. **Direction-inversion on Lachner et al. 2020/2021** for the fictitious-audience claim. Paper did *not* find imagined-audience > self-explaining for written modality. (Line 122, see E14 / C2.)

A fourth minor issue: the Fiorella & Mayer 2016 list of eight strategies in the chapter substitutes "explaining" for "enacting" (E12). Easy fix.

The McMurtrie attribution is the only citation in the chapter that should be either anchored to a specific dated issue or softened (see C-CUR1).

The chapter passes on cognitive-science rigor. It needs three citation fixes before it goes to a classroom.

---

## References Audit

The chapter cites in-line but does not maintain a separate References section. Adding one is recommended for student/teacher use. The citations relied upon (in order of first appearance):

1. Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö., & Mariman, R. (2025). Generative AI without guardrails can harm learning: Evidence from high school mathematics. *PNAS*, 122. [DOI](https://www.pnas.org/doi/10.1073/pnas.2422633122)
2. Bjork, R. A., & Bjork, E. L. (1992). A new theory of disuse and an old theory of stimulus fluctuation. In Healy, Kosslyn, & Shiffrin (Eds.), *From Learning Processes to Cognitive Processes* (Vol. 2, pp. 35–67).
3. Bjork, E. L., & Bjork, R. A. (2011). Making things hard on yourself, but in a good way: Creating desirable difficulties to enhance learning. In Gernsbacher et al. (Eds.), *Psychology and the Real World* (pp. 56–64). [PDF](https://bjorklab.psych.ucla.edu/wp-content/uploads/sites/13/2016/04/EBjork_RBjork_2011.pdf)
4. Roediger, H. L., & Karpicke, J. D. (2006). Test-enhanced learning. *Psychological Science*, 17(3), 249–255. [DOI](https://doi.org/10.1111/j.1467-9280.2006.01693.x)
5. Roediger, H. L., & Karpicke, J. D. (2006). The power of testing memory. *Perspectives on Psychological Science*, 1(3), 181–210. [DOI](https://doi.org/10.1111/j.1745-6916.2006.00012.x)
6. Karpicke, J. D., & Blunt, J. R. (2011). Retrieval practice produces more learning than elaborative studying with concept mapping. *Science*, 331(6018), 772–775. [DOI](https://doi.org/10.1126/science.1199327)
7. Fiorella, L., & Mayer, R. E. (2016). Eight ways to promote generative learning. *Educational Psychology Review*, 28(4), 717–741. [DOI](https://doi.org/10.1007/s10648-015-9348-9)
8. Lachner, A., Ly, K.-T., & Nückles, M. (2018). Providing written or oral explanations? *Journal of Experimental Education*, 86(3), 344–361. [DOI](https://doi.org/10.1080/00220973.2017.1363691) — **but direction in chapter is inverted; see E13.**
9. Lachner, A., Jacob, L., & Hoogerheide, V. (2021). Learning by writing explanations: Is explaining to a fictitious student more effective than self-explaining? *Learning and Instruction*, 74, Article 101438. [DOI](https://doi.org/10.1016/j.learninstruc.2020.101438) — **but direction in chapter is inverted; see E14.**
10. Ericsson, K. A., Krampe, R. Th., & Tesch-Römer, C. (1993). The role of deliberate practice in the acquisition of expert performance. *Psychological Review*, 100(3), 363–406. [PsycNet](https://psycnet.apa.org/record/1993-40718-001)
11. Macnamara, B. N., Hambrick, D. Z., & Oswald, F. L. (2014). Deliberate practice and performance. *Psychological Science*, 25(8), 1608–1618. [DOI](https://doi.org/10.1177/0956797614535810)
12. UNESCO. (2024). *AI Competency Framework for Students*. [UNESCO](https://www.unesco.org/en/articles/ai-competency-framework-students)
13. AI4K12 Initiative. *Five Big Ideas in AI*. [ai4k12.org](https://ai4k12.org/)
14. McMurtrie, B. *Teaching* newsletter, *Chronicle of Higher Education* (various 2025–2026 issues). [Author page](https://www.chronicle.com/author/beth-mcmurtrie) — **no specific dated piece anchors the paraphrase; see C-CUR1.**

---

## Reliability assessment

The chapter is well-researched and epistemically honest, with a few citation-direction errors that look like the kind of mistake that happens when a draft is built from notes rather than from re-reading the cited papers. The Bastani unit error, the two inverted Lachner directions, and the Fiorella & Mayer list discrepancy are correctable in 30 minutes by a careful pass over the four cited papers. The framework and pedagogy of the chapter survive the corrections intact.
