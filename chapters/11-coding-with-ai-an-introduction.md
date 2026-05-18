# Chapter 11 — Coding with AI: An Introduction

<!-- FACT-CHECK FLAG: CONFIRMED with minor citation issues — see factchecks/11-coding-with-ai-an-introduction-assertions.md -->

**TL;DR.** A teacher who cannot code can now build working software — a spreadsheet automation, a grading script, an interactive demo — by writing a careful specification and letting an AI coding assistant render the syntax. The durable skill is specification, and the durable responsibility is verification: not of the code (which the teacher cannot read), but of the tool's behavior with real students under real conditions.

---

## 1. Learning objectives

By the end of this chapter, you will be able to:

1. *(Understand)* Describe coding-with-AI for a non-programmer: the teacher writes the specification, the AI writes the code, the teacher verifies the output.
2. *(Apply)* Write a specification prompt for a simple teacher workflow automation (spreadsheet, grade-management, or communication task).
3. *(Apply)* Write a specification prompt for a simple interactive educational tool.
4. *(Analyze)* Identify the verification responsibility: testing the *output behavior* against the spec — including edge cases and privacy surface — not the source code.
5. *(Evaluate)* Apply the accountability principle: the teacher who deploys an AI-built tool with students bears responsibility for the tool's behavior, regardless of who wrote the code.

**Prerequisites:** Chapter 2 (the phase gate as the boundary between AI work and human work). Chapter 3 (prompting as task decomposition). Chapter 6 (anonymization before any AI interaction with student data).

---

## 2. Opening: a math teacher who does not code

A high school math teacher — call her Ms. R, *[composite-illustrative — the case combines patterns from teacher-built AI artifacts documented in practitioner essays during 2025–26; no single named district or person]* — wanted something she had wanted for fifteen years. An interactive page where a student could drag a slider, change the coefficient *a* in a cubic, and watch the curve bend in real time. She wanted the labels she wanted. She wanted the zoom range she wanted. She did not want Desmos's version of the demo or GeoGebra's version. She wanted *her* version, because the lesson she was teaching tomorrow had a specific point and she wanted the demo to land that specific point exactly.

She had three problems. She did not know how to code. The afternoon was Sunday. The lesson was Monday.

What she did know — because she had been thinking about this demo every spring for fifteen years — was exactly what she wanted the page to do. So she opened an AI coding assistant and started typing.

She did not type code. She typed a paragraph.

*Single HTML page. Plot y = ax³ + bx² + cx + d. x from −5 to 5. Three sliders — wait, four — for a, b, c, d, each ranging from −5 to 5 in steps of 0.1. When any slider moves, the curve updates. Show the equation across the top in standard form. Mark real roots as dots on the x-axis. Label the y-intercept. White background. Self-contained — no internet required at runtime.*

Three hours later she had a working HTML file she could email to herself, drop on a USB stick, and open on the classroom Chromebook in front of thirty students. The first attempt had a bug — the root detector missed repeated roots. She did not read the code to find the bug. She described the bug back to the assistant the same way she had described the page: *when a = 0, the cubic becomes a quadratic, and the root display does not update.* The assistant fixed it. She tested five coefficient combinations she had worked the answers for by hand, plus one configuration designed to break things — all zeros. She showed it to the math teacher next door to see if the labels made sense. She saved the prompt history. She closed the laptop.

She did not write a single line of code. She wrote specifications.

This chapter is about what she did, why it worked, why it might have gone badly, and what you would need to do to do the same thing for one of your recurring tasks — safely.

---

## 3. The concept: specification is the skill, syntax is not

For most of computing history, the bottleneck to building a tool was knowing how to type the right characters in the right order. *Syntax.* The semicolons, the brackets, the indentation, the names of the library functions. A person who could not type those characters could not build the tool, no matter how clearly they could describe what the tool should do.

What changed in 2022–2024 is that a particular kind of machine learning model — a large language model trained on enormous quantities of source code paired with natural-language descriptions — got good enough at translating English-shaped intent into code-shaped output that the *typing-of-the-characters* step could be delegated. The bottleneck moved.

