# Assertions Report: 11-coding-with-ai-an-introduction.md
**Date:** 2026-05-18
**Source file:** chapters/11-coding-with-ai-an-introduction.md
**Assertions flagged:** 18
**Breakdown:** STAT: 4 | GUIDELINE: 1 | APPROVAL: 1 | EVIDENCE: 7 | SPECIALIST: 3 | CURRENT: 2

**Verdict counts:** CONFIRMED: 15 | CONTRADICTED: 0 | UNVERIFIED: 1 | OUTDATED: 2

---

## ⚠️ Critical — Requires Immediate Expert Review

No critical contradictions. The chapter is unusually careful with quantitative claims and explicitly refuses the most common conflation in the AI-coding literature (productivity ≠ safety). Two non-critical issues:

1. **Karpathy "more oversight and scrutiny" quote attribution (line 123).** The chapter attributes the quote to Karpathy's "2025 LLM year-in-review post" on bearblog. The quote in fact appears in Karpathy's **February 2026 X post** marking the one-year anniversary of the "vibe coding" tweet (the post that coined "agentic engineering"), not in the year-in-review blog post. The substance of the chapter's claim — that Karpathy's framing moved toward oversight/scrutiny and away from pure vibe coding — is accurate. Attribution should be corrected to the February 2026 X post, or to a paraphrase of the year-in-review's "vibe coding" section. Flagged OUTDATED/citation.
2. **References section missing.** Added on this pass.

---

## Full Findings

### EVIDENCE category

