# Chapter 14 — What to Tell Your Students: AI Literacy in the Classroom

<!-- FACT-CHECK FLAG: MIXED — see factchecks/14-what-to-tell-your-students-assertions.md. Three citation issues need attention before classroom use: (1) Bastani 2025 magnitude is "17% relative reduction," not "17 percentage points" (line 78); (2) Lachner, Ly, & Nückles 2018 direction is INVERTED in the chapter (paper found written > oral, not oral > written, line 122); (3) Lachner, Jacob, & Hoogerheide 2021 [Learning and Instruction] direction is INVERTED (paper did NOT find imagined-audience > self-explaining for written modality, line 122). Minor: Fiorella & Mayer 2016 list substitutes "explaining" for "enacting." -->

**TL;DR.** Students already use AI; the question is whether the use builds a capability in their own heads or borrows one from a server, and the distinction is teachable. This chapter gives you the vocabulary (capability-building vs. capability-borrowing), the empirical anchor (Bastani et al. 2025), the three classroom uses that build rather than borrow, and one demonstration activity that lets students feel the gap with their own results in their hands.

---

## Suggested titles

1. What to Tell Your Students: AI Literacy in the Classroom
2. Building, Not Borrowing: A Teachable Framework for Student AI Use
3. The Question Your Students Are Already Asking: How Do I Use AI to Learn?

---

## 1. Learning objectives

By the end of this chapter you will be able to:

1. **Define** the capability-building vs. capability-borrowing distinction and explain it to a student in two sentences.
2. **Explain** the Bastani et al. (2025) finding in plain language — including why the prompt, not the tool, determined whether learning was harmed or preserved.
3. **Teach** three capability-building AI uses students can run on their own: Socratic questioning, deliberate practice generation, and the Feynman test conversation.
4. **Apply** Bjork's storage-strength vs. retrieval-strength distinction to diagnose the fluency trap when you see it in a student's work.
5. **Design** the performance-paradox demonstration as a 60–70 minute classroom activity that lets students see the gap between assisted practice and unassisted recall in their own scores.
6. **Adapt** the capability table for K–8, 9–12, and higher-ed contexts.

**Prerequisites.** The Preface (the *Frictional* argument that struggle is the mechanism of learning, not the cost). Chapter 2 (the phase gate as the teacher version of building-vs.-borrowing). Chapter 13 (academic integrity by design). This chapter is the student-facing application of the framework those three already established for you.

**The capability table previewed.** The chapter's central artifact lives in Section 3.7. Six rows. Three building uses on top; three borrowing uses below. The same AI tool can do any row. The difference is which row you are in, and whether you can tell.

---

## 2. Opening case: the message that arrived in my inbox

The message was three sentences. It came from a high schooler I had never met, forwarded by a teacher I had — a science teacher in a public high school outside Boston who runs a "How is your week?" channel for her students that occasionally produces messages too good to keep to herself. She forwarded this one with my name on it:

> *"My friends are using AI to write their papers but I want to use AI to learn and I don't know how. My teachers tell me what not to do with ChatGPT. Nobody tells me what I should do. Is there a right way?"*

I want you to read that again. Notice what is not in it. There is no defiance. There is no question about whether AI is okay. There is no fear of getting caught. The student has already made the decision the academic integrity literature spends most of its energy arguing about: she is going to use AI. The decision in front of her is the one no policy document has answered: *how*.

She is not the student your AI-use policy is written for. The policy is written for her friends. She is the student this chapter is for. And she is, in my experience over the last two years of running professional development for teachers, vastly more common than the AI-skeptic literature acknowledges. The students who are using AI to *avoid* the work get the news coverage. The students who want to use AI to do the work better — to study harder, to find their own gaps, to test themselves more honestly than a textbook chapter allows — outnumber them, and they are getting nothing from us.

This chapter is what I would say to her.

---

## 3. Core concept: capability-building vs. capability-borrowing

### 3.1 The distinction, named

I want to name this distinction precisely because the rest of the chapter rests on it.

**Capability-borrowing** is when you use AI to produce an artifact — a finished essay, a solved problem, a summary of the reading — without doing the cognitive operation that the artifact was supposed to evidence. The artifact exists. The capability does not. Your friend who texts you the answer is doing the same thing as ChatGPT in this mode: producing the deliverable while bypassing the mechanism that would have built the deliverable inside your head.

**Capability-building** is when you use AI as a partner in the cognitive operation that only your own brain can do. The AI is in the room; the work is yours. The AI asks questions you would not have asked yourself. The AI generates practice at the edge of your competence. The AI tells you where your explanation has a hole in it, and refuses to fill the hole. The artifact at the end is sometimes nothing — sometimes a list of things you got wrong. The capability is real.

I want to be clear about what this distinction is *not*.

It is not "human work good, AI work bad." That framing fails immediately at contact with the classroom. A student who looks up the formula for the area of a triangle and uses it has not failed to learn geometry; she has used a reference tool exactly as a working professional would. The question is whether the cognitive operation that *constitutes the learning at her current level* is happening.

It is not "no AI good, lots of AI bad." A student running a Feynman-test conversation with Claude for forty-five minutes is using more AI than a student who pasted a homework problem into ChatGPT and copied the answer. The first student is building. The second is borrowing. Quantity is not the axis. Operation is.

