# Assertions Report: 03-prompting-that-works.md

**Date:** 2026-05-18
**Source file:** chapters/03-prompting-that-works.md
**Assertions flagged:** 18
**Breakdown:** STAT: 0 | GUIDELINE: 2 | APPROVAL: 4 | EVIDENCE: 7 | SPECIALIST: 4 | CURRENT: 1

---

## Critical — Requires Immediate Expert Review

### C1. Anthropic guidance misrepresented (CONTRADICTED) — §3.3.1

**Quote:** "Anthropic's own guidance is explicit that telling the model what *not* to do — and stating downstream use — improves adherence and reduces drift."

**Type:** COMBINATION (Emphatic + Positive + Approval/Specialist)
**Category:** APPROVAL
**Verdict:** CONTRADICTED

**Finding:** Anthropic's actual prompt engineering documentation says the OPPOSITE. The official "Prompting best practices" page (platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices) advises that *positive* examples and instructions ("tell Claude what to do") are *more* effective than negative ones ("tell Claude what not to do"). The chapter's later §3.3.4 actually concedes a version of this ("a negative constraint works best when paired with a positive direction"), but the §3.3.1 framing of Anthropic's guidance as "explicit" that negatives improve adherence misrepresents the source. The chapter should be revised to say something like "Anthropic recommends positive framings, but allows that negative constraints can sharpen output when paired with positive direction."

**Source:** https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices

---

### C2. Misattributed authorship of K-12 STEM systematic review (CONTRADICTED) — §3.6

**Quote:** "The closest systematic reviews are Hsiao et al. (2024) on K-12 STEM ([arXiv 2410.11123](https://arxiv.org/abs/2410.11123))..."

**Type:** COMBINATION (Positive + Evidence)
**Category:** EVIDENCE
**Verdict:** CONTRADICTED

**Finding:** arXiv 2410.11123 — "A Systematic Review on Prompt Engineering in Large Language Models for K-12 STEM Education" — is authored by **Eason Chen, Danyang Wang, Luyi Xu, Chen Cao, Xiao Fang, and Jionghao Lin**. There is no author named "Hsiao" on this paper. The citation should read "Chen et al. (2024)" not "Hsiao et al. (2024)."

**Source:** https://arxiv.org/abs/2410.11123

---

## Full Findings

### F1. Liu et al. 2023 — "Pre-train, Prompt, and Predict" (CONFIRMED) — §3.3

**Quote:** "...a generic mix of trivia at an unspecified grade level in an unspecified format ([Liu et al., 2023](https://arxiv.org/abs/2107.13586))."

**Type:** BASIC (Evidence citation)
**Category:** EVIDENCE
**Verdict:** CONFIRMED

**Finding:** arXiv 2107.13586 by Pengfei Liu, Weizhe Yuan, Jinlan Fu, Zhengbao Jiang, Hiroaki Hayashi, Graham Neubig — "Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing." Published in ACM Computing Surveys (2023). Title, ID, and year all correct. However, this is a survey of prompt-based learning methods; it does not directly support the specific claim about "average of training data for those keywords." The citation is to a generally relevant paper but the inline support is loose. Recommend a more targeted citation or softening the inline attribution.

---

### F2. Four-component template framework attribution (UNVERIFIED, but acceptable framing) — §3.3.1

**Quote:** "Different people call it different things — CO-STAR, PAST, PLFR, role-task-format — but the structure underneath is the same. This book uses four components because four is enough."

**Type:** POSITIVE
**Category:** GUIDELINE
**Verdict:** PARTIAL CONFIRMATION / UNVERIFIED

**Finding:** CO-STAR is verifiable — developed by GovTech Singapore's Data Science and AI Division (Context, Objective, Style, Tone, Audience, Response). "Role-task-format" is a generic descriptor in common use. "PAST" and "PLFR" are not well-attested prompt engineering frameworks in the literature; web search returns no canonical sources for these acronyms as prompting frameworks. Consider either citing each acronym's origin or dropping the unverified ones. The book's own four-component framework (role/context/task/constraints) is **not** misattributed — it is presented as the book's chosen structure, which is appropriate.