**E1. Line 107 — Peng et al. 2023 arXiv:2302.06590; 95 developers; HTTP server in JavaScript; treatment group 55.8% faster.**
- Claim: "Ninety-five professional developers were asked to implement an HTTP server in JavaScript. The treatment group, with Copilot, completed the task **55.8% faster** than the control group. Less experienced developers gained more than experienced ones."
- Category: EVIDENCE
- Type: POSITIVE (precise authority + magnitude)
- **Verdict:** CONFIRMED
- **Finding:** Peng, S., Kalliamvakou, E., Cihon, P., & Demirer, M. (2023). "The Impact of AI on Developer Productivity: Evidence from GitHub Copilot." arXiv:2302.06590. Recruited 95 professional developers; HTTP-server-in-JavaScript task; treatment group completed 55.8% faster; heterogeneous effects favor less experienced developers. All four numbers/details match the paper exactly.
- Source: [arXiv:2302.06590](https://arxiv.org/abs/2302.06590); [Microsoft Research listing](https://www.microsoft.com/en-us/research/publication/the-impact-of-ai-on-developer-productivity-evidence-from-github-copilot/)

**E2. Line 109–111 — Peng et al. measures time-to-complete only, NOT code quality, security, maintainability, or learning.**
- Claim: "The number measures *time-to-complete on a clearly specified task.* That is all it measures. It does *not* measure whether the produced code is secure. It does *not* measure whether the code is maintainable six months later... Peng et al. is evidence that AI accelerates well-specified development tasks. It is not evidence that AI-generated code is good."
- Category: EVIDENCE / I-LANGUAGE
- Type: POSITIVE (correctly narrowed claim + named conflation)
- **Verdict:** CONFIRMED
- **Finding:** Peng et al. report only completion time as their dependent variable. The paper does not measure code quality, security, correctness on held-out inputs, maintainability, or learning. The chapter's narrowing is exact and the explicit refusal of the productivity-equals-safety conflation is on-method. This is the load-bearing claim the brief asked to verify and it is handled cleanly.
- Source: [arXiv:2302.06590](https://arxiv.org/abs/2302.06590)
- **AI-Pass note:** This is the cleanest treatment of Peng et al. across the chapters I have audited in this book — no conflation.

**E3. Line 113 — Veracode 2025: roughly 45% of AI-generated samples contain at least one OWASP Top 10 security flaw.**
- Claim: "[Veracode's 2025 evaluation](https://www.veracode.com/blog/ai-generated-code-security-risks/) found roughly **45% of AI-generated code samples contained at least one OWASP Top 10 security flaw**."
- Category: STAT / SPECIALIST
- Type: POSITIVE (precise magnitude + named source)
- **Verdict:** CONFIRMED
- **Finding:** Veracode 2025 GenAI Code Security Report tested 100+ LLMs across Java, JavaScript, Python, and C#. Headline finding: 45% of samples introduced OWASP Top 10 vulnerabilities. The chapter's "roughly 45%" is the precise reported figure. Veracode also reports language-specific failure rates (Java highest at 72%; Python/C#/JavaScript 38–45%) and 2.74× more vulnerabilities than human-written code — chapter does not cite these subsidiary numbers and that is fine.
- Source: [Veracode blog](https://www.veracode.com/blog/genai-code-security-report/); [Veracode 2025 report](https://www.veracode.com/resources/analyst-reports/2025-genai-code-security-report/); [Help Net Security coverage](https://www.helpnetsecurity.com/2025/08/07/create-ai-code-security-risks/)
- **AI-Pass note:** The exact URL the chapter links (`/blog/ai-generated-code-security-risks/`) may need verification — the canonical 2025 report URL is `/blog/genai-code-security-report/`. Both resolve to Veracode content on the same finding. UNVERIFIED on exact slug; CONFIRMED on substantive claim.

**E4. Line 113 — Cloud Security Alliance 2025: similar figures on AI-generated code security risks.**
- Claim: "The [Cloud Security Alliance's 2025 review](https://cloudsecurityalliance.org/blog/2025/07/09/understanding-security-risks-in-ai-generated-code) reached similar figures."
- Category: SPECIALIST / CURRENT
- Type: BASIC (named source, vague magnitude)
- **Verdict:** CONFIRMED
- **Finding:** CSA blog post "Understanding Security Risks in AI-Generated Code," published July 9, 2025, by Andrew Stiefel (Endor Labs). Reports a study finding ~62% of AI-generated code solutions contain design flaws or known vulnerabilities even with frontier models. Direction matches ("similar figures"). The 62% CSA figure is higher than Veracode's 45%, so "similar" is loose but defensible — both findings cluster in the "roughly half of AI-generated code has security problems" range.
- Source: [CSA blog](https://cloudsecurityalliance.org/blog/2025/07/09/understanding-security-risks-in-ai-generated-code)

**E5. Line 113 — arXiv:2510.26103 (2025) large-scale GitHub analysis: vulnerability rates ~16–18% for Python, ~9% for JavaScript.**
- Claim: "A [2025 large-scale arXiv analysis](https://arxiv.org/pdf/2510.26103) found vulnerability rates around 16–18% for Python and around 9% for JavaScript across LLM-generated samples."
- Category: EVIDENCE / STAT
- Type: POSITIVE (precise magnitudes, language-stratified)
- **Verdict:** CONFIRMED
- **Finding:** "Security Vulnerabilities in AI-Generated Code: A Large-Scale Analysis of Public GitHub Repositories" (arXiv:2510.26103). 7,703 files attributed to four AI tools (ChatGPT, Copilot, CodeWhisperer, Tabnine). CodeQL analysis. Python vulnerability rate 16.18–18.50%; JavaScript 8.66–8.99%; TypeScript 2.50–7.14%. Chapter's "around 16–18% / around 9%" matches the paper's reported ranges exactly.
- Source: [arXiv:2510.26103](https://arxiv.org/abs/2510.26103); [PDF](https://arxiv.org/pdf/2510.26103)
- **AI-Pass note:** Note: the brief mentioned "40–62%" language-stratified rates for arXiv:2510.26103. The paper's actual reported language-specific rates are in the single-digit to high-teens range (Python 16–18%, JS ~9%). The chapter quotes the paper correctly, not the 40–62% range. Either the brief was mixing this paper with the CSA 62% figure (Endor Labs study) or with Veracode's per-language failure rates. The chapter's numbers are accurate to the cited paper.

**E6. Line 113–115 — Controlled user study: AI-assisted participants wrote less secure code AND rated it more secure than controls. (Perry et al. paraphrase, uncited inline.)**
- Claim: "A controlled user study cited across this literature found participants using AI assistants wrote *less secure* code than controls *and rated their insecure solutions as more secure than controls' solutions.*"
- Category: EVIDENCE
- Type: POSITIVE (precise mechanism, no inline citation)
- **Verdict:** CONFIRMED
- **Finding:** Perry, N., Srivastava, M., Kumar, D., & Boneh, D. (2023). "Do Users Write More Insecure Code with AI Assistants?" ACM CCS 2023 (arXiv:2211.03622). 47 participants, codex-davinci-002 access. Finding: AI-assisted participants wrote significantly less secure code AND were more likely to believe they had written secure code. Specific vulnerabilities concentrated in string encryption and SQL injection. Chapter's paraphrase is exact. Should be cited inline; currently uncited (referred to as "cited across this literature").
- Source: [arXiv:2211.03622](https://arxiv.org/abs/2211.03622); [Stanford EE coverage](https://ee.stanford.edu/dan-boneh-and-team-find-relying-ai-more-likely-make-your-code-buggier)
- **AI-Pass note:** Recommend adding Perry et al. as a direct citation in the chapter — currently appears as an anonymous "controlled user study."

**E7. Line 121 — Karpathy February 2025 tweet coining "vibe coding."**
- Claim: "In February 2025, Andrej Karpathy... [posted a short tweet coining the phrase 'vibe coding'](https://x.com/karpathy/status/1886192184808149383)..."
- Category: EVIDENCE / CURRENT
- Type: POSITIVE (precise URL, date, attribution)
- **Verdict:** CONFIRMED
- **Finding:** Tweet posted February 2, 2025 by @karpathy. Status ID 1886192184808149383 is correct. Text: "There's a new kind of coding I call 'vibe coding,' where you fully give in to the vibes, embrace exponentials, and forget that the code even exists. It's possible because the LLMs (e.g. Cursor Composer w Sonnet) are getting too good." Went viral; >4.5M views.
- Source: [x.com/karpathy/status/1886192184808149383](https://x.com/karpathy/status/1886192184808149383)

**E8. Line 123 — Karpathy's later "more oversight and scrutiny" quote attributed to 2025 LLM year-in-review post.**
- Claim: "A year later, in his [2025 LLM year-in-review post](https://karpathy.bearblog.dev/year-in-review-2025/), Karpathy was sharper: 'Today (1 year later), programming via LLM agents is increasingly becoming a default workflow for professionals, except with more oversight and scrutiny.'"
- Category: EVIDENCE / CURRENT
- Type: POSITIVE (direct quote + URL attribution)
- **Verdict:** OUTDATED (attribution error; substance correct)
- **Finding:** The exact quoted sentence ("Today (1 year later)...with more oversight and scrutiny.") appears in Karpathy's **February 2026 X post** (status 2019137879310836075), posted as a one-year retrospective on the original vibe coding tweet. The bearblog year-in-review post does discuss vibe coding, LLM agents, and the shift in workflow ("vibe coding" listed as one of six paradigm shifts of 2025), but the specific quoted sentence is from the X anniversary post, not the year-in-review. The substantive claim (Karpathy moved toward an "oversight/scrutiny" framing) is correct. Recommendation: change the link to [x.com/karpathy/status/2019137879310836075](https://x.com/karpathy/status/2019137879310836075), or paraphrase from the year-in-review post directly.
- Source: [Karpathy year-in-review](https://karpathy.bearblog.dev/year-in-review-2025/); [Karpathy Feb 2026 anniversary post](https://x.com/karpathy/status/2019137879310836075); [The New Stack coverage](https://thenewstack.io/vibe-coding-is-passe/)

**E9. Line 123 — Industry converged on "spec-driven development."**
- Claim: "Industry practice did not converge on *vibe coding*. It converged on **spec-driven development** — the developer writes the specification, the AI writes the code, the developer reviews against the spec."
- Category: CURRENT
- Type: POSITIVE (generalization about industry practice)
- **Verdict:** CONFIRMED (with caveat)
- **Finding:** The framing "spec-driven development" is widely used in 2026 commentary on the vibe-coding-to-agentic-engineering shift (Towards Data Science, The New Stack, multiple industry blogs). Karpathy himself coined "agentic engineering" rather than "spec-driven development" specifically, but "spec-driven" is a faithful summary of the operative methodology and is in common use in the 2026 literature. The chapter is using "spec-driven development" as a generalization, which is supportable.
- Source: [Towards Data Science: From Vibe Coding to Spec-Driven](https://towardsdatascience.com/from-vibe-coding-to-spec-driven-development/); [The New Stack](https://thenewstack.io/vibe-coding-is-passe/)

**E10. Line 129 — Wing 2006 "Computational Thinking" *Communications of the ACM*, three-page viewpoint.**
- Claim: "In 2006, Jeannette Wing — then at Carnegie Mellon — published a short *Communications of the ACM* piece called ['Computational Thinking'](https://www.cs.cmu.edu/~wing/publications/Wing06.pdf)."
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (canonical citation)
- **Verdict:** CONFIRMED
- **Finding:** Wing, J. M. (2006). "Computational Thinking." *Communications of the ACM*, 49(3), 33–35. The chapter's framing (abstraction, decomposition, algorithmic reasoning, recognizing what is computable) is faithful to Wing's argument. PDF link at CMU is canonical. ACM DOI 10.1145/1118178.1118215.
- Source: [CMU PDF](https://www.cs.cmu.edu/~wing/publications/Wing06.pdf); [ACM DL DOI](https://dl.acm.org/doi/10.1145/1118178.1118215)

**E11. Line 129 — 2016 K-12 Computer Science Framework; developed by ACM, Code.org, CSTA, Cyber Innovation Center, NMSI; seven core practices.**
- Claim: "A decade later, the [2016 K–12 Computer Science Framework](https://k12cs.org/), developed by ACM, Code.org, CSTA, the Cyber Innovation Center, and NMSI, codified this into seven core practices for K–12 CS education."
- Category: EVIDENCE / GUIDELINE
- Type: POSITIVE (precise attribution, count of practices)
- **Verdict:** CONFIRMED
- **Finding:** The K-12 CS Framework was indeed released in 2016 (steering committee: ACM, Code.org, CSTA, Cyber Innovation Center, National Math + Science Initiative). It defines seven core practices (with computational thinking concentrated in practices 3–6). k12cs.org is the canonical project URL. ACM DL has the framework as a book (DOI 10.1145/3079760).
- Source: [k12cs.org](https://k12cs.org/); [k12cs.org/navigating-the-practices](https://k12cs.org/navigating-the-practices/); [ACM DL](https://dl.acm.org/doi/book/10.1145/3079760)

**E12. Line 67 — Ko et al. 2011 "The State of the Art in End-User Software Engineering," *ACM Computing Surveys*; cited via MIT Media Lab PDF; references Brad Myers (CMU) and Margaret Burnett (Oregon State).**
- Claim: "Brad Myers at Carnegie Mellon and Margaret Burnett at Oregon State, with collaborators across the human-computer interaction community, have been asking since the 1980s how to let people who are not professional programmers create software for their own purposes... The 2011 *ACM Computing Surveys* article ['The State of the Art in End-User Software Engineering'](https://web.media.mit.edu/~lieber/Publications/End-User-Software-Engineering.pdf) laid the field out clearly."
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (canonical citation + attribution to named researchers)
- **Verdict:** CONFIRMED
- **Finding:** Ko, A. J., Abraham, R., Beckwith, L., Blackwell, A., Burnett, M., Erwig, M., Lawrance, J., Lieberman, H., Myers, B. A., Rosson, M. B., Rothermel, G., Scaffidi, C., Shaw, M., & Wiedenbeck, S. (2011). "The State of the Art in End-User Software Engineering." *ACM Computing Surveys*, 43(3), Article 21, 44 pages. DOI 10.1145/1922649.1922658. Both Myers (CMU) and Burnett (Oregon State) are listed authors. MIT Media Lab mirror (Henry Lieberman's site) hosts a faithful PDF copy. Decades-since-1980s claim is accurate — both Myers and Burnett have publications going back to the late 1980s in this area.
- Source: [ACM DL DOI 10.1145/1922649.1922658](https://dl.acm.org/doi/10.1145/1922649.1922658); [MIT Media Lab PDF](https://web.media.mit.edu/~lieber/Publications/End-User-Software-Engineering.pdf)

### APPROVAL / GUIDELINE category

**E13. Line 141, 255 — FERPA applies to AI-generated code that touches identifiable student information.**
- Claim: "[FERPA](https://studentprivacy.ed.gov/ferpa) does not distinguish between a script you wrote and a script the AI wrote: if the script touches identifiable student information, FERPA's restrictions apply equally to both."
- Category: APPROVAL / GUIDELINE
- Type: POSITIVE (legal/regulatory claim)
- **Verdict:** CONFIRMED
- **Finding:** FERPA (20 U.S.C. § 1232g; 34 CFR Part 99) applies to personally identifiable information from education records regardless of the tool used to process it. studentprivacy.ed.gov is the U.S. Department of Education's official FERPA portal. The chapter's hedge ("specific FERPA criteria for AI-assisted teacher-built tools vary by district and state interpretation and are referred to district counsel") is on-method — there is no AI-specific FERPA guidance from the Department of Education as of May 2026 beyond general PII-handling rules.
- Source: [studentprivacy.ed.gov/ferpa](https://studentprivacy.ed.gov/ferpa)

### CURRENT category

**E14. Line 320 — "As of May 2026, no such [randomized K–12/higher-ed teacher study] exists."**
- Claim: "A randomized study of K–12 or higher-ed teachers — non-programmers — who built and deployed AI-coded classroom or workflow tools, measuring both deployment-time defect rates (functional and privacy) and student-facing-incident rates over a full school year... As of May 2026, no such study exists."
- Category: CURRENT / I-LANGUAGE
- Type: I-LANGUAGE (calibrated negative)
- **Verdict:** UNVERIFIED (negative existence claim, narrow)
- **Finding:** A targeted search did not surface such a randomized study with the specified design (non-programmer teachers, full school year, both defect and student-incident outcomes). The negative existence claim is plausible and well-scoped. Negative-existence claims are intrinsically hard to confirm; the chapter's "I would revise" framing makes the falsifiability condition explicit and on-method. Flagged UNVERIFIED rather than CONFIRMED because absence-of-evidence is harder to prove than presence.

### STAT / SPECIALIST category (chapter-internal)

**E15. Line 23 — "fifteen years" framing for Ms. R's polynomial demo desire.**
- Claim: "[Ms. R] — call her Ms. R, *[composite-illustrative...]*"
- Category: SPECIALIST / I-LANGUAGE
- Type: I-LANGUAGE (labeled composite)
- **Verdict:** CONFIRMED
- **Finding:** Composite-illustrative case explicitly labeled in the text as not a named single person. Compliant with the book's narrative-rules-for-composites convention (similar to Ch 10's handling of similar examples).

**E16. Line 45, 71 — "2022–2024" as the period when LLM code generation became viable.**
- Claim: "What changed in 2022–2024 is that a particular kind of machine learning model — a large language model trained on enormous quantities of source code paired with natural-language descriptions — got good enough..."
- Category: CURRENT / STAT
- Type: BASIC (date range)
- **Verdict:** CONFIRMED
- **Finding:** The 2022–2024 window aligns with: GitHub Copilot GA (June 2022), Codex/ChatGPT (late 2022), GPT-4 (March 2023), Claude 3.5 Sonnet / Cursor Composer / agentic coding rise (2024). Defensible as the period when AI coding assistants transitioned from research curiosity to mainstream tool.

**E17. Line 79 — "A script that systematically misweights one rubric category will produce wrong grades for the entire class with no visible symptom."**
- Claim: Generalization about silent failure mode of grade scripts.
- Category: SPECIALIST / I-LANGUAGE
- Type: POSITIVE (mechanism claim)
- **Verdict:** CONFIRMED (on-method)
- **Finding:** Standard software engineering observation about silent failure modes in numerical processing without independent verification. Not a citation-bearing empirical claim — a craft-knowledge generalization. Appropriate framing.

**E18. Line 151 — "$1 Kindle companion" reference.**
- Claim: "The full treatment of the legal questions is in the $1 Kindle companion *Coding with AI*."
- Category: SPECIALIST
- Type: BASIC (cross-reference to book artifact)
- **Verdict:** UNVERIFIED (book-internal artifact, not a fact-check target)
- **Finding:** This is an internal cross-promotion to a companion artifact. Not a citation-bearing factual claim and not a verification target for this report.

---

## Unverified Assertions

- E14 (May 2026 negative existence of randomized teacher study) — intrinsically hard to verify; well-scoped.
- E18 ($1 Kindle companion) — internal artifact reference.
- E3 (Veracode exact slug) — substantive finding CONFIRMED; specific URL slug should be verified against canonical Veracode 2025 report URL.

---

## AI-Pass Flags

- **No fabricated citations detected.** Every named author, year, paper, and venue checked out.
- **No magnitude inflation.** Peng et al. 55.8% is the exact published figure. Veracode 45% is the exact figure. arXiv:2510.26103's 16–18% Python / 9% JavaScript matches the paper's reported ranges. Karpathy quote text is exact (modulo attribution issue, E8).
- **Productivity-vs-safety conflation explicitly refused.** This is the most common rhetorical move in AI-for-education writing about coding assistants; the chapter names and refuses it (E2). Clean.
- **Bastani et al. is not cited in this chapter.** The cross-book "17 percentage points" trap does not apply here.
- **Karpathy quote attribution (E8) is the single citation issue.** Substantively accurate; the specific blog-post-vs-anniversary-tweet attribution should be corrected.
- **Perry et al. (E6) should be named inline** rather than left as anonymous "a controlled user study." Recommend adding citation.

---

## Recommended In-Text Edits

1. **Line 123 (Karpathy attribution).** Either (a) change the linked URL to the February 2026 anniversary X post (`https://x.com/karpathy/status/2019137879310836075`), or (b) paraphrase the year-in-review's "vibe coding" section rather than presenting the quoted sentence as if from that post.
2. **Line 113 (Perry et al.).** Add inline citation: "A controlled user study ([Perry et al., 2023](https://arxiv.org/abs/2211.03622)) found..."
3. **Line 113 (Veracode URL).** Verify the exact slug `/blog/ai-generated-code-security-risks/` resolves; canonical URL appears to be `/blog/genai-code-security-report/`.
4. **References section.** Added at the end of the chapter on this pass.

---

*Fact-check pass complete. Chapter is methodologically strong — the explicit refusal to conflate productivity with safety, the calibrated negative existence claim, and the careful labeling of the Ms. R composite are all on-method. Two minor citation issues recommended for revision.*