It is not the same as the calculator analogy, and I want to spend a paragraph on why because the analogy is everywhere and it is doing more damage than help. A calculator substitutes for the *execution* of a procedure the student already understands. Long division. Square roots. Trig functions. The cognitive operation of *understanding what you are computing and why* is left intact; only the arithmetic execution is offloaded. AI in capability-borrowing mode does the opposite: it leaves the surface task (the typing, the formatting) to the student and offloads the cognitive process itself — understanding the problem, choosing the approach, reasoning through the unfamiliar. A calculator is a transfer tool. A capability-borrowing AI use is a substitute for the thinking. The analogy works only if you misunderstand what calculators replaced.

This is the framework. Three building uses. Three borrowing uses. Same tool. Different operation. Different brain state at the end.

### 3.2 The empirical anchor — Bastani 2025, in plain language

I want to give you the version of this study I give to a tenth grader, because that is the version you will need.

A research team led by Hamsa Bastani at Wharton ran a randomized experiment with about a thousand high school students in Turkey, studying mathematics ([Bastani et al., 2025, *PNAS*](https://www.pnas.org/doi/10.1073/pnas.2422633122)). Three groups. Group 1 practiced with pencil, paper, and textbook — the way math has been practiced for a century. Group 2 practiced with unconstrained access to GPT-4 — they could ask it anything, including "just solve this for me." Group 3 practiced with a version of GPT-4 that had been wrapped in a pedagogically designed prompt — it was instructed to act like a tutor, to ask questions rather than supply answers, to give hints rather than solutions.

During practice, the unconstrained-AI group dramatically outperformed the no-AI group. Their homework looked better. Their accuracy on practice problems jumped substantially. They felt — and I am inferring from the post-test confidence measures rather than reading their minds — like they were learning faster than the kids working with paper.

Then the researchers gave everyone the same exam without any AI access. And the unconstrained-AI group scored *worse* than the no-AI group by a substantial margin. Better practice scores. Worse exam scores. The same students who had felt fluent during the homework froze on the test, because what they had practiced was not *doing the math* — it was *getting the right answer with ChatGPT's help*. Those are different skills. One transfers to the unassisted exam. The other does not.

The tutor-prompted group landed in a different place. Their practice gains were smaller than the unconstrained group's. Their exam scores were comparable to — and in some specifications, slightly above — the no-AI control. Same model. Different prompt. Completely different learning outcome.

I want to flag the numbers carefully. The published figures are a roughly 48% practice gain and a roughly 17% *relative* exam-score reduction in the unconstrained condition — that is, the GPT Base group scored about 17% lower than the no-AI control on the unassisted exam, not 17 absolute percentage points (the unit matters; earlier drafts of this chapter and several of the secondary summaries that paraphrase the paper get this wrong). The direction of the effect is unambiguous and well-attested across the paper, the working-paper precursor, and the [SRI seminar Bastani gave on the study](https://srinstitute.utoronto.ca/events-archive/seminar-2025-hasma-bastani). Before you put specific percentages in front of a class, verify them against the published paper directly. The qualitative finding — large practice gain, large exam drop, no harm in the tutor condition — is the part that matters and the part I am willing to teach without hedging.

The takeaway for your students is the cleanest sentence in this chapter: **the prompt determines the outcome.** The tool is neutral. Asking the AI to think for you and asking the AI to make you think harder are different cognitive operations with different effects on what ends up in your head, and the difference is large enough to flip you from passing to failing.

### 3.3 Bjork's two strengths — and why fluency lies to you

Here is the piece of learning science that makes the Bastani finding inevitable rather than surprising.

In the early 1990s, Robert Bjork and Elizabeth Bjork proposed that human memory has two distinct parameters that the introspective system cannot distinguish. They called them *storage strength* and *retrieval strength* ([Bjork & Bjork, 1992; framework reviewed in Bjork & Bjork, 2011](https://www.unh.edu/teaching-learning-resource-hub/sites/default/files/media/2023-06/itow-introducing-desirable-difficulties-into-practice-and-instruction-bjork-and-bjork.pdf)).

**Storage strength** is how deeply a piece of knowledge is wired in — how richly connected to other things you know, how durable across weeks and months, how available across surface variations of the problem. This is what you are actually trying to build when you learn something. It is what a teacher hopes is still there when an unannounced quiz lands two weeks later.

**Retrieval strength** is how easily a piece of knowledge comes to mind *right now*. It is the surface feeling of fluency. It is high after re-reading. It is high right after a study session. It is high when the prompt is on the screen in front of you. It does not measure how durable the knowledge is. It measures how accessible it is at this moment.

The Bjorks' central observation is that the conditions that maximize retrieval strength in the short term — re-reading, blocked practice, immediate feedback, smooth path through the material — *do not* maximize storage strength in the long term. The conditions that build storage strength feel worse in the short term: spaced practice, interleaved problems, retrieval before re-reading, generating answers before being told them, struggling for a beat before the help arrives. They called these *desirable difficulties* — counterintuitive on purpose. The discomfort is not the cost of learning. It is the mechanism.

I want to be honest about the evidence here. The *direction* of the desirable-difficulties effect — that conditions which feel harder in the moment tend to produce more durable learning — is one of the most robust findings in modern learning science, with thirty-plus years of converging evidence. The *exact size* of the effect varies by population, material, retention interval, and study. I cite the direction. I do not cite specific effect sizes from any single experiment as if they generalize.

Now bring AI into this. AI is, by design, a fluency machine. Its outputs are smooth, well-organized, grammatically clean. When a student reads an AI explanation, retrieval strength rises fast — the material feels familiar, the words are crisp, the logic seems clear. The introspective system reports *I understand this*. Storage strength has not moved. The student has reread, not retrieved. Two weeks later, on the unassisted exam, the gap shows up.

This is what the Bastani study measured. The unconstrained-AI group raised their retrieval strength dramatically — they could do problems with the AI present because retrieving the next step from a chat window is easy. Their storage strength never built, because they never had to generate the next step from their own memory. The exam without AI is a storage-strength test. The homework with AI is a retrieval-strength fiction.

Call this the **fluency trap**: smooth output produces a feeling of understanding the brain has not earned. The trap is what makes the Bastani gap inevitable. It is also what makes the gap invisible to the student until exam day, by which point they cannot fix it.

### 3.4 Retrieval practice — Roediger and Karpicke, and why testing yourself is learning

If the Bjorks' framework is the diagnosis, retrieval practice is the prescription that comes out of the same literature.

Henry Roediger and Jeffrey Karpicke ran what is now the canonical study in 2006 ([Roediger & Karpicke, 2006, *Psychological Science*](https://pubmed.ncbi.nlm.nih.gov/16507066/)). Students read a passage. One group then re-read it three more times. Another group read it once and took recall tests. Five minutes after the session, the re-readers outperformed the testers. Confidence followed performance: the re-readers felt they had learned more, and they had — at five minutes. A week later, the result reversed and the gap widened. The testers remembered substantially more than the re-readers. The same year, Roediger and Karpicke published the integrative review ([*Perspectives on Psychological Science*, "The Power of Testing Memory"](https://www.psy.gla.ac.uk/~chrisd/papers/RoedigerKarpicke2006.pdf)) that put the finding in front of educators.

The mechanism is the one Bjork's framework predicts. Re-reading raises retrieval strength fast. The recognition feeling at five minutes is real. Storage strength was built by the *act of attempting retrieval* — pulling the information out of memory rather than pushing it back in. A week later, retrieval strength has decayed in both groups, but only the testers had the underlying storage strength to compensate.

Karpicke and Blunt later showed that this effect is large enough to beat elaborative study methods — including concept mapping, which is *itself* a strong study technique. When students were tested on the same material a week later, the retrieval-practice group outscored the concept-mapping group even on tasks that required the student to draw a concept map ([Karpicke & Blunt, 2011, *Science*](https://www.science.org/doi/10.1126/science.1199327)).

The implication for AI literacy is direct, and I want students to hold it in their hands.

If you ask the AI to explain something, the AI does the retrieval. You watch the retrieval happen. Your storage strength does not move. If you ask the AI to *quiz you* — to generate retrieval prompts you have to answer from your own memory — *you* do the retrieval. Your storage strength moves. Same tool. Same chapter. The arrow of cognitive work points the other way.

This is the single highest-leverage piece of student-facing AI literacy in this chapter. You do not have to win the argument about whether AI is good or bad. You just have to teach the difference between *asking the AI to retrieve for you* and *asking the AI to make you retrieve*.

### 3.5 The Feynman test — explanation as generation

The third pillar comes from Richard Feynman, who insisted that the diagnostic for understanding was not recognition, not summarization, not even problem-solving. It was explanation. If you could not explain a concept simply, to someone who did not already know it, in plain language without jargon, you did not yet understand it. The work was to try to explain, notice where you got stuck, go back to the source, repeat.

The learning-science literature has a name for what Feynman was describing. It is called the *generative explanation effect*. When a learner produces an explanation rather than receives one — especially when the explanation is intended for an audience and must be made coherent — the cognitive operations involved produce stronger learning than reading, listening, or self-explaining with notes available. Fiorella and Mayer's review of generative learning collects the eight strategies that share this property: summarizing, mapping, drawing, imagining, self-testing, self-explaining, teaching, and enacting ([Fiorella & Mayer, 2016, *Educational Psychology Review*](https://link.springer.com/article/10.1007/s10648-015-9348-9)). The empirical picture inside that list is more complex than the slogan: Lachner, Ly, and Nückles (2018) found in *written-explanation* conditions that providing written explanations supported deeper conceptual organization than oral explanations ([*Journal of Experimental Education*](https://www.tandfonline.com/doi/full/10.1080/00220973.2017.1363691)), while in *spoken-explanation* and *video* paradigms the social-presence effect of explaining to an imagined or fictitious audience produces mixed results — Lachner, Jacob, and Hoogerheide (2021), for instance, found that writing explanations to a fictitious student did not reliably outperform self-explaining across their experiments ([*Learning and Instruction*](https://www.sciencedirect.com/science/article/abs/pii/S0959475220307337)). The takeaway is the conservative one: *producing* an explanation — in whichever modality is available — drives more learning than *receiving* one, and the modality and audience effects refine that core finding rather than overturn it.

Now put an LLM in that picture. The LLM is the perfect Feynman-test audience. It is patient. It is awake at midnight. It knows the material well enough to notice when your explanation has a gap. It feels lower-stakes than a human listener, which lowers the defensive crouch students go into when they are afraid of looking stupid. Used in this direction — *student explains, AI probes* — the LLM is doing exactly what the generative explanation literature wants the learner to do. The cognitive operation is the student's. The AI is the audience that forces it to be specific.

Used in the other direction — *student asks, AI explains* — the same tool delivers the opposite mechanism. The AI generates. The student recognizes. The fluency trap fires.

I want to give you the exact prompt I give students for the Feynman direction:

> *"I'm going to explain [concept] to you as if you've never heard of it. Your job: every time I use a word that needs to be defined, ask me to define it. Every time I make a claim that needs to be justified, ask me how I know. Don't help me. Don't fill in gaps. Just point to them. After we're done, list every place I got stuck."*

That prompt turns Claude or ChatGPT or Gemini from an answer machine into a Socratic interlocutor. It does not require a special tool. It does not require the student to know any cognitive science. It requires one sentence.

### 3.6 The three capability-building uses, operationalized

The framework collapses to three uses students can run on their own with any current LLM.

**Use 1 — Socratic questioning.** *Ask the AI to challenge your reasoning.* The student states a position; the AI is instructed to argue back, to find weaknesses, to ask "how do you know?" The cognitive operation — defending the position, noticing where the defense is thin — is the student's. The AI is the friction that exposes the gaps. Example prompt: *"I think the French Revolution was caused mostly by Enlightenment ideas. Push back on this. Ask me what I'm missing. Don't tell me the answer."* This is capability-building because it triggers what cognitive scientists call *prediction error* — the moment when what you expected does not match what you encountered, which is the signal that initiates the neurological cascade the Preface described.

**Use 2 — Deliberate practice generation at the edge of competence.** Anders Ericsson's framework for how expertise is built names four conditions: a specific well-defined goal, full concentration, immediate feedback, and operating at the edge of current competence ([Ericsson, Krampe, & Tesch-Römer, 1993, *Psychological Review*](https://psycnet.apa.org/record/1993-40718-001)). I want to be careful here: the "10,000-hour rule" popularization of this work was Gladwell's, not Ericsson's, and the strong version has been substantially complicated by subsequent meta-analyses ([Macnamara, Hambrick, & Oswald, 2014, *Psychological Science*](https://journals.sagepub.com/doi/10.1177/0956797614535810)). The general framework holds; the strong "practice is everything" reading does not. What is left after the caveats is the **edge-of-competence** principle: practice that operates at the level where you fail just often enough to learn from the failure produces more growth than practice in the comfort zone.

This is something a textbook problem set is structurally bad at. The textbook is calibrated to a hypothetical median student. The LLM can be calibrated to *this* student at *this* moment, based on what they just got wrong. Example prompt: *"Generate three integration problems that require u-substitution but at a slightly harder level than basic textbook problems. Don't give me the answers. After I attempt each one, tell me where my approach is wrong but not what the right approach is."* The capability is building because the cognitive operation — selecting the substitution, executing it, recognizing the mistake — is the student's.

**Use 3 — Feynman test conversation.** Described above (Section 3.5). The single most powerful study technique I know of that requires zero teacher infrastructure and zero specialized tools. Worth its own paragraph in the student handout.

The pattern that unites all three: the AI is doing *adjacent* cognitive work — generating questions, generating practice, listening for gaps — while the student does the *load-bearing* cognitive work that builds the storage strength. The AI is making the productive struggle more accessible. It is not removing the struggle.

### 3.7 The capability table

This is the chapter's central artifact. Cut it out. Post it on your classroom wall. Send it home with parents. Hand it to the student in the opening case.

| Student use of AI | Type | Why it works (or fails) |
|---|---|---|
| Ask AI to challenge your reasoning | **Building** | Triggers prediction error; builds the model |
| Ask AI to generate problems at the edge of your competence | **Building** | Creates productive struggle; drives consolidation |
| Ask AI to identify gaps in your explanation (Feynman test) | **Building** | Forces retrieval; reveals what's missing |
| Ask AI to write the first draft | Borrowing | Bypasses the generative struggle that builds schema |
| Ask AI to summarize the reading | Borrowing | Bypasses the deep processing that produces comprehension |
| Ask AI to solve the problem | Borrowing | Eliminates the productive difficulty that constitutes learning |

The same six rows scale from middle school to graduate school. The vocabulary, examples, and the degree of autonomy do not.

### 3.8 Age-appropriate framing

I want to be calibrated about this section because it is the one place where the chapter is extrapolating beyond directly established research. The capability table itself is principled and the building-vs.-borrowing distinction rests on standard learning science (Bjork, Roediger & Karpicke, Ericsson, Lachner) plus the Bastani 2025 empirical anchor. The K–8 deployment recommendations are a translation of that science to ages the science was not specifically validated on. The published frameworks for AI literacy at these ages — UNESCO's *AI Competency Framework for Students* ([UNESCO, 2024](https://www.unesco.org/en/digital-education/ai-future-learning)) and the [AI4K12 initiative](https://ai4k12.org/) — name what students should understand but provide thin empirical evidence about which instructional methods actually produce understanding at which age. The recommendations below are my best reading of the available frameworks plus the underlying cognitive science. Treat them as informed defaults, not as findings.

**K–2 (ages 5–7).** Direct student use of generative AI at this age is not appropriate, and most published guidance agrees. The literacy goal here is *recognition*: this is a machine, not a person; sometimes it gets things wrong. Your job at this level is to model the distinction in your own classroom AI use rather than to teach the student to make it. AI4K12's "Five Big Ideas" framework has K–2 grade-band guidelines for naming what AI is and is not.

**Grades 3–8 (ages 8–13).** The capability-building/borrowing distinction becomes teachable here, in concrete vocabulary. Try: *"AI is a tool that can either help your brain grow or do the thinking for it. When it does the thinking for you, your brain doesn't change. When it makes you think harder, your brain does. Knowing the difference is the skill."* The performance-paradox demonstration (Section 4) is feasible at this age and powerful. The Feynman test prompt works directly. The AI as Socratic interlocutor is age-appropriate in monitored settings.

**Grades 9–12 (ages 14–18).** Full vocabulary. The Bastani study can be taught directly. The Feynman test can be assigned as recurring homework. Students can run the performance-paradox demonstration on themselves and discuss the result honestly. Beth McMurtrie's reporting in *The Chronicle of Higher Education*'s "Teaching" newsletter documents that many high schoolers already self-organize into "use AI for the boring parts, do the hard parts yourself" patterns when given the framework — but most have not been given it. This is the chapter's central audience and the student in the opening case.

**Higher ed.** Same vocabulary; the student is expected to make the choice themselves and to be accountable for the consequence. The framework lands as autonomy rather than instruction. The student-facing companion volume to this book — *How to Learn with AI: A Student's Guide* — is aimed at this audience.

The vocabulary scales. The mechanism — the brain only learns from the work it does itself — does not.

---

## 4. Worked example: the performance-paradox demonstration

This is the activity I have seen land harder with students than any lecture. It is the Bastani finding compressed to a single class period, with the students themselves as the experimental subjects and the result as the lesson. It runs in 60–70 minutes. It requires AI access and a problem set in two isomorphic versions. It works at every level from middle school up.

### 4.1 Setup (15 minutes)

Tell the students what they are doing. Honesty is the design here, not deception. The pitch is: *"We are going to run a small experiment on ourselves today. You're going to do a problem set with AI help, then a different problem set without AI help. We will compare the two scores. The point is not to catch you doing anything wrong. The point is for you to see whether what you can do with AI matches what you can do without it."*

Distribute Problem Set A. It contains six to eight problems on a single concept the class has been working on — for a science class, this might be problems on the relationship between wave properties and energy transmission; for a math class, problems on a specific integration technique; for a history class, short-answer items requiring causal reasoning across a unit. Tell the students they have thirty minutes and full AI access. They may use ChatGPT, Claude, Gemini, whatever is available. They may use it however they want. Their scores on Problem Set A are not for a grade. Their *self-rated confidence* is what you will record.

Hand out a one-line confidence sheet. After they finish, before the test, they rate "How well do I understand this material right now?" on a 1–10 scale.

### 4.2 With-AI practice (30 minutes)

Let it happen. Walk the room. Notice patterns. Some students will offload heavily — paste, copy, submit. Some will use AI as a hint engine. Some will not use AI at all. All three patterns are data. Do not intervene.

At the end of thirty minutes, collect the work and the confidence sheet. Do not grade in front of them. Move directly to the next phase.

### 4.3 Without-AI test (15 minutes)

Distribute Problem Set B. Same difficulty. Same concept. Different surface — different numbers, different domain references, different framing. The cognitive structure is identical to Problem Set A. The recognition pattern is not.

No AI. No notes. No phones. Fifteen minutes.

This is the part where you will see something in the room you may not have seen before. The students who offloaded heavily on Problem Set A will freeze. They felt fluent twenty minutes ago. They have nothing to retrieve, because what they practiced was not the concept — it was the act of getting ChatGPT to produce an answer. The students who used AI sparingly, or as a hint engine, will perform roughly as they did on Problem Set A. The students who did not use AI at all will perform exactly as they did on Problem Set A. Their storage strength is what you are measuring on the second set, and storage strength is what the first phase did or did not build.

### 4.4 Reflection (10 minutes)

Score both problem sets quickly — these are formative, the scoring is rough, the point is the comparison. Hand each student a small card with three numbers: their Problem Set A score, their Problem Set B score, and the gap. Hand them a fourth number: the confidence rating they gave themselves between the two sets.

The reflection prompt is short: *"Look at the gap between your scores. Look at the confidence you reported. What do these three numbers tell you about what you actually learned today versus what you felt like you were learning?"*

Give them five minutes to write. Then discuss as a class. The discussion is the lesson. The numbers do the teaching; you facilitate. The students who got close to a zero gap have evidence that they were genuinely learning with AI. The students who got a large gap have evidence that they were practicing fluency, not capability. Neither result is a verdict on them as students. Both are diagnostic.

### 4.5 Lesson and limit

The lesson is in the room before you say anything. **Practice score and exam score are not measuring the same thing.** The students who confused the two have just felt the confusion in their own scores. The students who did not confuse them have a piece of evidence about their own study habits that no lecture would have given them.

The limit is worth naming explicitly. The demonstration is a single class period on a single concept under controlled conditions. It does not prove anything about AI in general. It produces a *felt* example of the gap the Bastani study measured at population scale. The student now has a personal data point. The Bastani study is the published version of the same phenomenon at a larger N with a randomized design. Both are useful. Neither alone is decisive. Together they teach the principle.

### 4.6 The Feynman test conversation, end-to-end

For the second half of the next class — or as homework if time is short — assign the Feynman test on a concept the students are still developing. I will walk through one example, on a concept that turns up in middle-school and high-school physics: *why a sound wave can carry energy without carrying matter*.

Here is a transcript of the kind of conversation a student should be running. The student is a tenth grader. The AI is Claude. I have abbreviated.

> **Student:** I'm going to explain to you why a sound wave can carry energy without carrying matter. You don't already know this. Stop me when I use words that need defining, and when I make claims that need justifying. Don't help me. Just point to gaps. List the stuck points at the end.
>
> **Claude:** Understood. Go ahead.
>
> **Student:** OK. A sound wave is a vibration that moves through a medium like air. When you clap your hands, the air molecules near your hands push the air molecules next to them, which push the next ones, and so on. So the *push* moves outward but the *molecules* mostly stay where they are.
>
> **Claude:** What do you mean by "vibration"?
>
> **Student:** Like, the molecules move back and forth a little.
>
> **Claude:** Back and forth in what direction relative to the wave's motion?
>
> **Student:** ...the same direction? I think? Like, they get pushed forward and then come back.
>
> **Claude:** That's a claim that needs justifying. How would you know whether they move in the same direction as the wave or perpendicular to it?
>
> **Student:** Uh. Honestly I don't know. I just memorized "longitudinal" but I'm not sure I understand why sound has to be longitudinal.
>
> **Claude:** Marked as a stuck point. Continue.
>
> **Student:** So the energy gets carried by the *pattern* of pushing, not by any individual molecule. The molecules end up roughly where they started.
>
> **Claude:** What is the energy doing during the part where a given molecule is moving forward? What is it doing when the molecule is moving back?
>
> **Student:** ...I think kinetic energy is high when it's moving and there's potential energy stored when the molecules are squished together? Like a spring?
>
> **Claude:** That's a claim that needs justifying. What's the spring made of, in this case?
>
> **Student:** The air. The squished air pushes back. So the air itself is the spring.
>
> **Claude:** OK. Then how does the energy keep moving outward if it's bouncing between kinetic and potential locally?
>
> **Student:** ...because each spring pushes the next spring?
>
> **Claude:** That's a claim that needs justifying. Can you describe what happens at the boundary between one "spring" and the next?
>
> **Student:** I think I'm stuck.
>
> **Claude:** Marked as a stuck point. We have two so far: (1) why sound is longitudinal rather than transverse, (2) how energy propagates from one parcel of air to the next without the parcels themselves moving net forward.

That is what capability-building AI use looks like at the level of a single sentence-by-sentence interaction. Notice what Claude is not doing. It is not explaining. It is not correcting. It is not supplying the answer. It is generating the questions that force the student to either produce or notice the absence of the next piece of the explanation. The student leaves this conversation with two specific gaps to go work on. Those gaps are *more* useful than a finished explanation, because the finished explanation would have been Claude's. The gaps are the student's own.

The lesson here is the one that closes the worked example: the AI was deeply involved. The cognitive work was entirely the student's. That is the operation we want to teach. The same student typing "explain to me why sound waves carry energy without carrying matter" would have gotten a polished paragraph and a fluency-trap feeling. Same tool. Opposite mechanism.

---

## 5. Common misconceptions

I want to name the misconceptions that come up reliably when this framework is taught, because each one fails for a specific reason and the specific reason is the teaching.

**Misconception 1: "AI is a calculator; using it is fine."**

This is the most frequent framing and the most damaging because it sounds reasonable. The argument: calculators did not destroy mathematics education; AI is the same thing one level up.

Here is why it fails. A calculator transfers a *procedural skill* (long division, square root extraction) that the student has been taught to understand conceptually. The cognitive operation of understanding what the calculation is *for* and why is left untouched; only the execution is offloaded. AI in capability-borrowing mode does the opposite. The surface task — the typing, the formatting — is left to the student; the cognitive process itself is offloaded. A calculator replaces a transfer skill. A capability-borrowing AI use replaces the thinking. The analogy works only if you misread what a calculator did. I have used some version of this paragraph in every professional development session I run on AI literacy and it has never failed to change at least one mind in the room.

**Misconception 2: "If I get the answer faster, I learn faster."**

This is the misconception the Bjork framework was built to refute. Speed-to-correct-answer is a measure of retrieval strength right now. Learning is a measure of storage strength two weeks from now. The two come apart, and AI is the largest single intervention currently available for making them come apart farther. A student who gets to the right answer in thirty seconds with AI has not learned faster; they have practiced retrieval-with-AI-present, which is not the same skill as retrieval without AI, which is what the exam measures.

The correction students respond to is honest: *"You learn faster when you struggle just below the level where you would give up. AI removes the struggle, so it removes the learning. That feels backwards. It is exactly backwards from what your brain needs."*

**Misconception 3: "Smooth output means I understood."**

This is the fluency trap, named. A student reads an AI explanation; the explanation is clear; the metacognitive system reports *I understand*. The understanding is not there. The feeling of understanding is real. The understanding is not.

The diagnostic for the trap is one sentence: *Can you produce this without the page open?* If the student can close the laptop and explain the concept from memory, the understanding is real. If they cannot, the fluency was the AI's, not theirs. Teach students to run this check on themselves the way you would teach a pilot to run a pre-flight check. It is short. It costs nothing. It catches the most common AI-era study failure.

**Misconception 4: "AI literacy means knowing how to prompt."**

This is the misconception the educational technology industry actively promotes, because it sells prompt engineering courses. It is wrong on the most basic level. A student who is fluent at prompting AI to do their homework is more capability-borrowing than a student who is bad at prompting. Fluent prompting raises the ceiling on what the AI can do *for* the student. It does not raise the ceiling on what the student can do *themselves*.

The honest definition of AI literacy is the metacognitive one: knowing, at every step of an AI interaction, which cognitive operation is yours and which is the AI's, and whether the operation that is yours is the one that builds the capability you are trying to build. A student with strong AI literacy can use the same tools as their friend and end up in a different place because they were running different operations the whole time.

---

## 6. Exercises

The exercises move from analysis to creation. The Bloom progression matters here because the framework is easy to recognize and hard to apply to one's own habits — recognition is not the same as practice.

### Exercise 1 (Apply) — The Capability Sort

Give students a list of twenty AI-use scenarios drawn from real student work: *"summarize this chapter for me," "ask me three questions about Le Chatelier's principle without telling me the answers," "rewrite my paragraph to make it sound smarter,"* and so on. Mixed across the building/borrowing axis. Students sort the twenty into two columns and write one sentence per scenario justifying the placement.

The discussion is the lesson. Students will disagree on the edge cases — *"summarize this chapter so I can decide whether to read it more carefully"* is interesting. *"Rewrite my paragraph to fix the grammar"* is interesting. The disagreement is where the framework gets sharpened against actual student practice.

**Deliverable.** The sorted list plus the one-sentence justifications. Twenty minutes.

### Exercise 2 (Create) — Design the Performance-Paradox Demo for Your Class

This is the chapter's TIKTOC-named deliverable, and it is the assignment that produces the most useful artifact for the rest of the semester.

The student (or teacher, if this is a professional development context) designs the performance-paradox demonstration for a specific class they teach or take. They produce:

1. Two isomorphic problem sets (six to eight problems each, same cognitive structure, different surface).
2. The 15/30/15/10 minute timing plan adapted to their class period.
3. The confidence rating instrument.
4. The reflection prompt students will write to.
5. A two-paragraph note on the discussion they expect to facilitate after.

The grading rubric is simple: does the demo, as designed, actually let students feel the gap? Does Problem Set B test the same concept as Problem Set A under a genuinely different surface, or is it just Problem Set A with different numbers (which AI would also handle fluently)? Does the reflection prompt force the student to look at their own data rather than at an abstraction?

**Deliverable.** A four-page activity packet plus a fifteen-minute reflection on what the designer expects to learn from running it. The designed activity should be runnable in a single class period with one revision after first deployment.

### Exercise 3 (Apply, then Analyze) — The Honest Self-Audit

Each student writes a one-paragraph honest accounting of one AI use they currently rely on. The prompt is structured:

> *"Name one specific way you currently use AI in your schoolwork. Describe in one sentence what cognitive operation you are doing. Describe in one sentence what cognitive operation the AI is doing. If the AI vanished right now and you had to do tomorrow's version of this task, could you? What would change about your work?"*

Then the student decides — based on their own honest accounting, not on a teacher's verdict — whether the use is capability-building or capability-borrowing, and writes one sentence on what they will change, if anything.

This is the exercise that converts the framework from vocabulary into self-monitoring. It is metacognition operationalized. Most students who do this honestly notice that at least one of their AI uses is in the borrowing column. Some decide to stop. Some decide to continue and accept the consequence. Both are legitimate outcomes. The point is that the decision is now visible to them.

**Deliverable.** A one-page reflection. Fifteen minutes to write; longer to think about.

---

## 7. What would change my mind

If a well-designed replication of the Bastani 2025 finding — same randomized design, different subject area or different age group — produced a null result on the unassisted exam in the unconstrained-AI condition, the empirical anchor of this chapter would weaken. The Bjork framework, the retrieval practice literature, and the generative explanation effect would still support the capability-building/capability-borrowing distinction; the framework would survive on cognitive-science grounds alone. But the chapter's strongest argument — that the gap between assisted practice and unassisted recall is large enough to flip students from passing to failing — would shrink to a more modest claim about long-term storage strength, and I would owe my students a corrected version of Section 3.2.

---

## 8. Still puzzling

Three things I do not yet understand and that I want to flag honestly rather than paper over.

First: I do not know how to operationalize this framework for grades 3–5 in a way that has been empirically tested rather than extrapolated from older students. The cognitive science underneath the framework is age-general. The classroom deployment is not. I am betting that the performance-paradox demonstration translates downward better than the Feynman test conversation does, because the demo's data is concrete and the conversation requires verbal sophistication. I do not have evidence for this. UNESCO 2024 and AI4K12 are the best available frameworks for age-appropriate AI literacy and they do not yet have the empirical base to settle this question. [verify whether any 2025–2026 replication studies have addressed grade 3–5 specifically]

Second: I do not know whether direct instruction in the capability-building/capability-borrowing distinction *transfers* across domains. A student taught the Feynman protocol in chemistry — does she apply it in history? Or does each domain require its own re-teaching? The metacognition literature suggests transfer is hard. I suspect, but cannot prove, that the building-vs.-borrowing distinction is durable enough to transfer because it is grounded in the student's own felt experience of the fluency trap rather than in a subject-specific skill. The performance-paradox demo, run once, may inoculate against the trap in a way that a vocabulary lesson cannot. This is testable. It has not yet been tested.

Third: I do not know what to tell the student in the opening case about the social pressure she is under. Her friends are using AI to write their papers. She wants to use AI to learn. In the short term, her friends will get better grades on the papers and she will get harder-earned grades on the unassisted exams. The gap will not close until the unassisted assessments are weighted heavily enough to dominate the course grade — which depends on her teachers, not on her. I can tell her the science. I cannot tell her she will be rewarded for following it in the next semester. That gap between *learning more* and *being assessed as having learned more* is the real challenge facing students who want to build capability rather than borrow it, and the response is partly individual and partly structural. Chapter 13 addressed the structural side. The individual side is harder, and I do not yet have a satisfying answer for the high schooler whose message opened this chapter.

---

## A reach forward

This is the last chapter of the book, and I want to close it in two directions at once.

The first direction is back to the Preface. The struggle is the mechanism of learning, and what makes this book different from the AI-evangelism and the AI-skepticism literature is the claim that the struggle can be protected even while many of the tasks that have nothing to do with learning are offloaded to a tool that is good at them. The phase gate in Chapter 2 is the teacher version of this. The capability table in this chapter is the student version. They are the same idea — *the cognitive operation that constitutes the learning must remain with the human who is trying to learn* — applied at two levels of the same system. The Conclusion that follows steps back to the research agenda: what we now know, what we do not, and what teachers who implement the framework systematically might contribute to the evidence base over the next several years.

The second direction is forward, to the companion volume *How to Learn with AI: A Student's Guide*. This chapter is what I would say to the high schooler in the opening case if I had eight thousand words. The student's guide is what I would say to her if I had a hundred and twenty thousand. It builds out every protocol named here, gives students the full deliberate-practice toolkit, walks through Feynman test conversations across a dozen subjects, and treats the student as the agent she is. If you teach in a setting where students would benefit from the framework in their own hands rather than mediated through yours, the student's guide is the publication to put on the shelf next to this one. The chapter you just read is the teacher's brief. The student's guide is the student's manual. The framework is the same. The audience is different. The cognitive operation — building the capability rather than borrowing it — is what both are designed to protect.

The struggle is the point. Your students are the ones who have to do it. This chapter is what you can give them so they know what they are doing while they do it.

— Nik Bear Brown
Boston, 2026

---

**Tags:** AI-literacy, capability-building, capability-borrowing, Bjork-desirable-difficulties, retrieval-practice, Feynman-test, Bastani-2025, performance-paradox, UNESCO-AI-framework, fluency-trap

*Voice anchor: feynman (workshop default).*

---

## References

- AI4K12 Initiative. *Five Big Ideas in AI*. https://ai4k12.org/
- Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö., & Mariman, R. (2025). Generative AI without guardrails can harm learning: Evidence from high school mathematics. *PNAS*, 122. https://www.pnas.org/doi/10.1073/pnas.2422633122
- Bjork, R. A., & Bjork, E. L. (1992). A new theory of disuse and an old theory of stimulus fluctuation. In A. F. Healy, S. M. Kosslyn, & R. M. Shiffrin (Eds.), *From learning processes to cognitive processes: Essays in honor of William K. Estes* (Vol. 2, pp. 35–67). Erlbaum.
- Bjork, E. L., & Bjork, R. A. (2011). Making things hard on yourself, but in a good way: Creating desirable difficulties to enhance learning. In M. A. Gernsbacher, R. W. Pew, L. M. Hough, & J. R. Pomerantz (Eds.), *Psychology and the real world: Essays illustrating fundamental contributions to society* (pp. 56–64). Worth Publishers. https://bjorklab.psych.ucla.edu/wp-content/uploads/sites/13/2016/04/EBjork_RBjork_2011.pdf
- Ericsson, K. A., Krampe, R. Th., & Tesch-Römer, C. (1993). The role of deliberate practice in the acquisition of expert performance. *Psychological Review*, 100(3), 363–406. https://psycnet.apa.org/record/1993-40718-001
- Fiorella, L., & Mayer, R. E. (2016). Eight ways to promote generative learning. *Educational Psychology Review*, 28(4), 717–741. https://link.springer.com/article/10.1007/s10648-015-9348-9
- Karpicke, J. D., & Blunt, J. R. (2011). Retrieval practice produces more learning than elaborative studying with concept mapping. *Science*, 331(6018), 772–775. https://www.science.org/doi/10.1126/science.1199327
- Lachner, A., Ly, K.-T., & Nückles, M. (2018). Providing written or oral explanations? Differential effects of the modality of explaining on students' conceptual learning and transfer. *Journal of Experimental Education*, 86(3), 344–361. https://www.tandfonline.com/doi/full/10.1080/00220973.2017.1363691
- Lachner, A., Jacob, L., & Hoogerheide, V. (2021). Learning by writing explanations: Is explaining to a fictitious student more effective than self-explaining? *Learning and Instruction*, 74, Article 101438. https://www.sciencedirect.com/science/article/abs/pii/S0959475220307337
- Macnamara, B. N., Hambrick, D. Z., & Oswald, F. L. (2014). Deliberate practice and performance in music, games, sports, education, and professions: A meta-analysis. *Psychological Science*, 25(8), 1608–1618. https://journals.sagepub.com/doi/10.1177/0956797614535810
- McMurtrie, B. *Teaching* newsletter, *Chronicle of Higher Education*. https://www.chronicle.com/author/beth-mcmurtrie
- Roediger, H. L., & Karpicke, J. D. (2006). Test-enhanced learning: Taking memory tests improves long-term retention. *Psychological Science*, 17(3), 249–255. https://journals.sagepub.com/doi/10.1111/j.1467-9280.2006.01693.x
- Roediger, H. L., & Karpicke, J. D. (2006). The power of testing memory: Basic research and implications for educational practice. *Perspectives on Psychological Science*, 1(3), 181–210. https://journals.sagepub.com/doi/abs/10.1111/j.1745-6916.2006.00012.x
- UNESCO. (2024). *AI competency framework for students*. https://www.unesco.org/en/articles/ai-competency-framework-students
