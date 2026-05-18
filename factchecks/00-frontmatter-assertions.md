# Assertions Report: 00-frontmatter.md

**Date:** 2026-05-18
**Source file:** chapters/00-frontmatter.md
**Assertions flagged:** 10
**Breakdown:** STAT: 2 | GUIDELINE: 0 | APPROVAL: 0 | EVIDENCE: 6 | SPECIALIST: 2 | CURRENT: 0

---

## Critical — Requires Immediate Expert Review

### EVIDENCE — CONTRADICTED
**Assertion type:** COMBINATION (positive + specific number)
**Sentence:** "The Bastani et al. (2025) study that appears throughout this book is the clearest demonstration: students who used AI during math practice scored 48% higher than the control group during the practice session, then scored 17 percentage points lower on the exam without AI."
**Claim checked:** The "17 percentage points lower" figure attributed to Bastani et al. (2025).
**Site visited:** https://www.pnas.org/doi/10.1073/pnas.2422633122 (and corroborating Wharton/Bastani working-paper coverage)
**Finding:** Bastani et al. report a **17% relative reduction** in exam grades for the GPT Base arm vs. control, not a **17 percentage-point** drop. These are different magnitudes — a 17% relative reduction on a baseline grade of ~50 would be roughly 8.5 percentage points, not 17. The 48% practice-session improvement is correctly stated (also a relative figure). The unit mismatch is a precision error that the chapter repeats elsewhere; recommend fixing throughout the book or recasting as "17% lower."
**Expert review needed:** Yes — affects every chapter that cites this number.
**Suggested reference:** Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö., & Mariman, R. Generative AI without guardrails can harm learning: Evidence from high school mathematics. PNAS, 2025. https://www.pnas.org/doi/10.1073/pnas.2422633122
**Notes:** The directional finding (practice improvement, exam regression) is correct and well-supported. Only the unit of the exam-side effect is mis-stated.

---

## Full Findings

### EVIDENCE — CONFIRMED
**Assertion type:** POSITIVE
**Sentence:** "students who used AI during math practice scored 48% higher than the control group during the practice session"
**Claim checked:** 48% practice-session improvement for the GPT Base / unfettered-access arm.
**Site visited:** https://www.pnas.org/doi/10.1073/pnas.2422633122 (and Wharton coverage)
**Finding:** Confirmed. Bastani et al. report a 48% improvement in practice-problem grades for the GPT Base arm vs. control (with 127% for the GPT Tutor arm). Phrased as a relative percentage gain, consistent with the source's wording.
**Expert review needed:** No
**Suggested reference:** Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö., & Mariman, R. Generative AI without guardrails can harm learning: Evidence from high school mathematics. PNAS, 2025. https://www.pnas.org/doi/10.1073/pnas.2422633122
**Notes:** None.

### SPECIALIST — CONFIRMED
**Assertion type:** POSITIVE
**Sentence:** "When you encounter material that genuinely challenges your current understanding — something that doesn't fit what you already know, that requires you to update your mental model — a cascade of neurological events occurs. Dopamine signals the prediction error. Synaptic connections strengthen. New structures form. Memory consolidates over hours and days."
**Claim checked:** Dopamine prediction-error signaling, synaptic strengthening, and time-dependent memory consolidation as the mechanism of learning following surprise/error.
**Site visited:** https://www.pnas.org/doi/10.1073/pnas.1014269108 (Glimcher, Understanding dopamine and reinforcement learning); https://pmc.ncbi.nlm.nih.gov/articles/PMC6625913/ (positive reward prediction errors strengthen memory encoding)
**Finding:** Confirmed at the level of generality the preface uses. Phasic midbrain-dopamine activity encodes reward prediction error and modulates synaptic plasticity in basal-ganglia and cortical circuits; reward prediction errors strengthen hippocampal-dependent memory encoding; systems consolidation proceeds over hours to days. The preface compresses several distinct literatures (RL/dopamine, LTP, systems consolidation) into one paragraph — defensible as a preface-level summary but not a precise mechanistic claim for any single study.
**Expert review needed:** No, at preface level. Yes if Appendix G makes stronger claims.
**Suggested reference:** Glimcher, P. W. Understanding dopamine and reinforcement learning: The dopamine reward prediction error hypothesis. PNAS, 2011. https://www.pnas.org/doi/10.1073/pnas.1014269108
**Notes:** "Prediction error" in the dopamine literature is specifically *reward* prediction error. The preface conflates it with the broader sense of "expectation violation," which is reasonable in a pedagogical text but is a known simplification.

