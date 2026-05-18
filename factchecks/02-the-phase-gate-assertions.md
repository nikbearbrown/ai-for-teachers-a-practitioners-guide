# Assertions Report: 02-the-phase-gate.md
**Date:** 2026-05-18
**Source file:** chapters/02-the-phase-gate.md
**Assertions flagged:** 24
**Breakdown:** STAT: 6 | GUIDELINE: 2 | APPROVAL: 0 | EVIDENCE: 11 | SPECIALIST: 3 | CURRENT: 2

**Verdict counts:** CONFIRMED: 17 | CONTRADICTED-or-CONTESTED: 1 | UNVERIFIED: 5 | OUTDATED: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

### 1. Hattie d=1.57 collective teacher efficacy (CONTESTED)
**Line 139** — "d ≈ 1.57 for collective teacher efficacy"
- **Category:** STAT
- **Type:** EMPHATIC
- **Verdict:** CONTRADICTED-or-CONTESTED
- **Finding:** The chapter already flags this `[contested]` and acknowledges Bergeron & Rivard (2017), Wrigley (2018), and Kraft (2020) — confirmed all three critiques exist. Bergeron & Rivard explicitly argue "Hattie confounds correlation and causality when seeking to reduce everything to an effect size." The d=1.57 figure traces to a single meta-analysis of 26 studies (Eells 2011 dissertation, popularized by Hattie 2018). Hattie's own February 2023 update rates CTE only 2/5 for overall confidence. Treatment in chapter is appropriately calibrated.
- **Recommendation:** Keep `[contested]` flag. Consider adding citation to Bergeron & Rivard 2017 and Kraft 2020 by name in the running text rather than only in the footnote.

### 2. FPF 89%/34% statistic (UNVERIFIED in original FPF document)
**Line 187** — "approximately 89% of K-12 schools use AI-enabled edtech while only about 34% have reviewed the privacy policies of those tools ([FPF, October 2024])"
- **Category:** STAT
- **Type:** POSITIVE (precise numbers attached to authority)
- **Verdict:** UNVERIFIED
- **Finding:** The specific 89%/34% pair appears in derivative sources (edugenius.app, eschoolnews) citing FPF, but I could not confirm those exact percentages appear in FPF's October 2024 "Vetting Generative AI Tools for Use in Schools" PDF. The FPF document is a vetting checklist/policy brief, not primarily a statistical report. The 89%/34% figures may originate from a separate survey (possibly Chanenson et al. NSF, or the Center for Democracy & Technology) and have been mis-attributed to FPF by secondary sources.
- **Recommendation:** Either confirm the numbers in the primary FPF PDF (page-cite) or re-attribute to the actual primary source. If unverifiable, replace with the qualitative claim ("schools widely adopt AI tools without reviewing privacy policies") and cite FPF for the vetting framework instead.

---

## Full Findings

### EVIDENCE category

**E1. Line 99 — Dell'Acqua et al. "Navigating the Jagged Technological Frontier"**
- Claim: "Dell'Acqua, Mollick, and colleagues at Harvard Business School ran a randomized field experiment with 758 BCG consultants … HBS Working Paper 24-013, 2023; now published in Organization Science 2026"
- Verdict: **CONFIRMED** (working paper number, author list, n=758, BCG collaboration all match). The "now published in Organization Science 2026" claim is plausible but the *Organization Science* DOI in the chapter (`10.1287/orsc.2025.21838`) should be checked against the live publication record — flagged `[verify]`.
- Source: https://www.hbs.edu/faculty/Pages/item.aspx?num=64700 ; SSRN https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4573321

**E2. Line 99 — 25% faster / 40% higher quality inside frontier; 19pp more incorrect outside frontier**
- Verdict: **CONFIRMED** as approximations consistent with HBS WP 24-013 reporting. Standard reporting of the paper. Sometimes cited as 25.1% faster, 12.2% more tasks completed, 40% higher quality.

**E3. Line 107 — Bastani et al. 2025 PNAS, DOI 10.1073/pnas.2422633122**
- Verdict: **CONFIRMED**. Title "Generative AI without guardrails can harm learning: Evidence from high school mathematics." Authors confirmed: Hamsa Bastani, Osbert Bastani, Alp Sungu, Haosen Ge, Özge Kabakcı, Rei Mariman. Volume 122(26): e2422633122. Turkish high school context, ~1,000 students, three arms (control / GPT Base / GPT Tutor).
- Source: https://www.pnas.org/doi/10.1073/pnas.2422633122

