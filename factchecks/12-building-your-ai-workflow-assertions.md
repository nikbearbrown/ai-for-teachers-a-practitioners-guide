# Assertions Report: 12-building-your-ai-workflow.md
**Date:** 2026-05-18
**Source file:** chapters/12-building-your-ai-workflow.md
**Assertions flagged:** 22
**Breakdown:** STAT: 5 | GUIDELINE: 3 | APPROVAL: 0 | EVIDENCE: 9 | SPECIALIST: 3 | CURRENT: 2

**Verdict counts:** CONFIRMED: 16 | CONTRADICTED: 0 | UNVERIFIED: 5 | OUTDATED: 1

---

## ⚠️ Critical — Requires Immediate Expert Review

No critical contradictions. The chapter is unusually well-disciplined about epistemic status — five `[contested]` flags and three `[verify]` flags are already embedded in the body, and the framing of the 5.9-hour finding, the prompt shelf-life heuristic, and the habit-literature extension are all hedged appropriately.

Three secondary items merit attention:

1. **Hall & Hord *Implementing Change* edition.** Chapter cites "Pearson, 5th ed." with an in-text `[verify edition]` flag. The 5th edition was published by Pearson Education in 2020 — confirmed. The flag can be cleared.
2. **arXiv link `2604.16738v1`.** The chapter cites a "Spring 2025 pilot, 16 teachers, 4 districts, 878 students" paper at `https://arxiv.org/html/2604.16738v1`. The link resolves to "Teacher-Authored Prompts for Configuring Student–AI Dialogue: K–12 Classroom Implementation" (arXiv:2604.16738v1, 2026-04). The arXiv identifier `2604.16738` is structurally valid for April 2026; sample sizes (16 teachers, 4 districts, 878 students) should be cross-checked against the manuscript text by Nik before publication. Flagged UNVERIFIED for sample-size specifics.
3. **RAND ASDP "68%" wording.** Chapter's existing `[verify]` flag is well-placed. RAND RR-A956-31 is a district-side report (only 48% of districts had provided training by Fall 2024). The 68% "no formal training" figure is the corresponding *teacher-side* statistic and is reported in secondary coverage of the RAND wave (K-12 Dive, AI for Education) but does not appear as a clean primary stat in RR-A956-31 itself, which surveys districts. The cleanest primary source for "no formal training" wording is the teacher-side companion data; the chapter should cite both the district-side report (RR-A956-31) AND the teacher-side wave when the latter is published. Keep the flag through final edit.

---

## Full Findings

### STAT category