### EVIDENCE — CONFIRMED
**Assertion type:** POSITIVE
**Sentence:** "They perform better during the practice session — the AI produces correct answers faster than they could. They perform worse on the subsequent test — because the struggle that would have produced learning never occurred."
**Claim checked:** The general pattern of better practice / worse test outcomes when AI does the cognitive work.
**Site visited:** https://www.pnas.org/doi/10.1073/pnas.2422633122
**Finding:** Confirmed by the Bastani et al. (2025) RCT (n≈1,000 Turkish high-school students) and consistent with the broader desirable-difficulties literature (Bjork). The directional claim is well-supported by at least one large-scale RCT.
**Expert review needed:** No
**Suggested reference:** Bastani, H., et al. Generative AI without guardrails can harm learning. PNAS, 2025. https://www.pnas.org/doi/10.1073/pnas.2422633122
**Notes:** None.

### SPECIALIST — UNVERIFIED
**Assertion type:** POSITIVE
**Sentence:** "The student who genuinely grappled with a concept takes more time on harder problems. Makes errors that follow the structure of the concept — wrong in ways that reveal a developing mental model rather than random guessing. Shows improvement when given a hint that activates partial understanding. Remembers the material two weeks later when tested without warning."
**Claim checked:** That these specific "process friction" signatures (time-on-task, structured-error patterns, hint responsiveness, delayed retention) reliably distinguish genuine learners from AI-assisted artifact producers.
**Site visited:** Could not locate a single source that operationalizes all four signatures jointly as a discriminative test.
**Finding:** Each individual signature is grounded in cognitive-science work (time-on-task: think-aloud / response-time literature; structured errors: misconception/diagnostic-assessment work; hint-response: dynamic assessment / Vygotsky zone-of-proximal-development; delayed retention: Roediger & Karpicke spacing/testing). But the chapter's framing — that these jointly identify "the struggle" as biological — is the author's synthesis. The preface notes Appendix G provides the formal framework; that is where the discriminative-validity claim needs to be checked, not here.
**Expert review needed:** Yes — verify in Appendix G that the listed signatures are presented as candidate indicators, not validated discriminators.
**Suggested reference:** Roediger, H. L., & Karpicke, J. D. Test-enhanced learning. Psychological Science, 2006. (For delayed retention component.) Could not identify a single source for the conjunction.
**Notes:** Preface is making a compressed argumentative claim; full vetting belongs to Appendix G.

### EVIDENCE — UNVERIFIED
**Assertion type:** EMPHATIC
**Sentence:** "This is not a temporary problem that better AI detection will solve. The tools that identify AI-generated writing are trained on today's outputs. Tomorrow's outputs will be different. The arms race between generation and detection has a predictable winner."
**Claim checked:** That AI-detection tools are structurally unable to keep up with generation.
**Site visited:** Not searched directly (interpretive claim).
**Finding:** This is an argumentative position widely held but not formally settled. Studies of detector accuracy (e.g., GPTZero, Turnitin AI detection) show degradation as models change and high false-positive rates on non-native English writers. The "predictable winner" framing is rhetoric, not a verified empirical claim. Defensible as preface-level argument; flagging as UNVERIFIED rather than CONTRADICTED.
**Expert review needed:** No (interpretive)
**Suggested reference:** Liang, W., Yuksekgonul, M., Mao, Y., Wu, E., & Zou, J. GPT detectors are biased against non-native English writers. Patterns (Cell Press), 2023. https://www.cell.com/patterns/fulltext/S2666-3899(23)00130-7
**Notes:** Consider softening to "the empirical record so far" rather than "predictable winner."

### EVIDENCE — CONFIRMED
**Assertion type:** BASIC
**Sentence:** "AI is genuinely excellent at the tasks that do not require the learner's cognitive struggle. Drafting the structure so the teacher can teach rather than format. Generating practice problems calibrated to the student's current level. Asking Socratic questions that push thinking rather than providing answers. Producing ten versions of a differentiated material so the teacher can select rather than produce from scratch. Providing immediate feedback on a first draft so revision becomes the cognitive work rather than the entire process."
**Claim checked:** That LLMs can perform these specific tasks well.
**Site visited:** anthropic.com / openai.com product documentation (general knowledge of current model capabilities, May 2026).
**Finding:** Consistent with documented capabilities of frontier models (Claude, GPT-4 class, Gemini) for lesson scaffolding, differentiated content generation, Socratic prompting, and formative feedback. "Genuinely excellent" is an editorial register but the underlying capability claim is supported.
**Expert review needed:** No
**Suggested reference:** Could not identify a single source — this is a survey-level claim that maps to vendor documentation and the practitioner literature (e.g., TeachAI, ISTE guidance).
**Notes:** None.