It moved to where it actually belongs: to the description of what the tool should do.

### What "specification" actually means

A specification is the document a careful person writes before they hand work to someone else. An architect's drawing for a contractor. A recipe for a baker. A wiring diagram for an electrician. The specification names what is to be built so that the person doing the building does not have to guess.

Botspeak — the prompt-as-specification framework introduced in Chapter 3 of this book — names five components a working specification contains:

- **Intent.** Not the immediate task, but the goal the task serves. *Make a spreadsheet that flags struggling students*, not *make a spreadsheet*.
- **Constraints.** What the work must respect — format, privacy, time, dependencies, environment.
- **Success criteria.** How you will know the output is good after the fact. *The script flags every student whose average is below 70 and no others on three test files I have already computed by hand.*
- **Exclusions.** What the work must *not* do. *Do not impute zero for missing scores. Do not send any data to a server.*
- **Output format.** What the deliverable looks like structurally. A second CSV. A single HTML file. A printable PDF.

A teacher who writes a paragraph that contains all five of those things, in any order, in plain English, can now generate working software. A teacher who writes one or two of them — say, intent plus format — will get something that compiles, runs, looks reasonable, and is wrong in ways the teacher will not immediately see.

The first paragraph is the durable skill. The second one is the trap.

### A short history: end-user programming, restated

