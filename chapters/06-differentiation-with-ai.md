# Chapter 6 — Differentiation with AI: Reading Levels, Scaffolds, and Supports

**TL;DR.** AI can produce three reading-level versions of a passage faster than you can pour coffee — and the speed is precisely the problem, because hitting a target Lexile band is not the same as preserving the cognitive demand the original passage was designed to elicit. This chapter teaches you the difference between scaffolding that opens access and leveling that strips the trigger for learning, and where the legal and clinical gates sit when AI proposals brush up against IEPs, 504s, and FERPA.

---

## Learning objectives

By the end of this chapter, you should be able to:

1. **Apply.** Use AI to adjust the reading level of a text to a specified target band while preserving the core conceptual content.
2. **Apply.** Generate a scaffolded version of an assignment for students with specified learning needs — sentence frames, vocabulary supports, graphic-organizer templates.
3. **Apply.** Write a prompt that anonymizes student information before any external AI submission.
4. **Analyze.** Apply the differentiation phase gate: AI proposes the accommodation scaffold; the teacher — or, for IEP/504, the licensed specialist and team — verifies and authorizes.
5. **Evaluate.** Identify what AI cannot supply: knowledge of the specific student's history, clinical judgment, legal authorization, and the distinction between simplification that helps and simplification that strips.

---

## 1. Opening case — twenty-eight readers, one passage

*This case is composite-illustrative. The teacher is not a single documented person. The pattern — wide Lexile spread in a heterogeneous middle-school science class, multi-version handouts as a prior workflow, AI-assisted leveling as a current one — matches the typical classroom profile described in the Walton Family Foundation / Gallup 2025* Teaching for Tomorrow *survey, which found that 64% of teachers who use AI for material modification report quality improvement* ([Walton/Gallup 2025](https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf)). *The specific minute-by-minute arithmetic below is illustrative, not measured.*

It is 4:47 on a Tuesday afternoon. A sixth-grade science teacher — call her Ms. Park — has a one-page article on coral bleaching open on her laptop. She wants the class to read it tomorrow and argue, in writing, whether the bleaching is reversible. Twenty-eight students. Reading levels run from roughly third grade to roughly tenth. Two newcomer multilingual learners — one Mandarin-dominant, one Haitian-Creole-dominant. One student with an IEP for a specific learning disability in reading; one with a 504 for ADHD and an extended-time accommodation. The article is somewhere around 1050L. The third-grade reader will see a wall of words.

A year ago, this is a three-hour Tuesday night. The article, retyped at three Lexile bands. A glossary for the multilingual learners. A graphic organizer for the IEP student. Three printouts to a folder. By 8 p.m. her dinner is in the microwave.

Tonight, Ms. Park opens Claude. She pastes the article and writes a prompt: rewrite at 600L, 800L, and 1050L; preserve every scientific claim and every date; flag any concept the rewrite simplified. Twelve minutes later she has three versions on screen.

Then she works for thirty minutes — and the thirty minutes are the chapter. She runs the 600L version through a Lexile analyzer; it reads as 590L. The dates survived. The two scientific claims survived. But the *causal* claim — that warmer water stresses the symbiotic algae the coral depends on — has been softened into "the coral gets sick when the water is warm." The mechanism that tomorrow's writing prompt is supposed to be arguing about has been sanded away. She edits one sentence back in. In the 800L version, *symbiotic algae* has become *tiny plants that live with the coral*; she keeps the original term and adds it as a glossed vocabulary item, because the word *symbiotic* is part of the lesson.

She generates a sentence-frame scaffold for the multilingual learners at WIDA Levels 2 and 4, and a compare-contrast graphic organizer for the student with the reading IEP. Both pass review with light edits. None of the prompts contains a student's name, ID, or identifying detail; the IEP-relevant prompt is phrased as *a sixth-grade student with an IEP for a specific learning disability in reading, who benefits from graphic organizers for compare-contrast tasks*.