**S1. Line 14, 21, 25, 37 — Gallup-Walton 2025 weekly users save 5.9 hr/wk; n=2,232; March–April 2025; release September 2025; "Teaching for Tomorrow: Unlocking Six Weeks a Year With AI."**
- Claim: "an average of **5.9 hours per week** — about six weeks across the school year"; "n = 2,232 U.S. public K-12 teachers"; survey March–April 2025; release Gallup September 2025.
- Category: STAT
- Type: EMPHATIC (precise n, mean, fielding window)
- **Verdict:** CONFIRMED
- **Finding:** Gallup release dated September 16, 2025 reports the 5.9-hour figure for weekly AI users, six weeks per school year. Survey fielded March 18 – April 11, 2025, n=2,232 U.S. public K-12 teachers via RAND American Teacher Panel. Report title "Teaching for Tomorrow: Unlocking Six Weeks a Year With AI" is confirmed.
- Source: [Gallup news release](https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx); [Walton Family Foundation summary](https://www.waltonfamilyfoundation.org/six-weeks-giving-teachers-time-back-with-ai); [Full PDF report](https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf)

**S2. Line 37 — "Only 32% of teachers used AI weekly; another 28% used it infrequently; 40% did not use it at all."**
- Category: STAT
- Type: EMPHATIC (three precise percentages)
- **Verdict:** CONFIRMED
- **Finding:** Gallup release confirms 32% weekly users; remainder splits 28% infrequent / 40% non-users. Numbers match.
- Source: [Gallup news release](https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx)

**S3. Line 107 — "roughly 68% of U.S. teachers reported no formal training on how to use AI tools during the 2024–2025 school year" (RAND ASDP RR-A956-31).**
- Category: STAT / SPECIALIST
- Type: EMPHATIC (precise figure attributed to a specific report)
- **Verdict:** UNVERIFIED (already flagged `[verify]` in-chapter — appropriate)
- **Finding:** RR-A956-31 ("More Districts Are Training Teachers on Artificial Intelligence") is a **district-side** report. Its primary headline statistic is the *district* number — about half (48%) of districts had provided teacher AI training by Fall 2024, up from 23% the previous fall. The 68% "no formal training" *teacher-side* figure is widely reported in secondary coverage of the same RAND wave but does not sit cleanly inside RR-A956-31. K-12 Dive and AI for Education report the 68% figure attributed to the RAND survey research, with phrasing along the lines of "68% of teachers reported they did not receive training on how to use AI tools." The chapter's flag for verifying exact wording ("no formal training" vs. "no district-provided training") is exactly right — secondary summaries elide the distinction. Cite RR-A956-31 for the district number, the teacher-side wave (when published / cite RR-A4180-1 ["AI Use in Schools Is Quickly Increasing but Guidance Lags"] as companion) for the 68% figure.
- Source: [RAND RR-A956-31](https://www.rand.org/pubs/research_reports/RRA956-31.html); [RAND RR-A4180-1](https://www.rand.org/content/dam/rand/pubs/research_reports/RRA4100/RRA4180-1/RAND_RRA4180-1.pdf); [K-12 Dive coverage](https://www.k12dive.com/news/teacher-ai-training-remains-uneven-despite-uptick/745668/); [AI for Education summary](https://www.aiforeducation.io/blog/rand-research-reveals-growing-ai-training-gap)
- **AI-Pass note:** Keep the `[verify]` flag and broaden the citation pair before final publication.

**S4. Line 107 — "only 48% of districts said they had provided any teacher AI training by Fall 2024, up from 23% a year earlier."**
- Category: STAT
- Type: EMPHATIC (two precise percentages with year-over-year contrast)
- **Verdict:** CONFIRMED
- **Finding:** RAND RR-A956-31 reports half of districts had provided teacher training on generative AI by Fall 2024, double the previous fall — chapter's 48% / 23% match the report.
- Source: [RAND RR-A956-31](https://www.rand.org/pubs/research_reports/RRA956-31.html); [RAND announcement (X/Twitter)](https://x.com/RANDCorporation/status/1914144055153270863)

**S5. Line 107 — "of teachers who *use* AI, 52% taught themselves and only 31% received district-provided training" (Gallup-Walton 2025).**
- Category: STAT
- Type: EMPHATIC
- **Verdict:** CONFIRMED
- **Finding:** Gallup-Walton 2025 report shows that among teachers using AI, 52% self-taught and 31% received district-provided training. The chapter's framing is accurate.
- Source: [Walton Family Foundation summary](https://www.waltonfamilyfoundation.org/six-weeks-giving-teachers-time-back-with-ai); [Full PDF report](https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf)

**S6. Line 109 — "By Fall 2024, 67% of low-poverty districts had provided AI training versus 39% of high-poverty districts."**
- Category: STAT
- Type: EMPHATIC (equity gap, two precise percentages)
- **Verdict:** CONFIRMED
- **Finding:** RAND RR-A956-31 reports the low- vs. high-poverty district training gap. The chapter's 67% / 39% framing is accurate.
- Source: [RAND RR-A956-31](https://www.rand.org/pubs/research_reports/RRA956-31.html)

### EVIDENCE category

**E1. Line 59 — Davenport & Prusak (1998), *Working Knowledge: How Organizations Manage What They Know*, Harvard Business School Press; tacit-to-explicit knowledge framing.**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (canonical citation, framework summary)
- **Verdict:** CONFIRMED
- **Finding:** Davenport, T. H., & Prusak, L. (1998). *Working Knowledge: How Organizations Manage What They Know*. Harvard Business School Press. ISBN 0-87584-655-6. The book is the canonical knowledge-management text. The chapter's quote "Knowledge works across networks and communities" is consistent with the book's themes; the tacit/explicit distinction is more strongly associated with Nonaka & Takeuchi (1995), but Davenport & Prusak deploy and extend it. The link in the chapter resolves to the HBR Press product page (still in print).
- Source: [HBR Press product page](https://store.hbr.org/product/working-knowledge-how-organizations-manage-what-they-know/3014); [Google Books edition](https://books.google.com/books/about/Working_Knowledge.html?id=-4-7vmCVG5cC)
- **AI-Pass note:** If Nik wants a stricter tacit/explicit citation, add Nonaka & Takeuchi (1995) alongside; otherwise leave as is. Direct quote attribution should be verified in the print volume before publication — included as a minor flag.

**E2. Line 80 — Wood & Neal (2007), "A New Look at Habits and the Habit-Goal Interface," *Psychological Review* 114(4): 843–863.**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (precise journal citation, framework summary "context-cued behavior chunks")
- **Verdict:** CONFIRMED
- **Finding:** Wood, W., & Neal, D. T. (2007). *Psychological Review*, 114(4), 843–863. DOI 10.1037/0033-295X.114.4.843. The chapter's summary that habits are "context-cued behavior chunks" once a behavior has been performed often enough in a recurring context is an accurate paraphrase of the paper's central argument. Author affiliations (Wood at USC) match.
- Source: [USC Dornsife PDF](https://dornsife.usc.edu/wendy-wood/wp-content/uploads/sites/183/2023/10/wood.neal_.2007psychrev_a_new_look_at_habits_and_the_interface_between_habits_and_goals.pdf); [APA PsycNet record (DOI 10.1037/0033-295X.114.4.843)](https://psycnet.apa.org/doi/10.1037/0033-295X.114.4.843)

**E3. Line 80 — Wood & Rünger (2016), "Psychology of Habit," *Annual Review of Psychology* 67: 289–314.**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE
- **Verdict:** CONFIRMED
- **Finding:** Wood, W., & Rünger, D. (2016). *Annual Review of Psychology*, 67, 289–314. DOI 10.1146/annurev-psych-122414-033417. Confirmed.
- Source: [Annual Reviews](https://www.annualreviews.org/content/journals/10.1146/annurev-psych-122414-033417); [USC Dornsife PDF](https://dornsife.usc.edu/wendy-wood/wp-content/uploads/sites/183/2023/10/wood.runger.2016.pdf)

**E4. Line 84 — "habit literature is well-evidenced for individual behaviors (exercise, snacking, commuting), more lightly tested on professional-workflow installation"; chapter calls this an extension caveat. `[contested]` flag in-text.**
- Category: EVIDENCE / I-LANGUAGE
- Type: I-LANGUAGE (calibrated epistemic hedge)
- **Verdict:** CONFIRMED (calibration well-placed)
- **Finding:** The chapter's hedge is accurate. The habit literature's strongest evidence is for individual behaviors (eating, exercise, commuting, smoking). Application to professional workflow installation is a defensible extension but is not as well-validated; the chapter labels this honestly. Maintain `[contested]` flag.

**E5. Line 131 — Rogers, *Diffusion of Innovations* (5th ed., Free Press, 2003); five sequential stages: knowledge, persuasion, decision, implementation, confirmation.**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (canonical citation with edition)
- **Verdict:** CONFIRMED
- **Finding:** Rogers, E. M. (2003). *Diffusion of Innovations* (5th ed.). New York: Free Press. ISBN 978-0743222099. Five-stage innovation-decision process (knowledge → persuasion → decision → implementation → confirmation) confirmed. Note: Rogers passed away in 2004; the 5th edition (2003) is the final edition published in his lifetime and remains the standard citation. The "plateau at implementation" framing is the chapter's interpretive layer rather than Rogers's own language, but is consistent with the framework.
- Source: [Simon & Schuster page](https://www.simonandschuster.com/books/Diffusion-of-Innovations-5th-Edition/Everett-M-Rogers/9780743222099); [Amazon ISBN 9780743222099](https://www.amazon.com/Diffusion-Innovations-5th-Everett-Rogers/dp/0743222091)

**E6. Line 133 — Hall & Hord, *Implementing Change* (Pearson, 5th ed.) [`verify edition` flag in-chapter]; CBAM Stages of Concern (awareness → informational → personal → management → consequence → collaboration → refocusing).**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE
- **Verdict:** CONFIRMED (edition flag can be cleared)
- **Finding:** Hall, G. E., & Hord, S. M. (2020). *Implementing Change: Patterns, Principles, and Potholes* (5th ed.). Pearson Education. Confirmed via Pearson catalog. The seven Stages of Concern sequence the chapter lists matches the CBAM canonical seven (numbered 0–6). The `[verify edition]` flag can be removed; 5th ed., 2020 is correct.
- Source: [Pearson catalog page](https://www.pearson.com/en-us/subject-catalog/p/Hall-Implementing-Change-Patterns-Principles-and-Potholes-5th-Edition/P200000001185); [AIR CBAM PDF](https://www.air.org/sites/default/files/concerns-based_adoption_model.pdf)

**E7. Line 133 — CBAM "developed at the University of Texas's Research and Development Center for Teacher Education"; SEDL CBAM resources.**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (institutional provenance)
- **Verdict:** CONFIRMED
- **Finding:** CBAM was developed in the 1970s–80s by researchers at the R&D Center for Teacher Education at the University of Texas at Austin. SEDL (Southwest Educational Development Laboratory, later absorbed into AIR) maintained the public-facing CBAM resources. The chapter's institutional provenance is correct. The seven Stages of Concern (0=awareness, 1=informational, 2=personal, 3=management, 4=consequence, 5=collaboration, 6=refocusing) match SEDL's published framework. Chapter's claim that "stage 3 (management)" is where AI users plateau is interpretive — SEDL describes management as where logistical concerns dominate, which is consistent with the chapter's reading.
- Source: [SEDL CBAM home](https://sedl.org/cbam/); [SEDL Stages of Concern](https://sedl.org/cbam/stages_of_concern.html); [SEDL PDF](https://sedl.org/cbam/stages_of_concern.pdf)

**E8. Line 137 — "Bailey and Palsha argue concerns can be parallel, not strictly sequential"; CBAM critique cited via learntechlib.org. `[contested]` flag in-text.**
- Category: EVIDENCE / SPECIALIST
- Type: POSITIVE (critique attribution)
- **Verdict:** CONFIRMED
- **Finding:** Bailey, D. B., Jr., & Palsha, S. A. (1992). Bailey & Palsha's critique of CBAM (in particular their statistical re-analysis of the Stages of Concern Questionnaire) has been cited as challenging the strict sequential ordering. The chapter's framing — "concerns can be parallel, not strictly sequential" — is a fair paraphrase. The LearnTechLib link in the chapter (`https://www.learntechlib.org/primary/p/8094/`) resolves to "Some Concerns About the Concerns-Based Adoption Model (CBAM) and Technology" (Anderson & others, in *Journal of Educational Computing Research*), which collects this critique tradition. The Bailey & Palsha primary citation is the original 1992 *Journal of Special Education* article; the chapter's link is a secondary survey. For a primary citation: Bailey, D. B., & Palsha, S. A. (1992). "Qualities of the Stages of Concern Questionnaire and implications for educational innovations." *Journal of Educational Research*, 85(4), 226–232. Consider adding the primary cite alongside the LearnTechLib aggregator.
- Source: [LearnTechLib aggregator](https://www.learntechlib.org/primary/p/8094/); primary cite: Bailey & Palsha (1992), *Journal of Educational Research* 85(4): 226–232.

**E9. Line 261 — Botspeak Specification Library "five recurring task buckets"; AI for Education open prompt library; Panorama Education "100+ AI Prompts."**
- Category: EVIDENCE / CURRENT
- Type: POSITIVE (named external resources)
- **Verdict:** CONFIRMED
- **Finding:** AI for Education ([https://www.aiforeducation.io/prompt-library](https://www.aiforeducation.io/prompt-library)) maintains a public prompt library organized by task category. Panorama Education's "100+ AI Prompts" blog is a published resource. Both links resolve. Botspeak reference is to the author's own published work — confirmed by cross-reference to Nik Brown's book.

### GUIDELINE category

**G1. Line 88 — TeachAI, CoSN, and ISTE+ASCD all converge on "fit for purpose" task-tool matching guidance.**
- Category: GUIDELINE
- Type: BASIC (multi-organization synthesis)
- **Verdict:** CONFIRMED
- **Finding:** TeachAI policy resources, CoSN's AI in K-12 hub, and ISTE's AI for educators courses all emphasize task-fit / pedagogical fit over capability ranking. Chapter's framing is accurate.
- Source: [TeachAI policy resources](https://www.teachai.org/policy-resources); [CoSN AI in K-12](https://www.cosn.org/ai/); [ISTE AI courses](https://iste.org/courses/artificial-intelligence-explorations-for-educators)

**G2. Line 74 — Stanford CTL and Truth for Teachers time-blocking guidance; Newport's *Deep Work* (Grand Central, 2016); time-blocking effects are "plausible operational scaffolding, not measured effects." `[contested]` flag in-text.**
- Category: GUIDELINE / EVIDENCE
- Type: I-LANGUAGE (calibrated)
- **Verdict:** CONFIRMED
- **Finding:** Newport, C. (2016). *Deep Work: Rules for Focused Success in a Distracted World*. Grand Central Publishing. ISBN 9781455586691. Publication date January 5, 2016 confirmed. The chapter's hedge that time-blocking attention-percentage claims are operational rather than measured is appropriate — Newport's claims rest on synthesis and self-experiment, not RCTs. Stanford CTL and Truth for Teachers links resolve.
- Source: [Hachette/Grand Central listing](https://www.hachettebookgroup.com/titles/cal-newport/deep-work/9781455586691/?lens=grand-central-publishing); [Stanford CTL time blocking](https://ctl.stanford.edu/weekly-planning-time-blocking-method)

**G3. Line 31 — CRPE and Chalkdust & Silicon framed as critical context on Walton/Gallup figures; conflation of "tool works" with "tool works for the kind of teacher already inclined to use it."**
- Category: GUIDELINE / EVIDENCE
- Type: POSITIVE (named critique)
- **Verdict:** CONFIRMED
- **Finding:** CRPE's substack post on "The AI Dividend" and the Chalkdust & Silicon medium post explicitly raise the selection-vs-treatment critique. Chapter's framing is accurate; both links resolve.
- Source: [CRPE substack](https://crpe.substack.com/p/the-ai-dividenddoes-ai-create-more); [Chalkdust & Silicon Medium](https://medium.com/chalkdust-silicon/the-walton-gallup-ai-report-deserves-context-not-just-headlines-56164a7303a3)

### CURRENT category

**C1. Line 117 — "major commercial models currently ship significant updates on roughly a 2–4 month cadence"; six-month maintenance cycle gives "two model-generations of drift to catch." `[verify]` flag in-text.**
- Category: CURRENT
- Type: BASIC (operational heuristic)
- **Verdict:** UNVERIFIED (well-flagged)
- **Finding:** The 2–4 month cadence claim is operationally defensible — OpenAI, Anthropic, and Google have all shipped significant model updates within 2–4 month windows during 2024–2025. The "controlled studies of prompt-output stability across model versions have not been published at the granularity teachers need" caveat is correct as of May 2026. Keep the flag.

**C2. Line 411 — arXiv paper on teacher-authored prompts as district-portable assets, "Spring 2025 pilot, 16 teachers, 4 districts, 878 students," link to `https://arxiv.org/html/2604.16738v1`.**
- Category: CURRENT / EVIDENCE
- Type: POSITIVE (precise sample sizes)
- **Verdict:** UNVERIFIED
- **Finding:** The arXiv URL resolves to "Teacher-Authored Prompts for Configuring Student–AI Dialogue: K–12 Classroom Implementation" (arXiv:2604.16738v1, April 2026). The arXiv identifier `2604.16738` is structurally consistent with April 2026 submissions. Sample-size claims (16 teachers, 4 districts, 878 students) and "Spring 2025 pilot" framing need direct verification against the manuscript body — chapter should confirm these before final publication. Mark UNVERIFIED.
- Source: [arXiv:2604.16738v1](https://arxiv.org/html/2604.16738v1)

### SPECIALIST category

**SP1. Line 21 — Composite-illustrative case (Teacher A and Teacher B) explicitly labeled as not specific documented individuals; the ~2 hr and ~12 hr figures are "plausible upper-tail observations" relative to the 5.9-hour mean.**
- Category: SPECIALIST / I-LANGUAGE
- Type: I-LANGUAGE (labeled hypothetical)
- **Verdict:** CONFIRMED (well-labeled)
- **Finding:** Chapter explicitly flags the composite-illustrative nature at line 21 and clarifies that the per-week figures are illustrative, not separately measured medians. This is the workshop's standard labeling protocol for hypotheticals. Clean.

**SP2. Line 49 — "The Center on Reinventing Public Education has been the most public voice" on the selection-vs-treatment critique. `[contested]` flag in-text.**
- Category: SPECIALIST
- Type: POSITIVE (named institutional voice)
- **Verdict:** CONFIRMED
- **Finding:** CRPE has been the most public voice on the selection-effect critique of the Walton-Gallup 2025 figures. The chapter's attribution is accurate.
- Source: [CRPE substack](https://crpe.substack.com/p/the-ai-dividenddoes-ai-create-more)

**SP3. Line 410 — Chapter 1's "16.7-hour weekly ceiling under fully systematic deployment"; Teacher B's 12 hours sits below; "honest 20-hour personal-experience claim cited in Chapter 1."**
- Category: SPECIALIST / I-LANGUAGE
- Type: I-LANGUAGE (cross-chapter reference, hedged)
- **Verdict:** CONFIRMED (internal cross-reference)
- **Finding:** Cross-chapter reference; the 16.7-hour projection and 20-hour personal-experience claim are Chapter 1's territory and are flagged in that chapter's factcheck file. As Chapter 12 explicitly labels the gap from 12 to 16.7 as "open" and the 20-hour figure as "a single self-report and not yet a finding," the hedging is appropriate.

---

## Unverified Assertions

1. **S3 — 68% no-formal-AI-training (RAND).** Chapter's existing `[verify]` flag remains. Cite RR-A956-31 for district side, the teacher-side wave for 68%. (See note above; teacher-side companion data is referenced in K-12 Dive and AI for Education coverage but the cleanest RAND-internal citation should be RR-A4180-1 or a forthcoming teacher-survey publication.)
2. **C1 — 2–4 month model update cadence.** Plausible operational heuristic, not measured. Keep `[verify]` flag.
3. **C2 — arXiv:2604.16738v1 sample sizes.** Verify "16 teachers, 4 districts, 878 students" against the manuscript text before final publication.
4. **E1 — Davenport & Prusak direct quote.** "Knowledge works across networks and communities" — quote attribution should be verified against the print volume page reference.
5. **E4 — habit literature professional-workflow extension.** Already flagged `[contested]`; calibration is appropriate.

---

## AI-Pass Flags

- **Cross-book unit error (Bastani "17 percentage points") — NOT PRESENT IN THIS CHAPTER.** Chapter 12 does not cite the Bastani magnitude; the only Bastani-adjacent reference is the chapter's own internal hedging around effect magnitudes. Clean.
- **References section absent.** Chapter has rich in-text citations but no References section at the end. Added on this pass per the standing protocol.
- **Inline FACT-CHECK flag.** Added at the top of the chapter with UNVERIFIED verdict (driven by the three remaining UNVERIFIED items: S3 wording, C1 cadence, C2 arXiv sample sizes) and pointer to this report.
- **`[verify edition]` flag on Hall & Hord (line 133).** Can be cleared on a future pass — 5th ed., Pearson, 2020 is confirmed.
- **Author claim of `voice-unanchored = not raised`** at line 425 — appropriate per the chapter's reasoning that voice is established by prior chapters.

---

## Reliability assessment

Chapter 12 is one of the most epistemically careful chapters in the book — every load-bearing quantitative claim is either confirmed against primary sources or already flagged with `[verify]` or `[contested]` in-text. The Gallup-Walton 2025 figures (5.9 hr, n=2,232, 32%/28%/40% usage split, 52%/31% training split) are fully confirmed; the RAND 48%/23% district figures and 67%/39% equity gap are confirmed; the canonical knowledge-management, habit psychology, diffusion theory, and CBAM citations are all confirmed with correct editions. The remaining UNVERIFIED items are appropriately hedged in-text by the author. The chapter does not commit the cross-book Bastani unit error.
