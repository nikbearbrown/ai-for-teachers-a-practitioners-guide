# TIKTOC — AI for Teachers: A Practitioner's Guide

**Working title:** AI for Teachers: A Practitioner's Guide
**Series:** Practitioner's AI Series · Northeastern University College of Engineering
**Author:** Humanitarians AI · ni.brown@neu.edu · Bear Brown & Company
**Document:** Full TIKTOC — Complete Architecture
**Version:** 2.0
**Status:** Pre-draft — research phase

---

## Book Concept and Thesis

This book teaches **the practical division of AI and human labor in K–12 and higher education** — the decisions about which tasks to delegate, how to delegate them well, and what to keep — to **teachers who are already using or considering AI tools**, by **giving them a task-level framework and tool-specific practices they can apply Monday morning**, through worked examples, copy-paste prompts, and phase-gate guidance that makes the boundary between AI work and human work explicit and enforceable. It fills the gap between breathless AI-for-education hype (which makes no task-level claims) and academic research (which makes task-level claims no teacher has time to read). It succeeds if the reader can **identify which of their recurring tasks AI should handle, write prompts that produce usable output, enforce the phase gates that protect their professional judgment, and recover more than five hours per week** after completing it.

**One-sentence logline:**
Six hours a week back to teaching — here is exactly which tasks to delegate, how to delegate them, and what you must never hand off.

**Theoretical spine:**
The book rests on the *Frictional* framework: learning requires struggle because the neurological events that constitute memory formation are triggered by cognitive friction. AI that removes struggle removes learning. AI that makes struggle more productive enhances learning. The phase gate is not a policy restriction — it is a pedagogical specification of which cognitive work must remain human because it constitutes learning rather than merely preparing for it. This argument is made in plain language in the Preface and in technical depth in Appendix G.

---

## Companion Publications

**$1 Kindle Companions** — standalone books for teachers who want the full treatment of specific domains introduced in Chapters 10 and 11:

- *Writing with AI* — full treatment of AI-assisted writing instruction and teacher writing workflows. Chapter 10 of this book is a summary introduction that orients readers toward this volume.
- *Coding with AI* — full treatment of AI-assisted computational thinking and teacher coding workflows. Chapter 11 of this book is a summary introduction that orients readers toward this volume.

**The Deployable Tool** — the master Claude Project system prompt (Appendix F) operationalizes the full book's framework as a phase-gated AI assistant with task-specific modes. Teachers paste once into a Claude Project; the tool enforces the entire book's framework in daily use.

---

## Learner Profile

**Primary reader:** A K–12 or higher-education teacher who has heard that AI can save time, has probably tried one or two tools, is skeptical of both the hype and the fear, and wants a practical framework — not philosophy, not policy, not another app recommendation. They want to know: which of my tasks should I actually give to AI, how do I do that well, and what do I protect?

**Prior knowledge assumed:**
- Basic computer literacy (email, word processing, learning management system)
- Familiarity with at least one AI tool (even just having heard of ChatGPT)
- Professional teaching context: a real class, real students, real workload

**Prior knowledge NOT assumed:**
- Programming or technical background
- Data science or statistics
- Prior structured AI training

**Prior misconceptions the book must address:**
1. "AI will grade for me" — AI can draft feedback; the professional judgment that makes feedback pedagogically sound is irreducibly human
2. "I just describe what I want and it produces something good" — prompting is a learnable skill with structure
3. "Using AI means I'm doing less teaching" — systematic AI use recovers time for more teaching, not less
4. "AI tools are interchangeable" — different tools have different architectures with different appropriate uses
5. "The time savings aren't real" — the Gallup-Walton finding is citable and real; 5.9 hours/week for ad hoc users
6. "The struggle is a problem to be solved" — the struggle is the mechanism of learning; AI that removes it removes learning

---

## Book Type and Deployment Specification

**Primary type:** Practitioner handbook — chapters are self-contained enough to be read out of order by teachers who need a specific task area, but build on a framework introduced in Chapters 1–3.

**Primary adoption context:**
Professional development programs, pre-service teacher education, instructional technology courses, individual teacher self-study.

**Secondary adoption context:**
District-level AI training programs, college faculty development workshops, school administrator reading groups.

---

## Three-Part Learning Arc

**Part I — The Framework (Chapters 1–3)**
Establishes the division-of-labor principle, the phase-gate concept, and prompting as a foundation skill. A teacher who reads only Part I has the mental model they need to evaluate any AI tool or claim.

**Part II — Core Tasks (Chapters 4–9)**
Applies the framework to the six highest-time-cost recurring tasks in a teacher's workweek: lesson planning, assessment and grading, differentiation, communication, slides, and data visualization. Each chapter delivers: the task taxonomy, the phase gate, copy-paste prompt templates, and a time-recovery estimate.

**Part III — Implementation and Integrity (Chapters 10–14)**
Extends into writing and coding (introductory, pointing to $1 Kindle companions), then addresses the practical and ethical questions every teacher faces: how to build a sustainable AI workflow, how to handle academic integrity and privacy, and what to tell students.

---

## Full Structure

```
Preface: The Struggle Is the Point
Part I: The Framework
  Chapter 1 — The AI Dividend
  Chapter 2 — The Phase Gate
  Chapter 3 — Prompting That Works
Part II: Core Tasks
  Chapter 4 — Lesson Planning with AI
  Chapter 5 — Assessment, Grading, and Feedback with AI
  Chapter 6 — Differentiation with AI
  Chapter 7 — Communication with AI
  Chapter 8 — Making Slides with AI
  Chapter 9 — Making Graphs and Data Visualizations with AI
Part III: Implementation and Integrity
  Chapter 10 — Writing with AI: An Introduction
  Chapter 11 — Coding with AI: An Introduction
  Chapter 12 — Building Your AI Workflow
  Chapter 13 — Academic Integrity, Privacy, and Honest Use
  Chapter 14 — What to Tell Your Students
Conclusion: The Research Agenda and What Comes Next
Appendix A — The Full Phase Gate Map
Appendix B — Prompt Library Starter (50 Prompts)
Appendix C — The Diagnostic Checklists
Appendix D — Research Reference
Appendix E — Series Map
Appendix F — The AI Teaching Assistant (Deployable Claude Project)
Appendix G — Frictional: The Full Framework
```

---

## Preface: The Struggle Is the Point

**One-line:** The artifact used to be proof of the process. It no longer is. Here is why that changes everything — and why the answer is humans plus AI, not humans or AI.

**Core argument:**
For most of educational history, the essay proved the thinking because only thinking could produce the essay. Generative AI severed this causal connection. The artifact now has two pathways: through genuine cognitive process, or around it entirely.

