# Chapter 12 — Building Your AI Workflow: Monday Morning to End of Year

<!-- FACT-CHECK FLAG: UNVERIFIED — see factchecks/12-building-your-ai-workflow-assertions.md -->

**TL;DR.** Two teachers in the same building with the same tools can end the year hours apart, and the gap is not skill but system — a small captured prompt library plugged into a fixed weekly schedule, each slot named for one task, one tool, and one phase gate. This chapter is how you build that system, the honest limits of what the research currently shows, and the maintenance habit that keeps it from rotting.

---

## Learning objectives

By the end of this chapter, you should be able to:

1. **Apply.** Build a personal prompt library organized by task type, with at least ten captured entries drawn from the recurring tasks in Chapters 4–9.
2. **Apply.** Design a weekly AI workflow that matches each AI-assisted task to a tool, a fixed time block, a library entry, and the correct phase-gate move from Chapter 2.
3. **Apply.** Identify the three highest-value AI opportunities in your own week and build one systematic workflow for each.
4. **Analyze.** Distinguish ad hoc AI use (around six hours per week recovered, on average, among weekly users in the Gallup-Walton 2025 survey) from systematic use (a higher, but contested, ceiling) — and name what the available evidence does and does not show.
5. **Evaluate.** Assess a personal AI workflow against the phase-gate map from Chapter 2 and against a six-month maintenance protocol.

---

## 1. Opening case — two teachers, same building, ten hours apart

