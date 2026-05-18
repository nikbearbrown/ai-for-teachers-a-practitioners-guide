# Assertions Report: 06-differentiation-with-ai.md
**Date:** 2026-05-18
**Source file:** chapters/06-differentiation-with-ai.md
**Assertions flagged:** 19
**Breakdown:** STAT: 3 | GUIDELINE: 7 | APPROVAL: 4 | EVIDENCE: 3 | SPECIALIST: 1 | CURRENT: 1

**Verdict counts:** CONFIRMED: 14 | CONTRADICTED: 1 | UNVERIFIED: 3 | OUTDATED: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

### 1. Stiti et al. 2025 *European Spine Journal* citation (CONTRADICTED)
**Line 53** — "a 2025 study by Stiti et al. in *European Spine Journal* found that GPT-4 reduced the average reading level of spine imaging reports from grade 11.47 to grade 8.50, but 34% of simplified outputs omitted at least one clinically relevant fact"
- **Category:** EVIDENCE
- **Type:** POSITIVE (precise numbers attached to authority)
- **Verdict:** CONTRADICTED
- **Finding:** The cited PMC article (PMC12743105) does exist and the numerical claims (11.47 → 8.50 reading level, 34% omission rate) are accurate to that paper. **However, the citation is wrong on two counts:**
  1. **Journal is incorrect.** The article is published in *Skeletal Radiology* (vol. 55, pp. 361–366, 2026; advance publication Sept 9, 2025), DOI 10.1007/s00256-025-05027-9 — NOT *European Spine Journal*.
  2. **Author "Stiti" does not appear in the author list.** Authors are Rushmin Khazanchi (first), Austin R. Chen, Parth Desai, Daniel Herrera, Jacob R. Staub, Matthew A. Follett, Mykhaylo Krushelnytskyy, Hanna Kemeny, Wellington K. Hsu, Alpesh A. Patel, and Srikanth N. Divi. The lead author is Khazanchi, not Stiti.
- **Recommendation:** Re-cite as "Khazanchi et al. 2025/2026, *Skeletal Radiology*, [DOI 10.1007/s00256-025-05027-9](https://link.springer.com/article/10.1007/s00256-025-05027-9); [PubMed 40921880](https://pubmed.ncbi.nlm.nih.gov/40921880/); [PMC12743105](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12743105/)." The pantry brief appears to have mis-attributed both the journal and the first author; the brief flagged this study correctly but the chapter inherited the error. **This is the highest-priority fix in the chapter** because the citation is the only specific empirical anchor for the §2.1 "model moves the metric but does not preserve substance" claim.

---

## Full Findings

### GUIDELINE category