The teacher writing a specification and getting working code is not a new idea — it is the latest move in a forty-year research program. Brad Myers at Carnegie Mellon and Margaret Burnett at Oregon State, with collaborators across the human-computer interaction community, have been asking since the 1980s how to let people who are not professional programmers create software for their own purposes. The answers they explored were spreadsheet formula authoring, visual programming languages, programming-by-example, web macro recording, and domain-specific tools for specific worlds. The 2011 *ACM Computing Surveys* article ["The State of the Art in End-User Software Engineering"](https://web.media.mit.edu/~lieber/Publications/End-User-Software-Engineering.pdf) laid the field out clearly. Each approach got partway. Each had a ceiling.

The ceiling was the same in every case: how do non-programmers *describe behavior to a computer when they cannot write code?* Spreadsheets answered it for grids of numbers. Visual languages answered it for simple control flow. Nothing generalized.

What changed in 2022–2024 is that the answer became *describe it in English*. Not because the question changed — it was the same question Myers and Burnett were asking in 1990 — but because a particular kind of model became good enough at the translation step. The forty-year research program did not end. It got a new tool.

### Three categories of teacher workflow automation

Most teacher coding tasks fall into one of three buckets, defined by what kind of data the script touches. They are sorted here from lowest to highest risk-of-deployment.

**1. Spreadsheet processing.** Take a CSV, transform it, output a CSV. Reformat a roster between platforms. Compute summary statistics on quiz scores. Pivot attendance from long to wide format. Merge an exported gradebook with rostering data. Produce the "students who missed three of the last five days" list a paper-based teacher used to make by hand. The risk is low if the data is anonymized. Moderate if it includes names. The script runs on your laptop, processes a file you already had access to, and produces a file you review before any other use.

**2. Grade management.** Compute grades from raw scores. Apply weighting policies. Generate per-student feedback summaries from a rubric. Flag students for intervention based on configured thresholds. The risk is elevated because grade calculations have consequences and bugs are *silent* — a script that systematically misweights one rubric category will produce wrong grades for the entire class with no visible symptom. The verification load is heaviest here, and the chapter says so explicitly.

**3. Communication tools.** Generate per-student communications — mail-merge progress emails, per-family slip translations, templated permission slip generators. The risk is highest because the artifact reaches families and any error is externally visible. A misnamed student, a misaddressed parent, a misstated grade in a templated message becomes a relationship problem you inherit. The phase gate from Chapter 7 applies: routine drafting can be automated; sensitive communications cannot.

These three categories share a shape — structured input, transformation, structured output — that is the shape current coding assistants handle most reliably. There are thousands of examples of each in the training data. The reason these are the entry points is that the model is most reliable on exactly these tasks.

A common misconception is that you should automate the most painful task first. Not quite. Automate the *highest-volume task with the lowest per-instance risk* first. That is almost always spreadsheet processing, not grade computation. Build the verification habit on a low-risk script before the script touches anyone's grade.

### Verification when you cannot read the code

Here is the hardest pedagogical move in this chapter, and the one your professional instincts may resist: *you must be able to verify a tool whose source code you cannot read.*

Most professionals verify work by inspecting it. A copy-editor reads the manuscript. A nurse reviews the chart. A teacher reads the essay. The natural move when you receive AI-generated code is to look at it — and the natural conclusion, when you see unfamiliar function names and library imports, is that the tool is unverifiable.

The reframe: you do not verify the *code*. You verify the *behavior*. The behavior is observable. The code is not, to you, legible. So you test what you can see.

Concretely, this means treating verification as five passes:

1. **Test the spec.** Re-read what you specified. Construct three inputs you have already computed the expected output for by hand. Run the script on each. Compare.
2. **Test the edges.** What if a cell is blank? What if a name has an apostrophe — *O'Brien*, *D'Angelo*? What if a score is `"95%"` with the percent sign rather than `95`? What if there are two hundred students instead of thirty? What if the CSV uses semicolons instead of commas? You do not need to know which case will break. You need to systematically test the cases the spec did not contemplate. AI-generated code most reliably fails on edges *because the typical training example does not include them.*
3. **Test the wrong input.** Feed it something that should fail. An empty file. A corrupted file. The wrong file. Does it fail gracefully — clear error message — or silently produce nonsense? Silent nonsense is the dangerous failure mode when the output reaches grades or families.
4. **Test the privacy surface.** Without reading the code, ask the assistant explicit questions. *What data does this script read? What does it write? Does it communicate over the network? Does it create files I did not request? Does it use any library that uploads data for processing?* Document the answers. (If a teaching colleague can read code, ask them the same questions and compare answers.)
5. **Re-run on real data with a sentinel.** Insert one row whose expected output you have hand-computed. If the script gets that row wrong, every other row is suspect.

That is the protocol. Slow the first time. Fast by the fifth.

### What the evidence does and does not say

The single most-cited piece of evidence for AI coding assistants is [Peng, Kalliamvakou, Cihon, and Demirer's 2023 study of GitHub Copilot](https://arxiv.org/abs/2302.06590). Ninety-five professional developers were asked to implement an HTTP server in JavaScript. The treatment group, with Copilot, completed the task **55.8% faster** than the control group. Less experienced developers gained more than experienced ones. The number is real.

The number measures *time-to-complete on a clearly specified task.* That is all it measures.

It does *not* measure whether the produced code is secure. It does *not* measure whether the code is maintainable six months later. It does *not* measure whether the code does the right thing on inputs not in the test set. It does *not* measure whether the developer would have learned the same thing by writing the code themselves. Peng et al. is evidence that AI accelerates well-specified development tasks. It is not evidence that AI-generated code is good. Conflating those two things is one of the most common rhetorical moves in the AI-for-education literature, and this textbook refuses it.

The follow-on evidence on code quality is more sobering. [Veracode's 2025 evaluation](https://www.veracode.com/blog/ai-generated-code-security-risks/) found roughly **45% of AI-generated code samples contained at least one OWASP Top 10 security flaw**. The [Cloud Security Alliance's 2025 review](https://cloudsecurityalliance.org/blog/2025/07/09/understanding-security-risks-in-ai-generated-code) reached similar figures. A [2025 large-scale arXiv analysis](https://arxiv.org/pdf/2510.26103) found vulnerability rates around 16–18% for Python and around 9% for JavaScript across LLM-generated samples. A controlled user study cited across this literature found participants using AI assistants wrote *less secure* code than controls *and rated their insecure solutions as more secure than controls' solutions.*

That last finding is the one teachers should not forget. The natural confidence-feeling produced by working with a fluent assistant is uncorrelated with whether what it produced is safe. For a teacher who cannot read the code, the most natural check — *does it look right?* — is not available. The second-most-natural check — *did it run?* — is also not enough. *Running* is not *working*. *Working* is not *safe*.

What protects teachers in this space is not technical sophistication. It is a few stubborn habits. Anonymize before any AI interaction with student data. Test on synthetic data first. Run the verification protocol. Refuse to deploy a student-facing tool the same day you built it.

### Vibe coding and the retraction

In February 2025, Andrej Karpathy — one of the better-known researchers in the field — [posted a short tweet coining the phrase "vibe coding"](https://x.com/karpathy/status/1886192184808149383): the practice of building software by describing what you want to an LLM and accepting what it produces, more or less by feel, without worrying much about reviewing the code. The phrase went viral. For a while it was the cultural moment.

A year later, in his [2025 LLM year-in-review post](https://karpathy.bearblog.dev/year-in-review-2025/), Karpathy was sharper: "Today (1 year later), programming via LLM agents is increasingly becoming a default workflow for professionals, except with more oversight and scrutiny." Industry practice did not converge on *vibe coding*. It converged on **spec-driven development** — the developer writes the specification, the AI writes the code, the developer reviews against the spec.

The retraction is not embarrassing. It is the field correcting itself. And it is the operative line for teachers: the workflow you are learning is not the one that briefly went viral. It is the one that survived.

### Computational thinking did not become obsolete

In 2006, Jeannette Wing — then at Carnegie Mellon — published a short *Communications of the ACM* piece called ["Computational Thinking"](https://www.cs.cmu.edu/~wing/publications/Wing06.pdf). Her argument: what students should learn from computer science is not how to code, but how to think computationally — abstraction, decomposition, algorithmic reasoning, recognizing the boundaries of what is computable. A decade later, the [2016 K–12 Computer Science Framework](https://k12cs.org/), developed by ACM, Code.org, CSTA, the Cyber Innovation Center, and NMSI, codified this into seven core practices for K–12 CS education.

Wing's argument matters here because it answers, from 2006, the question some now ask in 2026: *if AI can write the code, why teach CS at all?* Wing's answer pre-dates the question and survives it. Computational thinking is *what you need to be able to specify a problem to a computer at all* — whether the computer's translator is a compiler, a programmer-colleague, or a generative model. Decomposition is unchanged. Abstraction is unchanged. The discipline of imagining what could go wrong is unchanged. What changed is which step takes the most time.

Look back at Ms. R's polynomial specification. Every move in it is computational-thinking-shaped. She identified the inputs (four sliders, with ranges). She identified the outputs (curve, roots, intercept). She decomposed the problem into rendering, interaction, and calculation. She abstracted from the specific cubic to a parameterized polynomial form. She anticipated an edge case (what if *a* = 0?). She constrained the runtime environment (no internet). A teacher who can do this for a polynomial can do it for a script. A teacher who cannot, cannot. The bottleneck for non-coding teachers building tools with AI is not syntax. It is the thinking Wing named in 2006.

A common misconception is that *coding is obsolete and we should teach prompting instead.* That is the wrong dichotomy. Specification *is* the computational thinking work Wing named. It is what remains when the syntax burden is removed. The chapter teaches specification, not prompting-as-trick.

### The accountability principle

The teacher who deploys a tool with students is responsible for the tool's behavior with students, *regardless of who wrote the code*. The AI did not deploy the tool. You did. Accountability runs to the deployer.

This is the long-standing professional-responsibility doctrine in software engineering — the engineer is responsible for what they ship; "the IDE made me do it" is not a defense — applied to the teaching context. [FERPA](https://studentprivacy.ed.gov/ferpa) does not distinguish between a script you wrote and a script the AI wrote: if the script touches identifiable student information, FERPA's restrictions apply equally to both.

The practical consequences:

- Never paste real student data into a cloud coding assistant. Anonymize first (the Chapter 6 protocol). If the spec contains a real student name, the chapter has already failed.
- Test on synthetic data first. Real data only after the synthetic test passed.
- District IT review for any tool that crosses systems. A script that pulls from the student information system, transforms data, and pushes to the gradebook is not a personal automation — it is district-adjacent infrastructure. Run it past IT.
- Disclose when appropriate. If students interact with a teacher-built AI-coded artifact, the disclosure norms from Chapters 7, 13, and 14 apply.
- Keep a copy of the spec. Spec plus generated code, dated, with the assistant noted. This is the equivalent of keeping a lesson plan: a record of what was deployed and why.

The specific FERPA criteria for AI-assisted teacher-built tools vary by district and state interpretation and are referred to district counsel, not asserted here. *[verify with district counsel]* The full treatment of the legal questions is in the $1 Kindle companion *Coding with AI*. The principle — the teacher who deploys owns the deployment — is reportable as a principle.

---

## 4. Worked example: the missing-assignments emailer

Take one concrete teacher specification and walk it through end to end. The shape: a script that reads a CSV of students and their missing assignments and produces a draft email for each parent — anonymized before any AI interaction is involved.

### The bad spec

A reasonable first attempt:

> *Make me a script that emails parents about missing assignments.*

If you hand this to an AI coding assistant, you will get back code. The code will run. It will look professional. It will also be wrong, because it has no idea: what columns the CSV has, what counts as a missing assignment, what tone the emails should have, who *sends* the emails, what to do with families whose contact information is missing, whether to email the student too, what to do about students whose grades are merely low rather than absent, what to do about FERPA. The model will guess on each of these. Some guesses will be invisible to you.

### The good spec

```text
INTENT:
  Produce a per-student draft email summarizing missing assignments,
  ready for me to review and send. The drafts must be reviewed by me
  before any email is sent. The script does not send email.

INPUT:
  A CSV named "missing.csv" with these columns:
    student_pseudonym  — a code I have assigned (NOT a real name)
    parent_pseudonym   — a code for the parent (NOT a real name)
    assignment_name    — string
    due_date           — YYYY-MM-DD
    days_overdue       — integer

OUTPUT:
  A single file "drafts.txt". One block per student. Each block:
    To: [parent_pseudonym]
    Re: missing work for [student_pseudonym]
    Body: warm, factual, three sentences max, lists assignments
          with due dates. No grade information. No
          characterization of the student's character or effort.
  Blocks separated by a line of dashes.

CONSTRAINTS:
  - No network calls. Script runs entirely locally.
  - No external libraries beyond Python standard library.
  - Skip any student whose days_overdue < 3.
  - If parent_pseudonym is blank, skip that row and log it to
    a separate file "missing_contacts.txt".
  - Handle apostrophes and accented characters in pseudonyms
    correctly. (Example pseudonyms I will use: "Student_OB",
    "Student_DAng".)
  - Trim leading and trailing whitespace from every CSV field.

SUCCESS CRITERIA:
  Tested against my hand-prepared test file "test_missing.csv"
  with 5 rows, the output drafts.txt contains exactly 3 blocks
  (the other 2 should be skipped: 1 below threshold, 1 missing
  parent code), and missing_contacts.txt contains exactly 1 row.

EXCLUSIONS:
  - Do NOT include grade letters or numeric scores.
  - Do NOT include the student's real name or the parent's real
    name. The CSV contains pseudonyms only.
  - Do NOT call any AI service or any external API.
  - Do NOT impute missing data.
```

That is a specification. It contains all five Botspeak components: intent, constraints, success criteria, exclusions, output format. It anchors anonymization at the *spec* level (pseudonyms only). It anchors edge cases (apostrophes, blanks, whitespace) in advance, not after the script breaks on Ms. O'Brien.

### What the AI returns

The assistant produces about thirty lines of Python. You do not read those thirty lines. You save the file and run it on `test_missing.csv`.

### The verification

- **Spec pass.** You open `drafts.txt`. You count three blocks. You read each one. The third block says: *Re: missing work for Student_OB.* The apostrophe-style pseudonym handled correctly. Good.
- **Edge pass.** You open `missing_contacts.txt`. One row, the one with the blank parent code. Good. Now you try a fresh test file where every row has `days_overdue = 1`. Output: empty `drafts.txt`. Correct behavior. You try a file with two hundred rows. It still works. You try a file where one row has `days_overdue` as the string `"five"` instead of an integer. It crashes with a clear error. Acceptable — better than silent nonsense.
- **Wrong-input pass.** You try a file that does not exist. Clear error, no output. Good. You try an empty file. Clear error, no output. Good.
- **Privacy pass.** You ask the assistant: *Does this script make any network calls?* It answers no, lists the standard-library imports, confirms no external APIs. You verify by running the script with your laptop's Wi-Fi off — it still runs. Good.
- **Sentinel pass.** You insert one row whose draft you have hand-written in advance. The script's output for that row matches yours. Good.

### The lesson and its limit

What made the script work was the specification, written carefully, *before* the model wrote a line of code. What made it safe was the verification protocol, run by hand on a small synthetic file. Neither required the teacher to read a single line of Python.

Here is the limit. The specification cannot substitute for knowing what the spec needs to say. The teacher who wrote *"Skip any student whose days_overdue < 3"* knew that two-day-overdue assignments were not yet a parent-email-trigger in her class. The teacher who wrote *"No grade information. No characterization of the student's character or effort"* knew the difference between a factual communication and one that hardens into a record. Those are professional judgments the AI does not have. The specification is the place where professional judgment enters the workflow. If the judgment is missing, the spec is missing it, and no model can supply it for you.

---

## 5. Common misconceptions

**Misconception 1: "AI writes safe code."**

The most-cited study on AI coding assistants — [Peng et al. 2023](https://arxiv.org/abs/2302.06590) — measured *time-to-complete on a clearly specified task*. It did not measure safety, security, or quality. Subsequent studies have. [Veracode 2025](https://www.veracode.com/blog/ai-generated-code-security-risks/) reports roughly 45% of AI-generated samples contain at least one OWASP Top 10 security flaw. [arXiv:2510.26103](https://arxiv.org/pdf/2510.26103) reports language-stratified vulnerability rates in the high single digits to high teens. And the user-study finding worth repeating: developers using AI assistants both produced less secure code *and rated it more secure than the controls' code.* The fluency-confidence trap from earlier chapters reappears here. Speed is real. Safety is a different measurement. Do not assume one implies the other.

**Misconception 2: "If it runs, it's right."**

A script that runs without crashing is a script that *ran without crashing*. Whether it computed the right answer is a separate question answered only by hand-checking outputs against the spec. The most dangerous AI-generated failures are silent — they produce plausible nonsense the teacher cannot distinguish from correct output. *Ran* ≠ *worked*. *Worked* ≠ *safe*.

**Misconception 3: "I don't need to understand what the AI built."**

If you cannot describe what the tool does — what data it touches, what files it creates, what services it calls, how it behaves on missing input — you cannot deploy it responsibly. The verification protocol substitutes for code-reading. It does not substitute for understanding *behavior*. If you cannot answer "what does this tool do?" you are not yet ready to deploy.

**Misconception 4: "Teacher-built tools are exempt from district privacy rules."**

[FERPA](https://studentprivacy.ed.gov/ferpa) and related state laws apply to identifiable student information regardless of who wrote the script that handles it. A district that prohibits uploading student names to ChatGPT also prohibits uploading them to a cloud coding assistant. The tool's authorship is not the relevant question. The data it touches is. *[verify with district counsel]*

**Misconception 5: "I should learn Python first."**

For most teacher use cases this is backward. The bottleneck is not your lack of syntax fluency — it is your specification fluency. Time spent learning Python returns less than time spent learning to write a precise paragraph describing what a tool should do. (Teachers who want to *teach* coding to their students still benefit from syntax fluency. Different goal, different chapter.)

---

## 6. Exercises

**Exercise 1 — Write a workflow automation spec.**

Pick one recurring spreadsheet task you do by hand each week. Using the five-component template below, write a 100–200-word specification for it. Do not yet generate code. Trade the spec with a colleague (or paste it into a fresh AI chat and ask the assistant to describe back what it would build). If their description does not match what you want, the spec is not yet a spec.

```text
WORKFLOW AUTOMATION SPECIFICATION
INTENT:        [What the script is for. Why you want it.]
INPUT:         [Filename, columns, types, where it comes from.]
OUTPUT:        [Filename, structure, format. What goes in it.]
CONSTRAINTS:   [No network calls / library limits / runtime / locale /
                special characters / row volume.]
SUCCESS CRITERIA:
               [How you'll know it worked. 3 hand-computed test cases.]
EXCLUSIONS:    [What it must NOT do. What it must NOT include.
                What data it must NOT touch.]
```

**Exercise 2 — Verify against three edge cases.**

Take the spec from Exercise 1 and an AI-generated implementation of it. Design three edge cases the spec does not explicitly handle — a blank field, a special character (apostrophe, accent, em-dash), an unusually large input. For each, predict the output *before* you run, then run and compare. The cases where prediction diverges from reality are the spec's missing clauses. Update the spec. Regenerate. Test again.

**Exercise 3 — Design a deployment checklist for a student-facing AI-built tool.**

Imagine you have built an interactive practice tool (similar in shape to Ms. R's polynomial visualizer) that students will use during a lesson. Write a one-page deployment checklist that covers: anonymization (what student data, if any, the tool touches); environment (which device, which browser, whether internet is required); privacy surface (does the tool phone home? log anything? require accounts?); failure mode (what happens if the tool crashes mid-lesson?); documentation (what you would save so a colleague could re-deploy it next year); and disclosure (what you would tell students about the tool's origin). Then take the checklist to a colleague — ideally one who can read code — and walk through it together.

**Optional extension — Specification template for interactive tools.**

```text
INTERACTIVE TOOL SPECIFICATION
INTENT:           [What this should help a student do or see.
                   Which specific concept it teaches.]
ENVIRONMENT:      [Single HTML file? Web page? Runs offline?
                   Which device? Which browser?]
INPUTS:           [What the user can change. Sliders? Buttons?
                   Text fields? Ranges? Step sizes?]
OUTPUTS:          [What the user sees update. Graph? Text? Both?
                   How fast? What gets labeled?]
PEDAGOGICAL CONSTRAINTS:
                  [What the tool must show / must not show
                   so the demo lands the right point.
                   Example: "show roots, not derivative."]
TECHNICAL CONSTRAINTS:
                  [No external libraries requiring internet.
                   No analytics. No data collection.
                   Works on the classroom Chromebook.]
SUCCESS CRITERIA: [Three configurations you have worked the
                   expected display for. Confirm match.]
EXCLUSIONS:       [No student data collection.
                   No account creation. No external services.]
```

---

## 7. What would change my mind

A randomized study of K–12 or higher-ed teachers — non-programmers — who built and deployed AI-coded classroom or workflow tools, measuring both deployment-time defect rates (functional and privacy) and student-facing-incident rates over a full school year, with effects compared to teachers using off-the-shelf tools for the same purposes. If such a study found that the specification-and-verify protocol described in this chapter did *not* reliably catch the privacy and behavioral defects that current security literature documents, I would revise the chapter's central claim that careful specification plus behavior-level verification is sufficient. As of May 2026, no such study exists.

## 8. Still puzzling

*Maintenance.* What happens to a teacher-built script when the teacher leaves the school? The public literature on this question is essentially silent. *Cost.* Whether a public-school teacher can sustainably afford a coding-assistant subscription, and whether districts will procure them at scale, is a real practical question this chapter does not answer. *Special education.* AI-coded tools used in IDEA-covered contexts may carry obligations beyond FERPA — procedural safeguards, native-language access, IEP-specific clinical review — and the district-counsel referral above does not fully address them.

---

## Bridge to Chapter 12

Chapters 1 through 9 named the six recurring tasks where AI delivers the most time back to teachers. Chapters 10 and 11 extend that frame into writing and coding — terrain where the AI changes what is possible, not just what is faster. Chapter 12 puts all of it together: the prompt library, the weekly workflow, the personal system that turns ad hoc time savings into the systematic deployment ceiling the book has been pointing at since Chapter 1.

---

## $1 Kindle Companion

This chapter is the introduction. The full treatment — extended specifications, debugging when the assistant gets stuck, district-IT conversations, deployment patterns, the longer FERPA discussion, and worked examples of the harder tools (gradebook glue, mail-merge with translation, multi-page interactives) — is in **Bear Brown & Company's $1 Kindle companion *Coding with AI***. The companion is built for the teacher who finishes this chapter and wants to go further than one weekend's automation.

---

**Tags:** specification, end-user programming, computational thinking, AI coding assistants, FERPA, teacher workflows, verification protocol

---

## References

- Karpathy, A. (2025, February 2). "Vibe coding" [X post]. [x.com/karpathy/status/1886192184808149383](https://x.com/karpathy/status/1886192184808149383).
- Karpathy, A. (2025, December). *2025 LLM Year in Review*. [karpathy.bearblog.dev/year-in-review-2025/](https://karpathy.bearblog.dev/year-in-review-2025/).
- Karpathy, A. (2026, February). One-year retrospective on vibe coding [X post]. [x.com/karpathy/status/2019137879310836075](https://x.com/karpathy/status/2019137879310836075).
- K–12 Computer Science Framework Steering Committee (ACM, Code.org, CSTA, Cyber Innovation Center, NMSI). (2016). *K–12 Computer Science Framework*. [k12cs.org](https://k12cs.org/).
- Ko, A. J., Abraham, R., Beckwith, L., Blackwell, A., Burnett, M., Erwig, M., Lawrance, J., Lieberman, H., Myers, B. A., Rosson, M. B., Rothermel, G., Scaffidi, C., Shaw, M., & Wiedenbeck, S. (2011). "The State of the Art in End-User Software Engineering." *ACM Computing Surveys*, 43(3), Article 21, 1–44. [DOI 10.1145/1922649.1922658](https://dl.acm.org/doi/10.1145/1922649.1922658). [MIT Media Lab PDF mirror](https://web.media.mit.edu/~lieber/Publications/End-User-Software-Engineering.pdf).
- Peng, S., Kalliamvakou, E., Cihon, P., & Demirer, M. (2023). "The Impact of AI on Developer Productivity: Evidence from GitHub Copilot." arXiv:2302.06590. [arxiv.org/abs/2302.06590](https://arxiv.org/abs/2302.06590).
- Perry, N., Srivastava, M., Kumar, D., & Boneh, D. (2023). "Do Users Write More Insecure Code with AI Assistants?" *Proceedings of ACM CCS 2023*. arXiv:2211.03622. [arxiv.org/abs/2211.03622](https://arxiv.org/abs/2211.03622).
- Stiefel, A. (2025, July 9). "Understanding Security Risks in AI-Generated Code." *Cloud Security Alliance Blog*. [cloudsecurityalliance.org/blog/2025/07/09/understanding-security-risks-in-ai-generated-code](https://cloudsecurityalliance.org/blog/2025/07/09/understanding-security-risks-in-ai-generated-code).
- U.S. Department of Education. *Family Educational Rights and Privacy Act (FERPA)*. [studentprivacy.ed.gov/ferpa](https://studentprivacy.ed.gov/ferpa).
- Veracode. (2025). *2025 GenAI Code Security Report*. [veracode.com/resources/analyst-reports/2025-genai-code-security-report/](https://www.veracode.com/resources/analyst-reports/2025-genai-code-security-report/); [veracode.com/blog/genai-code-security-report/](https://www.veracode.com/blog/genai-code-security-report/).
- Wing, J. M. (2006). "Computational Thinking." *Communications of the ACM*, 49(3), 33–35. [DOI 10.1145/1118178.1118215](https://dl.acm.org/doi/10.1145/1118178.1118215). [CMU PDF](https://www.cs.cmu.edu/~wing/publications/Wing06.pdf).
- "Security Vulnerabilities in AI-Generated Code: A Large-Scale Analysis of Public GitHub Repositories." (2025). arXiv:2510.26103. [arxiv.org/abs/2510.26103](https://arxiv.org/abs/2510.26103).

---

*Draft for review. Nik Bear Brown, May 2026.*
