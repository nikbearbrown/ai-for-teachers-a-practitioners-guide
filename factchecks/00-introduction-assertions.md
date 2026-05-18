# Assertions Report: 00-introduction.md
**Date:** 2026-05-18
**Source file:** chapters/00-introduction.md
**Assertions flagged:** 14
**Breakdown:** STAT: 5 | GUIDELINE: 0 | APPROVAL: 0 | EVIDENCE: 6 | SPECIALIST: 2 | CURRENT: 1

---

## Critical — Requires Immediate Expert Review

None found. All load-bearing empirical anchors in the Introduction (Bastani 2025 numbers; Kosmyna 2025 EEG; Gallup/Walton 5.9 hours; NFER/EEF 31%; OpenAI classifier withdrawal; Vanderbilt Turnitin deactivation; Bastani PNAS correction date) are CONFIRMED to primary sources.

---

## Full Findings

### Assertion 1
- **Category:** STAT / EVIDENCE
- **Verdict:** CONFIRMED
- **Type:** BASIC + COMBINATION (two numbers anchoring the whole book)
- **Sentence:** "Students who used AI during math practice scored 48% higher than the control group during the practice session. They scored 17 percentage points lower on the exam."
- **Claim:** Bastani 2025 GPT-Base arm: +48% in practice, −17 pp on exam (vs control).
- **Site checked:** pnas.org (DOI 10.1073/pnas.2422633122), Wharton Knowledge summary, PubMed.
- **Finding:** Both numbers match the published paper. The GPT Base arm showed 48% improvement on practice problems and statistically significant 17-point decline on the (no-AI) final exam.
- **Expert review needed:** No.
- **Suggested reference:** Bastani H. et al. *Generative AI without guardrails can harm learning: Evidence from high school mathematics.* PNAS, 2025. https://www.pnas.org/doi/10.1073/pnas.2422633122
- **Notes:** This is the single most load-bearing claim of the book and it is solid.

