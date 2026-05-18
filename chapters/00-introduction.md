<!--
    00-introduction.md
    INTRODUCTION — Chapter 0 / roadmap chapter.
    Reader's roadmap. What the book argues. How it is organized.
    The Preface (in 00-frontmatter.md) says why I wrote it.
    This chapter says what it does, who it is for, and how to read it.
-->

# Introduction

## Two numbers

Students who used AI during math practice scored 48% higher than the control group during the practice session. They scored 17 percentage points lower on the exam.

Same students. Same material. Same teacher. Two numbers, one week apart. The first looked like AI was working. The second was the cost of believing it.

This is the Bastani et al. (2025) finding — n ≈ 1,000 Turkish high schoolers, three arms, randomized — and it is the single result every teacher should carry into every decision they make about AI this year. Not because it tells you to ban AI. It doesn't. There was a third arm of the study, GPT Tutor, where students used a version of the AI built with phase gates that made it refuse to give direct answers. That arm scored 127% higher in practice *and* held its exam score. Same tool. Different design. Opposite outcome.

The difference between the arm that lost 17 points and the arm that did not was not how much AI the students used. It was where the AI was allowed to stop and where the human cognitive work had to begin.

That boundary has a name in this book: the **phase gate**. Locating it correctly, then enforcing it, is the entire skill.

## The gap this book fills

This book is about the gap between *AI for education will save teachers time* (true, in a specific way) and *AI for education will improve learning* (true only when the phase gate is in the right place). The hype industry sells the first as if it implied the second. The research industry has shown the implication is false. There is no book between them written for teachers who do not have time to read either.

This is that book.

## The central argument

Three claims, none of them obvious, all of them contestable:

1. **Frictional is the biology.** Learning is a physical event triggered by cognitive friction. Remove the friction, remove the trigger. This is why the Bastani finding is so precise — not slightly worse, *dramatically* worse — and why the Kosmyna MIT EEG data showed reduced neural connectivity during AI-assisted writing relative to unassisted writing. The mechanism is not metaphorical.

2. **Phase gates are the biology made operational.** They specify exactly where AI stops and human cognitive work begins. Not "use AI responsibly" — *a specific gate, a specific trigger, a specific consequence for crossing it.* The gate is the structural commitment that protects the learning event. Twelve gates organize the practical work of this book.

3. **Humans + AI is the design principle.** Not less AI — *better placement* of AI. AI does what AI does well (structure, retrieval, scaffolding, practice problems, calibration) so humans can do what only humans can do (form judgments, build relationships, struggle toward understanding, construct original arguments, teach).

You will hear all three of these contested over the next few years. Settled science changes; framework names change. What is most likely to survive is the three-line version at the very end of this introduction. Carry that into the chapters.

## Who this is for

You are a teacher. K-12 or higher ed; subject does not matter. You have heard that AI can save time and you are skeptical of both the hype and the fear. You have probably tried one or two tools. You have not had formal training. You do not have a programming background and you do not want one.

You want practical answers. Which of *my* tasks should I delegate? How do I delegate them without breaking my own pedagogy? What do I protect? And — when district admins or parents or students ask — what do I say?

This is that teacher's book.

## What this book IS

This book is a practitioner handbook. It is organized around tasks, not technologies. Each chapter takes one high-time-cost recurring task in your week — lesson planning, grading and feedback, differentiation, parent communication, slides, charts, writing instruction, computational tools — and gives you the framework for which parts AI handles, which parts you handle, the exact prompts to use, and the time-recovery you can reasonably expect.

It is also, underneath, a pedagogy book. It teaches a vocabulary: *phase gate*, *AI-survivable assignment*, *PCK gap*, *fluency trap*, *capability-building vs capability-borrowing*. Without that vocabulary, the prompt templates are just recipes. With it, they become decisions you can defend.

The chapters are self-contained. Read them out of order. Read just the three you need. The framework holds.

## What this book IS NOT

It is not a tutorial on a specific tool. The platforms named here (Claude, ChatGPT, Gemini, NotebookLM, MagicSchool, Khanmigo, Diffit, Brisk) will change. Some will not exist in three years. The principles — what the prompt has to specify, where the gate has to sit, what the teacher has to verify — will outlive them.

