# Chapter 3 — Prompting That Works: The Foundation Skill

**TL;DR.** A prompt is not a search query. It is a specification — role, context, task, constraints — and the teachers who get usable output from AI write specifications, iterate on the gaps, and save the prompts that worked.

---

## 3.1 Learning objectives

By the end of this chapter you will be able to:

1. **Describe** why prompt quality determines output quality — the model has no context the prompt does not supply.
2. **Write** a basic prompt using the four-component structure: role, context, task, constraints.
3. **Add** grade level, subject, standard alignment, and student population detail to a prompt and compare output quality.
4. **Use** iterative prompting: evaluate the first output, identify the specific gap, write a follow-up that closes it.
5. **Distinguish** a feeling-prompt ("make this more engaging") from a specification.
6. **Create** prompts for three recurring tasks from your own workweek.

Prerequisite reading: Chapter 1 (which tasks are AI-suitable in the first place) and Chapter 2 (where the human handoff sits, so you know what the prompt is producing *for*).

---

## 3.2 Opening case — same tool, same minute, two outputs

It is a Sunday in late October. Two 8th-grade U.S. History teachers in the same building are writing a formative quiz on the causes of the American Revolution. Same standard. Same textbook chapter. Same week of school. Both open the same chatbot. Both type.

Teacher A types:

> Generate quiz questions about the American Revolution.

Five questions come back. Three are date-recall ("In what year did the Boston Tea Party occur?"). One is a multiple-choice item with the correct answer obviously longer than the distractors. The reading level lands somewhere around 11th grade. None of the items target the misconception this teacher knows her class carries — that "no taxation without representation" meant Americans paid higher taxes than Britons (they did not; they paid lower, but had no parliamentary voice). The questions are technically correct. They are not usable for this class on Monday. Teacher A rewrites them by hand. Forty minutes.

Teacher B types a longer prompt. Six sentences. It names the standard (C3 D2.His.14.6-8). It names the grade. It names which causes the unit has covered and which it has not yet. It asks for eight multiple-choice items with one item per cause, four answer choices per item, and one distractor per item that targets a documented 8th-grade misconception. It bans date-recall items and the phrase "the colonists were angry." It specifies 6th-grade reading level because three of the students read below grade level.

The output comes back. Eight items. One per cause. The distractors are sharp — one is the exact "Americans paid more tax" misconception the class is going to carry into the quiz. Teacher B edits two stems, swaps one distractor, and saves the prompt to a file called `quizzes/causes-of-revolution.md`. Twelve minutes start to finish. Next quarter, when she teaches the same unit, she will change one line — the standard reference — and run it again.

Same tool. Same minute. One teacher got generic trivia. The other got a usable draft she can reuse for years. The chatbot did not change. The prompt did.

That difference is what this chapter teaches.

---

## 3.3 The core idea — prompting is task decomposition