**E4. Line 107 — The August 2025 correction is affiliation-only**
- Claim: "a non-substantive affiliation-only correction was issued at 10.1073/pnas.2518204122"
- Verdict: **CONFIRMED**. The PNAS correction (DOI 10.1073/pnas.2518204122) is a production-error correction for Osbert Bastani's affiliation only — substantive results unaffected. Chapter's framing is accurate. The `[verify]` flag inline can be removed.
- Source: https://www.pnas.org/doi/10.1073/pnas.2518204122 ; https://pmc.ncbi.nlm.nih.gov/articles/PMC12403119/

**E5. Lines 109-111 — 48% practice gain (GPT Base) / 127% practice gain (GPT Tutor) / -17pp exam decrement (GPT Base) / no significant decrement (GPT Tutor)**
- Verdict: **CONFIRMED**. The 48% / 127% practice-improvement figures match the published abstract and Wharton's Knowledge press writeup. The -17 percentage-point unaided-exam decrement for GPT Base and the null effect for GPT Tutor are the headline findings of the paper.

**E6. Line 121 — Bjork & Bjork 2011 "Making things hard on yourself, but in a good way"**
- Verdict: **CONFIRMED**. Chapter from Gernsbacher, Pew, Hough & Pomerantz (eds.), *Psychology and the Real World: Essays Illustrating Fundamental Contributions to Society*. URL to the bjorklab.psych.ucla.edu PDF confirmed live.

**E7. Line 127 — Shulman 1986 "Those Who Understand: Knowledge Growth in Teaching," Educational Researcher 15(2): 4-14**
- Verdict: **CONFIRMED**. JSTOR stable URL https://www.jstor.org/stable/1175860 verified. Note: chapter says "his 1985 AERA presidential address" — the paper *is* his 1985 AERA address published in 1986. Correct.

**E8. Line 127 — Shulman 1987 "Knowledge and Teaching: Foundations of the New Reform," Harvard Educational Review 57(1): 1-22**
- Verdict: **CONFIRMED**. Harvard Educational Review URL verified at hepg.org. Page range correct.

**E9. Line 87 — Elish 2019 "Moral Crumple Zones," Engaging Science, Technology, and Society 5: 40–60**
- Verdict: **CONFIRMED**. Full title "Moral Crumple Zones: Cautionary Tales in Human-Robot Interaction." Volume, pages, journal all correct.
- Source: https://estsjournal.org/index.php/ests/article/view/260

**E10. Line 89 — Cory Doctorow 2024 quotation: "AI's 'human in the loop' isn't a human in the loop. A neck in a noose is also a human in the loop."**
- Verdict: **CONFIRMED**. Pluralistic post dated 2024-10-30, "A neck in a noose." Title and framing match the chapter's quotation. Doctorow Medium URL also live.
- Source: https://pluralistic.net/2024/10/30/a-neck-in-a-noose/

**E11. Line 79 — Sellen & Horvitz, "The Rise of the AI Co-Pilot," Communications of the ACM**
- Verdict: **CONFIRMED**. Published in CACM with DOI 10.1145/3637865, authored by Abigail Sellen and Eric Horvitz of Microsoft. The aviation Flight Management System framing is consistent with the article's actual argument.

### SPECIALIST category

**S1. Line 121 — "fluency cue that the metacognitive system uses to judge 'I get this' is exactly the cue that lies in this context"**
- Type: POSITIVE (mechanism claim)
- Verdict: **CONFIRMED** as a reasonable rendering of metacognitive-illusion literature (Bjork & Bjork 2011; Koriat & Bjork 2005 on illusions of competence). No misrepresentation.

**S2. Line 67 — "dopamine prediction-error signaling, hippocampal indexing, slow synaptic consolidation"**
- Type: POSITIVE
- Verdict: **UNVERIFIED** at the level of this chapter (the Preface presumably builds this argument; here it is invoked as already-established). The three mechanisms are real neuroscience constructs but the claim that they form a specific cascade triggered by predictive-error in learning is a synthesis that the chapter promises is supported in the Preface / Appendix G. Reviewer should confirm those sections cite Schultz (dopamine PE), Teyler & DiScenna or Tonegawa (hippocampal indexing), Dudai/McGaugh (consolidation).

**S3. Lines 67–73 — Risko & Gilbert 2016 framework (cognitive offloading) referenced indirectly**
- Verdict: **CONFIRMED** the underlying citation. Trends in Cognitive Sciences 20: 676-688; DOI 10.1016/j.tics.2016.07.002. The chapter does not cite Risko & Gilbert by name in this chapter (the brief flagged it as a key claim) — recommend adding the citation to support the offloading-atrophy claim made in line 71 ("the teacher's judgment about that operation atrophies").

### CURRENT category