### Assertion 2
- **Category:** EVIDENCE / STAT
- **Verdict:** CONFIRMED
- **Type:** BASIC + EMPHATIC ("the single result every teacher should carry")
- **Sentence:** "This is the Bastani et al. (2025) finding — n ≈ 1,000 Turkish high schoolers, two conditions, randomized…"
- **Claim:** n ≈ 1,000; Turkish high schoolers; randomized.
- **Site checked:** pnas.org, Wharton Knowledge, scribd of paper.
- **Finding:** Sample is reported as ~1,000 high-school math students in Turkey, randomized into three arms (control, GPT Base, GPT Tutor). The Introduction's phrasing "two conditions, randomized" is misleading — there were three arms, the third introduced later in the same paragraph. See AI-pass section.
- **Expert review needed:** No.
- **Suggested reference:** Bastani et al. 2025 PNAS (same as #1).

### Assertion 3
- **Category:** EVIDENCE / STAT
- **Verdict:** CONFIRMED
- **Type:** COMBINATION (numeric + specialist + emphatic)
- **Sentence:** "That arm scored 127% higher in practice *and* held its exam score."
- **Claim:** GPT Tutor arm: 127% better in practice, no significant deficit on the exam.
- **Site checked:** Bastani SSRN preprint, hamsabastani.github.io education_llm.pdf, Wharton summary.
- **Finding:** Confirmed. GPT Tutor arm = +127% in practice vs control; negative exam effect "essentially eradicated."
- **Expert review needed:** No.

### Assertion 4
- **Category:** EVIDENCE / SPECIALIST
- **Verdict:** CONFIRMED
- **Type:** COMBINATION (named-study + mechanism claim)
- **Sentence:** "…the Kosmyna MIT EEG data showed reduced neural connectivity during AI-assisted writing relative to unassisted writing."
- **Claim:** Kosmyna et al. MIT Media Lab EEG study found reduced brain connectivity in LLM-assisted writing condition.
- **Site checked:** media.mit.edu, arxiv.org/abs/2506.08872, PMC.
- **Finding:** Confirmed. The EEG analysis found Brain-only > Search > LLM in network strength; weaker alpha/theta in the LLM group. n=54.
- **Expert review needed:** No.
- **Suggested reference:** Kosmyna N. et al. *Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an AI Assistant for Essay Writing Task.* arXiv:2506.08872, 2025. https://arxiv.org/abs/2506.08872
- **Notes:** Note the paper is currently a preprint with a published commentary (arXiv:2601.00856) — chapter 13 should engage with the commentary; introduction's framing is fine.

### Assertion 5
- **Category:** STAT / EVIDENCE
- **Verdict:** CONFIRMED
- **Type:** BASIC + POSITIVE ("the floor")
- **Sentence:** "What the research actually says about teacher time savings (5.9 hours/week is the floor)…"
- **Claim:** 5.9 hours/week time savings figure from Gallup/Walton 2025.
- **Site checked:** waltonfamilyfoundation.org PDF, gallup.com poll/691967, EdSurge coverage.
- **Finding:** Confirmed. Teachers who use AI tools at least weekly estimate saving 5.9 hours per week on average; n=2,232 U.S. public K-12 teachers; March 18–April 11, 2025.
- **Expert review needed:** No.
- **Suggested reference:** Walton Family Foundation & Gallup. *Teaching for Tomorrow: Unlocking Six Weeks a Year With AI.* 2025. https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf
- **Notes:** The Introduction's framing of 5.9 hours as "the floor" is the author's interpretive move (chapter 1 details it). The 5.9 itself is accurate.

### Assertion 6
- **Category:** STAT
- **Verdict:** UNVERIFIED
- **Type:** BASIC (projection, not measurement)
- **Sentence:** "…what the systematic ceiling would look like (a projected 16.7 hours, not yet measured)."
- **Claim:** A 16.7-hour weekly ceiling exists as a projection.
- **Site checked:** Gallup/Walton report; web search.
- **Finding:** This appears to be the author's own projection (chapter 1 should document the derivation). The Introduction itself flags it as "projected, not yet measured" — honest labeling. Cannot verify against an external primary source because no such source exists; it's the book's own analytic move.
- **Expert review needed:** Cross-check chapter 1's derivation supports the 16.7 number.
- **Notes:** The honest "not yet measured" flagging means this is not a fact-check failure — it's an author projection labeled as such.

### Assertion 7
- **Category:** EVIDENCE / STAT
- **Verdict:** CONFIRMED
- **Type:** COMBINATION (named-study + quantitative)
- **Sentence:** "NFER/EEF RCT evidence anchors the time-savings claim."
- **Claim:** NFER/EEF Teacher Choices RCT (lesson prep using ChatGPT).
- **Site checked:** educationendowmentfoundation.org.uk, nfer.ac.uk, scale.stanford.edu.
- **Finding:** Confirmed. 259 Year 7/8 science teachers from 68 UK schools, 10-week trial, summer 2024. ChatGPT group spent 56.2 min vs 81.5 min/week (≈31% reduction in lesson-prep time). Quality unchanged per blinded panel review.
- **Expert review needed:** No.
- **Suggested reference:** NFER / Education Endowment Foundation. *ChatGPT in lesson preparation: A Teacher Choices Trial Evaluation Report.* 2024. https://www.nfer.ac.uk/publications/chatgpt-in-lesson-preparation-a-teacher-choices-trial/

### Assertion 8
- **Category:** EVIDENCE / SPECIALIST
- **Verdict:** CONFIRMED
- **Type:** BASIC (institutional event)
- **Sentence:** "…the chapter cites the institutional retreat (OpenAI withdrawing its AI text classifier in July 2023; Vanderbilt deactivating Turnitin's AI detection in August 2023)…"
- **Claim:** (a) OpenAI withdrew its AI text classifier in July 2023. (b) Vanderbilt deactivated Turnitin's AI detection in August 2023.
- **Site checked:** openai.com/index/new-ai-classifier-for-indicating-ai-written-text/, vanderbilt.edu/brightspace/2023/08/16/, TechCrunch, Search Engine Journal.
- **Finding:** (a) Confirmed — OpenAI added the "as of July 20, 2023, the AI classifier is no longer available" notice to its launch blog post. (b) Confirmed — Vanderbilt published "Guidance on AI Detection and Why We're Disabling Turnitin's AI Detector" on August 16, 2023.
- **Expert review needed:** No.
- **Suggested references:**
  - OpenAI. New AI classifier for indicating AI-written text (post with July 2023 update). https://openai.com/index/new-ai-classifier-for-indicating-ai-written-text/
  - Vanderbilt University, Brightspace. *Guidance on AI Detection and Why We're Disabling Turnitin's AI Detector.* August 16, 2023. https://www.vanderbilt.edu/brightspace/2023/08/16/guidance-on-ai-detection-and-why-were-disabling-turnitins-ai-detector/

### Assertion 9
- **Category:** EVIDENCE / SPECIALIST
- **Verdict:** CONFIRMED
- **Type:** BASIC + I-LANGUAGE ("named honestly in Chapter 13")
- **Sentence:** "The Bastani correction in August 2025 — affiliation-only, non-substantive — is named honestly in Chapter 13."
- **Claim:** A Bastani et al. PNAS correction was published in August 2025; it was affiliation-only.
- **Site checked:** pnas.org DOI 10.1073/pnas.2518204122, PubMed PMID 40833419.
- **Finding:** Confirmed. The August 26, 2025 correction (PNAS vol. 122, issue 34) updated Osbert Bastani's affiliation to "Department of Computer and Information Science, School of Engineering and Applied Science, University of Pennsylvania." Non-substantive — no numerical or methodological changes.
- **Expert review needed:** No.
- **Suggested reference:** Correction for Bastani et al., PNAS, August 2025. https://www.pnas.org/doi/10.1073/pnas.2518204122

### Assertion 10
- **Category:** SPECIALIST
- **Verdict:** CONFIRMED
- **Type:** BASIC (attribution of term)
- **Sentence:** "The slideument problem (Reynolds), Mayer's Redundancy Principle…"
- **Claim:** "Slideument" is Reynolds' term; "Redundancy Principle" is Mayer's.
- **Site checked:** garrreynolds.com, presentationzen.com (Reynolds' "Your moment of (slideument) Zen" 2008 post), Cambridge Handbook of Multimedia Learning (Mayer ed., Redundancy Principle chapter).
- **Finding:** Confirmed. Reynolds coined "slideument" (slide+document) in Presentation Zen materials; Mayer's Redundancy Principle is a standard entry in his Cambridge Handbook of Multimedia Learning and 12-Principles framework.
- **Expert review needed:** No.
- **Suggested references:**
  - Reynolds G. *Presentation Zen.* (slideument concept). https://www.presentationzen.com/presentationzen/2008/04/your-moment-of.html
  - Mayer R. E. (ed.) *The Cambridge Handbook of Multimedia Learning.* Cambridge University Press. (Redundancy Principle chapter.)

### Assertion 11
- **Category:** SPECIALIST
- **Verdict:** CONFIRMED (attribution); UNVERIFIED (exact phrasing as a quotable Cairo line)
- **Type:** BASIC (attribution)
- **Sentence:** "Cairo's 'compared with what?'"
- **Claim:** Alberto Cairo uses or popularized "compared with what?" as a data-viz heuristic.
- **Site checked:** realworlddatascience.net interview, storytellingwithdata.com, tableau.com Cairo "little gems" post, Cairo's books (How Charts Lie, The Truthful Art, The Art of Insight).
- **Finding:** Cairo is clearly the right attribution-zone for this kind of comparison-framing heuristic, but the specific quoted phrase "compared with what?" is more commonly traced to John Tukey ("The most important question is, 'compared to what?'") and Edward Tufte ("Compared to what?" as one of his canonical statistical-thinking questions). Cairo discusses comparison extensively but the exact phrasing as a Cairo line is not the strongest attribution. Recommend chapter 9 verify the original source.
- **Expert review needed:** Yes — verify in chapter 9 whether the phrase is Cairo's or whether it should be attributed to Tukey/Tufte with Cairo cited for the data-viz application.
- **Notes:** This is the one factual edge in the Introduction that warrants careful sourcing in chapter 9.

### Assertion 12
- **Category:** EVIDENCE / CURRENT
- **Verdict:** UNVERIFIED (framework name, not an external claim)
- **Type:** BASIC
- **Sentence:** "Twelve gates organize the practical work of this book."
- **Claim:** There are 12 phase gates.
- **Finding:** This is the book's own framework, not a citable external claim. Verifiable internally against chapter 2 and appendix G.
- **Expert review needed:** Internal consistency check — confirm chapter 2 enumerates exactly 12 gates.

### Assertion 13
- **Category:** EVIDENCE
- **Verdict:** CONFIRMED (institutional study type)
- **Type:** BASIC
- **Sentence:** "There was a third arm of the study, GPT Tutor, where students used a version of the AI built with phase gates that made it refuse to give direct answers."
- **Claim:** GPT Tutor arm had guardrails preventing direct answer-giving.
- **Site checked:** Bastani PNAS, hamsabastani.github.io.
- **Finding:** Confirmed. GPT Tutor was prompt-engineered to refuse direct solutions and instead provide Socratic/scaffolded hints. The Introduction's framing of these as "phase gates" is the book's terminological move — the underlying mechanism is correctly described.
- **Expert review needed:** No.

### Assertion 14
- **Category:** EVIDENCE / STAT
- **Verdict:** CONFIRMED (qualitative); minor framing nuance
- **Type:** I-LANGUAGE + EMPHATIC
- **Sentence:** "The difference between the arm that lost 17 points and the arm that did not was not how much AI the students used. It was where the AI was allowed to stop and where the human cognitive work had to begin."
- **Claim:** Both arms had similar AI usage volume; the difference was design (guardrails), not exposure.
- **Site checked:** Bastani SSRN / PNAS.
- **Finding:** Consistent with the paper's framing — the authors emphasize the same tool (GPT-4) with different scaffolding produced opposite outcomes. The paper does not, as far as the published abstract/main text shows, normalize on raw AI-interaction-minutes; the claim that "usage volume was similar" is the author's interpretive compression of the paper's main argument.
- **Expert review needed:** Chapter 13 should make sure the usage-volume comparison is explicitly supported in the paper or labeled as interpretation.
- **Notes:** Substantively correct; the precise empirical claim about usage equivalence is worth verifying in chapter 13's deeper treatment.

---

## Unverified Assertions

| Sentence | Category | Assertion Type | Reason unverified |
|---|---|---|---|
| "a projected 16.7 hours, not yet measured" (the 16.7-hour ceiling) | STAT | BASIC | Author's projection — flagged honestly in the text. Verify derivation in chapter 1. |
| "Twelve gates organize the practical work" | EVIDENCE | BASIC | Internal framework count, not externally citable. Verify chapter 2 enumerates 12. |
| "Cairo's 'compared with what?'" (exact phrasing attribution) | SPECIALIST | BASIC | Phrase more commonly attributed to Tukey / Tufte; Cairo cites the heuristic but is not its origin. Verify in chapter 9. |
| "two conditions, randomized" (in the Bastani sentence) | EVIDENCE | BASIC | Paper has three arms — see AI-pass. |

---

## AI-Pass Flags

**1. Internal contradiction — "two conditions" vs "third arm" in the Bastani description.**

The Introduction says: *"the Bastani et al. (2025) finding — n ≈ 1,000 Turkish high schoolers, two conditions, randomized"* and then in the same paragraph: *"There was a third arm of the study, GPT Tutor…"*

The Bastani paper randomizes students into **three** arms (control, GPT Base, GPT Tutor). "Two conditions, randomized" is inconsistent with "third arm." Recommend revising the first phrase to "three conditions, randomized" or "two treatment arms plus a control" for technical accuracy. The current phrasing reads like a setup-then-reveal but it's a small factual stumble.

**2. Minor framing — Kosmyna paper is a preprint with a published commentary.**

The Introduction calls it "the Kosmyna MIT EEG data." The paper is arXiv:2506.08872 (preprint, June 2025) hosted by MIT Media Lab — not peer-reviewed in a journal at time of this fact-check. A formal commentary (arXiv:2601.00856) raises methodological concerns. Chapter 13 should engage with the commentary; the Introduction is fine to cite the EEG finding directly but the "preprint" status is worth a sentence in chapter 13.

**3. Composite labeling — "Maya" and other composites are honestly flagged.**

The book's own phase-gate-4 commitment ("Anonymization") is honored in the Introduction itself. Maya is labeled composite. Good.

**4. Suggested wording fix.**

In "two conditions, randomized" → consider "three conditions, randomized" or "a control arm and two treatment arms, randomized."

---

*End of report.*