But genuine learning is a biological event — a cascade of neurological processes triggered by cognitive friction. Dopamine prediction error signaling. Synaptic consolidation. Dendritic spine formation. These events produce behavioral traces. An AI can produce the artifact without triggering these events. It cannot produce the traces.

The struggle is not the obstacle to learning. It is the mechanism of learning. AI that removes the struggle removes the trigger. AI that makes the struggle more productive enhances learning. The entire book rests on this distinction.

**Key passages:**
- "The artifact used to be proof of the process. It no longer is."
- "The struggle is not the obstacle. It is the mechanism."
- "The phase gate is not a restriction on AI capability. It is a specification of which cognitive work needs to happen for learning to occur."
- "Humans + AI, not humans or AI."

**Pointer:** Readers who want the full theoretical and neurobiological treatment should see Appendix G — *Frictional: The Full Framework*.

---

## Chapter-by-Chapter TIKTOC

---

### CHAPTER 1 — The AI Dividend: What Teachers Actually Get Back

**One-line:** The research on teacher time savings is real, specific, and less than the hype claims — here is what the evidence actually says and why six hours matters.

**Opening case:** A teacher who spent 11 p.m. on a Sunday re-reading thirty essays she had already read once, making the same marginal comments in different handwriting. She tried AI the next Sunday. The first draft feedback took four minutes instead of forty. She spent the recovered time rereading the three essays that needed her most. This is the AI dividend — not doing less, but doing the right things.

**Learning outcomes:**
1. (Understand) Describe the Gallup-Walton 2025 finding on teacher time savings: 5.9 hours per week for ad hoc users, with the conditions under which systematic deployment projects higher recovery.
2. (Understand) Distinguish between the ad hoc time savings (6 hours, research-supported) and the systematic deployment ceiling (16+ hours, projected but not yet fully measured).
3. (Apply) Identify three specific tasks from their own workweek that fall within the AI-appropriate category based on the task taxonomy introduced in this chapter.
4. (Evaluate) Assess a specific AI time-savings claim against the research evidence.

**Core content:**
- The Gallup-Walton Family Foundation survey (2024, n=2,232): 60% of K–12 teachers use AI tools; weekly users report 5.9 hours saved
- Why 5.9 hours is a floor, not a ceiling: ad hoc vs. systematic use
- The reinvestment finding: what teachers report doing with recovered time (individualized feedback, student relationships, instructional moves)
- The task taxonomy preview: AI-appropriate, hybrid, human-required
- The honest 20-hour claim: personal experience vs. research-supported number; the book uses 6 hours in all citations
- Australia comparison: 46.4 hours/week average, 60% non-instructional; Finland comparison: 36 hours/week, 1.5 hours administrative vs. 4.7 in Australia
- The projected 16.7-hour ceiling under systematic deployment: task-by-task model with empirical sources for each estimate

**Key concepts:** AI dividend, task taxonomy, ad hoc vs. systematic use, time recovery, non-instructional workload

**Time recovery estimates by task (introduced here, detailed in Chapters 4–9):**

| Task | Baseline weekly hours | AI reduction | Hours recovered |
|------|----------------------|-------------|----------------|
| Lesson preparation | 8.0 | 35% | 2.8 |
| Grading and feedback | 7.5 | 60% | 4.5 |
| Administrative tasks | 5.0 | 50% | 2.5 |
| Differentiation | 3.5 | 60% | 2.1 |
| Quiz/assessment development | 3.0 | 50% | 1.5 |
| Data analysis | 2.5 | 60% | 1.5 |
| Professional development | 2.0 | 40% | 0.8 |
| **Total projected** | **31.5** | **53%** | **16.7** |

*Source: NFER/EEF, Gallup-Walton, Australian workload audit data. Systematic deployment assumed.*

**Assessment/exercise:** Workweek audit — the reader identifies their five most time-consuming recurring tasks and classifies each as potentially AI-appropriate, potentially hybrid, or definitively human-required.

**Bridge:** The dividend is real. But not all time savings are equal — recovering six hours by delegating the wrong tasks produces worse outcomes than the status quo. Chapter 2 introduces the framework that makes delegation safe.

---

### CHAPTER 2 — The Phase Gate: What AI Handles, What You Must Keep

**One-line:** The phase gate is the explicit boundary between AI preparation and human teaching — learning where it sits, and enforcing it, is the entire skill.

**Theoretical connection:** This chapter is the practical application of the *Frictional* argument from the Preface. The phase gate specifies which cognitive work must remain human because it constitutes learning rather than preparing for it. The neurobiological justification is in Appendix G; the practical enforcement is here.

**Opening case:** A district that deployed an AI grading assistant without establishing a phase gate. The tool produced scores. Teachers approved them without reviewing. Students received feedback that was accurate by rubric but wrong for their specific learning. Three parents complained. The tool was shut down. The problem was not the tool — it was the absence of a gate.

**Learning outcomes:**
1. (Understand) Define the phase gate as the specific point at which AI processing stops and human professional judgment begins.
2. (Understand) Explain the neurobiological basis of the phase gate: human cognitive work on the right tasks constitutes learning; AI doing that work bypasses learning.
3. (Apply) Name the correct phase gate for each of the six AI-appropriate task categories.
4. (Analyze) Identify which of the Bastani et al. (2025) findings apply to teacher AI use: the performance paradox, the illusion of competence, and the conditions under which AI use degrades rather than supports outcomes.
5. (Evaluate) Assess a given AI-assisted workflow and identify whether the phase gate is correctly placed, missing, or in the wrong location.

**Core content:**
- The 12 phase gates: rubric calibration gate, discrepancy resolution gate, Socratic scaffolding gate, direct instruction gate, content accuracy gate, IEP/504 compliance gate, parent communication gate, student performance intervention gate, PCK misconception gate, RAG walled garden gate, behavioral crisis gate, student identity anonymization gate
- The "AI proposes, instructor disposes" principle
- The Bastani 2025 parallel: cognitive offloading applies to teachers too — if AI does the instructional thinking, instructional judgment atrophies
- The jagged technological frontier: tasks where AI is unexpectedly capable vs. tasks where AI fails unexpectedly
- Why the gate is not about trust in AI — it is about which outcomes require human accountability and which cognitive work constitutes learning
- Hattie meta-analysis connection: teacher-student relationship (d=0.72) and collective teacher efficacy (d=1.57) are irreducibly human — they cannot be delegated

**The 12 Phase Gates — operational specifications:**