**Sources:** https://www.promptquorum.com/prompt-engineering/co-star-framework ; https://aipromptsx.com/prompts/frameworks/costar

---

### F3. Wei et al. 2022 chain-of-thought (CONFIRMED) — §3.5

**Quote:** "There is real evidence behind some of this — chain-of-thought prompting genuinely improves multi-step reasoning on sufficiently large models ([Wei et al., 2022](https://arxiv.org/abs/2201.11903))."

**Type:** EMPHATIC ("genuinely improves")
**Category:** EVIDENCE
**Verdict:** CONFIRMED

**Finding:** arXiv 2201.11903 by Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed Chi, Quoc V. Le, Denny Zhou. "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models." Title, arxiv ID, year all correct. Main claim — that CoT prompting improves reasoning on sufficiently large models — is the paper's central finding. The qualification "on sufficiently large models" matches the paper's emergence-with-scale claim.

---

### F4. Zheng et al. 2023 personas study (PARTIALLY CONFIRMED) — §3.6

**Quote:** "Zheng et al. (2023) ran a careful study across four LLM families and found that adding personas in the system prompt produced no improvement or small negative effects on objective-knowledge benchmarks ([Zheng et al., 2023, arXiv 2311.10054](https://arxiv.org/abs/2311.10054))."

**Type:** COMBINATION (Emphatic + Specialist + Evidence)
**Category:** EVIDENCE
**Verdict:** CONFIRMED (with minor caveat)

**Finding:** arXiv 2311.10054 by Mingqian Zheng, Jiaxin Pei, Lajanugen Logeswaran, Moontae Lee, David Jurgens. Current title: "When 'A Helpful Assistant' Is Not Really Helpful: Personas in System Prompts Do Not Improve Performances of Large Language Models" (v3; v1 had a different title). Findings: 4 LLM families, 162 roles, 2,410 factual questions, accepted to Findings of EMNLP 2024. The chapter's framing — "no improvement or small negative effects on objective-knowledge benchmarks" — is accurate to the paper's headline finding. CONFIRMED.

---

### F5. Anthropic prompt engineering documentation URL (CONFIRMED with minor inconsistency) — §3.3.3

**Quote:** "...start with a prompt, look at the output, refine ([Anthropic](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview); [OpenAI](https://platform.openai.com/docs/guides/prompt-engineering))."

**Type:** BASIC (Approval / Doc citation)
**Category:** APPROVAL
**Verdict:** CONFIRMED

**Finding:** Both URLs exist and load. Note: Anthropic's canonical URL has migrated to `platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview`; `docs.anthropic.com/en/docs/...` redirects. The chapter uses both URL forms (this section uses `docs.anthropic.com`; §3.3.1 and §3.3.5 use `platform.claude.com`). Consider standardizing on `platform.claude.com` since that is the current canonical host. Either URL resolves correctly.

---

### F6. OpenAI prompt engineering guide URL (CONFIRMED) — §3.3.3

**Type:** BASIC
**Category:** APPROVAL
**Verdict:** CONFIRMED

**Finding:** https://platform.openai.com/docs/guides/prompt-engineering exists and contains the iterate-and-refine guidance. The chapter's loose framing ("start with a prompt, look at the output, refine") is consistent with OpenAI's "iterate and refine" guidance.

---

### F7. NotebookLM grounding behavior (CONFIRMED) — §3.3.5

**Quote:** "NotebookLM is built for this. It grounds answers in the uploaded sources and cites passages. The trade-off: it is conservative — it will refuse to extrapolate beyond what you uploaded."

**Type:** COMBINATION (Positive + Specialist + Current)
**Category:** SPECIALIST
**Verdict:** CONFIRMED

