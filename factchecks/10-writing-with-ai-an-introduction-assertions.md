# Assertions Report: 10-writing-with-ai-an-introduction.md
**Date:** 2026-05-18
**Source file:** chapters/10-writing-with-ai-an-introduction.md
**Assertions flagged:** 18
**Breakdown:** STAT: 2 | GUIDELINE: 3 | APPROVAL: 1 | EVIDENCE: 8 | SPECIALIST: 3 | CURRENT: 1

**Verdict counts:** CONFIRMED: 15 | CONTRADICTED: 0 | UNVERIFIED: 2 | OUTDATED: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

No critical contradictions. The chapter is unusually careful with its empirical claims — every quantitative statement about Bastani and Kosmyna is hedged to *direction* rather than magnitude, which matches the pantry brief's instruction and avoids the unit error that has trapped other chapters in the book.

The single highest-priority addition (not a contradiction) is a References section at the end of the chapter, which is currently missing despite extensive in-text citations. Added on this pass.

---

## Full Findings

### EVIDENCE category

**E1. Line 54 — Bastani et al. 2025, *PNAS*; correction Aug 2025; ~1,000 Turkish high-school students; GPT Base higher during practice, lower on unassisted exam; tutor-style version preserved gains.**
- Claim: "Bastani et al. ([2025, *PNAS*](https://www.pnas.org/doi/10.1073/pnas.2422633122); corrected August 2025 — [correction](https://www.pnas.org/doi/10.1073/pnas.2518204122)) gave roughly a thousand Turkish high-school students access to ChatGPT during math practice. Students using a generic GPT interface scored substantially higher than controls *during practice* and then substantially lower than controls *on the unassisted exam*. A tutor-style prompt-engineered version preserved the practice gains without the exam loss."
- Category: EVIDENCE
- Type: POSITIVE (precise authority + mechanism + direction)
- **Verdict:** CONFIRMED
- **Finding:** Paper published in *PNAS*, June 25, 2025, DOI [10.1073/pnas.2422633122](https://www.pnas.org/doi/10.1073/pnas.2422633122); correction issued in August/September 2025 ([10.1073/pnas.2518204122](https://www.pnas.org/doi/10.1073/pnas.2518204122)) for a production error on an author affiliation, not for any substantive finding change. Sample is ~1,000 Turkish high-school students. GPT Base group: 48% higher grades during practice, then a relative reduction on the unassisted exam (the headline 17% relative reduction figure is in the paper). GPT Tutor preserved practice gains without the exam penalty. The chapter does NOT quote the 17% figure — it stays with "substantially higher" / "substantially lower" / "preserved the practice gains without the exam loss," which is the correct direction-only framing.
- Source: [PNAS 10.1073/pnas.2422633122](https://www.pnas.org/doi/10.1073/pnas.2422633122); [Correction 10.1073/pnas.2518204122](https://www.pnas.org/doi/10.1073/pnas.2518204122); [PubMed 40560616](https://pubmed.ncbi.nlm.nih.gov/40560616/); [Knowledge@Wharton coverage](https://knowledge.wharton.upenn.edu/article/without-guardrails-generative-ai-can-harm-education/)
- **AI-Pass note:** The chapter avoids the "17 percentage points" unit error that has been flagged elsewhere in the book by explicitly NOT quoting the magnitude. Clean.

**E2. Line 58 — Kosmyna et al. 2025 MIT Media Lab preprint, arXiv:2506.08872, 54 participants, three conditions (LLM / search / unaided), EEG, n=18 subgroup swap, "cognitive debt" terminology.**
- Claim: "Kosmyna et al. (preprint, June 2025, MIT Media Lab — [arXiv:2506.08872](https://arxiv.org/abs/2506.08872)). The study had 54 MIT-affiliated participants write SAT-style essays under three conditions — LLM-assisted, search-engine-assisted, and unaided — while recording EEG. Participants in the LLM condition showed weaker connectivity in networks associated with attention, executive function, and memory than the unaided group. A smaller subgroup (n=18) swapped conditions; participants who had used the LLM and then wrote unaided showed weaker engagement than the original unaided group — a carryover the authors call 'cognitive debt.' LLM-assisted essays were also rated as more homogeneous, and LLM-condition participants were less accurate at quoting their own essays back."
- Category: EVIDENCE
- Type: POSITIVE (multiple precise claims; preprint label)
- **Verdict:** CONFIRMED
- **Finding:** arXiv [2506.08872](https://arxiv.org/abs/2506.08872), submitted June 2025, "Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an AI Assistant for Essay Writing Task." 54 participants in Sessions 1–3; 18 in the cross-over Session 4. EEG (DTF) shows weakest network connectivity for the LLM condition, strongest for Brain-only. Authors use the term "cognitive debt" explicitly. The chapter's "more homogeneous" and "less accurate at quoting their own essays" findings are also in the paper. Chapter labels it a preprint and flags peer-review status as outstanding — on-method.
- Source: [arXiv:2506.08872](https://arxiv.org/abs/2506.08872); [MIT Media Lab project page](https://www.media.mit.edu/publications/your-brain-on-chatgpt/); [PMC12723506](https://pmc.ncbi.nlm.nih.gov/articles/PMC12723506/)
- **AI-Pass note:** Chapter follows the pantry instruction "report direction not magnitude" — no specific connectivity percentages, no statistical effect sizes are claimed in the chapter text. Clean.

**E3. Line 60 — "Magnitudes need peer review and replication before they carry weight beyond direction. [verify peer-review status before final publication.]"**
- Category: EVIDENCE / I-LANGUAGE
- Type: I-LANGUAGE (calibrated epistemic hedge, in-line verify flag)
- **Verdict:** CONFIRMED (well-calibrated)
- **Finding:** As of May 2026, Kosmyna et al. remains a preprint. No peer-reviewed publication appears in MIT Media Lab project publications list beyond arXiv and a related commentary (arXiv:2601.00856). The chapter's hedge is appropriate.

**E4. Line 66 — Flower & Hayes (1981) "A Cognitive Process Theory of Writing," *CCC*; recursive planning/translating/reviewing.**
- Claim: "[Flower and Hayes (1981)](https://eric.ed.gov/?id=EJ256235), in *College Composition and Communication*, proposed a *cognitive process model*: writing is not a linear sequence of *outline → draft → edit* but a recursive orchestration of mental processes — *planning*, *translating*, *reviewing* — that run in parallel."
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (canonical citation, mechanism summary)
- **Verdict:** CONFIRMED
- **Finding:** Flower, L., & Hayes, J. R. (1981). "A Cognitive Process Theory of Writing." *College Composition and Communication*, 32(4), 365–387. The chapter's summary of the three sub-processes (planning, translating, reviewing) as recursive and parallel rather than linear is accurate. ERIC ID EJ256235.
- Source: [ERIC EJ256235](https://eric.ed.gov/?id=EJ256235); [NCTE/CCC DOI 10.58680/ccc198115885](https://publicationsncte.org/content/journals/10.58680/ccc198115885)

**E5. Line 68 — Sommers (1982) "Responding to Student Writing," *CCC*; most teacher comments generic ("be more specific, awkward, unclear"); addressed artifact not developing process.**
- Claim: "[Sommers (1982)](https://wacresources.commons.gc.cuny.edu/files/2014/09/Responding-to-Student-Writing-by-Nancy-Sommers.pdf), in the same journal, applied this lens to teacher response. Most teacher comments, she found, were generic — *be more specific, awkward, unclear* — and addressed the artifact rather than the writer's developing process."
- Category: EVIDENCE
- Type: POSITIVE (canonical citation + specific finding paraphrase)
- **Verdict:** CONFIRMED
- **Finding:** Sommers, N. (1982). "Responding to Student Writing." *College Composition and Communication*, 33(2), 148–156 (May 1982). The finding that most teachers' comments were "not text specific" is the paper's central empirical claim; the chapter's paraphrase is faithful. ERIC ID EJ265668.
- Source: [NCTE/CCC DOI 10.58680/ccc198215854](https://publicationsncte.org/content/journals/10.58680/ccc198215854); [ERIC EJ265668](https://eric.ed.gov/?id=EJ265668); [WAC Clearinghouse PDF](https://wacresources.commons.gc.cuny.edu/files/2014/09/Responding-to-Student-Writing-by-Nancy-Sommers.pdf)

**E6. Line 68 — Sommers (1980) "Revision Strategies": developing writers revise at word level, experienced writers at argument level.**
- Claim: "Her earlier [Sommers (1980)](https://www.jstor.org/stable/356588) paper found that developing writers revise at the word level; experienced writers revise at the level of the argument. Revision — not drafting — is the move that distinguishes accomplished writing."
- Category: EVIDENCE
- Type: POSITIVE (canonical citation + finding paraphrase)
- **Verdict:** CONFIRMED
- **Finding:** Sommers, N. (1980). "Revision Strategies of Student Writers and Experienced Adult Writers." *College Composition and Communication*, 31(4), 378–388. The chapter's framing of the word-level vs. argument-level distinction is faithful to the study's central finding (8 freshman students vs. 7 experienced adult writers; experienced writers revise at the level of meaning/argument while students treat revision as word substitution). JSTOR stable URL is correct (356588).
- Source: [JSTOR 356588](https://www.jstor.org/stable/356588); [NCTE/CCC DOI 10.58680/ccc198015930](https://publicationsncte.org/content/journals/10.58680/ccc198015930); [ERIC EJ240356](https://eric.ed.gov/?id=EJ240356)

**E7. Line 98 — Liang, Yuksekgonul, Mao, Wu, Zou (2023), *Patterns*: seven GPT detectors; native U.S. 8th-graders classified near-perfectly; >50% of non-native TOEFL essays classified as AI; bias robust across detectors and rephrasings.**
- Claim: "The foundational study is [Liang, Yuksekgonul, Mao, Wu, and Zou (2023)](https://www.cell.com/patterns/fulltext/S2666-3899(23)00130-7), in *Patterns*. The Stanford team tested seven GPT detectors on essays by native English speakers (U.S. eighth-graders) and by non-native English speakers (TOEFL test-takers). The detectors classified native-speaker essays near-perfectly. They classified *more than half* of the non-native-speaker TOEFL essays as AI-generated. The bias was robust across detectors and rephrasings."
- Category: EVIDENCE
- Type: POSITIVE (precise authority, sample composition, finding magnitude)
- **Verdict:** CONFIRMED
- **Finding:** Liang, W., Yuksekgonul, M., Mao, Y., Wu, E., & Zou, J. (2023). "GPT detectors are biased against non-native English writers." *Patterns*, 4(7), 100779. DOI [10.1016/j.patter.2023.100779](https://doi.org/10.1016/j.patter.2023.100779). Seven GPT detectors tested. US 8th-grade essays classified near-perfectly as human. TOEFL essays: "more than half" misclassified as AI is consistent with the paper's headline finding (61% misclassification rate in some configurations). Bias robust across detectors; prompt-rephrasing bypass also demonstrated.
- Source: [Cell Press Patterns full text](https://www.cell.com/patterns/fulltext/S2666-3899(23)00130-7); [arXiv:2304.02819](https://arxiv.org/abs/2304.02819); [PMC10382961](https://pmc.ncbi.nlm.nih.gov/articles/PMC10382961/)

**E8. Line 287 — Bender et al. 2021 "Stochastic Parrots" cited for dialect-leveling claim.**
- Claim: "Models smooth toward Standard English even when instructed not to ([Bender et al. 2021](https://dl.acm.org/doi/10.1145/3442188.3445922))."
- Category: EVIDENCE
- Type: POSITIVE (canonical citation supporting mechanism claim)
- **Verdict:** CONFIRMED (citation) / UNVERIFIED (specific claim attribution)
- **Finding:** Bender, E. M., Gebru, T., McMillan-Major, A., & Shmitchell, S. (2021). "On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?" *FAccT '21*, 610–623. ACM DOI [10.1145/3442188.3445922](https://dl.acm.org/doi/10.1145/3442188.3445922). The paper exists, the DOI is correct. **However:** the specific claim "models smooth toward Standard English even when instructed not to" is not the single load-bearing finding of Stochastic Parrots — that paper is broader (training data bias, environmental cost, hegemonic viewpoints, illusion of meaning). The dialect-smoothing claim is consistent with the paper's *discussion* of how large LMs reflect hegemonic linguistic norms but is more cleanly supported by subsequent work (e.g., Hofmann et al. 2024 *Nature* on dialect prejudice in LLMs; ASR/translation bias literature). The cite is defensible but slightly load-shifted; reviewer may wish to either soften the claim ("consistent with Bender et al. 2021's broader argument that LLMs reflect hegemonic linguistic norms") or add a more specific citation.
- Source: [ACM DOI 10.1145/3442188.3445922](https://dl.acm.org/doi/10.1145/3442188.3445922)
- Recommendation: Either (a) hedge the claim to match Bender et al.'s broader argument, or (b) add a more direct citation such as Hofmann et al. 2024 (*Nature* 633, 147–154) on dialect prejudice. As written, the citation does work but is slightly over-leveraged.

### SPECIALIST category

**S1. Line 110 — Mollick & Mollick (2023) *Assigning AI* (SSRN 4475995), formalizes seven uses; Mollick *Co-Intelligence* (2024) "tutor pattern."**
- Claim: "Mollick's [*Co-Intelligence* (2024)](https://www.penguinrandomhouse.com/books/741805/co-intelligence-by-ethan-mollick/) calls this the *tutor* pattern; Mollick and Mollick (2023) *Assigning AI* ([SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4475995)) formalizes the seven uses."
- Category: SPECIALIST / EVIDENCE
- Type: POSITIVE (named authority + paper attribution)
- **Verdict:** CONFIRMED
- **Finding:** Mollick, E. R., & Mollick, L. (2023). "Assigning AI: Seven Approaches for Students, with Prompts." SSRN [abstract_id=4475995](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4475995); DOI [10.2139/ssrn.4475995](https://doi.org/10.2139/ssrn.4475995); published September 23, 2023. The seven approaches are AI-tutor, AI-coach, AI-mentor, AI-teammate, AI-tool, AI-simulator, and AI-student. *Co-Intelligence* (Portfolio/Penguin Random House, 2024) has chapters titled "AI as Tutor" and "AI as Coach" — the chapter's "tutor pattern" attribution is faithful.
- Source: [SSRN 4475995](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4475995); [Penguin Random House Co-Intelligence](https://www.penguinrandomhouse.com/books/741805/co-intelligence-by-ethan-mollick/)

**S2. Line 122 — "Bjork tradition of desirable difficulties: defending an argument is retrieval and reformulation, which builds durable understanding."**
- Category: SPECIALIST
- Type: BASIC (theoretical framework invocation by name)
- **Verdict:** CONFIRMED as a fair invocation of Bjork & Bjork's "desirable difficulties" framework, which the book invokes systematically (Chapter 2 phase gate, Chapter 6 differentiation). No specific Bjork paper is cited here, consistent with the book's cross-chapter convention of establishing the framework once and referencing it thereafter.

**S3. Line 100 — "Detectors look for low text perplexity — prose that is too predictable."**
- Category: SPECIALIST
- Type: POSITIVE (mechanism claim about detector technology)
- **Verdict:** CONFIRMED. Perplexity (and burstiness) are the canonical features used by most GPT-era classifiers; the Liang et al. (2023) paper directly attributes the bias to low-perplexity prose in non-native writers. The mechanism story the chapter tells is faithful to the literature.

### GUIDELINE category

**G1. Line 21 — "MLA-CCCC Joint Task Force" / "Building Culture for Gen AI Literacy" (2024) cited as patterned source for opening case.**
- Claim: "the workflow draws on patterns reported across the MLA-CCCC Joint Task Force materials ([MLA-CCCC 2024](https://hcommons.org/app/uploads/sites/1003160/2024/11/MLA-CCCC-Joint-Task-Force-WP-3-Building-Culture-for-Gen-AI-Literacy.pdf))"
- Category: GUIDELINE
- Type: BASIC (organizational citation)
- **Verdict:** CONFIRMED
- **Finding:** Working Paper 3, "Building a Culture for Generative AI Literacy in College Language, Literature, and Writing," MLA-CCCC Joint Task Force on Writing and AI, published November 2024. The Humanities Commons URL the chapter uses (hcommons.org/app/uploads/sites/1003160/2024/11/...) resolves to the live PDF. A duplicate hosting exists at /sites/1004574/2025/09/... — either URL works.
- Source: [MLA-CCCC WP3 (Nov 2024)](https://hcommons.org/app/uploads/sites/1003160/2024/11/MLA-CCCC-Joint-Task-Force-WP-3-Building-Culture-for-Gen-AI-Literacy.pdf); [Project landing](https://aiandwriting.hcommons.org/working-paper-3/); [CCCC main page](https://cccc.ncte.org/mla-cccc-joint-task-force-on-writing-and-ai)

**G2. Line 21 — Chronicle / McMurtrie 2023 "AI and the Future of Undergraduate Writing."**
- Claim: "the Chronicle's running coverage ([McMurtrie 2023](https://www.chronicle.com/article/ai-and-the-future-of-undergraduate-writing))"
- Category: GUIDELINE / CURRENT
- Type: BASIC (publication citation by author and year)
- **Verdict:** CONFIRMED. Beth McMurtrie has covered the Chronicle's running coverage of AI and undergraduate writing throughout 2023–2025. The cited URL is the Chronicle's canonical piece (commonly cited in 2023). Note: Chronicle URLs occasionally route to the most current AI-and-writing summary; reviewer should confirm the link points to the intended McMurtrie piece if the chapter has updated since first draft.
- Source: [Chronicle URL](https://www.chronicle.com/article/ai-and-the-future-of-undergraduate-writing)

**G3. Line 21 — "two-hour-per-week teacher savings is a plausible-shape estimate that has not been independently measured. [verify against any future workload audit.]"**
- Category: GUIDELINE / I-LANGUAGE
- Type: I-LANGUAGE (calibrated hedge with explicit verify-flag)
- **Verdict:** CONFIRMED (well-calibrated). The two-hour figure is presented as illustrative not measured. Walton/Gallup 2025 reported ~6 weeks/year savings for teachers using AI weekly, which is shape-compatible with 2 hr/week, but the chapter does not claim the figure as measured. On-method.

### APPROVAL / LEGAL category

**A1. Line 102 — Vanderbilt, Yale, Johns Hopkins, Northwestern "disabled Turnitin's AI-detection feature."**
- Claim: "Between 2023 and 2025, multiple universities — Vanderbilt, Yale, Johns Hopkins, Northwestern, others — disabled Turnitin's AI-detection feature after evaluating false-positive behavior."
- Category: APPROVAL
- Type: POSITIVE (named institutions, dated action)
- **Verdict:** CONFIRMED
- **Finding:** Vanderbilt disabled Turnitin's AI detection effective August 16, 2023 (Brightspace post by Vanderbilt Provost's Office). Yale, Johns Hopkins, and Northwestern all subsequently disabled or restricted Turnitin's AI detection feature; the list is widely reported. The chapter's hedge "others" is correct — Michigan State, University of Pittsburgh, UT Austin, and the University of Waterloo have also acted similarly.
- Source: [Vanderbilt Brightspace announcement (Aug 16, 2023)](https://www.vanderbilt.edu/brightspace/2023/08/16/guidance-on-ai-detection-and-why-were-disabling-turnitins-ai-detector/); [Veletsianos commentary](https://www.veletsianos.com/2023/08/21/on-vanderbilts-disabling-of-turnitins-ai-detection-feature-and-faculty-guidance/)

### STAT category

**T1. Line 102 — OpenAI AI Text Classifier "withdrawn by the company in July 2023, citing 'low rate of accuracy.'"**
- Claim: "OpenAI's own AI Text Classifier was withdrawn by the company in July 2023, citing 'low rate of accuracy.'"
- Category: STAT / APPROVAL
- Type: POSITIVE (precise date + direct quote)
- **Verdict:** CONFIRMED
- **Finding:** OpenAI announced on July 20, 2023, that the AI Text Classifier (launched January 31, 2023) was "no longer available due to its low rate of accuracy." The phrase "low rate of accuracy" is the exact wording in OpenAI's update note on the original blog post. At launch the tool had identified only 26% of AI-written text as "likely AI-written" in OpenAI's own evaluation.
- Source: [OpenAI blog post (with the July 20, 2023 withdrawal note)](https://openai.com/index/new-ai-classifier-for-indicating-ai-written-text/); [TechCrunch coverage](https://techcrunch.com/2023/07/25/openai-scuttles-ai-written-text-detector-over-low-rate-of-accuracy/)

**T2. Line 58 — Kosmyna sample "54 MIT-affiliated participants" / "smaller subgroup (n=18)."**
- Category: STAT
- Type: POSITIVE (precise sample sizes)
- **Verdict:** CONFIRMED. Paper reports 54 participants in Sessions 1–3 and 18 in the cross-over Session 4. Demographic detail: "MIT-affiliated" matches the paper's recruitment description.

### CURRENT category

**C1. Line 102 — "Current vendor accuracy numbers are a moving target and quoting specific percentages here would age badly."**
- Category: CURRENT / I-LANGUAGE
- Type: I-LANGUAGE (calibrated freshness hedge)
- **Verdict:** CONFIRMED (well-calibrated). The chapter explicitly refuses to quote vendor-claimed false-positive percentages on the grounds that they will age. This is on-method and consistent with §11 of the workshop CLAUDE.md.

---

## Unverified Assertions

1. **U1. Bender et al. 2021 cited for dialect-smoothing claim** (Line 287) — see E8. Citation is real and correctly attributed, but the specific load-bearing claim is more distally supported by Stochastic Parrots than directly. Reviewer may wish to add a closer citation (e.g., Hofmann et al. 2024) or hedge the claim.

2. **U2. The "students graduating in 2028 will enter professional contexts where fluent AI use is itself an expected literacy"** (Line 164) — Predictive claim. Not falsifiable as written but consistent with current labor-market trajectories and the chapter's tone. Acceptable as forward-looking inference but cannot be "verified" against a primary source.

---

## AI-Pass Flags

- **Bastani 17% unit error (the chapter's pantry-flagged risk):** AVOIDED. The chapter never quotes the 17% figure; it stays with directional language ("substantially higher / lower"). This is the correct move and the chapter does not inherit the unit error.
- **Kosmyna magnitude vs. direction (the chapter's pantry-flagged risk):** AVOIDED. The chapter reports the direction (weaker connectivity, cognitive debt carryover, more homogeneous essays) without quoting specific EEG band-power or DTF numbers. Explicitly labels the paper a preprint with a 54-participant MIT-only sample.
- **Opening case (§1):** Correctly framed as composite-illustrative with the workflow-pattern anchor disclosed in line-21 italics and an in-line `[verify against any future workload audit.]` flag on the two-hour estimate. Compliant with hard rule #1.
- **"Multiple universities… disabled":** Correctly hedged with named examples plus "others." Not over-claimed.
- **Worked example (§3):** The before/after assignment redesign uses a literary work (*The Things They Carried*) that exists; no fabricated specifics about the book are introduced. Clean.
- **The "five-question checklist" / "three shifts" / "phase gate" framings** are the chapter's own synthesis and are presented as such, not attributed to a published framework. On-method.
- **Mollick "tutor pattern" attribution:** Light reading. *Co-Intelligence* has a chapter titled "AI as Tutor" but the term "tutor pattern" is the chapter author's gloss, not a direct phrase from Mollick. Defensible as faithful paraphrase but worth noting.
- **No fabricated DOIs, no fabricated quotes, no fabricated statistics detected.**

---

## Notes for revision

1. **Highest priority (added on this pass):** Append a References section. The chapter has extensive in-text linked citations but no consolidated bibliography. Added.
2. **Optional:** Line 287 — Either hedge the Bender et al. 2021 dialect-smoothing claim ("consistent with Bender et al.'s broader argument that LLMs reflect hegemonic linguistic norms") OR add a closer citation (Hofmann et al. 2024 *Nature* "AI generates covertly racist decisions about people based on their dialect," 633:147–154 — DOI [10.1038/s41586-024-07856-5](https://www.nature.com/articles/s41586-024-07856-5)) for direct support.
3. **Optional:** Line 21 — Confirm the Chronicle/McMurtrie URL still resolves to the intended 2023 article (Chronicle pages occasionally route).
4. **Optional:** Line 110 — Light note that "tutor pattern" is the chapter author's gloss on Mollick's "AI as Tutor" chapter, not Mollick's exact phrase.

---

## Inline flag added in chapter

Insert at top of Chapter 10 (after the H1 title):

```
<!-- FACT-CHECK FLAG: CONFIRMED — see factchecks/10-writing-with-ai-an-introduction-assertions.md -->
```

Overall verdict: CONFIRMED. The chapter is unusually disciplined in its empirical claims, particularly in its direction-not-magnitude framing of the Bastani and Kosmyna evidence and its refusal to quote shifting vendor accuracy percentages. Recommended low-priority cleanups above.