**G1. Line 45 — Lexile Framework: sentence length and word frequency as the two inputs**
- Claim: "MetaMetrics splits it into 125-word slices, compares each to a large reference corpus, and runs two statistics — sentence length and word frequency — through the Lexile equation and a Rasch psychometric model."
- Type: POSITIVE (mechanism claim)
- **Verdict:** CONFIRMED. MetaMetrics' published materials confirm: text is split into 125-word slices, compared to a ~600-million-word reference corpus; mean log word frequency (MLF) and sentence length are the two computed inputs to the Lexile equation; Rasch psychometric model is used. The proprietary exact equation is not published, but the two-input mechanistic claim the chapter relies on is the documented mechanism.
- Source: [MetaMetrics Lexile Reading whitepaper (PDF)](https://cdn.lexile.com/m/uploads/whitepapers/Lexile-Reading-Measurement-and-Success-0504_MetaMetricsWhitepaper.pdf); [metametricsinc.com Lexile Framework PDF](https://metametricsinc.com/wp-content/uploads/2017/07/The-Lexile-Framework-for-Reading.pdf)
- Note: The chapter's load-bearing claim ("everything an LLM does when it 'lowers the Lexile' is, mechanically, a manipulation of sentence length and word frequency") is correct for the *computational* operation but slightly overstated — MLF is computed against a corpus, so word *frequency* in the reference corpus matters, not just synonym-swapping in the LLM's output. The chapter's framing survives this nuance.

**G2. Line 49 — "The Lexile formula does not measure inferential demand, syntactic complexity beyond sentence length, prior-knowledge load, abstractness of referents, or organizational coherence."**
- Type: POSITIVE (limit claim about a guideline framework)
- **Verdict:** CONFIRMED. MetaMetrics itself acknowledges Lexile measures one slice of text difficulty. The Lexile Framework documentation is explicit that it does not measure conceptual difficulty, prior-knowledge requirements, or text cohesion. The 2024 panel meeting review (White & Clement) describes the same limit.
- Source: [White & Clement — Assessing the Lexile Framework](https://cdn.lexile.com/m/resources/materials/White__Clement-_Assessing_the_Lexile_Framework.pdf)

**G3. Line 73 — UDL 3.0 "(CAST, July 2024)" with three principles (Engagement, Representation, Action & Expression)**
- Claim: "UDL 3.0 (CAST, July 2024) is organized around three principles — Engagement, Representation, and Action & Expression — and frames learner identity as a dimension of variability"
- Type: BASIC (date + framework structure)
- **Verdict:** CONFIRMED. CAST officially released UDL Guidelines 3.0 on July 30, 2024. The three principles named are correct. The 3.0 update explicitly broadens learner identity and adds attention to systems of exclusion as a dimension of variability across all three principles.
- Source: [About the Guidelines 3.0 Update](https://udlguidelines.cast.org/more/about-guidelines-3-0/); [udlguidelines.cast.org](https://udlguidelines.cast.org/)

**G4. Line 81 — WIDA 2020 Edition: six proficiency levels, four Key Language Uses (Narrate, Inform, Explain, Argue), three dimensions (word/phrase, sentence, discourse)**
- Type: POSITIVE (framework structure)
- **Verdict:** CONFIRMED. WIDA 2020 Edition introduced Level 6 (Reaching, open-ended) and the four Key Language Uses (Narrate, Inform, Explain, Argue). The six-level proficiency scale (Entering, Emerging, Developing, Expanding, Bridging, Reaching) is correct. The three linguistic dimensions framing (word/phrase, sentence, discourse) is part of the Proficiency Level Descriptors structure.
- Source: [WIDA ELD Standards Framework 2020 Edition](https://wida.wisc.edu/resources/wida-english-language-development-standards-framework-2020-edition); [WIDA Standards FAQ](https://wida.wisc.edu/sites/default/files/Website/News/2021/February/WIDA-StandardsFAQ-Intro.pdf)

**G5. Line 81 — "41 states, territories, and federal agencies are WIDA consortium members"**
- Type: STAT (specific number)
- **Verdict:** OUTDATED (mild). The WIDA Annual Report for July 2023–June 2024 reports 41 members. Current WIDA materials state 42 members. The number has been volatile by a unit; both 41 and 42 appear in recent sources. The chapter's "41" is consistent with the 2024 annual report and is defensible. Reviewer may wish to update to "approximately 41" or "more than 40" to insulate against drift.
- Source: [WIDA Consortium](https://wida.wisc.edu/about/consortium); [2024 WIDA Annual Report (PDF)](https://wida.wisc.edu/sites/default/files/Website/About/Consortium/2024WIDAAnnualReport.pdf)

**G6. Line 93 — IDEA Part B IEP team minimum membership (parent, gen-ed teacher if applicable, sped teacher, LEA rep, evaluation interpreter)**
- Type: POSITIVE (statutory composition)
- **Verdict:** CONFIRMED. The IEP team composition under IDEA Part B (34 CFR §300.321) is correctly described. The five required participants the chapter names are accurate; statute additionally lists "the child, when appropriate" and "other individuals with knowledge or special expertise" but the chapter says "the minimum membership" which fairly characterizes the required floor.
- Source: [CRS R41833 — IDEA Part B](https://www.congress.gov/crs-product/R41833); [US Dept of Education — A Guide to the IEP](https://www.ed.gov/sites/ed/files/parents/needs/speced/iepguide/iepguide.pdf)

**G7. Line 93 — "Section 504 of the Rehabilitation Act of 1973 covers students with disabilities who do not qualify under IDEA but who require accommodations to access the general curriculum"**
- Type: BASIC (statutory framing)
- **Verdict:** CONFIRMED. Section 504 (29 U.S.C. § 794) prohibits disability discrimination by recipients of federal financial assistance and is the standard authority for student accommodations not rising to IDEA eligibility. The "developed through a similar team process" framing is consistent with Department of Education OCR guidance.

### APPROVAL / LEGAL category

**A1. Line 103 — FERPA (20 U.S.C. § 1232g) protects PII in education records**
- Type: BASIC (legal citation)
- **Verdict:** CONFIRMED. Statutory cite and the principle that FERPA restricts non-consensual disclosure of PII from education records are correct.
- Source: [studentprivacy.ed.gov](https://studentprivacy.ed.gov/); 20 U.S.C. § 1232g

**A2. Line 103 — COPPA (15 U.S.C. § 6501) governs collection of personal data from children under 13**
- Type: BASIC (legal citation)
- **Verdict:** CONFIRMED. COPPA is at 15 U.S.C. §§ 6501–6506; the "under 13" threshold and the data-collection focus are correctly described.
- Source: [FTC COPPA Rule page](https://www.ftc.gov/legal-library/browse/rules/childrens-online-privacy-protection-rule-coppa)

**A3. Line 103 — IMPLICIT: the chapter does not invoke the FTC 2025 COPPA Final Rule amendments by name**
- Type: BASIC (omission check requested by brief)
- **Verdict:** UNVERIFIED-by-omission. The brief flagged the FTC 2025 COPPA Final Rule amendments (published Federal Register April 22, 2025; effective June 23, 2025; compliance deadline April 22, 2026) as load-bearing. The chapter cites only the 1998 COPPA statute and does not mention the 2025 amendments. **The chapter would be strengthened by acknowledging the 2025 amendments**, especially the expanded "personal information" definition (biometric identifiers, government IDs) and the new separate-consent requirement for third-party disclosure tied to targeted advertising. The FTC explicitly *declined* to codify the long-standing "school-authorized" guidance in the 2025 amendments — citing pending FERPA changes — which is the relevant point for K-12 readers worried about ed-tech under the amended Rule.
- Source: [FTC press release Jan 2025](https://www.ftc.gov/news-events/news/press-releases/2025/01/ftc-finalizes-changes-childrens-privacy-rule-limiting-companies-ability-monetize-kids-data); [Federal Register April 22 2025](https://www.federalregister.gov/documents/2025/04/22/2025-05904/childrens-online-privacy-protection-rule)
- Recommendation: Add one sentence in §2.6 noting the 2025 amendments and that the FTC explicitly preserved (rather than codified) the school-consent doctrine pending FERPA action. Without this, the chapter's COPPA framing is current-as-of-2013, not 2025.

**A4. Line 103 — US Dept of Ed OET, May 2023, "Artificial Intelligence and the Future of Teaching and Learning"**
- Type: BASIC (publication metadata)
- **Verdict:** CONFIRMED. Released May 24, 2023, by the Office of Educational Technology. The URL the chapter cites is the live OET PDF.
- Source: [ed.gov AI report PDF](https://www.ed.gov/sites/ed/files/documents/ai-report/ai-report.pdf); [ERIC ED631097](https://eric.ed.gov/?id=ED631097)
- Note: OET also released a *Designing for Education with Artificial Intelligence* guide in July 2024 and a Toolkit for Education Leaders in October 2024 — both updates the chapter could optionally cite to demonstrate "the Department's view has continued to evolve since May 2023."

### STAT category

**T1. Line 21 — Walton/Gallup 2025 *Teaching for Tomorrow* "64% of teachers who use AI for material modification report quality improvement"**
- Type: POSITIVE (precise %, named survey)
- **Verdict:** CONFIRMED. The Gallup/Walton report (fielded March 18 – April 11, 2025, n=2,232 K–12 public school teachers) reports: "Sixty-four percent of the teachers surveyed say the materials they modify with AI to meet student needs are better quality." Chapter framing matches the source.
- Source: [Walton Family Foundation — Six Weeks](https://www.waltonfamilyfoundation.org/six-weeks-giving-teachers-time-back-with-ai); [Gallup news writeup](https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx); [Teaching for Tomorrow report (PDF)](https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf)

**T2. Line 103 — "As of mid-2025, at least 25 state departments of education have issued their own AI guidance documents"**
- Type: POSITIVE (specific count, dated)
- **Verdict:** CONFIRMED with a caveat. Student Privacy Compass lists 25 states whose departments of education had issued generative-AI guidance as of the cited compilation; by April 2025 the count had grown to "at least 28" per CDT/Stateline reporting, and by mid-2025 multiple sources put it at "more than half." The "at least 25" framing is conservative and accurate for the date hedge "as of mid-2025."
- Source: [Student Privacy Compass — State Guidance](https://studentprivacycompass.org/state-guidance-on-the-use-of-generative-ai-in-k-12-education/); [Stateline July 2025](https://stateline.org/2025/07/15/more-than-half-the-states-have-issued-ai-guidance-for-schools/)

**T3. Line 53 — Stiti et al. 11.47 → 8.50 reading level reduction; 34% omission of clinically relevant info**
- See Critical Finding 1 above. Numbers themselves are confirmed; journal and lead author are wrong.

### EVIDENCE category

**E1. Line 69 — Bjorkian distinction between storage strength and retrieval strength**
- Claim: "material that feels easy in the moment is not material that has been encoded deeply"
- Type: SPECIALIST (mechanism claim)
- **Verdict:** CONFIRMED as a fair rendering of Bjork & Bjork's New Theory of Disuse (storage/retrieval strength distinction) and Bjork's work on desirable difficulties. The chapter does not cite Bjork by paper here, relying on the Chapter 2 establishment of the Bjorkian frame. Consistent treatment.

**E2. Line 105 — FPF 2024 *Vetting Generative AI Tools for Use in Schools***
- Claim: "The Future of Privacy Forum's 2024 *Vetting Generative AI Tools for Use in Schools* lays out the compliance frame"
- Type: BASIC (publication reference)
- **Verdict:** CONFIRMED. The FPF guide (October 2024) exists at the cited URL and is widely cited as the K-12 vetting reference.
- Source: [FPF 2024 Vetting Generative AI Tools (PDF)](https://fpf.org/wp-content/uploads/2024/10/Ed_AI_legal_compliance.pdf_FInal_OCT24.pdf)

**E3. Line 21 — Opening case framing as "composite-illustrative" with case-pattern anchored to Walton/Gallup**
- Type: BASIC (composite-illustration disclosure)
- **Verdict:** CONFIRMED for honesty. The chapter explicitly labels the case as composite, the minute-by-minute arithmetic as illustrative not measured, and anchors only the *pattern* to the survey. This is the correct method for opening cases under §3 of the workshop CLAUDE.md.

### SPECIALIST category

**S1. Line 65 — "extraneous load" vs "germane load" framing from Cognitive Load Theory**
- Type: POSITIVE (mechanism claim, theory invocation)
- **Verdict:** UNVERIFIED-by-omission. The intrinsic/extraneous/germane load distinction is Sweller, Van Merriënboer & Paas (1998); the framework is well-established. The chapter does not cite the original CLT paper — defensible if Chapter 2 (the Phase Gate) already establishes the framework, but the chapter would be tightened by one footnote citation when these terms first appear.
- Recommendation: Add an inline citation to Sweller et al. 1998 (*Educational Psychology Review* 10(3): 251–296) or to Sweller's *Cognitive Load Theory* (2011) at first use of "extraneous/germane" terminology.

### CURRENT category

**C1. Line 53 — "Peer-reviewed work on whether GPT-class commercial models reliably hit specified Lexile bands at K–12 grade levels — and whether their simplifications preserve content fidelity — is thin as of this writing."**
- Type: I-LANGUAGE / COMBINATION (calibrated empirical claim)
- **Verdict:** CONFIRMED. As of May 2026, peer-reviewed literature directly evaluating LLM Lexile-targeting against K–12 content fidelity is genuinely thin — most relevant work sits in adjacent domains (medical-text simplification, plain-language summaries of scientific abstracts). The chapter's "thin as of this writing" hedge is well-calibrated and the §7 "What would change my mind" follow-through is on-method.

---

## Unverified Assertions

1. **U1. FTC 2025 COPPA amendments not cited** (Line 103) — see A3. Not contested, but the chapter's COPPA framing is functionally pre-2025 and would be strengthened by one sentence acknowledging the new Rule.
2. **U2. Sweller et al. 1998 CLT citation absent** (Line 65) — see S1. Established framework, but a first-use footnote is best practice.
3. **U3. The 11.47 → 8.50 numbers as "average reading level"** — the source uses Flesch-Kincaid grade level (FKGL), not Lexile, for the 11.47/8.50 measurement. The chapter is careful to say "reading level" not "Lexile" — accurate but a reader looking for the Lexile parallel might draw the wrong inference. Worth one clarifying clause if revising.

---

## AI-Pass Flags

- Opening case (§1) correctly framed as composite-illustrative with the survey-pattern anchor disclosed in line-21 italics. Compliant with hard rule #1.
- No Bastani "17 percentage points" reference in this chapter — cross-book issue does not apply here.
- The chapter EXPLICITLY OMITS the "TIKTOC 28% material modification" figure that was flagged as potentially conflated with Walton/Gallup's "28% infrequent users" — **omission is correct** and the chapter avoids the conflation cleanly.
- The "60% reduction / 2.1 hours saved" time-recovery estimate is correctly omitted; the chapter sticks to "twelve minutes of generation" and "forty-two minutes" worked-example arithmetic explicitly labeled illustrative. Omission is correct.
- Phase gate (§2.7) and three-sentence summary are the chapter's own synthesis — appropriately labeled, not presented as a published framework.
- Worked example (§3) uses an explicitly hypothetical article; "the article itself is hypothetical for this worked example; the underlying scientific claims are well-documented" disclosure is on-method.
- The "Stiti" citation error (Critical Finding 1) is the only false-attribution issue and is downstream of a pantry error rather than chapter fabrication — the underlying numbers and conclusions are correctly drawn from a real paper, just attributed to the wrong author and journal.

---

## Notes for revision

1. **Highest priority:** Line 53 — fix Stiti → Khazanchi et al., *Skeletal Radiology* (2025/2026), DOI 10.1007/s00256-025-05027-9. Update the PMC link and add the Springer Skeletal Radiology link.
2. **Recommended:** Line 103 — add one sentence noting the FTC's 2025 COPPA Final Rule amendments (Federal Register April 22, 2025; effective June 23, 2025) and that the FTC declined to codify the school-consent doctrine, deferring to pending FERPA action.
3. **Optional:** Line 65 — first-use footnote for Sweller et al. CLT terminology.
4. **Optional:** Line 81 — update "41 states, territories, and federal agencies" to "approximately 41" to insulate against drift (current WIDA materials cite 42).
5. **Optional:** Line 53 — clarify that the 11.47/8.50 measurement is Flesch-Kincaid grade level, not Lexile, so readers do not mis-map the metric to the chapter's central topic.

---

## Inline flag to be added in chapter

Insert at top of §2.1 (line 43, before the Lexile mechanism paragraph) or directly on Line 53:

```
<!-- FACT-CHECK FLAG: CONTRADICTED — Stiti et al. citation misattributes the paper.
Correct citation is Khazanchi et al., Skeletal Radiology (2025/2026),
DOI 10.1007/s00256-025-05027-9. See factchecks/06-differentiation-with-ai-assertions.md -->
```