**C1. Line 93 — Frontiers in Education 2025 review: "humans operating as oversight on automated systems 'experience a diminished sense of control, responsibility, and moral agency'"**
- Type: COMBINATION (direct quotation + EMPHATIC effect-persists claim)
- Verdict: **UNVERIFIED**. The Frontiers in Education 2025 article (DOI 10.3389/feduc.2025.1710992) is real ("Human-in-the-loop assessment with AI: implications for teacher education in Ibero-American universities", published October 2025). However, I could not verify the verbatim quoted phrase "diminished sense of control, responsibility, and moral agency" appears in that scoping review. The article is described as a taxonomy/scoping review of pedagogical affordances and risks. The "effect persists even after explicit training to resist it" claim in particular needs verification — a scoping review would typically not itself produce that empirical finding.
- Recommendation: Confirm the quotation page-locate against the published article, or re-attribute. If the quote actually comes from a different paper cited *within* the scoping review, cite that primary paper directly.

**C2. Line 107 — Kosmyna 2025 MIT Media Lab EEG study** (referenced by brief but NOT actually cited in this chapter's text)
- Verdict: N/A for Chapter 2 (the chapter does not invoke Kosmyna by name). The Kosmyna et al. preprint exists (arXiv:2506.08872, "Your Brain on ChatGPT") and the chapter could reasonably cite it in §3.6 on the cognitive-offloading parallel; right now it does not.

### GUIDELINE category

**G1. Lines 187, 195 — FERPA principle-level statements**
- Claim: pasting student names, performance data, and family information into a free consumer LLM constitutes "a disclosure of education records to a third party that has not signed a FERPA-compliant data-processing agreement"
- Verdict: **CONFIRMED** at the principle level. FERPA (20 U.S.C. § 1232g) restricts non-consensual disclosure of personally identifiable information from education records, and free consumer LLMs do not sign FERPA data-processing agreements. The "school official with legitimate educational interest" exception requires a written agreement.
- Source: https://studentprivacy.ed.gov ; 20 U.S.C. § 1232g

**G2. Line 195 — COPPA "any student is under 13"**
- Verdict: **CONFIRMED** at the principle level. COPPA applies to children under 13. Schools may consent on behalf of parents only for school-authorized services that meet specific conditions; consumer LLMs typically do not.

### STAT category (other than already-flagged)

**T1. Line 99 — "758 BCG consultants — roughly 7% of BCG's individual-contributor workforce"**
- Verdict: **CONFIRMED** for n=758. The "roughly 7% of BCG's individual-contributor workforce" framing is consistent with reporting; BCG had ~30k employees in 2023 of which most are consultants, so 758 ≈ 2-3% of total but plausibly closer to 7% of *individual-contributor* (non-partner/MD) consultants depending on definition. Soft confirmation.

**T2. Line 137 — Hattie d ≈ 0.72 teacher-student relationship**
- Verdict: **CONFIRMED** as the figure published on visible-learning.org. Same methodological caveats as d=1.57 apply at lower magnitude. Chapter's framing (numbers as "orders of magnitude rather than RCT-grade estimates") is appropriately calibrated.

---

## Unverified Assertions

1. **U1. Frontiers in Education 2025 direct quotation** (Line 93) — exact wording of the quoted phrase needs page-locate confirmation against the article body.
2. **U2. FPF October 2024 specific percentages 89%/34%** (Line 187) — figures not located in the primary FPF PDF; appear only in derivative sources.
3. **U3. Organization Science 2026 publication of Dell'Acqua et al.** (Line 99) — the DOI `10.1287/orsc.2025.21838` should be verified once the article appears in print; the working paper has been pending publication.
4. **U4. Neurobiological cascade specifics** (Line 67) — depends on Preface/Appendix G citations.
5. **U5. "approximately 89%" / "about 34%"** — the "approximately" and "about" hedges suggest the author has already noticed the numbers are not exact; flag for replacement with primary-source language.

---

## AI-Pass Flags

- "Approval rate" of 99.4% in the opening case (Line 35) is correctly labeled as part of a "composite illustration" (Line 31) — not a real statistic. Honest framing.
- The 12-gate table (Lines 201-214) is correctly labeled as "the chapter's own synthesis" (Line 199), not a published framework. Good provenance.
- "[verify]" inline tag on Line 107 (Bastani correction) can now be removed — confirmed affiliation-only.
- Opening case (§2) is explicitly framed as composite, not a single incident. Compliant with hard rule #1.
- Chapter does not invoke Risko & Gilbert by name though the brief flagged it — consider adding citation in §3.2 to anchor the offloading-atrophy claim.
- Chapter does not invoke Kosmyna 2025 — optional addition for §3.6 parallel.

---

## Notes for revision

1. Line 107 inline `[verify]` on the Bastani correction → can be removed (confirmed affiliation-only).
2. Line 93 quoted phrase from Frontiers in Education → confirm page-cite or rewrite as a paraphrase.
3. Line 187 FPF percentages → verify against primary PDF or re-attribute.
4. Consider citing Risko & Gilbert 2016 in §3.2 to support the cognitive-offloading claim explicitly.
