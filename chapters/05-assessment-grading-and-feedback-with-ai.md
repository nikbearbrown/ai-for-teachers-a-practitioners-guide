# Chapter 5 — Assessment, Grading, and Feedback with AI

**TL;DR.** In workflows that calibrate against your own rubric on a handful of samples and route every comment through a teacher review pass before release, AI-assisted grading reports cluster in the 50–80% range for time saved — measured for short-answer marking with manual review ([Weegar & Idestam-Almquist 2022](https://link.springer.com/article/10.1007/s40593-022-00322-1)), reported by vendors and individual teachers at the upper end, and corroborated at the survey level by Gallup-Walton's 5.9-hour weekly AI dividend ([Gallup-Walton 2025](https://www.waltonfamilyfoundation.org/the-ai-dividend-new-survey-shows-ai-is-helping-teachers-reclaim-valuable-time)). What no published trial has yet measured is whether *students* who receive teacher-reviewed AI feedback learn as well as students who receive teacher-written feedback — and that is the more important question this chapter ends on.

---

## Learning objectives

By the end of this chapter, you should be able to:

1. **Apply.** Use AI to generate first-pass feedback on a student work sample against a rubric.
2. **Apply.** Write a grading prompt that includes the rubric, assignment context, anchor examples, and a feedback format spec.
3. **Analyze.** Apply the grading phase gate: calibrate before bulk processing, review every comment, authorize before release, retain the final grade decision.
4. **Evaluate.** Name the four conditions under which AI grading assistance stops helping and starts hurting.
5. **Create.** Run a rubric-calibration workflow — five samples, AI vs. your scores, prompt revision, re-run — and document the prompt changes.

---

## 1. Opening case — the office hours that came back

*This case is composite-illustrative. The instructor is not a single documented person. The 90-to-22-hour arithmetic is illustrative — it sits inside the range that vendor reports, peer-reviewed short-answer marking studies, and the Gallup-Walton AI-dividend survey would predict for a calibrated workflow, but it is not measured. [verify against a documented case study before publication if a specific named instructor is needed.]*

A community-college composition instructor — call her Professor Daniels — teaches three sections of first-year writing. Ninety students. Three essays per student per semester. Two hundred and seventy essays. Twenty minutes per essay, the way she used to grade them — marginal comments, a paragraph at the end, the rubric checked in pen at the top. Ninety hours per semester. About a workweek's worth of evenings she did not have.

In Spring 2025 she changed two things. She built a Claude prompt that takes the assignment, the rubric, three anchor essays she had scored herself (low / mid / high), and a feedback-format spec — rubric score, three-sentence summary, one revision suggestion. She ran the prompt across the stack in a single batch, about twenty-five minutes of compute time. Then she opened each essay and the AI draft together and worked. She kept comments that were right. She rewrote comments that were generic. She deleted comments that were patronizing. She fixed two cases where the AI had read sarcasm as sincerity. She entered the grades.

Three minutes per essay on review. Two hundred and seventy times three is thirteen and a half hours. Add an hour and a half for calibration on the first batch, another seven hours across the semester for the cases the AI flagged as ambiguous or the cases she chose to mark from scratch because the writing was unusual. Twenty-two hours.

Sixty-eight hours she did not spend grading. She used them as office hours. She did not use them to grade more. She did not use them to publish more. She used them to be in her office on Tuesday and Thursday afternoons, every week, with the door open. Students came in. Some of them came in twice. By midterms there was a queue.

Two things are worth naming about this case before we go further. First, the time savings are the easy part of the story. The hard part is whether the *students* learn as well from a feedback workflow with a teacher review pass as they would have from feedback the teacher wrote from scratch. We do not yet have the trial that answers this. Second, the recovered time is not the dividend on its own. The dividend is what she did with it. Grading faster and going home earlier is one thing. Grading faster and being available for the students who needed her is a different thing. This chapter is about building the workflow that lets the second thing happen, and naming the failure modes that make it collapse into the first.

---

## 2. The grading task taxonomy

A teacher who says "I have to grade this stack" is naming four sub-tasks the profession has chosen to bundle into a single verb. Sorting them out is half the work of figuring out where AI fits.

### 2.1 Four sub-tasks inside "grading"

**First-pass scoring against a rubric.** The act of applying a known scale to a known artifact. The rubric exists; the student's work exists; the question is which level on the rubric this work sits at. This is a measurement task. It has a long history of being done by humans, by other humans, and increasingly by machines. AI-appropriate, with calibration.

**Feedback drafting.** The act of converting "this is a 3" into a paragraph that explains *why* it is a 3 and what would make it a 4. This is a prose-generation task against a structure. AI is good at generating prose against a structure. AI-appropriate, with review.

**Response grouping.** For short-answer or open-response items, the act of noticing that twenty-eight students said roughly the same thing in five different ways, and that four clusters of response will accommodate the whole class. This is a clustering task. Large language models do clustering well. AI-appropriate, with teacher confirmation of the clusters.

**The final grade decision and the student-facing communication that follows.** The act of putting a number in the gradebook, signing the rubric, and — when needed — being the person the student or the parent talks to about what the number means. This is not a sub-task AI performs at all. It is the sub-task in which the teacher carries the professional, legal, and relational weight of having assessed this student's work. The teacher of record is the assessor of record.

The taxonomy is the chapter in one move. Sub-tasks (1)–(3) are where AI helps. Sub-task (4) is where the teacher is irreducible. Mixing them up is how a workflow goes from saving time to losing the room.

### 2.2 Where the empirical ceiling actually sits

Two studies establish what AI can currently do on sub-tasks (1) and (2). Both are recent. Both are worth reading.

Steiss et al. (2024), in *Learning and Instruction*, compared ChatGPT-3.5 feedback to teacher feedback on secondary-student essays across five criteria: criteria-based (does the feedback align to the rubric), accurate, prioritizes essential features, gives clear directions, and uses a supportive tone. The result is precise. ChatGPT *matched or exceeded* humans on *criteria-based*. Humans *outperformed* ChatGPT on the other four — accuracy, prioritization, clarity, and tone ([Steiss et al. 2024](https://www.sciencedirect.com/science/article/pii/S0959475224000215)). The model could mechanically align to the rubric. It could not reliably tell what mattered most for this writer, give directions the student could actually act on, or hit the supportive register without sliding into either flattery or condescension.

Henkel et al. (2024), at *Learning at Scale 2024*, marked real K-12 short-answer questions from the Carousel quizzing platform across science and history, ages 5–16. They reported GPT-4 with few-shot prompting reaching quadratic-weighted kappa around 0.70 against human raters; human-rater agreement against itself sat around 0.75 ([Henkel et al. 2024](https://arxiv.org/abs/2405.02985)). The gap is small. For a short-answer item with a clear rubric, the model is in the second-human-rater agreement band.

The earlier benchmark for automated essay scoring — the Hewlett Foundation ASAP-AES Kaggle competition (2012) — established quadratic-weighted kappa as the field-standard agreement metric and produced systems that matched human raters on long-form essays in the same κ band ([Hewlett ASAP-AES 2012](https://www.kaggle.com/competitions/asap-aes)). ETS's production e-rater, the longest-running automated essay scorer, has reported human-machine agreement on TOEFL essays that approximates second-human agreement ([Attali & Burstein 2007](https://files.eric.ed.gov/fulltext/EJ843852.pdf)) <!-- FACT-CHECK FLAG: CONFIRMED with caveat — ERIC URL is to the 2006 JTLA paper; 2007 ETS RR has DOI 10.1002/j.2333-8504.2007.tb02063.x. See factchecks/05-assessment-grading-and-feedback-with-ai-assertions.md -->.

So the technical capability for sub-tasks (1) and (2) — at near-inter-rater-reliability with humans, on well-scoped tasks, with appropriate prompting — is established. What is *not* established by these studies is whether feedback produced under that capability, released without further review, produces student learning. That is a different study, and it has not been run.

### 2.3 The 70–85% time-saving claim, more carefully

There is a number floating around AI-grading conversations: that AI saves 70–85% of grading time. The TIKTOC for this book uses it. The marketing pages of grading vendors — EssayGrader chief among them — report 80%. Individual teacher reports cluster in the 70–80% range. The Springer 2022 short-answer study reported 64–74% workload reduction with full manual review ([Weegar & Idestam-Almquist 2022, *IJAIED*](https://link.springer.com/article/10.1007/s40593-022-00322-1)).

None of these is a peer-reviewed randomized trial across a representative population.

The honest reading: in workflows with calibration and review, the *upper plausible band* of reported time reductions sits around 50–80%, with vendor reports going to 85% and the peer-reviewed short-answer anchor sitting around 64–74%. The magnitude in any specific classroom depends on the rubric complexity, the essay length, the depth of the review pass, and the teacher's discipline about doing all four. The Gallup-Walton (2025) survey of 2,232 public school teachers, which reports 5.9 hours per week saved across all AI uses for ad hoc users, is the corroborating evidence at the population level ([Gallup-Walton 2025](https://www.waltonfamilyfoundation.org/the-ai-dividend-new-survey-shows-ai-is-helping-teachers-reclaim-valuable-time)). Grading is one of the highest-cost recurring tasks; the share of the 5.9 hours that comes from grading is exactly what you would expect to fall in the 50–80% band when the workflow is right.

I will use 50–80% in the rest of this chapter when I need a number. Citing the 85% figure as a measured effect would be repeating a vendor claim as a finding. We are not yet at the point where we can do that honestly.

### 2.4 Formative versus summative — where the gate slides

A formative assessment is *for* learning — a draft, a check-for-understanding, a low-stakes problem set the student uses to figure out what they do not yet know. A summative assessment is *of* learning — a final exam, a graded essay, a record that goes on a transcript. The legal, ethical, and pedagogical demands on the two are different, and the AI phase gate sits in different places along the workflow as a result.

AI is more defensibly used on the formative side, for two reasons. The cost of an error is lower: a bad formative comment can be ignored by the student or revised by the teacher with no consequence on the record. A bad summative grade carries consequences for the transcript, for scholarship eligibility, for the student's relationship to the work. And the regulatory environment around summative grading typically requires the *teacher of record* to be the assessor. In the United States, "teacher of record" statutes vary by state but generally locate summative grade authority with the licensed educator. In the European Union, the AI Act (2024) classifies AI used to evaluate students or determine educational access as *high-risk*, triggering documentation, oversight, and transparency requirements ([EU AI Act, Annex III, point 3](https://artificialintelligenceact.eu/the-act/)).

The workflow that follows from this: AI runs on the formative draft so the student gets feedback fast and revises against it; the teacher does the summative pass on the revision, informed by but not delegated to the AI's earlier work. The phase gate slides toward more human involvement as the stakes rise.

---

## 3. The rubric-calibration gate

This is the section to read twice. It is the single move that separates a workflow that saves you sixty hours a semester from a workflow that produces the failure case three sections later.

### 3.1 A rubric is a measuring instrument

The framing that helps me: a rubric is a measuring instrument, the way a kitchen scale is a measuring instrument. Like any instrument, it has to be calibrated against a known standard before it can be trusted on unknown cases. The "known standard" for a grading rubric is *your judgment* on a sample of student work — the work you have already scored.

If you put an AI in front of a rubric and ask it to grade, the AI is doing something specific: it is scoring against its own model of what the rubric means, shaped by every rubric it has seen in training. That model is usually close to yours. It is rarely identical. The discrepancy is what calibration measures and the prompt revision is what closes it.

There is a long parallel in educational measurement: inter-rater reliability. When two human raters score the same work and disagree, the standard repair is *norming* — sit the raters down, work through anchors, calibrate until the disagreement is within tolerance. The statistics are Cohen's kappa (κ) for nominal categories, quadratic-weighted kappa (QWK) for ordinal scales like most essay rubrics, and Krippendorff's alpha for mixed designs. Landis and Koch (1977) gave the widely-cited thresholds: κ above 0.61 is "substantial" agreement; above 0.81 is "almost perfect" ([Landis & Koch 1977](https://www.jstor.org/stable/2529310)). For Krippendorff's alpha the conventional cutoff is α ≥ 0.80 for usable data.

When you calibrate an AI against your own grading, you are doing the same thing two human raters do when they norm together. You are not "checking the AI's work." You are bringing a second rater into agreement with the first. The first rater, in this analogy, is you.

### 3.2 The calibration workflow

Five steps. The fifth one is the one most people skip.

1. **Pick five student samples you have already graded yourself.** Not the easiest five. Not the highest scoring five. A spread: one clear pass, one clear fail, three in the contested middle. The middle is where calibration earns its keep.
2. **Build the prompt.** Include the assignment, the full rubric, the five samples *without* your scores, and a request that the AI score each one against the rubric and explain its reasoning.
3. **Run the prompt and compare.** Lay your scores and the AI's scores side by side. If you scored a 2, a 4, a 3, a 4, a 3, and the AI returns 3, 4, 4, 5, 3, you have learned something specific: the AI runs about half a point higher than you on the bottom half of your range and matches you on the top half.
4. **Revise the prompt.** Add anchor examples. "Here is what a 2 looks like — short paragraph in the student's voice. Here is what a 3 looks like — same. Here is what a 4 looks like." Sharpen the rubric language where the AI seems to have read it permissively. Add negative anchors where the AI is being generous — "an essay that has these features but does not connect them is a 2, not a 3."
5. **Re-run on the same five samples and check.** If the AI's scores now sit within ±0.5 of yours on all five, you have a calibrated prompt and you can scale it. If they do not, repeat step 4 with one more revision. If after three rounds the gap has not closed, your rubric is probably underspecified — which is its own useful finding, separate from the AI question.

Most teachers I have watched do this for the first time skip step 5. They run the calibration, they see the off-by-one offset, they trust themselves to adjust mentally as they review later, and they scale immediately. The mental adjustment does not survive thirty essays. By essay forty they have forgotten that the AI runs half a point high, and the systematic upward drift has propagated into a real grade distribution. Calibration that is not closed in the prompt is calibration that is not happening.

### 3.3 The thing calibration does not catch

Calibration measures agreement between you and the AI on the rubric you both share. It does not measure whether the rubric itself is fair. This is where the equity question lives, and I want to be honest about it.

Automated essay scoring has a documented history of underscoring high-proficiency English language learner essays relative to their human-rated quality. The pattern is not unique to AI scoring — human raters underscore L2 writers too, on essays of equivalent argumentative and substantive quality. But automated scoring sometimes reproduces and sometimes amplifies the human bias rather than removing it. Recent work in this area is mixed and shifting; see ([Loukina et al. on bias in automated scoring, ETS Research Reports](https://files.eric.ed.gov/fulltext/EJ1233920.pdf)) <!-- FACT-CHECK FLAG: UNVERIFIED — confirm ERIC ID resolves to intended Loukina paper. See factchecks/05-assessment-grading-and-feedback-with-ai-assertions.md --> and recent preprint work on bias in LLM scoring of ELL essays ([arXiv 2505.10643](https://arxiv.org/abs/2505.10643)). [verify the bias-amplification finding from arXiv 2602.23580 — the citation in the research notes pointed to a paper I cannot fully confirm at this writing; the broader bias-against-L2-writers literature is settled, the amplification-versus-reproduction question is contested.] <!-- FACT-CHECK FLAG: CONFIRMED (paper exists; BRIDGE/Wang et al., Feb 2026) — see factchecks/05-assessment-grading-and-feedback-with-ai-assertions.md -->

So a calibration step that produces κ = 0.85 against your own grades may also conceal a fairness gap, especially if your sample of five anchor essays does not include any ELL submissions. The practical move: build at least one anchor from your highest-quality ELL submission, and after the first bulk run, disaggregate AI scores by student-language background and look at the mean. If the AI is systematically underscoring your ELL students relative to how you would score them, calibration with additional ELL anchors closes some of the gap. It does not close all of it. I will come back to this in section 7.

---

## 4. The Bastani parallel at the feedback level

This is the chapter's frictional move and I want to label it carefully: what follows is a *prediction*, not a measured effect. It is well-motivated by two findings — Bastani et al. (2025) at the practice level, Steiss et al. (2024) on feedback quality — but the direct feedback-level analog has not been run.

### 4.1 What Bastani actually found

Bastani et al. (2025), in *PNAS*, ran a controlled trial with about a thousand Turkish high school students learning mathematics. One condition had no AI. One condition (GPT Base) had unscaffolded GPT-4 access during practice. One condition (GPT Tutor) had GPT-4 access under a Socratic-scaffolded system prompt that withheld direct answers and asked questions instead.

The headline result is uncomfortable. During the practice sessions, students in the GPT Base condition outscored the no-AI control by 48%. Then everyone took a closed-book exam without AI. The GPT Base students scored 17% *lower* than the control — a 17% relative reduction, not 17 absolute percentage points (the unit matters; the original draft of this chapter got this wrong, and the misread is the kind of small precision error this chapter is about). The GPT Tutor condition — Socratic scaffolding — closed most but not all of that gap ([Bastani et al. 2025](https://www.pnas.org/doi/10.1073/pnas.2422633122); corrected version: [DOI 10.1073/pnas.2518204122](https://www.pnas.org/doi/10.1073/pnas.2518204122)).

The Frictional reading is the one the Preface and Appendix G develop in full: the practice gain was real, and the learning gain was negative, because the cognitive struggle that would have produced learning was bypassed by the AI doing the work. The artifact improved. The brain did not. The students felt like they had learned. They had not.

### 4.2 The analog at the feedback level

Now run the same logic on a feedback workflow that releases AI-drafted comments to students without teacher review.

The student receives a feedback paragraph that reads like their teacher's voice, that names the rubric, that identifies generic features in the writing — thesis clarity, evidence quality, transitions. The student reads it. The student feels they got feedback. The revision instinct fires. The student revises against the comments — sharpens the thesis the AI said to sharpen, adds the evidence the AI said to add, smooths the transitions the AI said to smooth.

The artifact improves. The conceptual gap the *teacher* would have named — the gap between this student's actual understanding of the topic and the understanding the assignment was designed to develop — was never named in the AI feedback, because the AI did not know what this student understood. The feedback was structurally correct and contextually disconnected. The student revised the surface and missed the substrate. The teacher's PCK — the knowledge that this student has been confusing X for Y all semester, or that this class has been hand-waving past Z — was the thing that would have made the feedback educational. The AI had none.

This is what I am calling the *fluency trap at the feedback level*. It is a prediction, not yet measured. The Steiss finding gives us reason to believe it: AI feedback was structurally aligned to the rubric and weaker on the four dimensions that make feedback educational — accuracy on this writer, prioritization of what matters most for this writer, clarity of directions this writer can act on, supportive tone for this writer. The Bastani finding tells us that decoupling the feel of cognitive engagement from its function is the central failure mode of unscaffolded AI use. Putting those together, the prediction is that AI feedback released without teacher review produces the same decoupling at the feedback level: the *feel* of getting feedback, without the *function* of getting feedback.

The 45 seconds it takes a teacher to read an AI-drafted comment and either keep it, edit it, or rewrite it is the friction that closes the gap. It is the cognitive insertion point at which the teacher's PCK gets added to a piece of feedback that otherwise has none. The phase gate is not a bureaucratic check. It is the move that converts structurally correct AI output into pedagogically active feedback.

The research that would settle this is straightforward in shape: a randomized trial across classrooms where one arm receives AI-drafted feedback released as-is, one arm receives AI-drafted feedback after teacher review, and one arm receives teacher-written feedback. Measure revision quality, exam performance two weeks later, and student-reported uptake. As of this writing, no such trial has been published. Until it has, the prediction stands as a prediction.

### 4.3 The four failure conditions

The Bastani parallel is the theoretical motivation for the four failure conditions in the workflow. They are the operational form of the same insight:

1. **No rubric calibration before bulk processing.** The AI scores against its own implicit rubric. Systematic bias propagates to the full class.
2. **No teacher review of AI-drafted comments.** The feedback-level fluency trap fires. Students receive structurally correct, contextually disconnected feedback. They revise the surface.
3. **Feedback released without human authorization.** The teacher of record has not signed off. The legal, ethical, and professional weight of summative communication has been dropped.
4. **Feedback that cannot be applied by this student.** The advice references a skill the student does not have ("sharpen the causal mechanism") or assumes a starting point the student is not at ("strengthen the counterargument" — to a student who has not written a counterargument).

If any of the four is missing, the workflow has stopped helping. It may not yet be hurting; it has stopped helping.

---

## 5. Worked example — calibrating a short-answer prompt

Here is the workflow on a concrete task. Numbers are illustrative; the prompt structure is the real artifact.

A high school world history teacher has 110 short-answer responses to the prompt *Explain one cause of the French Revolution and provide one piece of evidence for it.* The rubric:

- **4** — Names a specific cause, gives specific evidence, makes the causal connection explicit.
- **3** — Names a cause, gives evidence, leaves the causal connection implicit.
- **2** — Names a cause, evidence is vague or generic.
- **1** — Cause is missing, vague, or wrong.

She has already graded five samples herself: scores 2, 4, 3, 4, 3. Now she runs the first calibration pass.

**Calibration prompt v1:**

```
ROLE: You are a U.S. history teacher scoring 9th-grade short-answer responses.
CONTEXT: 9th-grade world history class. Students have just finished a two-week
unit on the French Revolution. The prompt asked them to explain one cause and
provide one piece of evidence.
TASK: Score each of the five responses below against the rubric. For each, give
the score and one sentence explaining the score.
RUBRIC:
  4 — Names a specific cause; specific evidence; causal connection explicit.
  3 — Names a cause; evidence; causal connection implicit.
  2 — Names a cause; vague or generic evidence.
  1 — Cause missing, vague, or wrong.
RESPONSES: [paste the five responses, anonymized, no scores]
OUTPUT FORMAT: One line per response: "Response N — Score X — [one-sentence reason]"
```

The AI returns: 3, 4, 4, 5, 3. (The "5" is the AI inventing a level the rubric does not have, which is its own diagnostic — the AI is reading the top sample as exceeding the rubric ceiling, which tells her either the rubric ceiling is set wrong or the AI is being generous.)

Off-by-one on three of five, plus a rubric ceiling violation. Systematic upward drift on the lower half. The fix is anchors.

**Calibration prompt v2 — add anchors:**

```
[Same as v1, plus:]
ANCHOR EXAMPLES:
  Example of a 2: "The French Revolution happened because the people were
    angry at the king." [Names a cause vaguely; evidence is generic; no
    specific causal mechanism named.]
  Example of a 3: "One cause was that bread prices went up in 1788–1789,
    which made the workers in Paris angry." [Names a specific cause and
    gives specific evidence; causal connection between price and revolution
    is implicit, not stated.]
  Example of a 4: "One cause was the fiscal crisis caused by France's
    support for the American Revolution, which forced Louis XVI to call
    the Estates-General in 1789. The Estates-General gave the Third
    Estate a venue to reorganize as the National Assembly." [Specific
    cause, specific evidence, causal mechanism named explicitly.]
NOTE: The rubric ceiling is 4. Do not assign scores above 4.
```

Re-run on the same five samples. AI returns: 2, 4, 3, 4, 3. Match on four of five, off-by-one on the fifth. Within tolerance. She can scale.

She now runs the same prompt against all 110 responses, then opens the responses in batches of twenty for review. For each she sees the response, the AI's score, the AI's one-line reason. She keeps about 80%, edits about 15%, overrides about 5%. The 5% she overrides are mostly responses where the AI missed a misconception specific to this class — students who said "bread prices went up *because* of the Revolution," getting the causal direction backward, which the AI scored as a valid causal statement because it was *a* statement of a causal relationship. The teacher has been correcting this misconception for two weeks. She knows what to look for. The AI does not.

Total time on the 110: about 80 minutes, including calibration. Without AI, about 4 hours. The 80 minutes recovered did not come from the AI grading the essays. They came from the AI doing 80% of the prose-generation work for 80% of the responses, *which the teacher reviewed*. The teacher made every grade decision. The AI drafted the comments she kept or revised.

The lesson, restated: the work is not delegated. The drafting is. The judgment stays.

The limit: this workflow worked because the rubric was tight (four levels with clear distinctions), the responses were short (one to three sentences), and the misconceptions she was looking for were ones she had already named for herself. If the rubric had been six levels with overlapping descriptors, or the responses had been three-page essays, or she had been teaching this unit for the first time and did not yet know what to look for, the workflow would have produced less savings and required more review. The dividend scales with the clarity of the teacher's prior judgment about what the work should look like.

---

## 6. Three prompt templates

Each of these is a starting point. The calibration step turns it into a prompt that fits your class. None of them should be used without the five-sample calibration pass first.

### 6.1 Essay first-pass feedback prompt

```
ROLE: You are a [grade-level] [subject] teacher giving formative feedback on a
draft essay. Your goal is feedback the student can act on for a revision.
CONTEXT:
  Assignment: [paste the assignment prompt]
  Rubric: [paste the full rubric]
  Class context: [grade level, subject, what the class has been working on]
  Student context: [one sentence about this student's general writing
    development — e.g., "developing thesis clarity; strong evidence
    selection; sometimes loses through-line." Optional.]
ANCHORS:
  Example of a [low] essay: [paste]
  Example of a [mid] essay: [paste]
  Example of a [high] essay: [paste]
TASK: Read the student's draft below. Produce:
  1. A rubric score for each criterion, with one sentence explaining each.
  2. A three-sentence summary of the essay's current state.
  3. One specific revision suggestion the student can act on for the next
     draft. The suggestion should reference a specific sentence or section
     of THIS student's draft, not a generic move.
DRAFT: [paste draft]
DO NOT: Use generic feedback phrases like "develop further" or "be more
specific" without naming where in the essay and what specifically.
OUTPUT FORMAT: [specify — markdown, plain text, length cap if any]
```

The third deliverable — one specific revision suggestion that references a sentence in this student's draft — is the place where the AI most often slides into generic feedback. The "DO NOT" line is the one that does the most work in the prompt.

### 6.2 Rubric-aligned comment prompt

```
ROLE: You are a [grade-level] [subject] teacher writing a rubric-aligned
end-comment on a student paper.
CONTEXT:
  Rubric: [paste rubric with criteria and levels]
  Score on this work: [criterion: level, criterion: level, ...]
  Anchor for the matching score: [paste anchor for the level the student
    landed on, for at least the criterion that scored lowest]
TASK: Write a three-paragraph end-comment that:
  1. Names what the student did well, citing a specific sentence or
     section from the work.
  2. Names the criterion on which the student scored lowest, explains
     why the work scored at that level (not the level below or above),
     and references a specific feature of the work as evidence.
  3. Gives one revision suggestion the student can act on.
TONE: Direct, professional, supportive. Address the student by [first name].
DO NOT: Praise features that are not actually present. Do not soften scores
that are accurate. Do not add encouragement that does not connect to the
specific work.
WORK: [paste work]
```

This is the prompt for the case where you have already scored the work and need the prose generated against the score. The score is yours; the AI is converting your judgment into the comment you would have written if you had three hours.

### 6.3 Response-grouping prompt for short-answer items

```
ROLE: You are clustering student short-answer responses to help a teacher
give feedback efficiently.
CONTEXT:
  Question: [paste the question students answered]
  Rubric: [paste the rubric]
  Class size: [N students]
TASK: Read all responses below. Cluster them by argument type — the
substantive claim each response is making, not the surface phrasing.
For each cluster:
  1. Give the cluster a one-phrase label (e.g., "Financial crisis as
     primary cause" or "Enlightenment ideas as primary cause").
  2. List the response IDs in this cluster.
  3. Note whether the responses in this cluster are mostly at the
     [4 / 3 / 2 / 1] level on the rubric.
  4. Draft a 3-sentence feedback comment appropriate for the cluster,
     referencing the typical strength and the typical weakness of
     responses in this cluster.
  5. Flag any responses inside the cluster that do not fit the cluster
     pattern and need individual teacher attention.
RESPONSES: [paste numbered responses]
```

The "flag responses that do not fit the cluster pattern" line is the place where the AI surfaces the cases that need you most. Those are the ones to read first.

---

## 7. Common misconceptions

I want to name four readings of this chapter that I have watched teachers slide into. Each is a wrong turn that the calibration workflow does not catch on its own.

### 7.1 "AI grades for me"

It does not. The AI drafts. You decide. The act of putting a grade in the gradebook is the act of taking professional responsibility for that grade, and you cannot delegate professional responsibility to a system that has no license, no employer, and no relationship with the student. The legal frame — "teacher of record" — is the same frame the EU AI Act extends to high-risk AI applications in education: the licensed educator is the assessor of record, and the system is an aid. The AI's contribution to a grade is no different in kind from a teaching assistant's contribution. The TA is consulted. The professor decides.

A teacher who skips review because "the AI is usually right" has stopped being the teacher of record for the work the AI was usually right about. The eventual failure is not technical. It is professional.

### 7.2 "First-pass AI feedback is final feedback"

It is structurally correct. It is contextually disconnected. The Steiss et al. (2024) finding is the citation: AI feedback wins on criteria-based alignment to the rubric and loses to humans on accuracy for this writer, prioritization of what matters most for this writer, clarity of directions this writer can act on, and supportive tone for this writer ([Steiss et al. 2024](https://www.sciencedirect.com/science/article/pii/S0959475224000215)). Releasing first-pass AI feedback as final feedback is the workflow that produces the Bastani parallel at the feedback level: the student feels they got feedback, revises the surface, and does not develop the underlying skill.

The 45 seconds per comment of teacher review is the cognitive insertion point. Without it, you are not running a feedback workflow. You are running a feedback theater.

### 7.3 "The same prompt works on every cohort"

The calibration that closed the gap on this fall's section may not close it on next spring's section, for two reasons. The students are different — different writing levels, different misconceptions, different prior preparation. The model is different — a calibration prompt that worked on GPT-4 in March may not score the same way on GPT-4o in October, because the model has been updated and the implicit rubric has shifted. Calibration drift across model versions is a real hazard, and there is no standard yet for re-calibrating when underlying models update. The practical move: recalibrate at the start of each grading cycle. The five-sample drill is fifteen minutes. It is cheap.

The deeper version of this misconception is the assumption that a *workflow* is a fixed asset rather than a recurring discipline. Calibration is not a one-time setup. It is a recurring move.

### 7.4 "AI grading is more objective than human grading"

It is more *consistent* than human grading, in the sense that the same prompt run against the same essay will produce closely related scores. It is not necessarily more *accurate*, and consistency without accuracy is a description of a measuring instrument that is reliably wrong. The ELL/ESL bias literature is the cleanest case: automated scorers and human scorers *both* underscore high-proficiency English language learner essays relative to their human-rated quality, and the automated scorers sometimes reproduce and sometimes amplify the human bias. High inter-rater reliability between an AI and a teacher who share a bias is not fairness. It is shared bias dressed in a kappa statistic.

The fix is not to abandon AI grading. The fix is to disaggregate AI scores by student subgroup after every bulk run, look at the means, and if a systematic gap appears, calibrate with anchor essays drawn from the underscored group. This will close some of the gap. It will not close all of it. The honest framing: AI does not introduce subgroup bias into a process that otherwise has none; AI participates in a process that already has bias, and the workflow must include a check that does not pretend otherwise.

---

## 8. Exercises

Three exercises. The first is the flagship — the one the chapter is asking you to run before you scale a workflow.

### 8.1 Calibration drill

Take five student samples from a recent assignment that you have already graded yourself. Do not pick the easiest five. Pick a spread: one clear pass, one clear fail, three in the contested middle.

1. Build a calibration prompt using the structure in section 5: assignment, rubric, anchor examples (use ones from a *different* set than your five test samples), the five test samples without your scores, and a request for scores plus one-sentence reasoning.
2. Run it. Note the AI's scores next to yours. Compute the mean offset (how much higher or lower the AI is, on average) and the maximum disagreement (the single largest gap on any sample).
3. Revise the prompt — add anchors at the levels the AI is missing, sharpen rubric language at the levels where it is being permissive, add negative anchors where it is being generous.
4. Re-run on the same five samples. Compute the offset and maximum again.
5. If you are within ±0.5 on all five, document the prompt and the changes you made. If you are not, do one more revision. If after three rounds the gap has not closed, write down what you think the rubric is missing — calibration that fails to close is usually telling you something about the rubric.

Deliverable: the final calibration prompt, plus a short note (one paragraph) on what the prompt changes were and why they closed the gap.

### 8.2 Failure-condition audit (Analyze)

Take three AI-drafted comments — from a workflow you have run, or generate three using a starter prompt and a sample essay. For each, ask the four failure-condition questions:

- Was the prompt calibrated against five samples before this comment was generated?
- Did the teacher (you) review the comment before it would have been released?
- Was the comment authorized — would you sign your name to it as is?
- Could this specific student act on this comment without skills they do not have?

Mark each as a pass or fail. Write one sentence per failure on what the prompt or workflow change would be to close it.

### 8.3 Bias check on a real batch (Create)

After running a bulk AI grading pass on a recent assignment, pull the AI's scores into a spreadsheet. Disaggregate by one student characteristic you have data on — most commonly ELL status, but it could be IEP/504 status, gender, or any cohort characteristic with at least five students in each subgroup.

Compute the mean AI score by subgroup. Compute the mean *your* score by subgroup on the same samples. If the AI's subgroup mean is more than 0.5 of a point below the corresponding subgroup mean *of your scores*, you have evidence of an AI-introduced subgroup gap. Build at least two anchor essays drawn from the underscored subgroup's high-quality submissions and re-run the prompt. Recompute the means. Document the change.

If the AI's subgroup means are not far from yours but *your* means show a subgroup gap, the AI is reproducing your existing pattern — which is a separate question, and one that this chapter does not solve. The bias check surfaces it. The chapter does not tell you what to do about it.

---

## 9. What would change my mind

A pre-registered randomized trial — at least two semesters, multiple institutions, mixed subjects — comparing student learning outcomes (measured by unassisted post-assessment, two weeks after instruction) across three conditions: (a) teacher-written feedback, (b) AI-drafted feedback released with teacher review, (c) AI-drafted feedback released without teacher review. If condition (b) does not produce learning outcomes statistically indistinguishable from (a), the chapter's central frictional move is wrong and the phase gate has to slide further toward the human side. If condition (c) produces outcomes statistically indistinguishable from (b), the chapter is overstating the cost of skipping the review pass.

Neither trial has been run at the time of writing. Both should be.

---

## 10. Still puzzling

A few questions I do not have clean answers to. They are the questions worth pulling on next.

- **The time-versus-learning question.** Even granting that calibration and review produce time savings in the 50–80% range, we do not yet know whether students learn as well from a calibrated AI-plus-review feedback workflow as they would from feedback the teacher wrote from scratch. The Bastani parallel predicts they should — provided the review pass is real — but no trial has measured it. The recovered hours are a real dividend. The question is whether the work the dividend funds (more office hours, more student conversations) closes any learning gap the workflow itself opens.

- **The bias question past calibration.** Anchor essays from underscored subgroups close some of the AI-introduced gap. They do not close all of it. They do not close the human-rater gap that the AI is partially inheriting. Whether a grading workflow can be both efficient and fair, given an underlying assessment process that has its own subgroup patterns, is a question the calibration drill surfaces but does not answer.

- **Calibration drift.** No standard exists for re-calibrating prompts when underlying models update. Teachers who run stable workflows are running them against a moving target. The practical workaround is the recurring five-sample drill; the systemic answer would require either model-version-locked prompts (which most teacher-facing platforms do not yet expose) or in-product calibration tooling that flags drift automatically.

- **Where the gate should slide for high-stakes summative work.** The chapter has argued that AI is more defensibly used on the formative side. It has not given a hard rule for where the gate sits on a final exam essay versus a portfolio cover letter versus a thesis defense. The principle (the higher the stakes, the more human involvement) is the right principle. The operational form of it — which AI-drafted comments are acceptable in which contexts — is unsettled.

---

## Bridge to Chapter 6

Grading is the work the teacher does on what students produced. Differentiation is the work the teacher does on what students will receive — the readings, the scaffolds, the supports adjusted for who is in the room. The phase-gate logic is the same: AI proposes, the teacher (and, for IEP/504 work, the licensed specialist) disposes. The anonymization gate is added because student data is now upstream of the AI rather than downstream of it. Chapter 6 takes that next.

---

*Tags: assessment, grading, AI feedback, rubric calibration, inter-rater reliability, Bastani 2025, Steiss 2024, Henkel 2024, formative summative, teacher of record, ELL bias, phase gate, AI dividend*

*Voice: feynman | Length: ~5,000 words | Status: draft for Nik's review*