A search engine takes keywords and looks up documents. A generative language model does something different. It samples the next word from a probability distribution that depends on every word preceding it. The prompt *is* the conditioning. The more your prompt narrows the probability space, the more the output collapses toward the slice you actually want. The less it narrows, the more the output drifts toward the average of what its training data contains for those keywords — which, for "quiz questions on the American Revolution," is a generic mix of trivia at an unspecified grade level in an unspecified format ([Liu et al., 2023](https://arxiv.org/abs/2107.13586)).

A useful way to hold this: **a vague prompt is a request for the average.** An average is rarely useful for a specific class.

The reason this matters is structural, not magical. The model does not know your school. It does not know the standard. It does not know that three of your students are ELLs at WIDA level 2, that the unit started two weeks ago, that last year's class tripped over taxation-without-representation, or that the assistant principal wants quizzes formatted as Markdown lists. **The model has no context the prompt does not supply.** Everything that is not in the prompt is filled in by the model's average guess. Average guesses produce average output.

### 3.3.1 The four-component structure

There is a structure that forces you to supply what an ad-hoc prompt forgets. Different people call it different things — CO-STAR, PAST, PLFR, role-task-format — but the structure underneath is the same. <!-- FACT-CHECK FLAG: UNVERIFIED — CO-STAR (GovTech Singapore) and role-task-format are attested; PAST and PLFR are not well-attested as canonical prompt frameworks. See factchecks/03-prompting-that-works-assertions.md (F2). --> This book uses four components because four is enough:

```
ROLE: You are [specific role relevant to this task].
CONTEXT: [Grade level, subject, standard, class profile, constraints].
TASK: [Specific deliverable with format, length, and quality criteria].
CONSTRAINTS: [What to avoid, what format to use, what the output will be used for].
```

Each line does distinct work.

**Role** tells the model which slice of its training corpus to draw from. "You are a veteran 8th-grade U.S. History teacher" pulls the vocabulary, pacing, and pedagogical instincts the corpus associates with that role. The evidence on role-prompting is mixed and we will be honest about it in §3.6 — but for tasks where register and style matter (most teacher tasks), it does work.

**Context** is the part teachers under-supply most. Grade. Subject. Standard. Class profile. What the class has already covered. What it has not. Without this, the model defaults to a generic high-school-adult reading level and a generic topic treatment. Context is what makes the output land in *your* classroom rather than in a hypothetical average classroom.

**Task** is the deliverable. Format, length, quality criteria. "Make quiz questions" is a task in the same way "make food" is a task at a restaurant. The model can comply with both, and you will not like either result. "Write eight multiple-choice questions, each with four answer choices and a one-sentence rationale for the correct answer and each distractor, output as a numbered Markdown list" is a task.

**Constraints** is what to avoid and what the output will be used for. Anthropic's own guidance recommends positive instructions over negative ones — telling Claude what *to* do is more reliable than telling it what *not* to do ([Anthropic prompting best practices](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices)). But negative constraints earn their place when paired with a positive direction and used sparingly: "Do not include date-recall items; this is for a formative quiz, not a unit exam." The pattern that works is *positive direction + a few sharp negatives + stated downstream use*. Long lists of "do not" rules degrade output more than they sharpen it (see §3.3.4).

The template is scaffolding. After thirty or forty prompts, the structure becomes reflex and disappears the way grammar disappears for a fluent speaker. But the moves underneath — name the role, supply the context, specify the task, set the constraints — those do not disappear. They become how you think about handing work to a model.

### 3.3.2 Specification beats feeling

Here is the most common way teacher prompts fail.

A teacher asks AI to draft a parent email. The draft sounds clinical. The teacher prompts back: *make it warmer and more personal*. The next version arrives with three exclamation points, a smiley face, and the phrase "we're all in this together!" That is the model's stereotype of "warm" — the average of what "warm" looks like in its training data. It is not warm. It is performative warmth. The teacher has asked for a feeling, and the model has produced the average impression of that feeling.

Now watch the specification version. Same teacher. Same email. The follow-up:

> Rewrite the email so the second sentence references one specific strength the student showed last week (her participation in the Tuesday group discussion on volcanoes). Replace "is struggling" with "is finding [specific skill] challenging." End with one specific concrete invitation: "Could we meet this Friday at 3:15 to look at the recent quiz together?" Remove any sentence that begins with "I just wanted to."

The specification version sounds personal because it *is* personal. The feeling version sounds like generic warmth because that is what the model produces when asked for a feeling without a specification.

The trap is that feeling-prompts feel natural. They are how humans talk to humans, who can interpret intent. Models do not interpret intent. They pattern-match. Asking for a feeling produces a stereotype of that feeling. Asking for a *move* — the specific operation that would produce the feeling — produces the move.

Cut on sight, in your own prompts: *make it engaging*, *make it pop*, *make it sound more like a teacher*, *make it rigorous*, *tighten it up*, *make it better*. Replace each with the operation underneath. *Engaging* might mean "open each section with a one-sentence concrete scene." *Rigorous* might mean "every claim links to a primary source." *Tighten* might mean "cut any sentence longer than 25 words to two shorter sentences." Those are operations the model can execute and you can verify.

### 3.3.3 Iterative prompting — the first output is a draft

Both Anthropic and OpenAI describe prompt engineering the same way: start with a prompt, look at the output, refine ([Anthropic](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview); [OpenAI](https://platform.openai.com/docs/guides/prompt-engineering)). The skill is not writing the perfect first prompt. The skill is the loop. Evaluate the output, identify the specific gap, write the follow-up that closes it.

The first output's job is to reveal what you forgot to specify. If the questions are too easy, "increase difficulty" is the wrong follow-up — it is a feeling. The specification follow-up names what to keep and what to change: *Rewrite items 3, 5, and 7 so the distractors target the taxation-without-representation misconception rather than date-recall errors. Keep items 1, 2, 4, 6, and 8.* That is bounded. The teacher does not have to re-read the whole quiz after the model responds. She only has to re-read items 3, 5, and 7.

Two prompts in a session is normal. Four is normal. Eight is a sign the prompt structure was wrong from the start and the teacher is debugging at the wrong level — better to rewrite the whole prompt than to keep patching it.

### 3.3.4 Negative prompting — telling the model what *not* to do

"Avoid emoji." "Do not include trivia about dates or numerical recall." "Do not use the phrase 'students will learn.'" These are negative constraints. They are first-class moves, not afterthoughts. What you tell a model *not* to do sharpens the output as much as what you tell it to do.

Two cautions. First: a negative constraint works best when paired with a positive direction. "Do not use emoji" leaves the model uncertain about how to fill the space; "Do not use emoji; use a short declarative sentence instead" gives it somewhere to go. Second: long lists of negative constraints degrade attention. A model that reliably honors three "do not" instructions may drop the fourteenth. Three or four well-chosen negatives beat fifteen.

### 3.3.5 Platform differences as task fit, not vendor ranking

This section is the most dangerous section in the chapter, because anything specific about a specific model is going to be wrong within a year. So we will frame it in terms of *task fit*, which has been stable across the 2024–2026 model generation, rather than in terms of which company is winning this month.

- **Long-document synthesis** — you upload three PDFs of curriculum materials and want a unit plan grounded in those documents. **NotebookLM** is built for this. It grounds answers in the uploaded sources and cites passages. The trade-off: it is conservative — it will refuse to extrapolate beyond what you uploaded. For synthesis that needs to bring in outside knowledge, a general chatbot does more.
- **Long-form drafting and writing-task feedback** — you want a 600-word lesson plan or a feedback paragraph on student writing. **Claude** tends to produce longer, more structurally coherent first drafts and follows complex multi-part instructions reliably. Anthropic's documentation leans heavily on prompt structure ([Anthropic best practices](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices)).
- **Conversational ideation and quick iteration** — you are brainstorming, refining as you go, talking it through. **ChatGPT**'s conversational tuning makes turn-by-turn refinement feel fluid.
- **Integration with Google Workspace artifacts** — you live in Google Slides, Docs, Classroom, and Forms. **Gemini** is inside those tools. Gemini in Classroom is free to Workspace-for-Education educators ([Google blog, 2024](https://blog.google/products-and-platforms/products/education/classroom-ai-features/)).

The point is not to rank vendors. The point is: **the four-component prompt works on all of them.** Vendor differences are real but secondary to specification discipline. Switching to a different AI rarely fixes bad output. Switching your prompt does.

### 3.3.6 Prompt libraries — saving what worked

The prompt that produced a usable quiz today will produce a usable quiz next quarter for the next unit. The teacher who writes prompts ad hoc pays the specification cost every time. The teacher who saves prompts pays it once and amortizes it across every reuse. This is the single highest-leverage move in this chapter.

A starter library is small. Five to fifteen prompts per recurring task category. A folder structure that is searchable. Each prompt has the four components filled in with the teacher's recurring context — grade, subject, standards, class profile — and the parts that change per use (the specific text, the specific unit, the specific student situation) marked as slots to fill. Chapter 12 builds this systematically; for now, the rule is: **if a prompt worked, save it.** You will not remember what you did differently three weeks from now. Save the prompt.

---

## 3.4 Worked example — one task, three prompts

Let us run the loop end to end on a single concrete task. A 5th-grade teacher wants a lesson plan on photosynthesis aligned to NGSS 5-LS1-1, the standard that requires students to support an argument that plants get the materials they need for growth chiefly from air and water (not, as the most common 5th-grade misconception holds, from the soil).

### Round 1 — the vague prompt and what it returns

**Prompt:**

> Write a lesson plan on photosynthesis for 5th grade.

**What comes back** (paraphrased — the exact wording varies by model and by run):

> **Photosynthesis Lesson Plan (Grade 5)** — Objective: students will learn about photosynthesis. Materials: paper, pencils, optional plant. Procedure: (1) Introduce the concept of photosynthesis. (2) Show a diagram. (3) Have students label the parts. (4) Discuss. Assessment: students will demonstrate understanding.

This is a draft of the *shape* of a lesson plan, not a usable plan. There is no standard alignment. There is no formative check. There is no differentiation. The objective is "students will learn about photosynthesis," which is not an objective — it is a topic. The materials list says "optional plant." The procedure does not address the misconception the standard exists to correct.

This is what a vague prompt produces. Not bad. Not usable. Generic.

### Round 2 — add role, context, task, constraints

**Prompt:**

> ROLE: You are a veteran 5th-grade science teacher writing a 60-minute lesson plan.
>
> CONTEXT: 5th grade, class of 26 students, including three ELLs at WIDA level 2 and two students reading two grade levels above. Standard: NGSS 5-LS1-1 (support an argument that plants get the materials they need for growth chiefly from air and water). The class has covered: parts of a plant, the water cycle. The class has NOT yet covered: cellular respiration, the carbon cycle. The most common student misconception we need to address is that plants get their food from the soil.
>
> TASK: Write a 60-minute lesson plan with: (1) one student-facing objective written in "students will be able to" form, (2) a 5-minute hook that surfaces the soil misconception, (3) a 15-minute direct-instruction segment, (4) a 25-minute lab using only paper plates, plastic cups, soil, bean seeds, and a lamp, (5) a 10-minute discussion, (6) a 5-minute exit ticket with two formative-check questions. Output as Markdown with headers for each segment.
>
> CONSTRAINTS: Reading level for any student-facing text: 5th grade. Do not use the word "produce" — students at this grade often parse it as "fruit." Do not include any segment that requires materials beyond those listed. Output is for tomorrow's class, so the lab must work with what is already in the room.

**What comes back:** the plan now has a real objective ("students will be able to argue, with evidence from a controlled investigation, that bean plants gain mass primarily from air and water rather than from soil"). The hook is a one-minute scenario where students predict whether a sealed bean seedling kept in light will gain or lose soil mass over a week. The lab uses paper plates and cups. The exit ticket asks students to weigh a hypothesis claim against two pieces of evidence. The differentiation section names one accommodation for ELLs (a labeled diagram for the lab) and one extension for above-level readers (a primary source from Joseph Priestley's 1771 experiment on mice and plants).

This is now a draft a teacher could edit in ten minutes and teach tomorrow.

### Round 3 — close the specific gap

The teacher reads it. One problem. The lab as written requires a week of observation before students can support an argument, but tomorrow's class is the only class on this topic before next Monday. She does not need a week-long investigation. She needs the *argument move* to happen tomorrow on data she can produce in the classroom.

**Prompt:**

> Revise the lab so it produces observable evidence within the 25-minute class segment, not over a week. The argument students make at the end of class should be supported by evidence they collect in that 25 minutes. Keep the rest of the plan.

**What comes back:** a revised lab in which students mass a sealed bag containing a sprouting bean and damp paper towel before and after a 20-minute exposure to a lamp, observing the rise in water vapor inside the bag. The mass change is too small to measure with classroom scales, so the lab instead has students observe and measure the condensation on the inside of the bag and discuss what it implies about where the mass of a growing plant must come from. The rest of the plan is unchanged.

Now it is a tomorrow-class lesson plan. Three prompts. Maybe seven minutes of typing. The teacher edits two sentences, swaps one vocabulary term, and saves the whole exchange to `lessons/05-photosynthesis-misconception.md` with a top comment: *next year, do the week-long version if the unit calendar allows.*

### What the worked example teaches — and what it does not

The teaches: each round of the loop narrowed the output. The first prompt was a request for the average. The second prompt was a specification. The third prompt named a specific gap (the time horizon of the lab) and asked the model to close that one gap without disturbing the rest.

The does not: **specification cannot substitute for domain knowledge you do not have.** A teacher who does not know that "plants get their food from soil" is the common 5th-grade misconception cannot ask the model to address that misconception. A teacher who does not know that "produce" is ambiguous for 5th-graders cannot constrain the model away from it. The four-component prompt is a tool for getting the model to deploy *your* knowledge of your classroom. It is not a substitute for having that knowledge. If you are teaching outside your subject area, the missing knowledge is the missing knowledge — the prompt cannot supply it.

This is the same limit the rest of the book will name in different ways. AI extends teacher judgment. It does not replace it. The prompt is where that distinction lives in practice.

---

## 3.5 Common misconceptions

### "Prompting is like Googling."

It is not. Google takes keywords and retrieves documents that already exist. A generative model takes the entire prompt as conditioning and produces output that does not exist until you ask for it. Keywords are sparse input. Sparse input produces output that is the *average* of what those keywords mean in the model's training data. A vague keyword search returns 50,000 documents and you pick. A vague prompt returns one document — and the picking already happened, badly, before you saw it. Specification is how you do the picking on the way in.

### "Magic phrases work universally."

You will hear that adding "think step by step" or "take a deep breath" to a prompt unlocks better answers. There is real evidence behind some of this — chain-of-thought prompting genuinely improves multi-step reasoning on sufficiently large models ([Wei et al., 2022](https://arxiv.org/abs/2201.11903)). But the gains vary wildly by model, by task, by benchmark, and by release. A phrase that helped on a 2023 model may have no effect or a negative effect on a 2026 model. Treat magic phrases as worth trying when you are stuck, not as rules. The four-component structure is durable across model generations because it is about specification, which models will always need. Specific phrases come and go.

### "Longer prompt = better."

Up to a point. Then no. Adding context that does work — the grade, the standard, the misconception, the constraints — improves output. Adding fifteen "do not" instructions makes models drop some of them. Adding three paragraphs of background a model does not need increases the noise the model has to filter. A 300-word prompt that supplies the right context outperforms a 1,500-word prompt that pads it. The discipline is *which* details to add, not how many.

### "The same prompt should work across models."

The structure does. The exact wording often does not. A prompt that produced an excellent output on Claude in March may produce a different output on a successor model in November, or on a different vendor's model on the same day. This is one reason to save prompts and to revisit your library annually. Treat prompt libraries as living documents, not as one-and-done assets. The structure (role-context-task-constraints) is the part you carry forward; the wording is the part you re-tune.

---

## 3.6 Where the evidence is contested

Two places in the chapter so far would have been easier to write as rules. They are not rules. They are worth-trying moves that the evidence is mixed on, and a textbook that pretended otherwise would age badly.

**Persona prompting.** Telling the model "You are a veteran 8th-grade U.S. History teacher" feels like it should help and often does — on tasks where the output's *register* and *style* matter (most teacher tasks). But on factual benchmarks, the evidence is mixed. Zheng et al. (2023) ran a careful study across four LLM families and found that adding personas in the system prompt produced no improvement or small negative effects on objective-knowledge benchmarks ([Zheng et al., 2023, arXiv 2311.10054](https://arxiv.org/abs/2311.10054)). The synthesis that holds up: role-prompting helps when the task pulls on a coherent corpus region the persona names (vocabulary, register, pedagogical pacing), and helps less or hurts when the task is asking for a calibrated factual answer the model should already know without role-priming. For teachers: role works in lesson planning and writing feedback. It does less work in fact-checking.

**"Magic phrases."** Same posture. Some phrases really do help some models on some tasks. None of them help every model on every task. Try them when stuck. Do not build a workflow around them.

The chapter is honest about this because **the empirical research on teacher-specific prompting is thin.** The closest systematic reviews are Chen et al. (2024) on K-12 STEM ([arXiv 2410.11123](https://arxiv.org/abs/2410.11123)) and Qian (2025) on education broadly ([SAGE](https://journals.sagepub.com/doi/10.1177/07356331251365189)), and both note that the field is young. Most claims you will read about teacher prompting effectiveness — including some of the ones in this chapter — rest on practitioner reports and vendor documentation, not on randomized trials with teacher participants. This is a place to hold beliefs loosely and to update them when better evidence arrives.

---

## 3.7 Exercises

### Exercise 1 — Prompt workshop (the chapter's keystone)

Choose one high-frequency task from your recent week: the next quiz, the next parent email, the next reading-level rewrite, the next lesson plan. Then do the following, in order, in writing.

1. Write a one-line vague prompt of the kind you might type without thinking. Run it. Save the output as `output-A.md`.
2. Rewrite the prompt using the four-component structure. Role. Context (grade, subject, standard, class profile). Task (format, length, criteria). Constraints (what to avoid, downstream use). Run it. Save the output as `output-B.md`.
3. Read `output-B.md` carefully. Identify *one specific gap*. Not a feeling — a gap. ("The distractors are wrong" is a gap. "The tone is off" is a feeling. Convert feelings to gaps.) Write the follow-up prompt that names what to change and what to keep. Run it. Save the output as `output-C.md`.
4. Save the final prompt — the version from step 3 — as the first entry in your personal prompt library. Give it a filename that you will be able to find in three months.

The output of this exercise is one prompt and three outputs. The point is to feel the difference between step 1 and step 3 in your own work. If you do not feel a difference, the prompt at step 2 was not specific enough — go back.

### Exercise 2 — Rewrite drill (vague to specific)

Below are three feeling-prompts. Rewrite each as a specification. Name the operation the model can execute, not the feeling you want it to evoke.

1. *Make this lesson plan more engaging.*
2. *Tighten up this parent email.*
3. *Make this rubric more rigorous.*

There is no single right answer. There is a wrong one — leaving the prompt as a feeling.

### Exercise 3 — Build a three-prompt starter library

Build three reusable prompt templates for three recurring tasks you do every week or every unit. Examples: quiz generator, differentiated rewrite at three reading levels, parent-email draft from bullet notes. Each template should have the four components filled in with the parts of your context that *do not change* (grade, subject, standards you teach, class profile in general terms), and the parts that *do change* (the specific text, the specific topic, the specific student situation) marked as slots — for example, `[INSERT PASSAGE HERE]` or `[INSERT STUDENT-SPECIFIC NOTE HERE]`.

Test each template on a real task this week. If it produces a usable draft with light editing, the template earned its place. If it took more editing than writing from scratch, revise the template and try again next week. The library is built one test at a time.

---

## 3.8 What would change my mind

This chapter argues that structured, specification-heavy prompts outperform unstructured conversational prompts for teacher tasks. The chapter would revise if a randomized trial — teachers using a four-component template versus teachers writing freeform prompts — measured time-to-usable-output, output quality (independently rated against rubrics), and time-saved-over-month, and found that the freeform group performed comparably or better at scale. As of this writing no such trial exists; the closest evidence is vendor documentation, practitioner reports, and adjacent research on prompt-engineering effects in non-teacher contexts. The chapter's confidence in the four-component structure rests on that adjacent evidence plus the structural argument that specification is the only way to give a model context it does not have. If a trial showed the structure did not matter — that conversational refinement converged to the same quality with comparable total time — the chapter would need to be rewritten around the iteration loop alone, dropping the template as the recommended starting point.

---

## 3.9 Still puzzling

A few things this chapter does not yet answer.

- **What is the right teacher prompt-library size?** Five prompts feels under-built. Fifty feels unmaintainable. The right answer is probably "as many as the recurring tasks require, no more," but I do not know what that number is empirically for a full-time teacher.
- **How fast do good prompts go stale across model releases?** The structure transfers. The wording sometimes does not. I do not know the typical half-life for a teacher prompt — whether it is six months, two years, or longer — and I have not found published data on this.
- **Does prompting *for student-facing material* preserve or bypass the friction traces the rest of this book argues are the mechanism of learning?** A differentiated reading written by AI lands in front of a student who reads it. The student's processing of that text is where the friction lives, not the production of it. But the further upstream prompting moves — generating practice problems, drafting Socratic questions — start to interact with the student's cognitive work in ways the literature has not measured. Chapters 13 and 14 will press on this.
- **Are there teacher tasks where the four-component template actively hurts?** I suspect yes — brainstorming and ideation may benefit from conversational openness. But I have not seen the comparison run.

---

## 3.10 Bridge to Chapter 4

Part I ends here. You have the dividend (Chapter 1), the phase gate (Chapter 2), and the foundation skill (this chapter). Part II is where the framework meets specific tasks — the six categories of work that consume most of a teacher's week.

Chapter 4 takes the foundation skill and applies it to the highest-frequency teacher use: lesson planning. Same four-component structure. New context: lesson-plan-specific role, grade-band-specific scope, the pedagogical content knowledge problem (the model has encyclopedic content knowledge and zero knowledge of *this* classroom), and the phase gate that protects the teacher's professional judgment over what to actually teach Monday morning. The prompt is the substrate. Chapter 4 builds the first thing on top of it.

---

**Tags:** prompting, foundation-skill, role-context-task-constraints, iterative-prompting, prompt-library, specification, teacher-AI

*What would change my mind:* an RCT comparing structured-template prompting to unstructured conversational prompting on teacher tasks, finding no meaningful difference in output quality or time-to-usable-output at scale.

*Still puzzling:* the half-life of a good teacher prompt across model releases, and whether prompting for student-facing material interacts with the friction traces the rest of the book argues are the mechanism of learning.

---

## References

- Anthropic. *Prompt engineering overview.* Claude API Docs. https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview
- Anthropic. *Prompting best practices.* Claude API Docs. https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices
- Chen, E., Wang, D., Xu, L., Cao, C., Fang, X., & Lin, J. (2024). *A Systematic Review on Prompt Engineering in Large Language Models for K-12 STEM Education.* arXiv:2410.11123. https://arxiv.org/abs/2410.11123
- Google. (2024). *Gemini in Classroom: No-cost AI tools that amplify teaching and learning.* Google Blog. https://blog.google/products-and-platforms/products/education/classroom-ai-features/
- Liu, P., Yuan, W., Fu, J., Jiang, Z., Hayashi, H., & Neubig, G. (2023). Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing. *ACM Computing Surveys, 55*(9). arXiv:2107.13586. https://arxiv.org/abs/2107.13586
- NGSS Lead States. (2013). *Next Generation Science Standards: For States, By States.* Standard 5-LS1-1. https://www.nextgenscience.org/
- OpenAI. *Prompt engineering.* OpenAI API. https://platform.openai.com/docs/guides/prompt-engineering
- Qian, Y. (2025). Prompt Engineering in Education: A Systematic Review of Approaches and Educational Applications. *Journal of Educational Computing Research, 63*(7-8), 1782–1818. https://journals.sagepub.com/doi/10.1177/07356331251365189
- Wei, J., Wang, X., Schuurmans, D., Bosma, M., Ichter, B., Xia, F., Chi, E., Le, Q. V., & Zhou, D. (2022). *Chain-of-Thought Prompting Elicits Reasoning in Large Language Models.* arXiv:2201.11903. https://arxiv.org/abs/2201.11903
- Zheng, M., Pei, J., Logeswaran, L., Lee, M., & Jurgens, D. (2023/2024). *When "A Helpful Assistant" Is Not Really Helpful: Personas in System Prompts Do Not Improve Performances of Large Language Models.* Findings of EMNLP 2024. arXiv:2311.10054. https://arxiv.org/abs/2311.10054
