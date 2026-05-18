# Chapter 4 — Lesson Planning and Curriculum Design with AI

**TL;DR.** An AI can produce a structurally correct lesson plan in seconds, and the most rigorous published trial to date — the NFER/EEF "ChatGPT in Lesson Preparation" RCT — found a 31% reduction in lesson preparation time, with no observed loss of resource quality on blind expert review. That same trial measured time and resource quality — not student learning — and that distinction is the entire chapter.

---

## Learning objectives

By the end of this chapter, you should be able to:

1. **Apply.** Use AI to generate a lesson plan skeleton with learning objectives, an activity sequence, and an assessment aligned to a named standard.
2. **Apply.** Write a lesson planning prompt that includes grade level, subject, standard, prior-knowledge context, and student-population detail.
3. **Analyze.** Identify which elements of an AI-generated lesson plan require teacher revision before the plan is usable in your room.
4. **Evaluate.** Apply the lesson-planning phase gate: AI generates the structure; you retain the pedagogical content knowledge decisions.
5. **Create.** Adapt an AI-generated lesson plan for a specific real class using knowledge the AI does not have.

---

## 1. Opening case — the Sunday-afternoon desk

*This case is composite-illustrative. The teacher is not a single documented person. The workflow described matches the pattern the NFER/EEF (2024) trial found at the population level — about a third of lesson preparation time recovered for KS3 science teachers using ChatGPT plus a structured guide ([NFER/EEF 2024](https://d2tic4wvo1iusb.cloudfront.net/production/documents/projects/chatgpt_in_lesson_planning_-_evaluation_report.pdf?v=1736353004)) — but the specific 4-hour-to-45-minute arithmetic for an individual teacher is illustrative, not measured. [verify the individual-teacher arithmetic against any documented case study before publication.]*

It is 3:14 on a Sunday afternoon, late February. A tenth-grade biology teacher — call her Ms. Alvarez — has the cellular respiration unit open on her laptop. Twenty-eight students. Three newcomer ELLs at intermediate Spanish-L1 proficiency. Two IEPs — one ADHD with extended time, one specific learning disability in reading. The class has just finished a unit on thermodynamics and can balance equations, but most of them cannot label the organelles of a cell. Photosynthesis is next, in three weeks. The cellular respiration unit has to leave a clean ATP foundation or photosynthesis collapses.

A year ago, this is a four-hour Sunday. The blank document. The textbook. The state framework PDF. The slow build of objectives, activities, exit tickets, differentiated handouts. The pre-emptive worry about what will and won't land. Dinner cold by the time the unit is done.

Today, Ms. Alvarez opens Claude. She types a four-paragraph prompt: class profile, prior unit, learning targets (already written on a sticky note from Friday), a sketch of how she will assess understanding by next Thursday, the differentiation she needs, and a request for a five-day unit skeleton plus one detailed lesson for Monday. She hits enter. Fifteen minutes later, she has a draft. Reasonable structure. Three activity options per day. A first-pass exit ticket. An NGSS HS-LS1-7 label on the assessment that she has not yet verified.

Then she works for thirty minutes. She crosses out "powerhouse of the cell" and writes "phosphate transfer" in the margin — her class has the chemistry vocabulary, and the powerhouse metaphor will stop them asking *how*, which is the whole point of the unit. She swaps the order of days 2 and 3 because she remembers last year's class getting stuck for two days on glycolysis vs. Krebs cycle when the contrast came too late. She rewrites the ELL sentence frame around the word *oxidation* — the AI's frame was generic; hers references the redox unit they did in chemistry. She throws out the AI's exit ticket and pastes in last year's version, which surfaced the specific misconception she wants surfaced again. She opens NGSS HS-LS1-7 in another tab, reads the actual standard language, and confirms that the assessment she has planned actually produces the evidence the standard asks for.

Forty-five minutes. The dishes are still warm.

Three things are worth naming about that forty-five minutes. First, the AI did not "plan the lesson." It produced a structural draft for a target Ms. Alvarez had already specified. Second, the thirty minutes of revision are not waste — they are the work, and they are the part of the job that AI cannot do. Third, the dividend is not in the fifteen minutes of generation. The dividend is in the substitution of *judgment time* for *typing time*. Production becomes revision. The blank page becomes a draft to argue with.

This chapter is about that substitution: what AI can productively draft, what only you can supply, and where the gate sits between them.

---

## 2. The core concept — a task taxonomy for lesson planning

A lesson plan is not one task. It is many tasks the profession has chosen to bundle into a single document. AI does some of them well. AI does some of them badly. AI cannot do others at all. Here is how to sort them.

### 2.1 What AI does well — the structural layer

A current large language model — GPT-5, Claude, Gemini — can produce, in seconds, a lesson plan skeleton that is structurally correct. Specifically, it does well at:

- **Objectives** written in standard verb-list form ("Students will be able to explain... compare... analyze...").
- **Activity variety** — three ways to teach the same concept (lab, simulation, case study, jigsaw).
- **Time blocking and transitions** — a 50-minute lesson with reasonable pacing.
- **Resource suggestions** — videos, articles, simulations, lab procedures to consider.
- **Differentiation frameworks** — tiered tasks, sentence frames, vocabulary supports, in standard templates.
- **Exit ticket and check-for-understanding prompts** — generic but serviceable.
- **First-draft worksheets and handouts.**

The NFER/EEF trial confirms the time savings here. In a cluster-randomised RCT across 68 English secondary schools and 259 Key Stage 3 science teachers, treatment teachers using ChatGPT plus a structured guide spent 56.2 minutes per week on lesson and resource preparation, compared with 81.5 minutes per week in the control group — a 25.3-minute weekly saving, or 31% ([NFER/EEF 2024](https://d2tic4wvo1iusb.cloudfront.net/production/documents/projects/chatgpt_in_lesson_planning_-_evaluation_report.pdf?v=1736353004); [EEF news summary](https://educationendowmentfoundation.org.uk/news/teachers-using-chatgpt-alongside-a-guide-to-support-them-to-use-it-effectively-can-cut-lesson-planning-time-by-over-30-per-cent)). A blind expert panel of five science teachers scored thirty resources — fifteen treatment, fifteen control — on clarity, engagement, age-appropriateness, and scientific accuracy. They found no statistically significant difference on any dimension. The time went down. The quality, as the panel could measure it, held.

<!-- FACT-CHECK FLAG: UNVERIFIED — "35% with templates" sub-condition not located in NFER report; recommend removal. See factchecks/04-lesson-planning-with-ai-assertions.md -->
This is, to my reading, the cleanest single piece of evidence in the field. It is also bounded in ways the chapter must say plainly. [verify whether the TIKTOC-cited "35% with templates" condition exists as a sub-analysis in the NFER evaluation report Appendix; the headline I can confirm is 31% for the ChatGPT-plus-guide arm vs. comparison.]

### 2.2 What AI cannot do — the PCK layer

Lee Shulman, in his 1986 *Educational Researcher* article "Those Who Understand: Knowledge Growth in Teaching," named a category of professional knowledge that the field had been treating as either subject knowledge or general pedagogy: **pedagogical content knowledge**, PCK ([Shulman 1986](https://journals.sagepub.com/doi/10.3102/0013189X015002004)). His 1987 *Harvard Educational Review* paper, "Knowledge and Teaching: Foundations of the New Reform," developed the construct into a model of pedagogical reasoning ([Shulman 1987](https://www.harvardeducationalreview.org/content/57/1/1)).

Strip the jargon. PCK is the blend a teacher acquires by teaching a particular thing to particular students over time. It is the answer to four questions a textbook cannot answer:

1. **What do students predictably get wrong about this concept, in this grade, in this room?**
2. **Which analogy lands and which one backfires?**
3. **Which sub-topic has to come first for the next one to make sense, given what this class already knows?**
4. **What is the smallest example that exposes the deepest confusion?**

Here is the worked example I keep coming back to. A chemistry teacher knows that students will confuse *weight* and *mass* in a particular way every year. They will say a brick has more mass on Earth than on the Moon. They will say it confidently. They will get it wrong on the same item on the unit test no matter how many times the textbook defines the difference. The teacher knows this because the teacher has taught it. The teacher knows that the move which actually works is not the textbook definition — it is the bathroom scale on an elevator floor that accelerates downward, where the *weight* drops and the *mass* is obviously unchanged because nothing about the student has gotten smaller. A different teacher with a different class might need a different move. PCK is not the textbook. PCK is the knowledge of which textbook moves work on which students.

An LLM has read the textbook. It has read many textbooks. It can produce the textbook definition of weight versus mass in any of nine grade-band registers. It has never taught the unit. It has never watched a tenth-grader stick to *weight equals heaviness* through three weeks of correction. It has no PCK for your room.

This matters because lesson plans live and die at the PCK layer. The structurally correct plan is the plan that names objectives, sequences activities, aligns to standards, and proposes assessment. The pedagogically correct plan is the one that *anticipates the actual confusion in the room*. AI gives you the first. You supply the second.

A reasonable misreading of this paragraph would be: *AI is just not very useful for lesson planning, then*. That is wrong. The PCK gap is exactly why AI is useful — it does the structural work fast, which leaves you the time and the bandwidth to do the PCK work well. The phase gate is the boundary between the two.

### 2.3 The phase gate, stated

Here is the gate, in two sentences:

> **AI generates the structure. You confirm — for this class, this week — that every learning objective is achievable, every activity is contextually appropriate, every misconception is anticipated, and every standard alignment is real, before the plan touches a student.**

Two sentences. Read them again. That is the entire skill.

### 2.4 Backward design — why most AI prompts get this wrong

Grant Wiggins and Jay McTighe's *Understanding by Design* (ASCD, 2nd ed. 2005) makes a discipline of not-starting-with-activities ([Wiggins & McTighe 2005](https://andymatuschak.org/files/papers/Wiggins,%20McTighe%20-%202005%20-%20Understanding%20by%20design.pdf)). Their method has three stages, in order:

1. **Identify desired results.** What should students understand? Know? Be able to do?
2. **Determine acceptable evidence.** How will we know they got there? What does the assessment look like?
3. **Plan learning experiences and instruction.** Only now, given (1) and (2), choose activities and resources.

A default LLM prompt — "Write a 50-minute lesson on cellular respiration for 10th-grade biology" — collapses Stages 1 and 2 into an implicit guess and runs straight to Stage 3. The output is fine on its own terms. It is also Stage 3 work done before the targets were set. The teacher who accepts the output has not skipped lesson planning; the teacher has skipped backward design *by accident*.

The fix is mechanical. Before opening the prompt, write down — on paper, on a sticky note, in a notes app — two things:

- **Stage 1, one sentence:** What should students understand by the end of this unit / lesson?
- **Stage 2, one sentence:** What evidence would convince me they understand it?

Then the prompt is a Stage 3 brief: *Given these targets and this evidence, propose activities and resources*. The AI is now doing what it does well — proposing structure for targets you have already chosen.

This is the move most teachers skip on the first six months of AI use, then discover, then never go back from.

### 2.5 Unit scope vs. single lesson — where the dividend actually sits

Counter-intuitively, AI is more useful for unit-scale planning than for next-day lesson planning. The reason: unit-scale planning is largely structural — sequencing, mid-unit formative checks, cognitive-load staging. The model is reasonable at this. Next-day planning is heavily context-bound — what students did yesterday, what confused them, who is absent on Thursday, what energy the room had at the end of last period. The model knows none of this.

So the dividend is largest when you give AI the work it has the most context for, and smallest when you give AI the work it has the least context for. Many teachers do the opposite — they ask for tomorrow's lesson because tomorrow's lesson is what's burning. That is exactly the scope where the AI knows the least. The dividend is in Sunday's unit-design work, not in Monday-night triage. (I have to remind myself of this every Monday night.)

### 2.6 Standards alignment — cross-reference, not authority

A current LLM can name standards. It can write "NGSS HS-LS1-7" next to an assessment and produce the kind of confident citation that *looks* like alignment. The look is not the alignment. A 2025 preprint by Xincheng Liu evaluated AI-generated lesson plans across five models and three prompt frameworks in high-school physics (the Electromagnetic Spectrum), and found that prompt framework dominated curricular alignment accuracy — not model size ([arXiv 2510.19866](https://arxiv.org/abs/2510.19866)). This is a preprint, not yet peer-reviewed.

The rule: treat any AI standards citation as a **cross-reference to verify**, not as an **authority to accept**. Open the actual standard. Read the actual language. Confirm that the assessment in Stage 2 produces work that *demonstrates* the standard rather than merely *mentions* the topic. Standards alignment is one of the highest-stakes places where a model can be confidently wrong because the citation looks exactly like correct citation.

### 2.7 Differentiation as a prompt component, not an afterthought

If the prompt does not name your class, the model produces a plan for a generic class — which means a plan you have to differentiate from scratch. That is the work the AI dividend was supposed to remove. The fix is to put differentiation *into the prompt*, not into the revision pass. At minimum:

- ELL students and proficiency level
- IEP / 504 accommodations
- Reading-level distribution
- Prior-knowledge strengths and gaps
- Anything else that changes what counts as an accessible task

A prompt with this metadata produces tiered tasks and scaffolds that are at least plausible. A prompt without it produces a generic plan and a long Sunday. We will see this directly in the worked example.

---

## 3. The worked example — cellular respiration, prompt to plan to revision

Take the case from Section 1. Here is what the actual workflow looks like, with the prompt and the revision moves visible.

### 3.1 Stage 1 and Stage 2, on a sticky note

Before opening the prompt:

- **Stage 1.** Students will explain how cellular respiration converts the chemical energy in glucose into the chemical energy in ATP, including where in the cell each major stage happens and what each stage produces.
- **Stage 2.** A short written response in which a student traces one glucose molecule from cytoplasm through the mitochondrion, naming inputs and outputs at each stage, plus a labelled diagram. The exit ticket on day five asks the same thing in miniature.

This took ninety seconds with a pen. It is the most important ninety seconds of the workflow.

### 3.2 The prompt — the single-lesson generator

```
ROLE: You are an experienced 10th-grade biology teacher in the United States,
familiar with NGSS performance expectations and with the specific
challenges of teaching cellular respiration to chemistry-strong,
biology-weak students.

CONTEXT:
- Class: 10th grade biology, 28 students, 50-minute periods.
- Prior unit: thermodynamics (students can balance equations and
  reason about energy transfer).
- Prior knowledge gaps: most cannot label cell organelles; "ATP"
  and "energy" are used interchangeably.
- Student population: 3 newcomer ELLs (Spanish L1, intermediate
  proficiency), 2 IEPs (1 ADHD with extended time on assessments,
  1 specific learning disability in reading).
- Targeted standard: NGSS HS-LS1-7.
- Next unit: photosynthesis (the ATP foundation here must be clean).

TASK:
- Produce a 5-day unit skeleton (one paragraph per day: objective,
  activities, formative check).
- Then produce a fully detailed Day 1 lesson plan (50 minutes:
  opening hook, three activity blocks with timings, exit ticket,
  homework).
- Include differentiation explicitly for ELLs (sentence frames,
  visual supports) and for the IEP students (extended time,
  text-light alternatives where possible).

CONSTRAINTS:
- Do not use the "powerhouse of the cell" framing — students need
  to ask HOW, not be told WHAT.
- Use the chemistry vocabulary students already have (redox,
  electron transfer).
- Cite NGSS HS-LS1-7 explicitly in the assessment design but flag
  the alignment as draft pending teacher verification.
- Format the unit skeleton as a 5-row table; format Day 1 as a
  numbered list with timings in parentheses.
```

That is roughly four hundred words. It looks like a lot. It is half a Sunday morning's worth of typing, done once, and it is the difference between fifteen minutes of generation that produces a usable draft and fifteen minutes of generation that produces wallpaper.

### 3.3 What the AI produces

The model returns a 5-row unit table and a detailed Day 1 lesson plan. The structure is reasonable. The objectives use SWBAT-style verbs. The activity blocks are timed. The exit ticket asks students to label a diagram and write two sentences. The differentiation includes sentence frames for ELLs and a text-light alternative for the IEP-reading student. The plan cites NGSS HS-LS1-7 — flagged as draft, as instructed.

Read in isolation, the plan looks done. It is not done. It is a draft.

### 3.4 Three revisions only the teacher can make

These three are the kinds of moves that distinguish an AI plan a teacher accepts from an AI plan a teacher uses.

**Revision 1 — the misconception this class will actually carry.**
The plan's Day 1 hook is a video on the chemistry of glucose oxidation. Reasonable. But Ms. Alvarez knows from last year that this class will hit the same wall at the same moment: students will say "ATP is energy" and not be able to say what *energy* is. The AI does not know this. The revision: replace the video hook with a five-minute opening in which students try to explain, from the thermodynamics unit they just finished, what the word "energy" actually means in the equation `glucose + O2 -> CO2 + H2O + energy`. Surface the misconception on day one, before the rest of the unit calcifies on top of it. This is a PCK move. The AI could not have made it.

**Revision 2 — the order of days 2 and 3.**
The AI proposes cellular respiration overview on Day 2, photosynthesis-vs-respiration contrast on Day 3. Last year, Ms. Alvarez tried this order and lost two days to glycolysis vs. Krebs-cycle confusion. This year she puts the photosynthesis-vs-respiration contrast first: students compare the two equations as inverse processes, which gives them a framework into which glycolysis and Krebs then slot. The AI had no way to know this — it has not taught the unit. The revision is one minute of clicking. The decision behind it is two years of teaching.

**Revision 3 — the exit ticket.**
The AI's exit ticket asks students to label a diagram and write two sentences explaining what happens in each stage. Structurally fine. But Ms. Alvarez's exit ticket from last year asked students to draw the path of one glucose molecule from cytoplasm to mitochondrion and label every input and output. That version surfaced the specific misconception — that students think glucose enters the mitochondrion whole, rather than as pyruvate after glycolysis — that the unit is trying to dislodge. She replaces the AI's exit ticket with last year's. Two minutes. PCK pure and simple.

There is also a fourth revision that is not strictly PCK but is the chapter's other discipline: she opens NGSS HS-LS1-7 in another tab, reads the actual standard text ("Use a model to illustrate that cellular respiration is a chemical process whereby the bonds of food molecules and oxygen molecules are broken and the bonds in new compounds are formed resulting in a net transfer of energy" — and the related HS-LS1-5 on photosynthesis as the upcoming next unit), and confirms that the assessment in Stage 2 produces evidence the standard asks for. It does. If it had not, the assessment would be revised before the plan moved a step further.

### 3.5 The arithmetic

Fifteen minutes generating. Thirty minutes revising. Forty-five minutes total. The four-hour Sunday becomes a forty-five-minute Sunday because the substitution is from *typing time* (where the dividend lives) to *judgment time* (where the work lives). The 31% population figure from NFER/EEF and the individual arithmetic here are not the same kind of number — the trial measures group averages over ten weeks of KS3 science teachers in England, not a specific tenth-grade biology teacher's specific Sunday in February ([NFER/EEF 2024](https://d2tic4wvo1iusb.cloudfront.net/production/documents/projects/chatgpt_in_lesson_planning_-_evaluation_report.pdf?v=1736353004)). The individual case is illustrative of a pattern the trial supports at the population level. [The "8-hour baseline" cited in Chapter 1 needs a primary source — verify against the UK DfE workload survey or against Walton/Gallup self-report data before treating it as load-bearing.]

### 3.6 The lesson, and the limit

Here is the lesson, stated plainly. AI accelerates the production of structurally correct lesson plans. It does not, and cannot, supply the PCK that makes a plan land in your specific room. The 31% time saving in the NFER/EEF trial is real. The trial measured *teacher time* and *resource quality*. It did not measure *student learning outcomes*. We do not yet have rigorous evidence on whether students taught from AI-assisted lesson plans learn more, less, or the same as students taught from teacher-prepared plans. That is the central empirical question of this chapter, and the answer is *not yet established*. [This is a flag I will name again in the "still puzzling" section. It matters.]

The dividend exists. The dividend's pedagogical value is, at the level of evidence we currently have, an open question.

---

## 4. The three prompt templates

These three templates are the chapter's takeaway artifact. They build on the four-component prompt structure from Chapter 3 (role / context / task / constraints) and specialise it for lesson planning. Save them to your prompt library. Edit them in place. They are starting points, not commandments.

### 4.1 Template — single lesson generator

```
ROLE: You are an experienced [grade level] [subject] teacher in
[country/state], familiar with [standards framework] and with the
specific challenges of teaching [concept] to [population descriptor].

CONTEXT:
- Class: [grade], [subject], [N] students, [period length] periods.
- Prior unit: [what students just finished and what they can now do].
- Prior knowledge gaps: [what most students cannot yet do].
- Student population: [ELL count and proficiency; IEP/504 counts
  and accommodations; reading-level distribution].
- Targeted standard: [code and one-sentence content].
- Next unit: [what this lesson must set up].

TASK:
- Produce a [N]-minute lesson plan for [concept] with:
  - Opening (timed)
  - [2-3] activity blocks (timed)
  - Exit ticket
  - Homework or follow-up
- Include differentiation for [named subgroups].
- Format as a numbered list with timings in parentheses.

CONSTRAINTS:
- Do not use [framing(s) to avoid] — explain why if needed.
- Use the [prior-unit vocabulary] students already have.
- Cite the standard explicitly in the assessment, flagged as draft
  pending teacher verification.
- [Any other class-specific constraint.]
```

### 4.2 Template — unit scope-and-sequence generator

```
ROLE: You are an experienced [grade level] [subject] teacher
designing a [N]-day unit on [topic] for [population descriptor].

CONTEXT:
- Class: [grade], [subject], [N] students.
- Stage 1 (desired understanding, one sentence):
  [What students should understand by end of unit.]
- Stage 2 (acceptable evidence, one sentence):
  [What assessment will show they understand it.]
- Prior unit / prior knowledge:
  [What students bring in.]
- Differentiation needs:
  [ELL, IEP/504, reading-level, prior-knowledge specifics.]
- Standards: [codes].

TASK:
- Produce a [N]-day unit skeleton as a table with columns:
  Day | Objective | Activities | Formative check | Homework
- Identify the day(s) most likely to need PCK revision and flag.
- Identify the mid-unit formative checkpoint and what it should
  reveal.

CONSTRAINTS:
- Sequence sub-topics in an order learnable for this class.
- Do not assume prior knowledge of [topics not yet covered].
- Treat all standard alignments as draft pending teacher
  verification.
- Format as a markdown table.
```

### 4.3 Template — differentiation layer generator

```
ROLE: You are an experienced [grade level] [subject] teacher
adapting a lesson for differentiated learners.

CONTEXT:
- The existing lesson plan is below.
- Class population:
  - ELLs: [count, L1, proficiency level]
  - IEP/504: [accommodation details, anonymised]
  - Reading-level range: [Lexile band or grade equivalent]
  - Other relevant variation: [sensory, attention, prior-knowledge gaps]

TASK:
For the lesson plan below, produce:
- One sentence-frame set for ELLs around the lesson's key concept
- One scaffolded version of the main activity for students reading
  below grade level (preserve content; reduce reading load)
- One extension version of the main activity for students who finish
  early or need more challenge
- One adapted exit ticket variant for the IEP-reading student

CONSTRAINTS:
- Do not change the lesson's learning objective.
- Do not include any student name, ID, or identifying detail in
  your output.
- Flag any accommodation that requires specialist authorisation
  (IEP/504 modifications) rather than producing it as final.

[Paste lesson plan here.]
```

A note on the differentiation template: never paste student-identifying information into an external AI tool. The anonymisation discipline belongs to Chapter 6, but it applies here too. Describe the class profile abstractly; never name a specific student.

---

## 5. Common misconceptions

Four misreadings that show up in workshops and emails. Each fails in a slightly different way.

### 5.1 "AI replaces my lesson planning."

It doesn't. It produces Stage 3 of a backward-designed lesson — the activities and resources, given the targets and evidence. If you skip Stages 1 and 2, the AI does Stage 3 fluently for a target you didn't choose. The output is a lesson plan for a class that is not yours, taught to a target you did not set. The fluency makes this hard to notice. The phase gate exists to make you notice.

The deeper failure: lesson planning is not a production task. It is a judgment task that produces a document as a side effect. The document looking right is necessary but not sufficient. AI is excellent at making documents look right. Looking right is the trap.

### 5.2 "AI knows my standards."

It does not. It knows what standards look like — the codes, the formatting, the verb registers — and it can produce alignment claims that are syntactically correct. Whether the assessment in Stage 2 actually produces evidence the standard asks for is a separate question, and the model has no way to verify it.

Treat every AI standards citation as a cross-reference to verify by opening the actual standard text. The Liu 2025 preprint suggests prompt framework dominates alignment accuracy, not model size ([arXiv 2510.19866](https://arxiv.org/abs/2510.19866)) — but even strong prompt frameworks do not eliminate the need for the teacher to read the standard. The check takes ninety seconds. Skipping it is a Sunday-night habit; it is also the one place a confident-looking lesson plan can quietly miss its target.

### 5.3 "The plan is done when AI hands it back."

This is the fluency trap, in Trust the Teacher's vocabulary (see [TrustTeacher.md](../pantry/TrustTeacher.md)). Smooth output produces the feeling that the work has been done. The feeling is not the work. The AI plan is a draft. The plan is done when *you* have made the PCK revisions, verified the standards, and authorised the plan for *this* class.

The mechanical check is the question Ms. Alvarez ran on every section of her draft: *what does this plan assume about the room, and is that assumption true?* When the assumption is false — when the analogy will backfire, when the exit ticket misses the misconception, when the sequence is wrong for this class — revise. When the assumption is true, accept. The AI cannot ask itself this question because it does not know the room.

### 5.4 "I should generate a year of plans at once."

A reasonable instinct that produces unusable output. Two reasons.

First, a year of plans generated up front cannot reflect what you will learn about your class in the first three weeks. The Tuesday-of-week-eight lesson is going to depend on what surfaced in Tuesday-of-week-seven's exit ticket. PCK accumulates through the year; locking in a year of plans in August discards that accumulation.

Second, AI's dividend scales with the specificity of the prompt. A year-of-plans prompt is by definition generic — you don't yet know what specifics to put in. Generic prompt, generic output, more revision work downstream, not less.

The right unit of AI lesson planning is the unit, not the year. Generate a unit at a time, a week or two ahead, with class-specific context that has accumulated over the prior weeks.

---

## 6. Exercises

The exercises are graduated: a warm-up that gets your hands on the workflow, a synthesis exercise that documents what you learned, a creation exercise that builds the artifact you will use Monday morning.

### Exercise 1 — Generate, review, and document the PCK gaps

This is the chapter's core exercise.

1. Pick an upcoming unit you have to plan anyway.
2. Use the unit scope-and-sequence template (4.2) to generate a draft. Spend no more than fifteen minutes on the prompt and generation.
3. Read the draft against the four PCK questions from Section 2.2:
   - What will students predictably get wrong?
   - Which analogy lands and which will backfire?
   - What sub-topic order does this class need?
   - What is the smallest example that exposes the deepest confusion?
4. List every revision you make. Categorise each as: (a) PCK — knowledge of this class; (b) standards verification; (c) structural correction; (d) stylistic preference.
5. Calculate the ratio of PCK revisions to total revisions. That ratio is roughly the share of the work AI cannot do for you. The higher the ratio, the more the AI is buying you focus on the work that matters.

Expected output: a one-page document with the prompt, the draft, the revised plan, and the categorised revision list.

### Exercise 2 — Vague vs. specified prompt comparison

A diagnostic exercise. Take one upcoming lesson. Generate it twice.

- **Prompt A.** One sentence: "Write a [N]-minute [grade] [subject] lesson on [concept]."
- **Prompt B.** The full single-lesson template (4.1), filled in for your actual class.

Compare the two outputs side by side. Document:

- Which output required less revision to make usable?
- What did Prompt B's class-specific context get you that Prompt A could not?
- Which prompt produced a plan you would actually teach from?

The point of this exercise is not to prove that specified prompts work — they do — but to feel, in your own room, how much of the AI dividend is a function of what you put into the prompt rather than what the model knows.

### Exercise 3 — Create your unit-scope prompt template

A creation exercise. By the end of this exercise you should have one reusable artifact saved to your prompt library.

1. Take the unit scope-and-sequence template (4.2).
2. Customise it for *your* subject, *your* grade, *your* state's standards framework, and *your* typical class profile. Fill in the recurring elements so the template is ready to use with minimum editing each unit.
3. Add a "PCK notes" section at the bottom — three bullet points naming the misconceptions, analogies-to-avoid, and prior-knowledge gaps you know this class carries year after year. These are PCK notes you can paste into any unit prompt for this class.
4. Save the customised template, with the PCK notes, to a single document you can reopen for every unit you plan this year.

Expected output: one reusable template, saved and named, ready to use on the next unit. This is the first entry in your prompt library (Chapter 12).

---

## 7. What would change my mind

The argument in this chapter — that AI generates structure, the teacher supplies PCK, and the phase gate is where the two meet — would revise if a rigorous randomised trial with student learning outcomes as the primary endpoint showed that students taught from AI-generated lesson plans, *without* substantive teacher PCK revision, learn at least as much as students taught from teacher-revised plans, across diverse populations and subjects. That trial does not yet exist. If it appears — with pre-registered outcomes, blinded scoring of student learning, and stratification by ELL, IEP, and prior-knowledge subgroups — the chapter's central claim about the necessity of the PCK revision step would need to be revised, possibly significantly.

A weaker but still consequential update: a long-running observational study showing that teachers using AI lesson planning at steady state for a full academic year, across multiple subjects and grade bands, produce student outcomes statistically indistinguishable from a matched non-AI cohort. That would soften the time-vs-learning ambiguity even without a randomised intervention on student outcomes directly.

---

## 8. Still puzzling

A few questions I cannot yet answer.

**Time saved vs. learning gained.** The NFER/EEF trial measured time and resource quality. It did not measure student learning ([NFER/EEF 2024](https://d2tic4wvo1iusb.cloudfront.net/production/documents/projects/chatgpt_in_lesson_planning_-_evaluation_report.pdf?v=1736353004)). The Walton/Gallup self-reports ([Gallup 2025](https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx)) measure teacher-reported hours. Neither tells us whether students taught from AI-assisted plans learn more, less, or the same. This is the central empirical question of this chapter, and it is unanswered. The whole chapter's pedagogical argument rests on a finding (PCK matters) that has been measured for decades, applied to a workflow (AI lesson planning) for which the learning-outcome evidence has not yet been collected. That is not a comfortable place to write a chapter from. It is the honest place.

**Equity of access.** RAND finds that higher-poverty schools use AI *less* than lower-poverty schools, and that principals in those schools provide AI guidance less often ([RAND 2025, RR-A134-25](https://www.rand.org/pubs/research_reports/RRA134-25.html); [RAND 2025, RR-A4180-1](https://www.rand.org/pubs/research_reports/RRA4180-1.html)). The pattern is the opposite of what one might hope: the schools whose teachers stand to gain the most from a competent structural-draft tool are the schools where the tool is least available and least supported. If the PCK revision step is the part that turns a structural draft into a usable plan, and the front-end access to the draft itself is uneven, the technology that should be most useful for closing gaps could quietly widen them. I do not yet know what this gap produces at the student-outcome level. I want to know.

**Daily steady-state vs. ten-week summer term.** The NFER trial ran ten weeks in summer. Steady-state daily use across a full academic year — with novelty worn off, with prompts decaying, with the model versions changing under you — is not what the trial measured. The 31% might hold. It might drift up. It might drift down. I would like to see a longitudinal replication.

**Cross-model variance.** A current preprint suggests that prompt framework dominates alignment accuracy, not model ([Liu 2025, arXiv 2510.19866](https://arxiv.org/abs/2510.19866)). That is consistent with the chapter's argument that the prompt is the primary lever. But I have not seen an independent, like-for-like comparison of GPT-5, Claude, and Gemini on lesson plans for the same class profile and the same standards, scored on PCK-relevant dimensions. The vendor-internal numbers do not substitute for it.

---

## Bridge to Chapter 5

Lesson planning is preparation. What students *produce* in response to the lesson — essays, short answers, problem sets, exit tickets — is the next time sink, and the place where the phase gate sits at a much sharper angle. Chapter 5 takes the same framework into assessment and feedback, where the time savings are larger, the failure modes are louder, and the question of who is doing the cognitive work cuts both at the teacher's grading desk and at the student's writing desk.

---

**Tags:** lesson-planning, pedagogical-content-knowledge, NFER-EEF-RCT, backward-design, Shulman, prompt-templates, phase-gate, AI-in-education

*Voice anchor: workshop default (Feynman). Composite-illustrative opening case clearly labelled. NFER/EEF figures bounded to trial conditions. Student-outcome gap flagged repeatedly. [verify] markers retained inline where primary-source confirmation is pending.*

---

## References

- NFER (2024). *ChatGPT in Lesson Preparation: A Teacher Choices Trial — Evaluation Report.* National Foundation for Educational Research and Education Endowment Foundation. https://d2tic4wvo1iusb.cloudfront.net/production/documents/projects/chatgpt_in_lesson_planning_-_evaluation_report.pdf?v=1736353004
- EEF (2024). *Teachers using ChatGPT — alongside a guide to support them to use it effectively — can cut lesson planning time by over 30 per cent* (news summary). Education Endowment Foundation. https://educationendowmentfoundation.org.uk/news/teachers-using-chatgpt-alongside-a-guide-to-support-them-to-use-it-effectively-can-cut-lesson-planning-time-by-over-30-per-cent
- Shulman, L. S. (1986). Those Who Understand: Knowledge Growth in Teaching. *Educational Researcher*, 15(2), 4–14. https://journals.sagepub.com/doi/10.3102/0013189X015002004
- Shulman, L. S. (1987). Knowledge and Teaching: Foundations of the New Reform. *Harvard Educational Review*, 57(1), 1–22.
- Wiggins, G., & McTighe, J. (2005). *Understanding by Design* (2nd ed.). Alexandria, VA: ASCD. https://www.ascd.org/books/understanding-by-design-expanded-2nd-edition?variant=103055
- Liu, X. (2025). *An Evaluation of the Pedagogical Soundness and Usability of AI-Generated Lesson Plans Across Different Models and Prompt Frameworks in High-School Physics.* arXiv:2510.19866. https://arxiv.org/abs/2510.19866
- Walton Family Foundation / Gallup (2025). *Teaching for Tomorrow: Unlocking Six Weeks a Year With AI.* https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx
- RAND Corporation (2025). *Uneven Adoption of Artificial Intelligence Tools Among U.S. Teachers and Principals in the 2023–2024 School Year* (RR-A134-25). https://www.rand.org/pubs/research_reports/RRA134-25.html
- RAND Corporation (2025). *AI Use in Schools Is Quickly Increasing but Guidance Lags Behind* (RR-A4180-1). https://www.rand.org/pubs/research_reports/RRA4180-1.html
- NGSS Lead States (2013). *Next Generation Science Standards*, HS-LS1-7 (cellular respiration) and HS-LS1-5 (photosynthesis). https://www.nextgenscience.org/pe/hs-ls1-7-molecules-organisms-structures-and-processes