| Gate | Trigger condition | AI boundary | Human step | Consequence of skipping |
|------|------------------|-------------|------------|------------------------|
| 1. Rubric calibration | Before bulk grading | AI runs on 5 samples | Teacher calibrates before bulk processing | Systematic bias propagates to full class |
| 2. Discrepancy resolution | Student contests AI score | AI barred from resolution | Teacher reviews and decides | Grade disputed without human judgment |
| 3. Socratic scaffolding | Student practice interaction | AI cannot give direct answers | AI gives hints only; student does cognitive work | Bastani performance paradox: practice gain, learning loss |
| 4. Direct instruction | Live classroom | AI cannot deliver instruction | Teacher teaches; AI may analyze afterward | Learning stripped of PCK and relationship |
| 5. Content accuracy | Before distributing AI-generated materials | AI generates draft | Teacher verifies for errors, hallucinations, grade-level fit | Students receive incorrect content |
| 6. IEP/504 compliance | Drafting accommodations | AI may suggest based on anonymized profile | Licensed specialist authorizes | Legal and clinical risk |
| 7. Parent communication | Sensitive communications | AI adjusts tone only | Teacher drafts core message | Authentic relationship replaced by generated text |
| 8. Student intervention | Academic risk flagging | AI flags patterns | Teacher designs and executes intervention | Intervention without human judgment about cause |
| 9. PCK misconception | Complex concept instruction | AI suggests analogies | Teacher selects based on this class's misconceptions | Generic instruction that misses actual barrier |
| 10. RAG walled garden | Planning with AI using curriculum materials | Only verified curriculum in the corpus | Teacher verifies source grounding | Hallucinated standards references |
| 11. Behavioral crisis | Live classroom disruption | AI excluded entirely | Teacher and staff handle | AI has no appropriate role in crisis |
| 12. Student anonymization | Any student data input to AI | PII removed before any AI interaction | Teacher anonymizes | FERPA/COPPA violation; student privacy breach |

**Key concepts:** Phase gate, AI proposes/instructor disposes, jagged technological frontier, pedagogical content knowledge (PCK), cognitive offloading, Frictional principle

**Assessment/exercise:** Phase gate mapping — for each task from the Chapter 1 workweek audit, the reader writes one sentence: "AI stops when ___. I begin when ___."

**Bridge:** The framework is established. Chapter 3 teaches the foundational skill that makes the framework usable: prompting.

---

### CHAPTER 3 — Prompting That Works: The Foundation Skill

**One-line:** Prompting is not talking to a search engine — it is task decomposition made explicit, and the teachers who do it well describe what they want, not what they feel.

**Opening case:** Two teachers use the same AI tool to generate quiz questions on the American Revolution. Teacher A types: "Generate quiz questions about the American Revolution." Teacher B types a specific prompt with grade level, standard alignment, difficulty distribution, and distractor guidance. Teacher A gets generic trivia. Teacher B gets a usable draft. The skill is in the specification.

**Learning outcomes:**
1. (Understand) Describe why prompt quality determines output quality: the AI has no context the prompt doesn't give it.
2. (Apply) Write a basic prompt using the four-component structure: role, context, task, constraints.
3. (Apply) Add grade level, subject, standard alignment, and student population detail to a prompt and compare output quality.
4. (Apply) Use iterative prompting: evaluate the first output, identify the specific gap, write a follow-up that addresses it.
5. (Analyze) Distinguish between a prompt that describes a feeling ("make this more engaging") and one that describes a specification.
6. (Create) Write prompts for three tasks from the reader's own workweek audit.

**Core content:**
- The four-component structure: role / context / task / constraints
- Why the model has no context the prompt doesn't supply
- Iterative prompting: the first output is a draft, not a product
- Grade level and subject specificity: why "for 7th grade science" produces different output
- Standard alignment in prompts
- Student population context: differentiation starts in the prompt
- Negative prompting: telling the AI what not to do
- Platform differences: Claude, ChatGPT, and Gemini/NotebookLM — practical task-based guidance, not vendor comparison
- The prompt library concept: treating good prompts as reusable assets

**Prompt structure template:**
```
ROLE: You are [specific role relevant to this task].
CONTEXT: [Grade level, subject, standard, class profile, constraints].
TASK: [Specific deliverable with format, length, and quality criteria].
CONSTRAINTS: [What to avoid, what format to use, what the output will be used for].
```

**Key concepts:** Prompt structure, role/context/task/constraints, iterative prompting, prompt library, platform-specific considerations

**Assessment/exercise:** Prompt workshop — write a prompt for a high-frequency task, evaluate the output, write a second-pass prompt addressing the specific gap, save the refined prompt as the first entry in a personal prompt library.

**Bridge:** With the framework and prompting as foundation, Part II applies both to the specific task categories where teachers spend the most time.

---

### CHAPTER 4 — Lesson Planning and Curriculum Design with AI

**One-line:** AI can generate lesson structures, activity options, and resource recommendations in seconds — the teacher's job is to bring the pedagogical content knowledge and contextual judgment the tool cannot have.

**Opening case:** A high school biology teacher who needs to design a unit on cellular respiration for a class with three ELL students, two students on IEPs, and strong chemistry background but weak biology background. She used to spend Sunday afternoons on this. She now spends forty-five minutes: fifteen generating with AI, thirty on the contextual decisions the AI cannot make.

**Learning outcomes:**
1. (Apply) Use AI to generate a lesson plan skeleton with learning objectives, activity sequence, and assessment alignment.
2. (Apply) Write a lesson planning prompt that includes grade level, subject, standards, prior knowledge context, and student population detail.
3. (Analyze) Identify which elements of an AI-generated lesson plan require teacher revision.
4. (Evaluate) Apply the lesson planning phase gate: AI generates structure; teacher retains PCK decisions.
5. (Create) Adapt an AI-generated lesson plan for a specific real class using knowledge the AI does not have.