**Finding:** NotebookLM's RAG-based architecture, source citations linking to specific passages, and source-grounded answer behavior are well-documented. The "refuses to extrapolate" framing is a reasonable practitioner-level description of NotebookLM's intentional grounding. Note: NotebookLM has gained some web/extended-source modes in 2025–2026; the "refuses to extrapolate beyond what you uploaded" claim may be more nuanced in current versions. Worth a light review for currency.

**Sources:** https://support.google.com/notebooklm/answer/16164461

---

### F8. Claude long-form drafting capability (UNVERIFIED) — §3.3.5

**Quote:** "Claude tends to produce longer, more structurally coherent first drafts and follows complex multi-part instructions reliably."

**Type:** EMPHATIC
**Category:** SPECIALIST
**Verdict:** UNVERIFIED

**Finding:** This is a practitioner-level claim, not directly supported by a benchmark or vendor doc. It's the kind of comparative model-capability claim the chapter itself flags as "going to be wrong within a year" (§3.3.5 intro). The framing as task-fit rather than ranking partially insulates the claim, but consider citing a comparative evaluation or softening to "in many practitioner reports."

---

### F9. ChatGPT conversational tuning claim (UNVERIFIED) — §3.3.5

**Quote:** "ChatGPT's conversational tuning makes turn-by-turn refinement feel fluid."

**Type:** POSITIVE
**Category:** SPECIALIST
**Verdict:** UNVERIFIED

**Finding:** Practitioner-level claim. No vendor doc or benchmark directly substantiates it. Soft claim, low risk.

---

### F10. Gemini in Classroom free to Workspace-for-Education educators (CONFIRMED) — §3.3.5

**Quote:** "Gemini in Classroom is free to Workspace-for-Education educators ([Google blog, 2024](https://blog.google/products-and-platforms/products/education/classroom-ai-features/))."

**Type:** POSITIVE
**Category:** APPROVAL / CURRENT
**Verdict:** CONFIRMED

**Finding:** Google's official blog post and subsequent Workspace Updates confirm that Gemini in Classroom is available at no cost to educators with Google Workspace for Education accounts. The cited URL resolves to the relevant Google blog post. As of 2025, Gemini in Classroom rolled out to all Workspace for Education editions.

**Sources:** https://blog.google/products-and-platforms/products/education/classroom-ai-features/ ; https://workspaceupdates.googleblog.com/2025/06/gemini-google-classroom-all-edu-editions.html

---

### F11. Qian (2025) systematic review (CONFIRMED) — §3.6

**Quote:** "...and Qian (2025) on education broadly ([SAGE](https://journals.sagepub.com/doi/10.1177/07356331251365189))..."

**Type:** BASIC
**Category:** EVIDENCE
**Verdict:** CONFIRMED

**Finding:** Yufeng Qian, "Prompt Engineering in Education: A Systematic Review of Approaches and Educational Applications," *Journal of Educational Computing Research*, Vol. 63, Issue 7-8, pp. 1782–1818, August 2025. DOI matches. Title, year, journal correct.

---

### F12. C3 D2.His.14.6-8 standard reference (UNVERIFIED) — §3.2

**Quote:** "It names the standard (C3 D2.His.14.6-8)."

**Type:** BASIC
**Category:** SPECIALIST
**Verdict:** UNVERIFIED (likely correct format)

**Finding:** The C3 Framework (College, Career, and Civic Life) does use the format "D2.His.x.y-z" for history standards by grade band. "D2.His.14.6-8" denotes Dimension 2, History, Standard 14, Grades 6-8 in the C3 framework. The exact existence of standard #14 in that grade band should be spot-checked against the C3 Framework document, but the citation format is consistent with the framework's conventions.

---

### F13. NGSS 5-LS1-1 standard reference (CONFIRMED) — §3.4

**Quote:** "Standard: NGSS 5-LS1-1 (support an argument that plants get the materials they need for growth chiefly from air and water)."

**Type:** BASIC
**Category:** SPECIALIST
**Verdict:** CONFIRMED

**Finding:** NGSS 5-LS1-1: "Support an argument that plants get the materials they need for growth chiefly from air and water." Verbatim match to the actual NGSS performance expectation for 5th grade.