Forty-two minutes. Three things are worth naming. First, the AI did not "differentiate the text" — it produced three versions at specified bands; the teacher *differentiated* by deciding which simplifications were pedagogically defensible. Second, the dividend is not in the twelve minutes of generation; it is in the substitution of *judgment time* for *retyping time*. Third, the lowest-Lexile version was the one most in danger of leveling its way out of the lesson. The teacher's spot-check found it. Without the spot-check, the AI would have shipped a 600L handout in which the concept the unit is about no longer appears.

This chapter is about that forty-two minutes. What AI can productively generate. What only you — or the licensed specialist on your IEP team — can authorize. And where the gates sit between them.

---

## 2. The core concept — leveling, scaffolding, and the trigger for learning

Differentiation is not one move. It is a family of moves, and the AI dividend depends entirely on knowing which one you are making. Sort them carefully, because the same tool that produces an excellent scaffold can produce a beautifully simplified text that has quietly removed the cognitive work the lesson was designed to elicit.

### 2.1 What Lexile actually measures (and why AI is good at moving it)

The Lexile Framework, maintained by MetaMetrics, is a psychometric scale placing reader ability and text complexity on a single axis from below 0L to above 1600L ([MetaMetrics — Lexile Framework](https://www.metametrics.com/lexile-for-reading/)). To assign a Lexile to a text, MetaMetrics splits it into 125-word slices, compares each to a large reference corpus, and runs two statistics — sentence length and word frequency — through the Lexile equation and a Rasch psychometric model ([Lexile Technical Report](https://metametricsinc.com/wp-content/uploads/2017/07/Stenner_Burdick_Sanford__Burdick-_The_LFR_Technical_Report.pdf)).

That two-input formula — sentence length and word frequency — is the load-bearing fact for this chapter. Everything an LLM does when it "lowers the Lexile" of a passage is, mechanically, a manipulation of sentence length and word frequency. The model shortens clauses, breaks compound sentences, swaps low-frequency words for higher-frequency ones. *Symbiotic* becomes *tiny plants that live with the coral*. *Photosynthesis* becomes *the way plants make food from sunlight*.

This is why the technique works. It is also why it is shallower than it looks. The Lexile formula does not measure inferential demand, syntactic complexity beyond sentence length, prior-knowledge load, abstractness of referents, or organizational coherence. A passage rewritten to hit 700L can still be conceptually opaque if the underlying ideas are abstract. The Lexile label measures one slice of text difficulty, not all of it.

Two consequences: (1) The AI is doing something real when it lowers the Lexile — it is doing exactly the operation the Lexile formula scores. (2) Hitting the Lexile is necessary, not sufficient. Whether the *content* survived is a separate question that no readability formula answers. That is the teacher's job at the gate.

A note on evidence. Peer-reviewed work on whether GPT-class commercial models reliably hit specified Lexile bands at K–12 grade levels — and whether their simplifications preserve content fidelity — is thin as of this writing. The closest adjacent evidence is in medical-report simplification: a 2025 study by Khazanchi et al. in *Skeletal Radiology* found that GPT-4 reduced the average reading level of spine imaging reports from grade 11.47 to grade 8.50, but 34% of simplified outputs omitted at least one clinically relevant fact ([Khazanchi et al., 2025, *Skeletal Radiology*, DOI 10.1007/s00256-025-05027-9](https://doi.org/10.1007/s00256-025-05027-9)). Different domain, different metric, adult text — so the rate is not transferable. The transferable point is the *shape* of the failure. The model reliably moves the readability metric. It does not reliably preserve the substance. The chapter's spot-check exists because that pattern shows up wherever it has been measured.

### 2.2 Leveling versus scaffolding — the Frictional distinction

This is the move most teachers miss in the first weeks of AI-assisted differentiation, and it is the move the whole chapter turns on.

**Leveling** changes the text. The student reads a different version. The cognitive work the original passage was designed to elicit may or may not survive the rewrite.

**Scaffolding** does not change the text. The student reads the original. Around the text, the teacher places supports — a sentence frame, a vocabulary glossary, a graphic organizer, a model paragraph, a partner read — that absorb the *extraneous* load (the load that is not the learning) so the *germane* load (the load that *is* the learning) can be carried.

The Frictional argument in this book's Preface ([Preface](../preface.md)) says that genuine learning is triggered by cognitive friction — the prediction-error event that occurs when a learner's current model meets material that does not fit. Productive struggle is the mechanism of learning. Without it, no trigger; without the trigger, no consolidation; without consolidation, no durable change.

A scaffold that absorbs the *extraneous* load preserves the trigger. A leveled text that absorbs the *germane* load removes it. They look similar. They are not. A 600L rewrite of a coral-bleaching passage that has gently dropped the causal mechanism has not differentiated; it has decided, on the student's behalf, that this student should not have to think about cause and effect today. That is a removal, not a support.

The discipline: every time you lower the band, ask whether the simplification dropped any of the work the lesson was designed to do. If yes, edit the work back in, or pick a different scaffold instead. The shortest test in plain English: *would I be teaching the same concept tomorrow if every student were on this version?* If no, you have not differentiated. You have routed some students out of the lesson.

The Bjorkian distinction between *storage strength* and *retrieval strength* applies here: material that feels easy in the moment is not material that has been encoded deeply. A 400L version of a 900L science passage can produce a student who reads fluently, answers questions on the easier text, and remembers none of it two weeks later. AI-assisted leveling is particularly susceptible to that pattern, because the simplification target — fluent reading — is exactly the surface signal the Bjorkian research warned us not to trust.

### 2.3 UDL — designing for variability up front

The Universal Design for Learning (UDL) framework, developed and maintained by CAST, is the canonical framework for designing instruction that anticipates learner variability from the start, rather than retrofitting accommodations afterward ([CAST UDL Guidelines](https://udlguidelines.cast.org/)). UDL 3.0 (CAST, July 2024) is organized around three principles — Engagement, Representation, and Action & Expression — and frames learner identity as a dimension of variability across all three.

The distinction matters for the AI workflow. AI is fast at the retrofit: *give me a 700L version, give me sentence frames, give me a graphic organizer.* AI is less reliable at the upstream UDL move: *design this lesson so the same content is accessible at multiple reading levels and through multiple modes of expression from the start.*

The temptation, with a tool that retrofits this fast, is to skip the design move. Don't. The UDL audit is one question: *where do students have a choice in how they show what they learned?* If the answer is "nowhere," your differentiation is one-dimensional — you have varied the input and left the output identical. Use AI for multiple means of *representation* (multiple Lexile bands, multiple media, vocabulary support). Use it for multiple means of *action and expression* too (audio response options, structured outline templates, alternatives to a written paragraph). The teacher's design move is to ask for both.

### 2.4 ELL/MLL scaffolds — what WIDA gives you that the LLM doesn't

The WIDA English Language Development Standards Framework (2020 edition) is the most widely adopted ELD framework in U.S. K–12; 41 states, territories, and federal agencies are WIDA consortium members ([WIDA 2020](https://wida.wisc.edu/resources/wida-english-language-development-standards-framework-2020-edition)). The framework differentiates language development across six proficiency levels — Entering, Emerging, Developing, Expanding, Bridging, Reaching — along three dimensions (word/phrase, sentence, discourse) and organizes around four Key Language Uses: Narrate, Inform, Explain, Argue.

For AI-assisted differentiation, WIDA gives you vocabulary the model does not have. The vague prompt "*generate sentence frames for ELL students*" produces generic frames. The specific prompt "*generate sentence frames at WIDA Level 2 (Emerging) and WIDA Level 4 (Expanding) for sixth-grade students arguing whether coral bleaching is reversible, with one frame per Key Language Use of Argue*" produces a usable artifact. The framework also names what the LLM cannot supply: where this specific student sits on the continuum, the home language she is translanguaging from, the registers she has encountered.

A misconception to name flat: **translation is not differentiation.** A perfectly translated Spanish version of an inaccessible English text is still an inaccessible text in Spanish. WIDA's framing — that multilingual learners can engage with grade-level content given appropriate scaffolds — explicitly resists the deficit reading in which "ELL version" means "easier content." The scaffold gives access to the same content; it is not a substitute for it.

A sentence frame at WIDA Level 3 — *"One piece of evidence for [claim] is [evidence]. This is important because [reasoning]."* — gives the multilingual learner the structure of academic argument while leaving the cognitive work, the actual claim and evidence, to her. The frame lowers the *linguistic* friction. It does not lower the *conceptual* friction, which is the trigger we are trying to preserve.

### 2.5 IEP and 504 supports — AI proposes, the team authorizes

*This section operates at the principle level. Specific compliance decisions — what counts as sufficient anonymization, what is and is not authorized to be drafted by AI, what your district's contracted tools permit — must be made in consultation with your district's data-privacy officer, special-education director, licensed specialist staff, and counsel. None of what follows is legal advice.*

Individualized Education Programs (IEPs) under the Individuals with Disabilities Education Act (IDEA, Part B) are legal documents developed by a multi-disciplinary team. Federal law specifies the minimum membership: a parent, a general-education teacher (if applicable), a special-education teacher, a Local Education Agency representative qualified to supervise special education, and someone who can interpret evaluation results ([Congressional Research Service R41833 — IDEA Part B](https://www.congress.gov/crs-product/R41833); [US Department of Education — A Guide to the IEP](https://www.ed.gov/sites/ed/files/parents/needs/speced/iepguide/iepguide.pdf)). The team — not the general-education teacher alone, not the AI — authorizes accommodations and modifications. Section 504 of the Rehabilitation Act of 1973 covers students with disabilities who do not qualify under IDEA but who require accommodations to access the general curriculum; 504 plans are developed through a similar team process.

The phase gate falls out of the law and the clinical reality together: AI can read an anonymized profile and propose accommodations from the standard library — extended time, frequent breaks, audio versions of text, sentence frames, preferential seating, modified workload, graphic-organizer templates. The proposal is a starting point. The authorization is a legal act made by the team, with the licensed specialist present, on the basis of *this* student's history, evaluation results, and prior response to intervention.

The misconception to name flat: **AI cannot write the IEP.** It can draft accommodation language. It can suggest accommodations consistent with an anonymized profile. It cannot substitute for the team's judgment that an accommodation is appropriate for this student. A teacher who accepts AI-generated accommodations without team review has violated both the procedural requirement under IDEA and the substantive judgment the gate exists to exercise. The phase gate, stated: *AI proposes from an anonymized profile; the licensed specialist and team authorize; the teacher implements what the team authorized.* Implementing it correctly requires deferring specifics to the people licensed to make them.

### 2.6 The anonymization gate — FERPA, COPPA, and the principle under them

*Again: the principle here is general. Specific district policies, state guidance, and contracted-tool exceptions vary, and your district's data-privacy officer and counsel are the people who decide what is permitted in your setting.*

The Family Educational Rights and Privacy Act (FERPA, 20 U.S.C. § 1232g) protects personally identifiable information (PII) in education records. The Children's Online Privacy Protection Act (COPPA, 15 U.S.C. § 6501) governs the collection of personal data from children under 13. Together they form the legal floor under any decision to send student information to a third-party AI tool. The U.S. Department of Education's Office of Educational Technology published its first major guidance on AI in education in May 2023 — *Artificial Intelligence and the Future of Teaching and Learning* ([OET](https://www.ed.gov/sites/ed/files/documents/ai-report/ai-report.pdf)). As of mid-2025, at least 25 state departments of education have issued their own AI guidance documents ([Student Privacy Compass](https://studentprivacycompass.org/state-guidance-on-the-use-of-generative-ai-in-k-12-education/)).

The principle is straightforward to state and harder to enforce in a hurry. PII in education records cannot be disclosed to a third party without consent, except under specific exceptions. When a teacher pastes a student's name, ID, behavioral history, or evaluation results into a public chatbot, the teacher has disclosed PII to a third party — the AI vendor, who is not bound by FERPA unless under a written service agreement with appropriate provisions. The Future of Privacy Forum's 2024 *Vetting Generative AI Tools for Use in Schools* lays out the compliance frame ([FPF 2024](https://fpf.org/wp-content/uploads/2024/10/Ed_AI_legal_compliance.pdf_FInal_OCT24.pdf)).

The operational rule, at the principle level: **anonymize before submitting.** Replace student names with role labels (*"Student A, 6th grade, reads at approximately Lexile 600, has an IEP for ADHD with extended-time and break-frequency accommodations"*). Strip identifying detail. Keep educationally relevant features. The AI's suggestion can then be applied back to the specific student by the teacher and team who know who Student A is.

What counts as *sufficient* anonymization is contested — whether quasi-identifiers like free-lunch status combined with grade and class size can re-identify a student in a small school depends on population size, the data, and tool terms of service. **Your district's data-privacy officer and counsel decide what is sufficient in your setting.** If your district has contracted with a vendor under a FERPA-compliant agreement (a Microsoft Copilot for Education deployment, a Google Gemini for Education deployment, a vetted MagicSchool or Brisk deployment), the rules inside that walled garden differ from the rules in a public chatbot. Default outside the walls: the anonymization rule.

### 2.7 The differentiation phase gate, stated

> **AI proposes the differentiation. The teacher verifies that the simplification did not strip the cognitive demand the lesson was designed to elicit, and that no student PII left the room. For accommodations under IEPs and 504 plans, the licensed specialist and team authorize before anything is delivered to a student.**

Three sentences. They are the entire skill of this chapter.

---

## 3. Worked example — one paragraph, three Lexile bands, one decision

Take a single paragraph from a middle-school science article on the 2014–2017 mass bleaching event on the Great Barrier Reef (the article itself is hypothetical for this worked example; the underlying scientific claims are well-documented). Original (estimated ~1050L):

> *Between 2014 and 2017, repeated marine heatwaves drove the Great Barrier Reef into the most severe bleaching event on record. When sea surface temperatures rose more than one degree Celsius above the long-term summer maximum, the symbiotic algae that live inside coral tissues — called zooxanthellae — were expelled, leaving the coral skeleton visible through transparent tissue. Without the algae's photosynthetic products, much of the affected coral starved within weeks.*

Three Lexile bands, generated with a prompt structured this way:

```
ROLE: You are an editor adapting science writing for grade-level readers.
CONTEXT: Source paragraph is approximately 1050L, from a sixth-grade science
unit on coral reef ecology. Class includes readers from ~600L to ~1100L.
TASK: Produce three versions of the paragraph at target bands 600L, 800L,
and 1050L. Preserve every scientific claim, every date, and the causal
mechanism (heat -> algae expulsion -> coral starvation).
CONSTRAINTS:
- Do not invent facts not in the source.
- Keep the term "zooxanthellae" in the 1050L and 800L versions; in the
  600L version, define it with the simpler phrase and keep the term in
  parentheses.
- After each version, list any concept you simplified that the teacher
  should double-check before using.
- Do not include student names or identifying information.
```

A reasonable output (illustrative — yours will vary):

**1050L:** *Between 2014 and 2017, a series of marine heatwaves drove the Great Barrier Reef into the worst bleaching event ever recorded. When sea surface temperatures climbed more than 1 °C above the long-term summer maximum, the symbiotic algae living inside coral tissues — zooxanthellae — were expelled, and the white coral skeleton became visible. Without the algae's photosynthetic products, much of the affected coral starved within weeks.*

**800L:** *From 2014 to 2017, repeated heat waves caused the worst coral bleaching ever recorded on the Great Barrier Reef. When the water became more than 1 °C warmer than the usual summer high, the tiny algae inside the coral — called zooxanthellae — were pushed out. Without the food the algae made through photosynthesis, much of the coral starved within weeks.*

**600L:** *Between 2014 and 2017, the ocean got very warm three years in a row. The tiny algae that live inside coral (called zooxanthellae) leave when the water gets too warm. Without the algae, the coral turns white. Without the food the algae made, much of the coral died within weeks.*

Now run the spot-check.

**Did the AI hit the band?** Run each version through a Lexile analyzer. In this example, the 800L probably comes in around 770–820L, the 600L around 580–650L, the 1050L around 1000–1080L. If a version misses by more than a hundred points, prompt again. If it hits within a hundred points, that is about as accurate as you should expect — and you should still run the analyzer to know which way it missed.

**Did every claim survive?** Walk down the original. Dates: yes, all three. Temperature threshold of 1 °C above the long-term summer maximum: yes in 1050L and 800L; in 600L, "too warm" — the *specific threshold* was lost. Photosynthetic products as the food source: yes in 1050L and 800L; in 600L, "the food the algae made" — the *process* was lost. Coral starvation: yes, all three.

**Did the cognitive demand survive?** This is the Frictional check. Tomorrow's lesson asks students to argue whether the bleaching was reversible — an argument that depends on the causal chain from heat to algal expulsion to lost photosynthetic products to starvation. Does the 600L version preserve enough of the chain to argue from?

The 600L version preserves the *sequence* — water warms, algae leave, coral turns white, coral dies — but the chain has become four facts in a row rather than a mechanism. The threshold (1 °C above the long-term summer maximum) and the process (photosynthesis as food production) are gone. A sixth-grade reader who can only access the 600L version can answer *what happened* but will struggle with *why* and *under what condition*. The argument the lesson is designed to elicit — *was the bleaching reversible?* — needs the conditions.

This is the moment. You have a choice:

- **Option A.** Accept the 600L version as written. The lowest-band readers will get *what happened.* The argument will be inaccessible to them. This is leveling that has stripped the cognitive demand. Avoid.
- **Option B.** Edit the 1 °C threshold and the word *photosynthesis* back into the 600L version with a short gloss. The text becomes a ~680L version that preserves the mechanism. Differentiation that kept the trigger.
- **Option C.** Hand the lowest-band readers the 800L version paired with a partner-read scaffold and a graphic organizer that maps the causal chain. This uses *scaffolding* to compensate for the higher band rather than *leveling* to remove it. Often the best choice when the mechanism is the lesson.

The AI cannot make this choice for you. It produced three versions; you decide which, with which scaffolds, preserves the lesson. That decision is the differentiation. The Lexile rewrite is a draft you argued with.

**The named trade-off.** Lower-Lexile versions buy fluent reading at a cost paid in mechanism, conditional reasoning, and process language. Buying the fluency is sometimes right (when fluent access is the goal — a current-events read-aloud, a daily journal entry). Buying it is sometimes wrong (when the mechanism *is* the lesson). The teacher who reflexively reaches for the 600L version every time has not chosen, has defaulted. The teacher who reflexively reaches for the original every time has also not chosen. Choose, paragraph by paragraph, with the trade-off named out loud.

**The lesson and the limit.** AI-leveled text is a draft. The Lexile move is real, repeatable, fast — that is the lesson. The Lexile move does not measure inferential demand, prior knowledge, or organizational coherence — that is the limit. The spot-check is the part of the job AI cannot do.

---

## 4. The three prompt templates

Each template assumes the anonymization rule has already been applied — no student names, no IDs, no identifying detail. The bracketed placeholders are where the teacher fills in context the AI does not have.

### 4.1 Lexile-adjustment prompt

```
ROLE: You are an editor adapting [grade-level] science / social studies /
literature text for grade-level readers.
CONTEXT: Source passage below is approximately [estimated Lexile] L, from
a [grade] unit on [topic]. Class includes readers from approximately
[lower band] L to [upper band] L.
TASK: Produce [n] versions of the passage at target bands [band 1, band 2,
band 3]. Preserve every factual claim, every date, every named entity,
and the causal mechanism the passage is built around.
CONSTRAINTS:
- Do not invent facts not present in the source.
- Keep the following terms in all versions: [term 1], [term 2]. In the
  lowest band, define the term in plain English and keep the term in
  parentheses on first use.
- After each version, list any concept you simplified that I should
  double-check before delivering the text to students.
- Do not include student names, IDs, or any identifying information.

SOURCE PASSAGE:
[paste passage here]
```

Anonymization built in by default: the prompt accepts text, not students.

### 4.2 Scaffolded-assignment prompt

```
ROLE: You are an instructional designer producing scaffolded versions of
a writing or discussion task for a mixed-ability classroom.
CONTEXT: Grade [grade], subject [subject], aligned to standard [standard].
The task asks students to [task in one sentence]. Student population
includes [description without identifying detail — e.g., "two multilingual
learners at approximately WIDA Levels 2 and 4," "one student with an IEP
for a specific learning disability in reading who benefits from graphic-
organizer supports"].
TASK: Produce the base task plus three scaffolded supports: (1) sentence
frames at the specified WIDA levels using the Key Language Use of
[Narrate/Inform/Explain/Argue]; (2) a graphic-organizer template matching
the task structure; (3) a vocabulary glossary of 5–8 academic terms with
student-friendly definitions.
CONSTRAINTS:
- Supports should reduce extraneous load (linguistic, organizational),
  not the cognitive demand of the task itself.
- Do not produce a "simpler version" that removes conceptual work.
- Do not include student names, IDs, or identifying information.
- Label any supports intended for use under an IEP or 504 plan as
  "draft for IEP/504 team review."
```

The constraint that scaffolds reduce extraneous and not germane load is the Frictional check, baked into the prompt.

### 4.3 Vocabulary-support prompt

```
ROLE: You are a vocabulary coach producing tiered word supports for
grade-level readers.
CONTEXT: Grade [grade], subject [subject], unit on [topic]. The target
academic vocabulary is: [list of 6–12 terms]. Class includes multilingual
learners at WIDA Levels [list of levels present].
TASK: For each term, produce:
- A grade-appropriate, student-friendly definition (one sentence).
- One example sentence using the term in context.
- A common misconception or confusable near-synonym to flag.
- For WIDA Levels 1–2: a visual cue suggestion (icon, image, or simple
  diagram description).
- For WIDA Levels 3–4: a sentence frame that uses the term in argument
  or explanation.
CONSTRAINTS:
- Do not substitute simpler synonyms in place of the academic term in the
  definition — the goal is access, not avoidance.
- Do not include student names, IDs, or any identifying information.
```

Note what the prompt explicitly forbids — substituting simpler synonyms for the academic term — because that is the failure mode where vocabulary support quietly becomes vocabulary avoidance.

---

## 5. Common misconceptions

These are the four most common misreadings of the chapter, and why each fails.

### 5.1 "Lower Lexile equals appropriate scaffold."

The central confusion. Hitting a target Lexile band is a manipulation of sentence length and word frequency. It tells you nothing about whether the conceptual content survived or whether the lower-band reader can do the work the lesson is asking for. The Lexile match is necessary, not sufficient. A 600L version that has dropped the causal mechanism is not an accommodation — it is a quiet rerouting of a student out of the lesson. The fix: every time you accept a lower-band version, run the three-question spot-check from the worked example.

### 5.2 "AI can handle IEP recommendations."

It cannot. It can draft accommodation language. It can suggest accommodations consistent with an anonymized profile. It cannot substitute for the procedural and substantive judgment that an IEP or 504 team is required by federal law to exercise. The IEP team — including the licensed special educator — is the authorizing body under IDEA. The 504 team authorizes under Section 504. The teacher's role is to implement what the team has authorized. The fix is procedural: AI proposes from an anonymized profile; the team authorizes; the teacher implements.

### 5.3 "I can paste student work into ChatGPT."

Not by default, and not in a public chatbot, without violating the principle that PII in education records cannot be disclosed to a third party without consent. The chatbot is a third party. Identifiable student work is an education record. Pasting it in is a disclosure. The fix is the anonymization gate. Strip names, IDs, and identifying detail before submitting. Replace with role labels. Keep educationally relevant features. *What counts as sufficient anonymization in your district is decided by your district's data-privacy officer and counsel.* If your district has contracted with a vendor under a FERPA-compliant agreement, the rules inside that walled garden may differ. Find out which tools your district has contracted.

### 5.4 "Translation equals differentiation."

A perfectly translated Spanish version of an inaccessible English text is still an inaccessible text in Spanish. WIDA is explicit: multilingual learners can engage with grade-level content when the *language* scaffolds are in place; "ELL version" should not mean "easier content." The fix is to keep the conceptual demand and add the linguistic supports — sentence frames at the appropriate WIDA level, vocabulary glossaries with the academic term preserved, bilingual glossaries that *bridge* home language to academic English rather than replace it. Translation is one supplementary support among many.

---

## 6. Exercises

Three exercises, graduated from application to evaluation to creation.

### 6.1 The Lexile audit (Apply)

Take one passage from a current unit at its native Lexile. Use the Lexile-adjustment prompt from §4.1 to generate two lower-band versions and one same-band cleanup. For each version: (1) estimate the Lexile yourself; (2) measure it with an analyzer (MetaMetrics provides one through the Lexile Hub); (3) note the gap between the AI's claim, your estimate, and the measurement; (4) list every claim, named entity, date, and causal connection in the original — check whether each survived; (5) run the Frictional check: would the lesson the original was designed to teach still be the lesson if the student read this version? Write one sentence about what the audit revealed about how the AI was simplifying.

### 6.2 The FERPA-safe prompt (Apply)

Take a real student profile from your current class — mentally, not on the page. Without writing the student's name, ID, or any identifying detail, rewrite the profile as a prompt: replace the name with a role label, strip identifying detail (specific school, classroom, date of birth, household composition), keep educationally relevant features (grade, approximate reading level, IEP/504 status by category, WIDA level if applicable, known supports). Use the scaffolded-assignment prompt from §4.2 to generate a differentiation move. Then ask, in writing: *would this prompt have exposed any PII to the AI vendor if I had submitted it?* The exercise is the editing.

### 6.3 The differentiated unit (Create)

Choose one upcoming unit (two to five lessons). Design the differentiation up front rather than retrofitting it. (1) **Representation:** generate Lexile-adjusted versions of the central text covering the spread in your class; run the Lexile audit on the lowest band. (2) **Scaffolding:** generate WIDA-aligned sentence frames and a graphic-organizer template for each lesson, anchored to the Key Language Use (Narrate, Inform, Explain, Argue). (3) **Action and expression:** generate at least two alternative modes of expression for the assessment (audio response, outlined-paragraph scaffold, Venn diagram option); apply the Frictional check to each. (4) **IEP/504 review:** for any student with an IEP or 504, identify the accommodations the team has already authorized and build them in. Do not introduce new accommodations without team review. Flag any AI proposal that goes beyond the authorized plan for the next team meeting. After teaching the unit, write one sentence about what worked, one about what did not, one about what the AI could not have known.

---

## 7. What would change my mind

A well-powered, peer-reviewed study showing that commercial LLMs reliably (within ±100L, 95% of the time) hit specified Lexile bands at K–12 grade levels *while* preserving inferential demand, mechanism fidelity, and standards-aligned content — measured by independent expert review, not by the readability metric alone — would force this chapter to relax its heavy emphasis on the teacher's spot-check. The spot-check would become quality assurance rather than the substantive differentiation act. As of this writing, the evidence base is thin enough that the spot-check *is* the differentiation, not an audit of it.

## 8. Still puzzling

Three questions I do not yet have a confident answer to.

First — what counts as sufficient anonymization under FERPA when AI vendors' terms of service have changed in the last six months. The principle is settled; the threshold is moving. District policies and counsel are the right people to track it.

Second — whether AI-leveled materials, used at scale across a district, widen or narrow exposure gaps. Students who routinely read lower-band versions may be getting accessible practice (good) or being routed away from grade-level concepts repeatedly (not good). The longitudinal evidence is emerging.

Third — whether the Frictional check transfers cleanly to AI-generated scaffolds (sentence frames, graphic organizers) or whether scaffolds are categorically different from leveling and require their own audit. My current reading is that the check transfers, but I have not seen the controlled studies that would let me say it confidently.

---

**Bridge to Chapter 7.** Differentiation is what students *receive*. Chapter 7 turns the camera around: what teachers communicate *outward* — to parents, administrators, IEP team members — and how AI can draft progress reports, meeting summaries, and behavioral records from rough notes while the teacher retains the relationship and the core message. The anonymization gate from this chapter does not relax in the next one; it tightens.

---

**Tags:** differentiation, Lexile, UDL, WIDA, IEP-504, FERPA, scaffolding, Frictional, anonymization, multilingual-learners