It is not a philosophy book. The full theoretical framework — the neurobiological basis, the seven friction-trace components, the formal model of Genuine Learning Probability — is in Appendix G for readers who want it. The fourteen chapters do not require it.

It is not a policy document. School-level and district-level guidance is mentioned where it matters (FERPA, COPPA, IDEA, state AI policies), but specific compliance decisions defer to your district counsel, your special-education team, and your union representative. The book gives you principles strong enough to ask the right questions.

It is not a book about replacing teachers. Reading this carefully will not make you redundant; it will make you the one your students need more.

**Prerequisites:** computer literacy (email, word processing, your district's learning management system). One AI tool you have at least tried. A real class, real students, a real workweek that is already too long.

**Not assumed:** programming, data science, statistics, or any structured AI training.

## A central concept that runs throughout

The recurring idea worth watching across every chapter is the **phase gate**.

Every task chapter has one. The chapter on grading has *rubric calibration before bulk processing*. The chapter on differentiation has *anonymization before any external AI*. The chapter on writing instruction has *the AI-survivable assignment*. The chapter on slides has *the five-question diagnostic*. The chapter on communication has *teacher drafts the core for any sensitive message*.

When you finish the book, the prompts will fade from memory. The gates will not. They are the part you will carry.

## A running thread

One thread recurs across chapters: a teacher I'll call Maya. (She is composite — drawn from real classrooms but no individual.) Maya teaches 6th-grade science. Maya has 28 students who read at levels ranging from 3rd to 10th grade. Maya has three ELL students and two students on IEPs. Maya has a partner, a kid, a Sunday afternoon that used to belong to lesson prep and now sometimes belongs to her again. You will meet Maya in Chapter 1 doing a workweek audit. You will meet her again in Chapter 6 generating five Lexile versions of a reading passage in twelve minutes. You will meet her in Chapter 13 redesigning an assignment that her students cannot pass by AI alone. The framework is general. Maya is the specific case where it lands.

## How this book is organized

Three parts. Fourteen chapters. The Preface and Appendix G frame the argument; the chapters do the work.

**Part I — The Framework (Chapters 1–3).** The argument and the foundation skill.

- **Chapter 1 — The AI Dividend.** What the research actually says about teacher time savings (5.9 hours/week is the floor) and what the systematic ceiling would look like (a projected 16.7 hours, not yet measured). The honest version of the number, and the task taxonomy that earns it.
- **Chapter 2 — The Phase Gate.** The twelve gates. Where AI stops, where you begin, what crossing the gate costs. The chapter that makes everything else operational.
- **Chapter 3 — Prompting That Works.** The four-component template (role, context, task, constraints) and the iterative loop. Not a magic-phrase tour; the structural skill that makes the rest of the book usable.

**Part II — Core Tasks (Chapters 4–9).** The six task areas that cover the most teacher hours.

- **Chapter 4 — Lesson Planning.** AI generates structure; you bring the pedagogical content knowledge (PCK) that AI cannot have. NFER/EEF RCT evidence anchors the time-savings claim.
- **Chapter 5 — Assessment, Grading, and Feedback.** The rubric calibration gate. The four failure conditions for AI grading. The Bastani parallel applied to feedback at the student level.
- **Chapter 6 — Differentiation.** Lexile, scaffolds, IEP/504 — what AI proposes and what licensed humans must authorize. The anonymization gate that protects FERPA compliance.
- **Chapter 7 — Communication.** Parent notes, meeting summaries, behavioral reports. The routine-vs-sensitive split, and the translation accuracy problem nobody warns you about.
- **Chapter 8 — Slides.** The slideument problem (Reynolds), Mayer's Redundancy Principle, and the five-question diagnostic for telling a slide that teaches from one that merely displays.
- **Chapter 9 — Graphs and Data Visualizations.** Cairo's "compared with what?" <!-- FACT-CHECK FLAG: UNVERIFIED — see factchecks/00-introduction-assertions.md (phrase more commonly attributed to Tukey/Tufte; verify Cairo attribution in chapter 9) --> The truncated y-axis problem in education data. Why bar charts of means hide the equity story.

**Part III — Implementation and Integrity (Chapters 10–14).** What to do with the time, and how to run the system honestly.

- **Chapter 10 — Writing with AI.** Teacher writing (AI reduces workload) vs writing instruction (AI changes what must be taught). Three instructional uses: Socratic AI, feedback AI, elaboration AI. Points to the $1 Kindle companion *Writing with AI*.
- **Chapter 11 — Coding with AI.** Specification, not syntax. How a non-coding teacher builds workflow automations and interactive tools. The accountability principle. Points to the $1 Kindle companion *Coding with AI*.
- **Chapter 12 — Building Your AI Workflow.** The synthesis chapter. The prompt library, the weekly schedule, the platform strategy. Two teachers, same tools, very different outcomes — and what separates them.
- **Chapter 13 — Academic Integrity, Privacy, and Honest Use.** The Bastani finding in full. The AI-survivable assignment framework. Why detection-and-discipline is the wrong design move.
- **Chapter 14 — What to Tell Your Students.** Capability-building vs capability-borrowing. The Feynman test. The performance-paradox demonstration. The student-facing version of the whole argument.

The Conclusion frames what the book gets right (the 5.9-hour finding) and what remains hypothesis (the 16.7-hour ceiling, the longitudinal effect on learning). The seven appendices are reference material: the full phase-gate map, fifty starter prompts, the diagnostic checklists, the research bibliography, the series map, the deployable Claude Project that operationalizes the framework as an AI assistant, and the *Frictional* theoretical foundation.

## How to read this book

Read the Preface and this Introduction in order. Then choose:

- **Linear path.** Read the chapters in order. The framework builds. By Chapter 12 you can build a workflow; by Chapter 14 you can teach the framework to students.
- **Task-first path.** Skim Chapters 1, 2, and 3, then jump to whichever task is consuming your week. The chapters are self-contained. Every chapter restates the gate it depends on so you don't have to flip back.
- **Skeptic's path.** Read the Preface, Chapter 2, Chapter 13, and Appendix G. If the argument holds for you there, the rest is implementation. If it does not, you'll have read enough to argue with the book honestly.

Every chapter ends with two recurring features. **What would change my mind** names the specific empirical finding that would force the chapter's argument to revise. **Still puzzling** names two-to-four open questions the chapter raises but cannot resolve. Read these. They are where the book is honest about its own limits.

Exercises are graduated. Warm-up exercises check whether you understood. Apply exercises produce something you can use tomorrow. Synthesis and challenge exercises ask you to do the thing the chapter taught for a specific case in your own classroom.

If you read no other chapter, read Chapter 2. Everything depends on it.

## A note about AI in this book

This is a book about AI in teaching. It would be dishonest if I did not say how AI was used to make it.

Drafts of every chapter were produced with the assistance of large language models (Claude primarily, GPT-class models for specific cross-checks). The research notes in the pantry — chapter-by-chapter source synthesis — were assembled with AI assistance from a corpus I curated. The book's own architecture (the four-component prompt template, the twelve phase gates, the AI-survivable assignment checklist, the capability-building/borrowing distinction) is original. The voice — the choice of where to be Feynman-flavored, where to soften, where to flag a number as projected rather than measured — is mine.

Every contestable factual claim in the chapters carries a citation to a primary source. Where a number could not be verified to a primary source, the draft was flagged `[verify]` rather than published. The Bastani 2025 numbers, the Gallup/Walton 2025 5.9-hour finding, the NFER/EEF 31% lesson-prep RCT, the Kosmyna 2025 MIT EEG study — each is traced to the publication, with the constraints and methodology the publication actually reported, not the headline-version. Where a vendor accuracy number was current as of one press release and stale as of the next, the chapter cites the institutional retreat (OpenAI withdrawing its AI text classifier in July 2023; Vanderbilt deactivating Turnitin's AI detection in August 2023) rather than the vendor figure.

I held to four phase gates while drafting:

1. **Rubric calibration.** Every chapter was read against the workshop's voice rules and the book's hard rules (no fabricated sources, primary sources only, every contestable claim cited or `[verify]`-flagged, mechanism shown not gestured at). The pass was mine, not the model's.

2. **Content accuracy.** Every quoted study was cross-checked against the published version where I could obtain it, and flagged where I could not. The Bastani correction in August 2025 — affiliation-only, non-substantive — is named honestly in Chapter 13.

3. **PCK selection.** The analogies, the named misconceptions, the worked examples that pivot on what students actually get wrong — those came from teaching, not from a model. A model that has not stood in front of a classroom does not know which misconception your students carry into Tuesday's lesson. I do, and where I do not, I named the gap.

4. **Anonymization.** No student work, no district data, no parent communication, no individual teacher's identifiable case is in this book without consent and labeling. The composites (Maya, the 11:42 p.m. deck, the community college instructor with 270 essays) are drawn from real patterns and labeled as composites.

That is the book's own phase-gate map. It is the same one I am asking you to use.

This matters because *how* the book was made is part of what the book is teaching. If the argument is that AI without phase gates harms learning, then producing a book about AI without phase gates would refute the argument by example. The chapters cite, the composites are labeled, the numbers are bounded, the gates are honored. If you find a place where they were not, that is a serious complaint and I would like to know about it.

## Closing

The teacher I started with — the one whose students lost 17 points on the exam — is not a villain. She used the tool the way she was told to use it. She did what most teachers will do this year unless someone gives them a different framework.

This book gives you the different framework.

Six hours a week back to teaching. Here is exactly which tasks to delegate, how to delegate them, and what you must never hand off.

The three lines that are the whole argument:

> AI removes the struggle that triggers learning.
> The phase gate specifies where the struggle must be human.
> Humans + AI means AI does AI things so humans can do the irreplaceable human things — not less human involvement, but better human involvement in the right places.

Let's go.

---

## References

1. Bastani H., Bastani O., Sungu A., Ge H., Kabakcı Ö., Mariman R. *Generative AI without guardrails can harm learning: Evidence from high school mathematics.* PNAS, 2025. https://www.pnas.org/doi/10.1073/pnas.2422633122
2. Correction for Bastani et al. (affiliation only). PNAS, 122(34), August 2025. https://www.pnas.org/doi/10.1073/pnas.2518204122
3. Kosmyna N., Hauptmann E., Yuan Y. T., Situ J., Liao X., et al. *Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an AI Assistant for Essay Writing Task.* MIT Media Lab / arXiv:2506.08872, 2025. https://arxiv.org/abs/2506.08872
4. Walton Family Foundation & Gallup. *Teaching for Tomorrow: Unlocking Six Weeks a Year With AI.* 2025. https://static.waltonfamilyfoundation.org/df/fb/eba12807470a9402d7433cc47dba/teaching-for-tomorrow-unlocking-six-weeks-a-year-with-ai-report.pdf
5. NFER / Education Endowment Foundation. *ChatGPT in lesson preparation: A Teacher Choices Trial Evaluation Report.* 2024. https://www.nfer.ac.uk/publications/chatgpt-in-lesson-preparation-a-teacher-choices-trial/
6. OpenAI. *New AI classifier for indicating AI-written text* (post with July 20, 2023 withdrawal notice). https://openai.com/index/new-ai-classifier-for-indicating-ai-written-text/
7. Vanderbilt University, Brightspace. *Guidance on AI Detection and Why We're Disabling Turnitin's AI Detector.* August 16, 2023. https://www.vanderbilt.edu/brightspace/2023/08/16/guidance-on-ai-detection-and-why-were-disabling-turnitins-ai-detector/
8. Reynolds G. *Presentation Zen* — slideument concept. https://www.presentationzen.com/presentationzen/2008/04/your-moment-of.html
9. Mayer R. E. (ed.) *The Cambridge Handbook of Multimedia Learning* — Redundancy Principle chapter. Cambridge University Press.

---

**Tags:** AI in education · K-12 teaching · higher education · pedagogical content knowledge · phase gates · Frictional framework · Bastani 2025 · lesson planning · grading · differentiation · academic integrity · AI-survivable assignments · capability-building · prompt engineering · teacher workflow · practitioner handbook