---

### F14. Soil-as-food misconception for 5th graders (CONFIRMED) — §3.4

**Quote:** "The most common student misconception we need to address is that plants get their food from the soil."

**Type:** POSITIVE
**Category:** SPECIALIST
**Verdict:** CONFIRMED

**Finding:** Widely documented in science-education research as a persistent K-8 misconception. The NGSS 5-LS1-1 standard exists precisely to address it. Reasonable, well-attested claim.

---

### F15. Priestley 1771 experiment reference (CONFIRMED) — §3.4

**Quote:** "a primary source from Joseph Priestley's 1771 experiment on mice and plants."

**Type:** BASIC
**Category:** SPECIALIST
**Verdict:** CONFIRMED

**Finding:** Priestley's August 1771 bell-jar experiments with mint and mice are correctly dated and described.

**Sources:** https://www.acs.org/education/whatischemistry/landmarks/josephpriestleyoxygen.html

---

### F16. "Empirical research on teacher-specific prompting is thin" (CONFIRMED via reviews) — §3.6

**Type:** POSITIVE (concession, with field-level claim)
**Category:** EVIDENCE
**Verdict:** CONFIRMED

**Finding:** Both Chen et al. (2024) and Qian (2025) systematic reviews note that the empirical literature is young; Chen et al. screened 2,654 papers and retained 30. This supports the chapter's "thin" framing.

---

### F17. WIDA level 2 ELL designation (CONFIRMED) — §3.2, §3.4

**Quote:** "WIDA level 2"

**Type:** BASIC
**Category:** SPECIALIST
**Verdict:** CONFIRMED

**Finding:** WIDA proficiency levels 1–6 are a standard ELL framework. Level 2 ("Emerging") is the conventional descriptor. Accurate.

---

### F18. Claim that the prompt structure "is the part you carry forward" across model generations (UNVERIFIED) — §3.5

**Quote:** "The structure (role-context-task-constraints) is the part you carry forward; the wording is the part you re-tune."

**Type:** POSITIVE
**Category:** GUIDELINE
**Verdict:** UNVERIFIED

**Finding:** This is the chapter's own pedagogical claim — and it explicitly hedges in §3.8 by saying no RCT exists. The reflexive honesty in §3.8 ("if a trial showed the structure did not matter ... the chapter would need to be rewritten") is appropriate. Flag as a working claim that the chapter itself flags as untested.

---

## Unverified Assertions

- F2 (PAST, PLFR frameworks): not attested as canonical
- F8 (Claude long-form drafting): practitioner-level, no benchmark
- F9 (ChatGPT conversational tuning): practitioner-level
- F12 (C3 D2.His.14.6-8 exact existence): format correct, exact standard not spot-checked
- F18 (template durability across generations): chapter's own claim, flagged by chapter

## AI-Pass Flags

- C1 misrepresents Anthropic guidance — should be revised to match the actual "positive instructions are more effective than negative" stance, OR cite the specific Anthropic passage that supports the chapter's framing if one exists. This is a load-bearing claim in §3.3.1.
- C2 author misattribution — straightforward fix: "Chen et al. (2024)" not "Hsiao et al. (2024)."
- F5 inconsistent Anthropic URL hosts — standardize on `platform.claude.com/docs/...`.
- F2 — consider dropping or citing PAST and PLFR; the rhetorical move ("different people call it different things") holds with CO-STAR and role-task-format alone.

## Reliability Assessment

The chapter's load-bearing academic citations (Wei 2022, Zheng 2023, Liu 2023, Qian 2025) are accurate. The chapter's own framework is presented honestly as its own choice, not misattributed. The two consequential errors are (1) a **contradicted** characterization of Anthropic's prompt-engineering guidance on negative constraints, and (2) an **author misattribution** (Hsiao → Chen) on the K-12 STEM systematic review. Both are easy fixes. Practitioner-level vendor-comparison claims in §3.3.5 are appropriately hedged by the section's own framing about volatility. Overall reliability: high, with two specific corrections needed before publication.