### EVIDENCE — CONFIRMED
**Assertion type:** BASIC
**Sentence:** "Generative AI severed this connection. A well-structured essay can now be produced in seconds by a system that has performed none of the cognitive work the essay was designed to demonstrate."
**Claim checked:** That generative AI can produce a well-structured essay in seconds.
**Site visited:** anthropic.com / openai.com product documentation.
**Finding:** Confirmed. Frontier LLMs reliably produce structured prose at the multi-paragraph essay length in seconds. This is a basic and uncontroversial capability claim as of 2026.
**Expert review needed:** No
**Suggested reference:** Could not identify a single source — this is a widely documented baseline capability.
**Notes:** None.

### STAT — UNVERIFIED
**Assertion type:** POSITIVE
**Sentence:** "The six hours a week this book aims to return to you are six hours of preparation that does not require your professional judgment."
**Claim checked:** "Six hours a week" as an empirical target.
**Site visited:** walton.org / gallup.com (general teacher-AI-time-savings reports).
**Finding:** Gallup/Walton (2025) reported teachers using AI weekly save an average of ~5.9 hours per week. The "six hours" figure is consistent with that finding (rounded). The preface uses the number as a book-wide promise rather than citing a source; this is defensible since the source is elaborated in Chapter 1, but the unverified-here status flags it for cross-checking against Chapter 1's citation.
**Expert review needed:** No — verify Chapter 1 carries the citation.
**Suggested reference:** Gallup & Walton Family Foundation. Teaching with AI: A 2025 Status Report. Walton Family Foundation, 2025. https://www.waltonfamilyfoundation.org/learning/teaching-with-ai-a-2025-status-report
**Notes:** Preface use is fine; ensure the source is named where the number is first introduced in the body.

### EVIDENCE — UNVERIFIED
**Assertion type:** BASIC
**Sentence:** "And for the high schooler who wrote: 'My friends are using AI to write their papers but I want to use AI to learn and I don't know how.' This book is one answer."
**Claim checked:** Authenticity of the quoted student message.
**Site visited:** Not externally verifiable.
**Finding:** Personal-correspondence quote attributed to the author's experience. Not subject to web verification. Flagging only because hard rule #1 (no fabricated quotes) requires that quotes correspond to real source material; the author should confirm the quote is verbatim and from a real exchange.
**Expert review needed:** Author confirmation only.
**Suggested reference:** N/A — personal correspondence.
**Notes:** If paraphrased rather than verbatim, recommend reformatting without quote marks.

---

## Unverified Assertions

| Sentence | Category | Assertion Type | Reason unverified |
|---|---|---|---|
| "The arms race between generation and detection has a predictable winner." | EVIDENCE | EMPHATIC | Rhetorical/predictive; empirical record consistent but not settled. |
| "The student who genuinely grappled with a concept takes more time on harder problems... [four-signature list]" | SPECIALIST | POSITIVE | Each signature is grounded individually; the joint discriminative claim belongs to Appendix G. |
| "Six hours a week this book aims to return to you" | STAT | POSITIVE | Source named in Chapter 1, not in preface. |
| "And for the high schooler who wrote: '...'" | EVIDENCE | BASIC | Personal correspondence — author confirmation only. |

---

## AI-Pass Flags

**Unit mismatch on Bastani exam-effect figure.** The preface says "17 percentage points lower on the exam." Bastani et al. report a "17% reduction in grades" — a relative percentage, not a percentage-point difference. A 17% reduction on a typical control grade is roughly 8 percentage points, not 17. This is the highest-priority correction in the file and likely propagates elsewhere in the book. Recommend either (a) recast as "17% lower on the exam" or (b) report the underlying mean exam scores so the unit is unambiguous.

**Definition drift on "prediction error."** The preface uses "prediction error" in two senses without distinguishing them: (1) the technical reward-prediction-error signal in the dopamine literature, which is about reward, not arbitrary expectation violation; (2) the broader pedagogical sense of "your expectation didn't match what you encountered." This is a defensible compression for a preface but the chapter and Appendix G should be checked for consistency.

**Internal pointer.** References "Appendix G" — confirm the appendix exists in the back matter; if not yet drafted, flag as forward-reference TODO.