*This case is composite-illustrative. The two teachers are not specific documented individuals. The ~2 hr and ~12 hr per-week figures are plausible upper-tail observations consistent with the Gallup-Walton 2025 mean of 5.9 hours saved per week among weekly users ([Walton Family Foundation summary](https://www.waltonfamilyfoundation.org/six-weeks-giving-teachers-time-back-with-ai); [RAND landing — Gallup Teacher Workload and AI Survey, Spring 2025](https://www.rand.org/education-employment-infrastructure/survey-panels/aep/surveys/items/gallup-teacher-workload-and-ai-survey-spring-2025.html)). The distribution behind the 5.9 hr mean has not, as of writing, been published in percentile form. [verify against any future Gallup-Walton distributional release.] The figures are illustrative, not separately measured medians.*

It is 7:14 on a Friday evening in February. Two teachers leave the same public high school carrying the same set of obligations into the weekend — five preps, two sections of an honors class, an IEP meeting Monday at 7:30, progress reports due Wednesday, a department curriculum-revision document waiting in a shared drive. Call them Teacher A and Teacher B. Same district. Same school. Same students walking past in the hallway. Same paid subscription to one general-purpose AI tool.

Teacher A drives home and does what she has been doing since October. She uses AI. She does not have a system. When a task surfaces — *I should generate a discussion-question set for Monday* — she opens the chatbot, types something like *"give me discussion questions for Animal Farm chapter 7,"* skims the output, lifts what she likes, closes the tab. The prompt is gone. Next week, when she needs discussion questions for chapter 8, she opens the chatbot and types something similar from scratch. The tool helps. The output is fine. Across the week she estimates two hours saved compared to last year, maybe a little more. Across the year, that is the lower edge of what the Gallup-Walton survey would call a weekly user.

Teacher B drives home and opens a single document on her laptop. It is twelve pages, organized into six sections, named *workflow.md*. The first section is a list of ten captured prompts, each labeled by task — *lesson skeleton, rubric-aligned feedback, Lexile pass, parent note from bullets, slide rewrite, attendance chart.* Each prompt has a header that names the role she wants the model to play, the variable slots she fills in each time, and a one-line note that says *last verified Jan 14.* The second section is her week, laid out hour by hour — fixed commitments first, then four named time blocks where she runs prompts from the library. The third section is a one-line phase-gate move for each block — *"I review every rubric-aligned comment before any score releases"; "I anonymize before any student data goes near the model."* Across the week she estimates twelve hours saved compared to last year. She has been doing this since August.

Both teachers use the same tool. Teacher A is using it as a chatbot. Teacher B is using it as the back half of a system whose front half is a document she wrote and a calendar she keeps. The gap is not skill. It is not personality. It is what was captured and what was scheduled.

We have to be careful here. The honest reading is that *some* of the gap between Teacher A and Teacher B is selection effect — the kind of teacher who builds a *workflow.md* is also the kind of teacher who would have stayed organized without AI. The Gallup-Walton survey is observational; it cannot separate the two ([CRPE — *The AI Dividend* commentary](https://crpe.substack.com/p/the-ai-dividenddoes-ai-create-more); [Chalkdust & Silicon — context on the Walton/Gallup figures](https://medium.com/chalkdust-silicon/the-walton-gallup-ai-report-deserves-context-not-just-headlines-56164a7303a3)). What it can tell us is that the systematic pattern is associated with the higher savings. Whether you, specifically, will go from two hours saved to twelve by installing the system is a hypothesis you will test in your own week. The remainder of this chapter is how to run that test honestly.

---

## 2. The core concept — systematic beats ad hoc, and why

The headline finding behind this chapter is one number. Across the Gallup-Walton Family Foundation *Teaching for Tomorrow* survey (March–April 2025, n = 2,232 U.S. public K-12 teachers), teachers who used AI weekly reported saving an average of **5.9 hours per week** — about six weeks across the school year ([Gallup release, September 2025](https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx); [Walton Family Foundation summary](https://www.waltonfamilyfoundation.org/six-weeks-giving-teachers-time-back-with-ai)). Only 32% of teachers used AI weekly; another 28% used it infrequently; 40% did not use it at all. The 5.9 hours is the mean among the weekly users. It is the floor of what the chapter is teaching you to chase, not the ceiling.

### 2.1 Selection effect vs. treatment effect — the part we cannot yet settle

Before we build anything, name the limit of the evidence.

Two readings of the 5.9-hour finding live side by side and the published survey cannot distinguish them.

*The selection-effect reading.* Teachers who become weekly AI users are the kind of teacher who would already be saving time — well-organized, motivated, comfortable with new tools. The AI is correlated with the savings, not causing them. A less-organized teacher dropped into the same tool would not see the same recovery.

*The treatment-effect reading.* The systematic use — the captured prompts, the recurring schedule, the phase gates — produces the savings, and any teacher who installs the system could see a similar pattern.

The Gallup-Walton design is observational. It surveys teachers, asks them what they do, asks them what they save. It does not randomly assign teachers to systematic-workflow training versus tool-access-only and measure the difference. No published study has done that, as of the chapter's writing. The Center on Reinventing Public Education has been the most public voice on this — pointing out that the headline number conflates *the tool works* with *the tool works for the kind of teacher already inclined to use it.* [contested]

I want you to hold this honestly. The system I am about to teach you is **a credible hypothesis you can test in your own week**, not a guaranteed dose-response curve. If after six weeks of installing the workflow your saved time has not moved, the system did not work for you and you should reorganize or stop. If your saved time *has* moved, you have your own data point — which is the only data point that finally answers the question for your week.

### 2.2 The prompt library as personal knowledge asset

Here is the mechanical heart of the chapter.

When a teacher uses AI ad hoc, every use is a fresh decision. *What should I ask? In what order? In what voice? With what guardrails?* The teacher writes the prompt, evaluates the output, takes what she needs, and closes the tab. The prompt is gone. The next time the same task surfaces, she starts over.

When a teacher uses AI systematically, the prompts that *worked* get captured. Each captured prompt is a small piece of codified knowledge — what Davenport and Prusak, in their canonical treatment of organizational knowledge management, called the move from *tacit* knowledge (what one person knows how to do) to *explicit* knowledge (a documented procedure that can be transferred, reused, and improved) ([Davenport & Prusak (1998). *Working Knowledge: How Organizations Manage What They Know.* HBS Press](https://store.hbr.org/product/working-knowledge-how-organizations-manage-what-they-know/3014)). Their caution applies: "Knowledge works across networks and communities," and the library is a tool, not a goal. The goal is that you do not start from scratch next Tuesday.

A captured prompt is not the same thing as a screenshot of the chat. A library has four operational properties — without them, you have a junk drawer:

1. **Organized.** Grouped by recurring task — lesson planning, feedback, differentiation, communication, slides, charts.
2. **Named.** Each entry has a one-line task label so future-you can find it in under fifteen seconds.
3. **Parameterized.** The per-instance variables (this week's unit, this student's level, this parent's situation) are explicit slots, not buried in prose. A prompt with `[GRADE LEVEL]`, `[STANDARD]`, and `[CLASS PROFILE]` slots is reusable; a prompt that bakes "7th grade life science" into the body is single-use.
4. **Maintained.** Entries that stop working get revised or retired (Section 2.6).

The Template Pattern from Chapter 3 — role, context, task, format, constraints — is the skeleton for each entry. The library is what happens when you stop letting good prompts disappear.

### 2.3 The weekly workflow — schedule is the other half

A library without a schedule sits unused. A schedule without a library makes you write prompts from scratch inside the time block. Both halves are required.

The pattern across the teacher time-blocking literature is straightforward: fixed commitments first (classes, duty, meetings), then dedicated blocks for the work that benefits from concentration, then buffer time for the residual ([Stanford CTL — Weekly Planning: Time Blocking Method](https://ctl.stanford.edu/weekly-planning-time-blocking-method); [Truth for Teachers — Time blocking](https://truthforteachers.com/truth-for-teachers-podcast/time-blocking-for-teachers-align-your-priorities-energy-and-tasks-to-create-a-sustainable-schedule/)). This literature is largely craft and self-help — Cal Newport's *Deep Work* (Grand Central, 2016) is the most-cited synthesis — and the claims about exact attention-percentage gains from time blocking should be read as plausible operational scaffolding, not measured effects. [contested]

The AI-specific move is to pair each block with a **task → tool → library entry → phase gate** quadruple. Not *"open Claude and see what happens,"* but *"Sunday 4–6 p.m., lesson planning for the week, Claude, library entry #1 (lesson-skeleton prompt), phase gate: I verify every learning objective is achievable by this class before I accept the plan."* The pairing is what turns a vague block of "AI work" into a recoverable hour.

### 2.4 Why the schedule beats willpower — Wood and Neal on habits

There is a deeper reason to schedule. Wendy Wood and David Neal's program of work on habit psychology — the canonical synthesis is their 2007 *Psychological Review* paper and the 2016 *Annual Review of Psychology* review — finds that habits are **context-cued behavior chunks**: once a behavior has been performed often enough in a recurring context, the *context* itself triggers the behavior, with limited conscious mediation by the current goal ([Wood & Neal (2007). "A New Look at Habits and the Habit-Goal Interface." *Psychological Review* 114(4): 843–863](https://dornsife.usc.edu/wendy-wood/wp-content/uploads/sites/183/2023/10/wood.neal_.2007psychrev_a_new_look_at_habits_and_the_interface_between_habits_and_goals.pdf); [Wood & Rünger (2016). "Psychology of Habit." *Annual Review of Psychology* 67: 289–314](https://dornsife.usc.edu/wendy-wood/wp-content/uploads/sites/183/2023/10/wood.runger.2016.pdf)).

The teacher who relies on motivation — *"I should use AI more this week"* — is using the goal system. The goal system is effortful, depletable, and vulnerable to a hard Wednesday. The teacher who installs the workflow as a context-cued routine — *Sunday at 4 p.m., laptop open at the kitchen table, lesson-planning template loaded, Claude in the browser* — is using the habit system. Context triggers behavior. The work happens whether motivation is high or low. The accumulated difference across a school year is not trivial.

Honest extension caveat: the habit literature is well-evidenced for individual behaviors (exercise, snacking, commuting), more lightly tested on professional-workflow installation. The application here is plausible by extension, not specifically validated for teacher AI workflows. [contested]

### 2.5 Platform strategy — task fit, not fashion

The temptation, once you have decided to use AI systematically, is to chase whichever model topped the most recent benchmark. The empirical record makes this a losing strategy. Model rankings shift on a quarterly cadence; the leader on reasoning is not always the leader on document-grounded retrieval; vendor benchmarks are not designed for educator workflows. The industry guidance from TeachAI, CoSN, and ISTE+ASCD converges on the same principle: **fit for purpose**, not raw capability score ([TeachAI policy resources](https://www.teachai.org/policy-resources); [CoSN — AI in K-12](https://www.cosn.org/ai/); [ISTE — AI courses for educators](https://iste.org/courses/artificial-intelligence-explorations-for-educators)).

The operational division below is task-based, not product-based — because the products will change and the tasks will not. Treat the named tools as *examples at time of writing*, not endorsements.

| Task type | Tool family well-suited | Why it fits |
|---|---|---|
| Open-ended writing, reasoning, structured outputs, lesson design, rubric calibration | General reasoning model (Claude is one example) | Strong instruction-following on long structured prompts; predictable behavior under the Template Pattern; persistent project memory |
| Document-grounded study guides, summaries of multiple PDFs, audio overviews | Document-grounded model (NotebookLM is one example) | Outputs cite back to the user-supplied source; reduces hallucination risk for content the teacher must trust |
| Search-augmented quick lookups, image generation, spreadsheet-integrated tasks | Search-integrated general model (Gemini is one example) | Native search integration; office-suite integration; image generation in the same flow |
| Bulk rubric scoring and per-student feedback | Specialized graders integrated with the school LMS | Designed around rubric ingestion and FERPA-compatible logging; verify the specific product against your district's data-handling rules |
| Slide generation | Slide-generation tools (see Chapter 8 for the slideument-risk caveats) | Speed at the cost of default design; teacher must run the five-question diagnostic before use |
| Charts and data visualization | General model with code execution, or a specialized chart tool | See Chapter 9 — the chart-honesty checklist applies regardless of producer |

The principle the chapter teaches: **assign tools to task categories, not to time slots; pick the tool that fits the task in front of you, not the tool that is fashionable this month.**

### 2.6 The 68% training gap — why you may be building this alone

If you are reading this chapter without having received any formal AI training from your district, you are not the exception. You are the majority.

RAND's 2024–2025 work on the American School District Panel found that **roughly 68% of U.S. teachers reported no formal training on how to use AI tools** during the 2024–2025 school year ([RAND ASDP — *More Districts Are Training Teachers on Artificial Intelligence*, RR-A956-31](https://www.rand.org/pubs/research_reports/RRA956-31.html); [AI for Education summary of the RAND findings](https://www.aiforeducation.io/blog/rand-research-reveals-growing-ai-training-gap); [K-12 Dive — teacher AI training remains uneven](https://www.k12dive.com/news/teacher-ai-training-remains-uneven-despite-uptick/745668/)). The complementary district-side number from the same RAND wave: only 48% of districts said they had provided any teacher AI training by Fall 2024, up from 23% a year earlier. The Gallup-Walton 2025 survey gave a related but distinct figure — of teachers who *use* AI, 52% taught themselves and only 31% received district-provided training. [verify exact RAND wording: "no formal training" versus "no district-provided training" — the secondary summaries occasionally elide the distinction; the chapter should cite RR-A956-31 directly and the corresponding teacher-survey wave before publication.]

The equity dimension is sharp. By Fall 2024, 67% of low-poverty districts had provided AI training versus 39% of high-poverty districts. The training gap is also a poverty gap.

A misreading worth flagging: *the holdouts are the resistant teachers*. The data shows the opposite. The barrier to systematic AI use is mostly *no training was offered*, not *teachers refused training that was offered*. If your district has not yet trained you, the workflow in this chapter is what you are substituting for the training they have not yet provided.

### 2.7 The six-month shelf life — captured prompts decay

A captured prompt is not a permanent artifact. The model updates and the prompt's behavior shifts. Your needs shift. The standards or curriculum update. Within twelve months, a prompt that produced clean rubric-aligned feedback in August may produce drift you have to fight.

The major commercial models currently ship significant updates on roughly a 2–4 month cadence. A **six-month maintenance cycle** gives you two model-generations of drift to catch. This is a working heuristic, not a measured shelf life — controlled studies of prompt-output stability across model versions have not been published at the granularity teachers need. [verify against any future work on prompt-behavior decay across model versions.] Treat the six-month interval as an operating guess; if you observe drift sooner, shorten the cycle.

The maintenance move is a calendar entry. Twice a year — say, January and July — you pull the top 5–10 entries in the library, rerun each on a current task, and ask three questions:

1. Does this still produce a useful first draft?
2. Are the variable slots still the right slots, or has the task shape shifted?
3. Is there a new template I have been writing from scratch repeatedly that should be promoted into the library?

Each entry gets marked **renewed, revised,** or **retired,** and the "last verified" date gets updated.

### 2.8 Rogers and CBAM — why most teachers plateau

Two adoption frameworks help name what happens between *"I tried it"* and *"I use it systematically."*

Everett Rogers's *Diffusion of Innovations* (5th ed., Free Press, 2003) describes five sequential stages of individual adoption: knowledge, persuasion, decision, implementation, confirmation. Rogers's empirical pattern is that most adopters reach *implementation* — the tool is being used — and stop short of *confirmation* — the stage where the user has integrated the innovation into ongoing practice and confirmed it is working. The plateau at implementation looks exactly like ad hoc adoption: the tool is used, but each use is a fresh decision.

Gene Hall and Shirley Hord's Concerns-Based Adoption Model (CBAM), developed at the University of Texas's Research and Development Center for Teacher Education and synthesized in Hall and Hord's *Implementing Change* (Pearson, 5th ed.) [verify edition], is the more granular instrument. CBAM's Stages of Concern progression — *awareness → informational → personal → management → consequence → collaboration → refocusing* — describes a typical psychological arc. The systematic-AI plateau is consistent with teachers stuck at **stage 3 (management)** — *"Do I have time and materials to make this work?"* — and not yet moved into **stage 4 (consequence)** — *"How is this affecting students?"* — because the workflow has not stabilized enough to free attention from logistics ([SEDL — CBAM resources](https://sedl.org/cbam/)).

Both frameworks frame the plateau as a *structural* feature, not a character flaw. The fix is structural support: peer collaboration, observable evidence of impact, time to refocus from management to consequence. The systematic workflow you are about to build is itself the structural support.

Honest limit: CBAM has been criticized for its sequential-concerns assumption — Bailey and Palsha argue concerns can be parallel, not strictly sequential, and AI adoption may show this more strongly than older innovations because the technology itself shifts mid-adoption ([Bailey & Palsha critique](https://www.learntechlib.org/primary/p/8094/)). Use CBAM operationally; do not treat the order as iron. [contested]

---

## 3. Worked example — building *workflow.md*

What follows is what Teacher B's document looks like. Treat it as a template you adapt, not a script you copy. Specifics — grade level, subject, the exact tools — should match your week, not mine.

### 3.1 The starter ten-prompt library

The library has ten entries minimum, one or two from each task category covered in Chapters 4–9. Each entry follows the Template Pattern from Chapter 3: role, context, task, format, constraints. Variable slots are in `[ALL CAPS]`.

```markdown
# workflow.md — Personal AI Workflow Document
Last reviewed: 2026-01-14
Owner: [TEACHER NAME]

---

## Section 1 — Prompt library (10 entries)

### 01 · Lesson skeleton (Ch 4)
ROLE: You are a [GRADE LEVEL] [SUBJECT] curriculum designer.
CONTEXT: Standard: [STANDARD CODE]. Class profile: [N STUDENTS, KNOWN
MISCONCEPTIONS, ELL/IEP COUNT IF ANY — NO NAMES]. Prior unit: [PRIOR UNIT].
TASK: Draft a 45-minute lesson skeleton: objective, hook, two activities,
exit ticket aligned to the standard.
FORMAT: Markdown; objective as one sentence; activities timed.
CONSTRAINTS: No assumptions about resources beyond [LIST]. Note one
likely misconception with a one-line check.
Phase gate (Ch 2 #9): I verify the objective is achievable by THIS class
before accepting the plan.
Last verified: 2026-01-14

### 02 · Unit scope-and-sequence (Ch 4)
ROLE: ... [same pattern]
TASK: Sketch a [N]-day scope-and-sequence for [UNIT TOPIC] aligned to
[STANDARDS], with one assessment per [INTERVAL].
Phase gate: I confirm sequencing matches PCK for this class.
Last verified: 2026-01-14

### 03 · Rubric-aligned feedback (Ch 5)
ROLE: You are a [SUBJECT] teacher writing first-pass feedback against a
rubric.
CONTEXT: Rubric: [PASTE RUBRIC]. Assignment: [BRIEF DESCRIPTION].
Student work: [PASTE]. [NO STUDENT IDENTIFYING INFO.]
TASK: Score each rubric dimension; draft one comment per dimension; do
not assign a letter grade.
FORMAT: Table — dimension, score, comment.
CONSTRAINTS: Comments must be actionable; no praise without specificity.
Phase gate (Ch 2 #1, #2): I calibrate on 5 samples before bulk run; I
review every comment before release; I make the final grade decision.
Last verified: 2026-01-14

### 04 · Lexile pass (Ch 6)
ROLE: You are a reading specialist.
CONTEXT: Target reading level: [LEXILE BAND]. Source text: [PASTE].
TASK: Rewrite preserving content fidelity; produce [N] versions at
[BANDS].
CONSTRAINTS: No simplification of technical terms central to the unit.
Phase gate (Ch 2 #12, #5): No student identifying info; I verify content
accuracy before use.
Last verified: 2026-01-14

### 05 · Parent note from bullets (Ch 7)
ROLE: You are drafting a parent communication in the school's register.
CONTEXT: Family relationship: [BRIEF]. Bullets from my notes: [PASTE].
TASK: Three sentences. Open with specific observation; one growth
target; invite contact.
CONSTRAINTS: Warm, not bureaucratic. No claims not in my bullets.
Phase gate (Ch 2 #7): I review prose against bullets; sensitive
communications — I write core message first.
Last verified: 2026-01-14

### 06 · Meeting summary from rough notes (Ch 7)
ROLE: You are summarizing a meeting.
CONTEXT: Rough notes: [PASTE].
TASK: Decisions, action items with owners and dates, open questions.
FORMAT: Three sections, bulleted.
Phase gate: I verify decisions against my notes before circulating.
Last verified: 2026-01-14

### 07 · Slide rewrite (Ch 8)
ROLE: You are a slide editor enforcing assertion-headline discipline.
CONTEXT: Current slide: [PASTE]. Audience: [GRADE LEVEL]. Speaker
narration plan: [SUMMARY].
TASK: Rewrite headline as a claim, not a topic label. Move duplicated
speaker text to the notes field. Cut seductive detail.
Phase gate (Ch 8): I run the 5-question diagnostic before accepting.
Last verified: 2026-01-14

### 08 · Chart-from-data (Ch 9)
ROLE: You are a data-visualization designer for an educator audience.
CONTEXT: Data: [PASTE OR DESCRIBE]. Question the chart answers:
[ONE SENTENCE]. Reader: [WHO, IN HOW MUCH TIME].
TASK: Recommend chart type; produce; title states the finding.
CONSTRAINTS: y-axis from zero for bar charts; no more than five
categories in a pie; explicit comparison.
Phase gate (Ch 9): I run the 5-question checklist before use.
Last verified: 2026-01-14

### 09 · Document-grounded study guide (Ch 4 / Ch 10)
ROLE: You are a study-guide writer working ONLY from supplied sources.
CONTEXT: Sources: [UPLOAD TO DOCUMENT-GROUNDED TOOL]. Audience:
[GRADE LEVEL].
TASK: Six study questions, each citing the source page; one synthesis
prompt.
CONSTRAINTS: No claim without source citation.
Tool note: Run this in a document-grounded tool (e.g., NotebookLM), not
in a general chatbot.
Phase gate (Ch 2 #10): I verify each citation traces.
Last verified: 2026-01-14

### 10 · Specification prompt for a small automation (Ch 11)
ROLE: You are a software assistant. I am not a programmer.
CONTEXT: Inputs available: [DESCRIBE]. Desired output: [DESCRIBE].
Constraints: [PRIVACY, TIME, DEPENDENCIES].
TASK: Propose the simplest solution. List the test cases I should run.
Produce the code.
Phase gate (Ch 11): I test against specification including edge cases
before deploying with students.
Last verified: 2026-01-14
```

Ten entries is the floor, not the ceiling. The Botspeak Specification Library in Nik Brown's *Botspeak* names five recurring task buckets as the entry-level library; AI for Education's open library and Panorama Education's district-level "100+ AI Prompts" both organize by task type and parameterize the slots ([AI for Education prompt library](https://www.aiforeducation.io/prompt-library); [Panorama Education — 100+ AI Prompts](https://www.panoramaed.com/blog/100-ai-prompts)). The shape converges. Yours will too.

### 3.2 The weekly schedule — *workflow.md* Section 2

```markdown
## Section 2 — Weekly schedule (AI-assisted blocks)

Fixed first (classes, duty, IEP meetings, prep period, PLC).

AI-assisted blocks:

| Day | Time | Task | Tool | Library entry | Phase gate (Ch 2) |
|---|---|---|---|---|---|
| Sun | 4:00–6:00 PM | Lesson planning for the week | General reasoning model | #01, #02 | #9 PCK; #5 content accuracy |
| Mon | 7:00–7:45 AM | Differentiation pass on the week's text | General reasoning model | #04 | #12 anonymize; #5 verify |
| Wed | 10:30–11:15 AM (prep) | Feedback drafting batch | General reasoning model | #03 | #1 calibrate on 5; #2 review every comment |
| Thu | 3:30–4:30 PM | Parent / admin communication batch | General reasoning model | #05, #06 | #7 sensitive = teacher drafts core |
| Fri | 2:30–3:15 PM | Next week's slides (if any) | General reasoning model + slide tool | #07 | Ch 8 5-question diagnostic |
| Rolling | as needed | Assessment items, charts, small automations | Tool varies | #08, #09, #10 | Per chapter |

Slack budget: 30% of each block reserved for the inevitable thing that
takes longer. A block that hits 100% utilization the first time is
miscalibrated.
```

### 3.3 The platform-assignment note — *workflow.md* Section 3

```markdown
## Section 3 — Platform assignments (task-fit, not fashion)

- Open writing/reasoning/calibration → general reasoning model
  (e.g., Claude). Project memory holds the standards reference.
- Document-grounded summaries / study guides → document-grounded model
  (e.g., NotebookLM). Outputs cite the source.
- Search-augmented quick lookups / spreadsheet-integrated tasks →
  search-integrated general model (e.g., Gemini).
- Bulk grading on rubric → school-LMS-integrated grader. Verify FERPA
  compatibility with district.
- Slides → slide tool of choice, with Ch 8 diagnostic.
- Charts → general model with code execution, or specialized chart tool.

Product names are placeholders. Review this section at the six-month
maintenance check; products change faster than principles.
```

### 3.4 The phase-gate map — *workflow.md* Section 4

```markdown
## Section 4 — Phase-gate map (from Ch 2)

For every AI-assisted task above, name the gate explicitly:

- Rubric calibration gate: 5 samples before bulk
- Discrepancy resolution gate: AI barred from contested scores
- Content accuracy gate: verify before distribution
- Anonymization gate: no PII to external tools
- PCK gate: I confirm the plan fits THIS class
- Sensitive communication gate: I draft core message
- Document grounding gate: verify each citation traces

This map gets printed and posted above the desk.
```

### 3.5 What goes wrong — the lesson and the limit

Build the document in August. Watch it survive November.

The schedule fails when your week fails. A parent meeting Wednesday morning eats the Wednesday feedback block. A snow day moves Monday to Tuesday. The IEP that runs an hour long takes Thursday's communication block. The system cannot prevent any of that. What it can do is make the recovery cheap: when the week breaks, you have a captured library that still works in whatever 25-minute slot you can find. The ad hoc user, in the same broken week, has neither the schedule nor the captured prompts. She does the work from scratch or she does not do it at all.

Build slack into the schedule. Treat the system as a default, not a contract. The point is not to recover every minute; it is to make the average week meaningfully better.

---

## 4. Common misconceptions

**Misconception 1: "Tool knowledge equals systematic use."**
*Why it fails.* Knowing what Claude or Gemini can do is necessary; it is not sufficient. Teachers who watch the demos, read the blog posts, and try the tools once or twice — and then stop capturing prompts and stop scheduling the blocks — get the literacy without the fluency, exactly the pattern Chapter 0 of *Botspeak* names. The Gallup-Walton survey is consistent with this: the 28% of teachers who use AI *infrequently* are largely tool-aware. They are not systematic users. Knowledge of the tool does not, on its own, convert to recurring use. The capture and the schedule do.

**Misconception 2: "More platforms = more savings."**
*Why it fails.* Adding a third or fourth tool without a task-fit reason adds switching cost and decision cost without adding output. The teacher who tracks the model leaderboards and migrates her workflow every quarter is paying a tax — every move costs library rewrites, retraining her own habits, and the inevitable "where did I save that prompt?" loss. The pattern in the TeachAI and CoSN guidance is the opposite: pick the right tool for each task category and stay with it until it stops working for that category, not until something newer shows up.

**Misconception 3: "A prompt that worked last year still works."**
*Why it fails.* Models update on a two-to-four-month cadence. The prompt that produced clean rubric-aligned feedback in September can drift by March — perhaps the model is more cautious, perhaps less, perhaps the output structure has shifted to a new default format. A teacher who runs an unmaintained prompt against a changed model may not notice the regression until a grading dispute surfaces it. The six-month maintenance check is the cheapest insurance you have. The shelf life is a working heuristic, not a measured rate. [contested]

**Misconception 4: "Systematic = rigid."**
*Why it fails.* This is the most common reason teachers resist the system. The fear is that *workflow.md* turns teaching into a script. It does not. The library captures the *form* of recurring tasks (lesson skeleton, rubric comment, parent note). The *substance* — which standard, which class, which student, which family — is what you fill in. The slots are where your professional judgment goes. Systematic use frees attention from logistics so the judgment can be the bottleneck instead of the prompt-writing. The opposite of rigid is not unsystematic; it is responsive. The system is what makes responsiveness affordable.

A fifth misconception worth a flag, because it lurks behind several of the above: *"If I use the system enough, my hours saved will match Teacher B's."* The honest answer is: maybe. The selection-vs-treatment question is unresolved (Section 2.1). Track your own hours. The data point that matters is yours.

---

## 5. Exercises

### Exercise 12.1 — Build the personal AI workflow document (CREATE)

Open a new document. Name it *workflow.md*. Build all four sections (library, schedule, platform assignments, phase-gate map). The library has at least ten entries drawn from prompts you have *actually* written in the past month — not aspirational entries, captured ones. The schedule names four to six AI-assisted blocks across your real week, each with task / tool / library entry / phase gate. The phase-gate map is printable on one page.

*Time budget.* 90 minutes for the first pass. Iterate in 15-minute touch-ups across the following two weeks.

*Submission.* Bring the document to a colleague who teaches the same grade band. Read it together. If a slot or a phase gate does not survive their reading, the slot or gate is not yet ready.

### Exercise 12.2 — Audit your current week against the document

Track your AI use across one full school week without changing anything. For each AI interaction, log: date and time, task, tool, time spent, whether a captured prompt was used, whether a phase gate was named, whether the output was used.

At the end of the week, lay the log next to *workflow.md*. Compare. Three diagnostic questions:

1. **Capture rate.** What fraction of your AI uses ran from a library entry versus from a fresh prompt? Below 50% is a sign the library needs entries you actually need, not entries that seemed plausible at build time.
2. **Schedule rate.** What fraction of your AI uses happened inside a scheduled block versus opportunistically? Below 50% is a sign either the schedule is wrong (the blocks are at the wrong times) or the habit has not yet installed (give it three more weeks).
3. **Phase-gate rate.** What fraction of your AI uses had a named gate inspection? Below 100% is a problem; fix it before the next week.

Revise the document on the basis of what you actually did, not what you planned to do.

### Exercise 12.3 — Design a six-month maintenance check

Put two calendar entries six months apart — one in January, one in July. Each is 30 minutes. The protocol:

1. Pull the top 5–10 library entries by use frequency.
2. Rerun each on a recent real task.
3. Mark each as **renewed** (works as is, update verification date), **revised** (works after edits, update prompt and date), or **retired** (no longer useful, archive).
4. Identify any new prompt patterns you have been writing repeatedly from scratch in the past six months. Promote at least one into the library.
5. Update the platform-assignment section if products have changed.

Write the protocol into Section 5 of *workflow.md*. Calendar entries that do not survive into next year are calendar entries you have to set again every year. Make them recurring.

### Exercise 12.4 (optional) — Run the habit-installation protocol on one slot

Pick the single highest-value slot from your schedule (often Sunday lesson planning or the feedback batch). Run it for three consecutive weeks. Same day, same time, same physical setup, same browser tab order. Track activation effort on a 1–5 scale after each session.

The Wood-and-Neal prediction: activation effort drops by week three. If it has not, the slot is in the wrong place — try a different day or time. If it has, you have just installed one habit; pick the next slot.

### Exercise 12.5 (optional) — Self-stage diagnostic

Place yourself on Rogers's five stages (knowledge / persuasion / decision / implementation / confirmation) and CBAM's seven Stages of Concern. Name the specific structural support that would move you to the next stage. Write it into Section 6 of *workflow.md*. Honest answer beats flattering answer.

---

## 6. What would change my mind

A randomized controlled trial that assigned teachers to (a) systematic-workflow training with a starter prompt library plus weekly schedule, (b) tool access without workflow training, and (c) a no-tool control — and that measured weekly hours saved across a full school year — would settle the selection-vs-treatment question this chapter cannot. If a well-powered RCT found that systematic prompt-library use produced no greater time savings than ad hoc use once selection on motivation and organization was controlled, the chapter's core claim — that the *system* drives the higher savings — would be falsified. The workflow document would still be useful as a personal organization tool; it would no longer be defensible as a route to the 12-hour upper-tail observation. As of writing, no such RCT has been published. The chapter's recommendation rests on observational data plus craft-derived knowledge-management principles, and is presented as a hypothesis the reader tests in her own week.

---

## 7. Still puzzling

Four questions I do not yet know how to answer.

1. **Selection versus treatment.** What share of the systematic-vs-ad-hoc savings gap is selection effect and what share is treatment effect? The observational data cannot say. Until a randomized study runs, every teacher's *workflow.md* is, in part, a personal experiment whose results she is the only person who can read.
2. **Prompt shelf life by task type.** Is the decay rate the same for rubric-aligned feedback prompts and for communication-tone prompts? My working guess is no — model alignment behavior on grading shifts faster than its tone behavior on parent emails — but I have not measured it. The six-month rotation is a safe default; the optimal cadence may differ by entry.
3. **The ceiling.** Chapter 1's task-by-task model projects a 16.7-hour weekly ceiling under fully systematic deployment. Teacher B's 12 hours sits below that ceiling. Whether the gap from 12 to 16.7 is real, or whether it is the difference between what a model adds up to and what a person can sustain across a full school year, is open. The honest 20-hour personal-experience claim cited in Chapter 1 is consistent with the upper edge of the projection; it is also a single self-report and not yet a finding.
4. **District-portable libraries.** When a teacher's library is good enough that a colleague benefits from a copy, does the copy work as well in the colleague's classroom? The codified-knowledge literature predicts partial transfer — the captured prompt is explicit, but the calibration is partly tacit. The arXiv work on teacher-authored prompts as district-portable assets ([Spring 2025 pilot, 16 teachers, 4 districts, 878 students](https://arxiv.org/html/2604.16738v1)) is suggestive but small. The bigger version of this question is open.

---

## Bridge to Chapter 13

A systematic workflow is also an auditable workflow. The same *workflow.md* that saves you ten hours a week is, on the other side, a documented record of what AI did and what you did — the foundation for the integrity disclosure Chapter 13 builds out. The library is the substrate of honest practice, not just efficient practice. Chapter 13 turns this around: when a student, a parent, or an administrator asks what role AI played in something you produced, the workflow document is the answer.

---

**Tags:** prompt-library, weekly-workflow, systematic-vs-ad-hoc, habit-formation, RAND-ASDP, Gallup-Walton, Davenport-Prusak, CBAM, Rogers-diffusion, platform-fit, six-month-maintenance, phase-gate-map

---

*Voice anchor: root `style/` (workshop baseline). No per-book `style/` overrides resolved at draft time; `voice-unanchored` flag not raised because Chapters 1–8 in this book have established voice patterns this chapter follows directly.*

---

## References

- Bailey, D. B., Jr., & Palsha, S. A. (1992). Qualities of the Stages of Concern Questionnaire and implications for educational innovations. *Journal of Educational Research*, 85(4), 226–232. Aggregator: [LearnTechLib synthesis](https://www.learntechlib.org/primary/p/8094/).
- Davenport, T. H., & Prusak, L. (1998). *Working Knowledge: How Organizations Manage What They Know.* Harvard Business School Press. ISBN 0-87584-655-6. [HBR Press page](https://store.hbr.org/product/working-knowledge-how-organizations-manage-what-they-know/3014).
- Diliberti, M. K., Lake, R. J., & Weiner, S. R. (2025). *More Districts Are Training Teachers on Artificial Intelligence: Findings from the American School District Panel* (RR-A956-31). RAND Corporation. [RAND landing page](https://www.rand.org/pubs/research_reports/RRA956-31.html).
- Diliberti, M. K., Schwartz, H. L., Doan, S., Shapiro, A., Rainey, L. R., & Lake, R. J. (2024). *AI Use in Schools Is Quickly Increasing but Guidance Lags Behind* (RR-A4180-1). RAND Corporation. [RAND PDF](https://www.rand.org/content/dam/rand/pubs/research_reports/RRA4100/RRA4180-1/RAND_RRA4180-1.pdf).
- Gallup & Walton Family Foundation. (2025). *Teaching for Tomorrow: Unlocking Six Weeks a Year With AI.* Survey fielded March 18 – April 11, 2025 via RAND American Teacher Panel, n=2,232 U.S. public K-12 teachers. Release September 16, 2025. [Gallup release](https://news.gallup.com/poll/691967/three-teachers-weekly-saving-six-weeks-year.aspx); [Walton summary](https://www.waltonfamilyfoundation.org/six-weeks-giving-teachers-time-back-with-ai); [full PDF](https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf).
- Hall, G. E., & Hord, S. M. (2020). *Implementing Change: Patterns, Principles, and Potholes* (5th ed.). Pearson Education. [Pearson catalog](https://www.pearson.com/en-us/subject-catalog/p/Hall-Implementing-Change-Patterns-Principles-and-Potholes-5th-Edition/P200000001185).
- Newport, C. (2016). *Deep Work: Rules for Focused Success in a Distracted World.* Grand Central Publishing. ISBN 9781455586691. [Hachette listing](https://www.hachettebookgroup.com/titles/cal-newport/deep-work/9781455586691/).
- Rogers, E. M. (2003). *Diffusion of Innovations* (5th ed.). New York: Free Press. ISBN 978-0743222099. [Simon & Schuster page](https://www.simonandschuster.com/books/Diffusion-of-Innovations-5th-Edition/Everett-M-Rogers/9780743222099).
- SEDL (Southwest Educational Development Laboratory). *Concerns-Based Adoption Model (CBAM)* resources, including Stages of Concern. [SEDL CBAM home](https://sedl.org/cbam/); [Stages of Concern](https://sedl.org/cbam/stages_of_concern.html).
- Wood, W., & Neal, D. T. (2007). A New Look at Habits and the Habit-Goal Interface. *Psychological Review*, 114(4), 843–863. DOI 10.1037/0033-295X.114.4.843. [USC Dornsife PDF](https://dornsife.usc.edu/wendy-wood/wp-content/uploads/sites/183/2023/10/wood.neal_.2007psychrev_a_new_look_at_habits_and_the_interface_between_habits_and_goals.pdf).
- Wood, W., & Rünger, D. (2016). Psychology of Habit. *Annual Review of Psychology*, 67, 289–314. DOI 10.1146/annurev-psych-122414-033417. [Annual Reviews](https://www.annualreviews.org/content/journals/10.1146/annurev-psych-122414-033417).
- TeachAI policy resources: [https://www.teachai.org/policy-resources](https://www.teachai.org/policy-resources).
- CoSN — AI in K-12: [https://www.cosn.org/ai/](https://www.cosn.org/ai/).
- ISTE — AI courses for educators: [https://iste.org/courses/artificial-intelligence-explorations-for-educators](https://iste.org/courses/artificial-intelligence-explorations-for-educators).
- AI for Education open prompt library: [https://www.aiforeducation.io/prompt-library](https://www.aiforeducation.io/prompt-library).
- Panorama Education — *100+ AI Prompts*: [https://www.panoramaed.com/blog/100-ai-prompts](https://www.panoramaed.com/blog/100-ai-prompts).
- CRPE — *The AI Dividend* commentary: [https://crpe.substack.com/p/the-ai-dividenddoes-ai-create-more](https://crpe.substack.com/p/the-ai-dividenddoes-ai-create-more).