**Core content:**
- The lesson planning task taxonomy: AI does well (structure, activity variety, resource suggestions, differentiation frameworks); AI cannot do (know this class, know student misconceptions, know what didn't work last year)
- The PCK gap: Shulman's pedagogical content knowledge means the AI has encyclopedic content knowledge but zero PCK for this classroom
- Backward design with AI: starting from the assessment and working backward
- Unit planning vs. single lesson: AI is better at unit scope and sequence than day-level plans
- Standard alignment checking: using AI to cross-reference, with teacher verification
- Differentiation in the prompt: how to ask for tiered versions in a single prompt

**Phase gate:** AI generates the structure. Teacher confirms every learning objective is achievable by this class before accepting the plan.

**Prompt templates:**
1. Single lesson plan generator
2. Unit scope and sequence generator
3. Differentiation layer generator

**Time recovery estimate:** EEF/NFER RCT data: 31% reduction in lesson preparation time under standard ChatGPT conditions; 35% under systematic prompt templates. For 8 hours/week: 2.8 hours recovered.

**Assessment/exercise:** Generate a lesson plan for an upcoming unit using the chapter's prompts, review it against PCK, make the contextual revisions, document what the AI could not supply.

**Bridge:** Lesson planning is preparation. Chapter 5 addresses the task that consumes more teacher time than any other: assessment and grading.

---

### CHAPTER 5 — Assessment, Grading, and Feedback with AI

**One-line:** AI can reduce manual grading labor by 70–85% — the teacher retains the final grade decision and the professional judgment that makes feedback pedagogically sound.

**Frictional connection:** This chapter contains the most direct application of the Bastani finding: AI feedback that students receive without teacher review may produce the performance paradox at the feedback level — students feel they received good feedback, but the lack of human calibration means the feedback doesn't connect to what they actually need to learn.

**Opening case:** A community college composition instructor who grades 270 essays per semester at 20 minutes each — 90 hours. She now uses AI for first-pass feedback and review. Her grading time dropped from 90 hours to 22 hours per semester. She spends the recovered time in office hours. Student outcomes improved.

**Learning outcomes:**
1. (Apply) Use AI to generate first-pass feedback on student work against a rubric.
2. (Apply) Write a grading prompt that includes the rubric, assignment context, and feedback format.
3. (Analyze) Apply the grading phase gate: teacher reviews every AI-drafted comment before release, adjusts for student context, retains final grade decision.
4. (Evaluate) Identify the four conditions under which AI grading assistance degrades rather than supports student learning.
5. (Create) Build a rubric calibration workflow: run AI on five samples, compare to own grades, adjust until outputs are consistently within acceptable range.

**Core content:**
- The grading task taxonomy: first-pass scoring, feedback drafting, response grouping — AI-appropriate with gates; final grade decision and communication — human-required
- The rubric calibration gate: why you never use AI grading without calibrating on sample submissions first
- The 70–85% reduction claim: source and conditions
- The feedback quality problem: AI feedback is often structurally correct but contextually wrong
- Formative vs. summative: AI is more defensibly used for formative feedback
- The Bastani parallel for feedback: feedback without teacher review can produce the fluency trap at the student level

**The four failure conditions for AI grading assistance:**
1. No rubric calibration before bulk processing
2. No teacher review of AI-drafted comments
3. Feedback released without human authorization
4. Feedback that cannot be applied by the student (too generic, wrong level)

**Phase gate:** Rubric calibration on 5 samples → teacher review of every comment → teacher authorization before release → teacher retains final grade decision.

**Prompt templates:**
1. Essay first-pass feedback generator
2. Rubric-aligned comment generator
3. Response grouping prompt for short-answer items

**Time recovery estimate:** 60% reduction in grading time. For 7.5 hours/week: 4.5 hours recovered.

**Assessment/exercise:** Run the rubric calibration workflow on five real student samples. Compare AI output to own grades. Write the follow-up prompt adjustments that bring outputs within acceptable range.

**Bridge:** Grading addresses what students produce. Chapter 6 addresses what they receive: differentiated materials and supports.

---

### CHAPTER 6 — Differentiation with AI: Reading Levels, Scaffolds, and Supports

**One-line:** AI can modify reading levels, generate scaffolded versions, and draft IEP accommodation suggestions in seconds — the teacher and specialist retain the clinical and legal judgment.

**Opening case:** A 6th-grade science teacher with 28 students reading at levels ranging from 3rd to 10th grade. Before AI: three Lexile-adjusted versions of each document — three hours per document. Now: five Lexile versions in twelve minutes. She spends the recovered time teaching the concept.

**Learning outcomes:**
1. (Apply) Use AI to adjust the reading level of a text to a specified Lexile band while preserving core content.
2. (Apply) Generate a scaffolded version of an assignment for students with specified learning needs.
3. (Apply) Write a prompt that produces vocabulary support, sentence starters, or graphic organizer templates.
4. (Analyze) Apply the differentiation phase gate: AI proposes accommodation scaffold; teacher (and licensed specialist for IEP/504) verifies and authorizes.
5. (Evaluate) Identify what AI cannot supply: knowledge of the specific student's history, behavioral and emotional context, clinical or legal requirements.

**Core content:**
- Lexile adjustment with AI: specifying the target level and what the AI can and cannot preserve
- ELL differentiation: language scaffolds, sentence frames, bilingual glossaries — AI-appropriate with teacher review
- IEP and 504 supports: AI suggests standard accommodations based on anonymized profiles; licensed specialist must authorize
- The anonymization gate: never upload student names, IDs, or identifying information to external AI tools
- Visual organizers and graphic supports: AI generation of templates
- The 28% figure: share of teachers using AI for material modification; 64% rate improvement in instructional quality

**Phase gate:** Anonymize all student information before any AI interaction. AI suggests; licensed specialist (for IEP/504) or teacher (for general differentiation) authorizes.

**Prompt templates:**
1. Lexile adjustment prompt (specify target level)
2. Scaffolded assignment generator (specify learning need)
3. Vocabulary support generator

**Time recovery estimate:** 60% reduction in differentiation preparation. For 3.5 hours/week: 2.1 hours recovered.

**Assessment/exercise:** Select one text or assignment from the current unit, run the Lexile adjustment prompt to produce three versions, review each for content accuracy, document the teacher judgment decisions the AI could not make.

**Bridge:** Differentiation addresses what students receive. Chapter 7 addresses what the teacher communicates outward.

---

### CHAPTER 7 — Communication with AI: Parents, Admin, and Documentation

**One-line:** AI can draft parent communications, behavioral reports, meeting summaries, and administrative documents from rough notes — the teacher reviews the tone, retains the core message, and sends.

**Opening case:** A middle school teacher with 150 students. Progress reports four times per year. 600 comments per year. Manually: 72 hours per year. With AI: 16 hours per year. She spent 56 hours in parent conferences instead of writing comments.

**Learning outcomes:**
1. (Apply) Use AI to draft a parent communication from rough bullet notes, specifying tone and relationship context.
2. (Apply) Use AI to produce a meeting summary or action items document from rough notes.
3. (Apply) Write a prompt for a behavioral report including factual record, family tone, and documentation format.
4. (Analyze) Apply the communication phase gate: routine communications — AI drafts, teacher reviews and sends; sensitive communications — teacher drafts core message, AI adjusts tone only.
5. (Evaluate) Identify the communications AI should not draft: those where the teacher's authentic relationship is the primary value.

**Core content:**
- Communication task taxonomy: routine (newsletters, progress updates) — AI-appropriate with light review; sensitive (behavioral concerns, academic struggles, family conflict) — teacher drafts core message
- The tone adjustment use case: AI excels at converting rough notes into polished professional prose
- Translation: AI for multilingual parent communications, with accuracy verification caveat
- Administrative documentation: meeting notes, compliance forms, incident reports
- The sensitive communication gate: teacher must draft the core narrative for any communication with legal, behavioral, or family-conflict implications

**Phase gate:** Classify communication type before generating. Sensitive communications: teacher writes core message first. All communications: teacher reviews tone and authorizes before sending.

**Prompt templates:**
1. Parent progress note generator (from teacher bullet notes)
2. Meeting summary generator (from rough notes)
3. Newsletter/announcement generator

**Time recovery estimate:** 50% reduction in administrative communication time. For 5 hours/week: 2.5 hours recovered.

**Assessment/exercise:** Select three parent communications from a recent week, draft bullet notes for each, generate AI drafts, evaluate which are acceptable with minor review vs. which required substantial revision. What does the pattern reveal about phase gate placement?

**Bridge:** Chapters 4–7 address text-based tasks. Chapters 8 and 9 address visual output.

---

### CHAPTER 8 — Making Slides with AI

**One-line:** AI can generate slide content and structure; the teacher needs a working vocabulary for what makes a slide teach rather than merely display — without that vocabulary, AI defaults produce slides that look professional and communicate nothing.

**Opening case:** The 11:42 p.m. problem. The deck is forty-three slides. Slide twelve has a paragraph from the textbook with one word bolded. Slide nineteen has a five-color bar chart of three categorical variables. Slide twenty-seven has a stock photo of a stethoscope for reasons the teacher cannot reconstruct. The slides look professional. They look done. They look wrong. Two hours later the deck is no better. The problem is not AI. The problem is the absence of a vocabulary for what is wrong.

**Learning outcomes:**
1. (Understand) Describe the slideument problem: a slide that tries to be both speaker's anchor and self-contained document fails at both.
2. (Apply) Distinguish between a claim headline and a topic label, and rewrite a topic label as a claim.
3. (Apply) Write a slide generation prompt that specifies: headline as assertion, body as visual evidence, notes field as speaker explanation.
4. (Analyze) Apply the Mayer Redundancy Principle: text on a slide that duplicates the speaker's narration degrades learning.
5. (Evaluate) Run the five-question diagnostic on any deck in under five minutes.
6. (Create) Iterate on an AI-generated deck using targeted follow-up prompts that name the specific failure and the specific fix.

**Core content:**
- The slideument problem (Garr Reynolds): the slide that tries to be both speaker's anchor and study document
- Mayer's Redundancy Principle: verbal channel collision degrades learning
- The assertion headline vs. the topic label
- Visual hierarchy: size ratios for projection readability (2:1 minimum at projection distance)
- The three text-density failure modes: redundancy (move to notes), seductive detail (cut), density (segment)
- The wrong visual form: when bullets are a list pretending to be a comparison
- Color encoding: two colors doing real work vs. six doing nothing
- The textbook figure problem: designed for 14-inch reading, placed in a 50-foot projection environment
- The five-question diagnostic (30 seconds per slide):
  1. Is the headline a claim or a topic label?
  2. Would this slide teach the content without a speaker?
  3. Is there a sentence on this slide I'm about to say aloud?
  4. Does the visual form match the content structure?
  5. Is every color encoding something?

**Phase gate:** Teacher runs the five-question diagnostic before accepting any AI-generated deck as final.

**Prompt templates:**
1. Slide revision prompt (slideument → speaker's anchor)
2. Assertion headline rewriter
3. Full deck diagnostic prompt

**Note:** This chapter draws on the Brutalist slide design framework. Teachers who want the complete treatment should see *How to Build Slides That Teach* (bearbrown.co/brutalist).

**Assessment/exercise:** Select a ten-slide deck currently in use, run the five-question diagnostic, identify the three highest-priority failures, write targeted follow-up prompts to address each.

**Bridge:** Slides communicate to rooms. Chapter 9 addresses a different visual problem: communicating data honestly.

---

### CHAPTER 9 — Making Graphs and Data Visualizations with AI

**One-line:** Teachers sit on assessment data they cannot use because they cannot visualize it — AI can produce publication-quality charts from plain-language descriptions, but the teacher must know what kind of chart their question requires.

**Opening case:** A department chair with three years of student performance data by teacher, by unit, and by demographic group. She knows the data contains a story about which students are being left behind and when. She cannot see the story. She has Excel. She does not have time to learn D3. She has a class of students today.

**Learning outcomes:**
1. (Understand) Identify the five functional categories most useful for teacher data: comparison, change over time, distribution, relationship, part-to-whole.
2. (Apply) Write a plain-language chart request prompt that specifies: what the chart is trying to show, what the data contains, and what the reader needs to understand in five seconds.
3. (Apply) Identify the three most common chart errors in education data: truncated y-axes, overcrowded pie charts, line charts connecting unrelated categories.
4. (Analyze) Apply Cairo's "compared with what?" check: every quantitative claim requires an explicit reference.
5. (Evaluate) Run the proportional ink check and the honest title check.
6. (Create) Produce a chart of real assessment data using the AI prompting workflow.

**Core content:**
- The five functional categories for teacher data
- The chart selection question: what does the reader need to understand in five seconds?
- Cairo's "compared with what?" check applied to education data
- The truncated y-axis problem: assessment score charts with y-axes starting at 60 systematically overstate differences
- Pie chart limits: five categories maximum; sorted bar chart communicates more accurately
- Distribution charts for teachers: what a box plot shows vs. what a bar chart of means hides (connects to Bastani — mean scores hide distributions that reveal who is being left behind)
- The five-question chart checklist:
  1. What question does this chart answer?
  2. What is the reader being asked to compare this to?
  3. Does the y-axis start at zero for a bar chart?
  4. Can the reader read the ranking in five seconds?
  5. Does the title state the finding, not just the subject?

**Phase gate:** Teacher runs the five-question checklist before using any AI-generated chart in a presentation or report.

**Prompt templates:**
1. Chart type selector (describe data, get recommendation)
2. Bar chart generator from grade data
3. Trend chart for attendance or assessment over time

**Assessment/exercise:** Select one set of assessment data from the current semester, write a chart request prompt using the functional category framework, generate a chart, run the checklist, write one sentence describing what the chart reveals about student learning.

**Bridge:** Part II covers the six core task areas. Part III extends into writing and coding, then addresses implementation and integrity.

---

### CHAPTER 10 — Writing with AI: An Introduction

**One-line:** AI changes writing instruction and teacher writing workflows in ways that are both powerful and pedagogically dangerous — this chapter maps the terrain; the full treatment is in the $1 companion *Writing with AI*.

**Opening case:** An English teacher who uses AI to draft her own syllabi, assignment descriptions, and department communications — saving roughly two hours per week — while simultaneously watching students use the same tool to produce essays they cannot discuss or defend. Same tool. Opposite uses. The chapter distinguishes them.

**Learning outcomes:**
1. (Understand) Distinguish teacher writing (AI reduces workload) from writing instruction (AI changes what must be taught).
2. (Apply) Use AI to draft professional writing from rough notes.
3. (Analyze) Identify three ways AI changes the goals of writing instruction: from product to process, from first draft to revision, from submission to conversation.
4. (Evaluate) Assess a writing assignment for AI-survivability.
5. (Apply) Use three instructional prompting strategies: Socratic AI, feedback AI, elaboration AI.

**Core content:**
- Teacher writing workflows: professional writing AI can assist with vs. writing AI should not replace
- The Bastani 2025 parallel for writing: students who produce essays without doing the drafting gain fluency-confidence without learning
- AI-survivable assignment design: assignments that require the student to do cognitive work AI cannot do
- The three instructional uses: Socratic AI (asks questions instead of answering), feedback AI (responds to drafts), elaboration AI (asks student to explain their own claims)
- What writing instruction must now teach: revision as the primary skill, argument defense as assessment mode

**Phase gate:** Teacher writing workflows — AI drafts, teacher reviews and sends. Writing instruction — AI plays the Socratic, feedback, or elaboration role; student does the cognitive work.

**Prompt templates:**
1. Syllabus draft from bullet notes
2. Assignment description generator
3. Socratic writing coach prompt

**$1 Kindle Companion:** *Writing with AI* (Bear Brown & Company) — full treatment of writing instruction redesign, AI-survivable curriculum, academic integrity in writing courses, and using AI as a writing tool in the classroom.

**Bridge:** Writing is language-based. Chapter 11 addresses the computational side.

---

### CHAPTER 11 — Coding with AI: An Introduction

**One-line:** AI can write code — which means every teacher can now automate their own workflows, create interactive materials, and teach computational thinking differently than before.

**Opening case:** A high school math teacher who does not code. She has always wanted an interactive visualization of polynomial functions — the kind where you drag a coefficient and watch the graph change. Three hours with an AI coding assistant. She now has a working web page. She did not write a single line of code. She wrote specifications.

**Learning outcomes:**
1. (Understand) Describe what coding with AI means for non-programmers: the teacher writes the specification, AI writes the code, teacher verifies the output.
2. (Apply) Write a specification prompt for a simple teacher workflow automation.
3. (Apply) Write a specification prompt for a simple interactive educational tool.
4. (Analyze) Identify the verification responsibility: teacher tests output against specification, not code.
5. (Evaluate) Apply the accountability principle: teacher is responsible for the tool's behavior with students regardless of who wrote the code.

**Core content:**
- Specification as the skill, not syntax
- Three categories of teacher workflow automation: spreadsheet processing, grade management, communication tools
- The specification prompt: what to include
- Verification without code literacy: testing against specification, edge cases, privacy
- Educational tool creation: interactive visualizations, simple games, assessment generators
- The accountability principle: a teacher who deploys an AI-built tool bears responsibility for that tool's behavior

**Phase gate:** AI generates → teacher tests against specification including edge cases and privacy check → teacher decides to deploy.

**Prompt templates:**
1. Workflow automation specification prompt
2. Interactive tool specification prompt

**$1 Kindle Companion:** *Coding with AI* (Bear Brown & Company) — full treatment of computational thinking instruction, redesigning CS curricula around AI-assisted coding, and technical workflow automation at scale.

**Bridge:** With the six core task areas covered and the two extended domains introduced, Chapter 12 addresses putting it all together.

---

### CHAPTER 12 — Building Your AI Workflow: Monday Morning to End of Year

**One-line:** The teachers who get the most from AI are not the most technically sophisticated — they are the most systematic; this chapter builds the system.

**Opening case:** Two teachers at the same school. Both use AI. Teacher A: opportunistic, ~2 hours/week savings. Teacher B: systematic, ~12 hours/week savings. Same tools. Different systems.

**Learning outcomes:**
1. (Apply) Build a personal prompt library organized by task type.
2. (Apply) Design a weekly AI workflow with AI-assisted versions of each task category and the correct phase gate named for each.
3. (Apply) Identify the three highest-value AI opportunities and build one systematic workflow for each.
4. (Analyze) Distinguish ad hoc AI use (~6 hours/week savings) from systematic AI use (higher ceiling).
5. (Evaluate) Assess a personal AI workflow against the phase gate map from Chapter 2.

**Core content:**
- The prompt library: how to build, organize, and maintain it
- The weekly workflow design: matching task categories to AI tools
- The total time recovery model: adding up per-task savings from Chapters 4–9
- The adoption curve: why most teachers plateau at ad hoc use
- Platform strategy: Claude (writing and reasoning), Gemini/NotebookLM (document-grounded tasks), specialized tools (grading, slides)
- The 68% gap: share of teachers receiving no formal AI training; what this book substitutes for
- Maintenance: prompts that worked six months ago may not work today

**The personal AI workflow document (chapter deliverable):**
- Prompt library starter (10 prompts minimum)
- Weekly task schedule with AI-assisted versions identified
- Phase gate map
- Platform assignments

**Assessment/exercise:** Build the personal AI workflow document with all four components.

**Bridge:** A working system is in place. Chapter 13 addresses the hardest questions about running it honestly.

---

### CHAPTER 13 — Academic Integrity, Privacy, and Honest Use

**One-line:** Academic integrity with AI is not about catching students — it is about designing learning environments where cognitive struggle produces learning rather than where AI eliminates the struggle before learning can happen.

**Frictional connection:** This chapter is the most direct application of the Preface's argument. The Bastani finding is presented in full. The response is not detection — it is design. AI-survivable assignments protect the learning mechanism the Frictional framework describes.

**Opening case:** A professor who designed an AI-detection workflow. By the end of the semester she has referred 23% of students for academic integrity review. She is exhausted. Three students contest their referrals. The appeals process takes four weeks. She teaches less. Her students learn less. She solved the wrong problem.

**Learning outcomes:**
1. (Understand) Describe the Bastani 2025 finding in full: the performance paradox, the illusion of competence, and why cognitive struggle is the learning mechanism.
2. (Apply) Redesign one assessment using the AI-survivable assignment framework.
3. (Analyze) Evaluate AI detection tools: accuracy rates, false positive rates, discriminatory patterns against ELL students and non-native writers.
4. (Evaluate) Apply the privacy checklist: FERPA and COPPA implications for student data and AI tools.
5. (Create) Draft a student AI use policy that is specific, enforceable, and pedagogically motivated.

**Core content:**
- The Bastani 2025 finding in full: why detection and prohibition are not the right response
- The AI-survivable assignment framework: assignments requiring defended reasoning, novel application, process documentation, or real-time performance
- AI detection tools: accuracy limitations, false positive rates (up to 30% in some studies), documented bias against ELL students and non-native writers, legal risk of false positives
- FERPA and COPPA in the AI context: what PII cannot be submitted to external tools
- The student AI policy design: what effective policies specify beyond prohibition
- The equity dimension: differential access to AI tools; policies must account for this
- The teacher transparency question: what teachers should tell students about their own AI use

**The AI-survivable assignment checklist:**
1. Does the assignment require the student to defend claims in conversation?
2. Does the assignment require applying concepts to a situation that didn't exist when AI was trained?
3. Does the assignment require process documentation (drafts, annotations, decision records)?
4. Does the assignment require real-time unassisted performance?
5. If a student used AI freely and produced a good artifact, would you know whether they learned anything?

**Assessment/exercise:** Write a student AI use policy for one course using the chapter's framework. Evaluate against three criteria: specific, enforceable, pedagogically motivated.

**Bridge:** Chapter 13 addressed what teachers tell students about AI in the classroom. Chapter 14 addresses what teachers teach students about using AI themselves.

---

### CHAPTER 14 — What to Tell Your Students: AI Literacy in the Classroom

**One-line:** Students already use AI — the question is whether they use it to do work or to learn, and teachers are the only people positioned to teach the difference.

**Opening case:** The high schoolers who reached out. Their message was precise: "My friends are using AI to write their papers but I want to use AI to learn and I don't know how." This is the question Chapter 14 answers. Not for the students who want to avoid the work — for the students who want to do it better.

**Frictional connection:** This is the student-facing application of the Frictional argument. Capability-building vs. capability-borrowing maps directly to learning that leaves friction traces vs. borrowing that leaves none.

**Learning outcomes:**
1. (Understand) Describe the capability-building vs. capability-borrowing distinction for students.
2. (Apply) Explain the Bastani finding to students in plain language: why the students who used AI freely during practice scored lower on the unassisted exam.
3. (Apply) Teach three capability-building AI uses: Socratic questioning, deliberate practice generation, the Feynman test.
4. (Analyze) Help students identify capability-borrowing uses to avoid.
5. (Create) Design one classroom activity that demonstrates the performance paradox to students experientially.

**Core content:**
- The capability-building vs. capability-borrowing framework for students
- The Bastani finding in plain language
- The Feynman test: if you cannot explain it without AI, you do not know it yet
- Three capability-building uses: Socratic questioning, deliberate practice generation, Feynman test conversation
- The fluency trap: why smooth AI output produces false confidence
- The storage vs. retrieval distinction for students: retrieval practice builds durable memory; AI retrieving for you eliminates the practice
- The performance paradox demonstration activity: students complete a problem set with AI, test themselves without AI, see their own results
- Age-appropriate versions: K–8, 9–12, higher education

**The capability-building vs. capability-borrowing distinction:**

| AI use | Type | What it does to learning |
|--------|------|------------------------|
| Ask AI to challenge your reasoning | Capability-building | Triggers prediction error; builds the model |
| Ask AI to generate problems at the edge of your competence | Capability-building | Creates productive struggle; drives consolidation |
| Ask AI to identify gaps in your explanation (Feynman test) | Capability-building | Forces retrieval; reveals what's missing |
| Ask AI to write the first draft | Capability-borrowing | Bypasses the generative struggle that builds schema |
| Ask AI to summarize the reading | Capability-borrowing | Bypasses the deep processing that produces comprehension |
| Ask AI to solve the problem | Capability-borrowing | Eliminates the productive difficulty that constitutes learning |

**Assessment/exercise:** Design a classroom activity (20–30 minutes) that demonstrates the performance paradox. Includes a self-reflection prompt asking students to identify one AI use they currently rely on that may be borrowing rather than building capability.

---

## Conclusion — The Research Agenda and What Comes Next

**One-line:** 6 hours is the research finding; the question this book is designed to help answer is what happens when teachers implement the framework systematically.

**Content:**
- What the research says now: the 5.9-hour finding, the 16.7-hour projection, the conditions under which the projection holds
- What Medhavy is measuring: the Genuine Learning Probability framework, adaptive testing, what systematic data collection on AI-assisted teaching might eventually show
- The honest 20-hour hypothesis: personal experience with well-implemented tools is a hypothesis, not a finding; this is the research agenda
- What teachers can do with a finding vs. a hypothesis: act on the 6-hour finding now; treat the ceiling as a reason to implement systematically and see what your data shows
- The practitioner's research role: teachers who implement systematically and document outcomes are contributing to the evidence base

---

## Appendices

---

### Appendix A — The Full Phase Gate Map

All 12 phase gates from Chapter 2 in operational terms: trigger condition, AI boundary, human authorization step, and the consequences of skipping the gate. One-page reference, ready to post above a workstation.

---

### Appendix B — Prompt Library Starter (50 Prompts)

50 copy-paste-ready prompts organized by task category:
- Lesson planning (8 prompts)
- Grading and feedback (8 prompts)
- Differentiation (8 prompts)
- Parent and administrative communication (7 prompts)
- Slides (7 prompts)
- Data visualization (6 prompts)
- Writing support (3 prompts)
- Coding specification (3 prompts)

Each prompt annotated: what it does well, what context the teacher must supply, and what to watch for in the output.

---

### Appendix C — The Diagnostic Checklists

Three one-page checklists:

**The Slide Diagnostic (5 questions, 30 seconds per slide)**
1. Is the headline a claim or a topic label?
2. Would this slide teach without a speaker?
3. Is there a sentence on this slide I'm about to say aloud?
4. Does the visual form match the content structure?
5. Is every color encoding something?

**The Chart Honesty Checklist (5 questions, 30 seconds per chart)**
1. What question does this chart answer?
2. What is the reader being asked to compare this to?
3. Does the y-axis start at zero for a bar chart?
4. Can the reader read the ranking in five seconds?
5. Does the title state the finding?

**The Assignment AI-Survivability Checklist (5 questions, 5 minutes per assignment)**
1. Does it require defending claims in conversation?
2. Does it require applying concepts to a novel situation?
3. Does it require process documentation?
4. Does it require real-time unassisted performance?
5. If a student used AI freely and produced a good artifact, would you know whether they learned anything?

---

### Appendix D — Research Reference

Key studies the book cites, each with a plain-language summary:

- **Gallup-Walton Family Foundation (2024):** Teacher time savings — 5.9 hours/week for ad hoc users. n=2,232 public school teachers. What the conditions were for the finding.
- **Bastani et al. (2025), PNAS:** The performance paradox. n=~1,000 Turkish high school students. The GPT Base condition (48% practice gain, 17-point exam loss) and the GPT Tutor condition (127% practice gain, mitigated loss). What the conditions were for each.
- **NFER/EEF Teacher Choices RCT (2024):** Lesson preparation time reduction — 31% under standard ChatGPT conditions. n=259 secondary science teachers across 68 schools. What the conditions were.
- **Hattie meta-analyses:** Teacher-student relationship effect size (d=0.72), collective teacher efficacy (d=1.57). What these numbers mean and how to interpret them.
- **Sadler et al.:** Pedagogical content knowledge and misconception research. Why teachers need both subject-matter knowledge and knowledge of student misconceptions — the two are not substitutable.
- **Kosmyna et al. (2025), MIT Media Lab:** EEG evidence of reduced neural connectivity during AI-assisted writing. What the finding shows about the Frictional argument.

---

### Appendix E — Series Map

How this book connects to the other publications in the series:

| Publication | What it covers | Who it's for |
|-------------|---------------|--------------|
| *AI for Teachers: A Practitioner's Guide* (this book) | The full framework — all 14 task areas, phase gates, workflow | All teachers |
| *Writing with AI* ($1 Kindle) | Full treatment of writing instruction and teacher writing workflows | English teachers, writing instructors, humanities faculty |
| *Coding with AI* ($1 Kindle) | Full treatment of computational thinking and coding workflows | CS teachers, tech-adjacent educators, teachers interested in automation |
| *How to Learn with AI: A Student's Guide* | The student-facing companion — capability-building uses, the Feynman test, AI-survivable learning | Students, teachers who want to teach AI literacy |
| *Frictional* (academic paper) | The full theoretical framework: GLP, the seven friction trace components, ensemble architecture | Researchers, institutional assessment designers, graduate students |

---

### Appendix F — The AI Teaching Assistant (Deployable Claude Project)

A single master system prompt that operationalizes the full book's framework as a phase-gated AI assistant.

**How to deploy:**
1. Go to claude.ai and create a new Project
2. Name it "AI Teaching Assistant"
3. Paste the system prompt from this appendix into the Project Instructions field
4. The tool opens with a welcome menu and command reference

**What the tool knows:** All 12 phase gates from Chapter 2. The 6-hour research finding. The Bastani warning. The anonymization requirement. The four-component prompt structure. Platform-specific guidance. The slide diagnostic. The chart checklist. The assignment survivability checklist.

**Task modes (commands):**
```
/lesson        — Lesson planning with phase gates
/grade         — Grading and feedback workflow with calibration gate
/differentiate — Lexile, scaffolds, supports with anonymization gate
/communicate   — Parent and admin communications with sensitivity gate
/slides        — Slide diagnostic and generation with assertion gate
/chart         — Data visualization with Cairo check
/workflow      — Weekly workflow builder with prompt library
/policy        — Student AI use policy designer
/help          — Full command reference
```

**Silent mode:** Append `silent` to any command for immediate clean output with no phase gates. Use when you know exactly what you need.

**Interactive mode (default):** All phase gates active. The tool pushes back on thin input. Will not generate lesson plans from "7th grade science." Will not process bulk grading without calibration. Will not output student materials that skip the anonymization gate.

[Full system prompt follows — see Appendix F in the complete book]

---

### Appendix G — Frictional: The Full Framework

The theoretical foundation beneath the book's practical recommendations.

**What this appendix covers:**
- The neurobiological basis of friction traces: dopamine prediction error signaling, BDNF upregulation, dendritic spine formation
- The Bjorkian insight: storage strength vs. retrieval strength, and why the fluency trap produces false confidence
- The seven GLP components: temporal engagement pattern, error trajectory coherence, cross-context transfer, uncertainty calibration, social knowledge texture, retrieval strength decay signature, scaffolding response curve
- Why the composite score is harder to fake than any individual component
- The ensemble architecture: component models → tier-conditioned combination → meta-model
- The instructor as meta-model: how professional judgment combines with formal measurement
- The ethics of process observation: what distinguishes learning support from surveillance

**For further reading:**
Brown, N.B. (2026). *Frictional: Measuring the Struggle: Process Friction Traces as Independent Evidence of Genuine Learning in the Age of Generative AI.* Preprint at irreduciblyhuman.com.

[Full appendix text follows — see Appendix G in the complete book]

---

## Adoption Risk Register

| # | Risk | Likelihood | Impact | Mitigation |
|---|------|-----------|--------|------------|
| 1 | Tool-specific content ages rapidly | High | Medium | Platform guidance is task-based, not tool-specific; update annually |
| 2 | 6-hour finding superseded by better data | Medium | Low | Book uses "at least 6 hours" framing; ceiling claims are explicitly projected |
| 3 | Frictional framework contested | Medium | Medium | Book presents practical framework; Appendix G presents theoretical version; each stands independently |
| 4 | $1 Kindle companions not yet published | Medium | Low | Chapters 10 and 11 are self-contained introductions; companions are extensions |
| 5 | Appendix F tool requires Claude account | Medium | Medium | Tool is optional; all chapter content works without it |
| 6 | LLM prompt behavior changes | High | Medium | Prompt templates designed for structure, not platform quirks; resilient to model updates |
| 7 | Academic integrity section outdated | High | Medium | Chapter 13 focuses on design principles, not specific detection tools |

---

## Open Questions

| # | Question | Stakes | Decision deadline |
|---|---------|--------|------------------|
| 1 | Does Appendix F ship as a book appendix, a separate document at bearbrown.co, or both? | Production planning | Before manuscript |
| 2 | Are the $1 Kindle companions published before or after the main book? | Series sequencing | Before proposal |
| 3 | Which research claims need institutional review board language? | Academic credibility | Before manuscript |
| 4 | Does the book include a foreword from Richard Culatta (ISTE) given that relationship? | Market positioning | Before proposal |
| 5 | How does the book handle platform-specific content that will age? (Update policy?) | Evergreen design | Before proposal |

---

*TIKTOC v2.0 — Full Architecture · Pre-draft / Research phase*
*All chapters specified with sufficient detail for research note generation*
*Preface, all 14 chapters, conclusion, and 7 appendices documented*
*No chapter prose written — research phase precedes drafting*
