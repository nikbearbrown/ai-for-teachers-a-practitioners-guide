# Chapter 13 — Academic Integrity, Privacy, and Honest Use

<!-- FACT-CHECK FLAG: MOSTLY CONFIRMED — see factchecks/13-academic-integrity-privacy-and-honest-use-assertions.md -->


**TL;DR.** Detection-first responses to AI in education fail on their own terms — the tools are unreliable, the errors are biased against non-native English writers, and the institutions that took them seriously have walked back. The durable response is design: assignments built so a student who used AI freely could not produce a good artifact without leaving the friction traces of having learned the material, and a small set of privacy and disclosure habits that keep the teacher's own AI use legally defensible and pedagogically honest.

---

## 1. Learning objectives

By the end of this chapter, you should be able to:

1. **Understand.** Describe the Bastani et al. (2025) finding in full: the 48% practice gain and 17-percentage-point exam loss in the unguarded condition, the 127% practice gain and preserved exam performance in the tutor-wrapped condition, and the performance paradox the contrast reveals.
2. **Apply.** Redesign one of your current assessments using the AI-survivable assignment checklist (five questions) so a student who used AI freely could not produce a passable artifact without doing the cognitive work the assessment is supposed to surface.
3. **Analyze.** Evaluate AI-detection tools against the peer-reviewed evidence on accuracy and bias — Liang et al. (2023) on non-native English writers, Weber-Wulff et al. (2023) on reliability across tools — and against the documented institutional retreat (OpenAI July 2023; Vanderbilt August 2023).
4. **Evaluate.** Apply principle-level FERPA and COPPA reasoning to your own AI-assisted workflow: identify the moments student personally identifiable information would leave the room, and apply the anonymization protocol from Chapter 6.
5. **Create.** Draft one paragraph of a student AI-use policy that is specific (names tools and uses), enforceable (violations are observable without detection software), and pedagogically motivated (cites the learning mechanism it protects).

**The AI-survivable assignment checklist** — used throughout this chapter and reproduced in Appendix C:

1. Does the assignment require the student to defend claims in conversation?
2. Does the assignment require applying concepts to a situation that did not exist when the AI was trained?
3. Does the assignment require process documentation (drafts, annotations, decision records)?
4. Does the assignment require real-time unassisted performance?
5. If a student used AI freely and produced a good artifact, would you know whether they learned anything?

---

## 2. Opening case — the professor who solved the wrong problem

*This opening case is composite-illustrative. The professor is not a specific documented individual. The 23% referral rate, the three contested cases, the four-week appeals window are plausible figures consistent with publicly documented detection-first deployments at universities that subsequently retreated (see §3 on Vanderbilt's published arithmetic). The point of the case is the structure of the failure, not a single named instance.*

It is the end of finals week. A professor of writing at a mid-sized state university is sitting at her kitchen table at 9:40 on a Sunday night with a stack of essays beside her laptop, a spreadsheet open in one window, and a detection tool open in another. She built the workflow in August. The workflow was honest, and at the time it seemed proportional to the threat. Every essay would be run through a commercial AI detector. Any flagged paper would be re-read by hand. Any paper that, on second read, still looked AI-generated would be referred to the Office of Academic Integrity. She would document every step. She would not accuse without evidence.

By December she has referred 23% of her students.

She has not slept well since October. Three students have formally contested their referrals — one a senior whose graduation is now contingent on the outcome, one a returning adult learner who arrived in office hours crying, one a sophomore whose father is an attorney. The Office of Academic Integrity, which was not staffed for this volume, has confirmed the appeals process will take four weeks. During those four weeks she has stopped accepting late work because the policy felt arbitrary against the backdrop of the detection regime. She has stopped writing the kind of marginal comments she used to be proud of, because every comment now feels like preparation for a hearing. Her course evaluations have come in. They are bad in a specific way — students who used to describe her as demanding now describe her as suspicious.

She has taught less this semester than at any point in her career. Her students have learned less.

The detector, it turns out, was not the wrong tool for the right job. It was the right tool for the wrong job. The job she was solving was *catch the students who cheated.* The job she needed to solve was *design the assessment so that cheating and learning are not the same task.* By picking up the detector, she made the second job harder rather than easier — because every hour she spent in the detection workflow was an hour she did not spend redesigning the prompt, the rubric, the conferencing schedule, the in-class component, the process documentation that would have let her see whether the writing in front of her was the trace of a student who had encountered the material.

This chapter is the redesign.

---

## 3. Core concept — design beats detection, and here is why

The argument has three parts: an empirical anchor (what Bastani et al. 2025 actually found), a structural critique (why detection-first cannot work even if it worked), and a design move (the AI-survivable assignment).

### 3.1 The Bastani 2025 finding in full

This is the load-bearing study. It deserves the careful treatment.

Bastani, Bastani, Sungu, Ge, Kabakcı, and Mariman (2025) ran a field experiment in a Turkish high school across grades 9–11, approximately 1,000 students, multi-week math curriculum, random assignment to one of three conditions: a no-AI control, an "GPT Base" condition in which students could use GPT-4 in a standard ChatGPT-style interface during practice, and a "GPT Tutor" condition in which the same underlying model was wrapped in a teacher-designed system prompt that refused to give complete answers and structured the interaction around the student externalizing a reasoning step before the model advanced ([PNAS, 2025](https://www.pnas.org/doi/10.1073/pnas.2422633122); DOI [10.1073/pnas.2422633122](https://doi.org/10.1073/pnas.2422633122); a [correction](https://www.pnas.org/doi/10.1073/pnas.2518204122) was published in August 2025 — author affiliation only per pantry cross-check, no change to the substantive numbers).

The three numbers the chapter cannot do without:

*During practice, with AI available:*
- **GPT Base** students performed **48% higher** than the no-AI control.
- **GPT Tutor** students performed **127% higher** than the no-AI control.

*On the post-practice exam, with no AI available:*
- **GPT Base** students scored **17 percentage points lower** than the no-AI control.
- **GPT Tutor** students were statistically indistinguishable from the no-AI control.

Same underlying model. Same students, randomly assigned. Opposite durable-learning outcomes. The only variable was the wrapper — the pedagogical commitments expressed in the system prompt.

Three precision moves before going further.

*First, the harm is 17 percentage points, not 17 percent.* On the scale of the exam, that is roughly half a standard deviation of durable learning. Popular summaries sometimes garble this. The chapter will not.

*Second, the 127% practice gain in the tutor condition is not a footnote. It is a finding of equal weight to the 17-point loss.* Pedagogically-designed AI can substantially boost in-session practice performance *without* destroying durable learning. The Bastani study is not "AI harms learning." It is *unguarded AI deployed without pedagogical guardrails harms durable learning while appearing to help in the moment, and guarded AI does not.* The distinction is everything.

*Third, this is one study, one country, one subject, one age group.* It is the most rigorous current evidence on the question, but a single experiment is not a settled science. If Bastani does not replicate, the chapter's central empirical anchor moves to a narrower base. The framework should be held with the certainty the evidence supports — strong, not absolute. [verify replication status periodically.]

The mechanism the numbers exhibit is the *performance paradox*: in-session performance with AI assistance feels like learning to the student (the answers are right; the work is moving; the affect is positive). The brain receives a different signal — no prediction error, no effortful retrieval, no consolidation. Robert and Elizabeth Bjork's storage-versus-retrieval distinction is the cognitive-psychology backbone here: storage strength (what is encoded) and retrieval strength (what feels fluent right now) come apart, and AI-assisted practice can raise retrieval strength in the moment while leaving storage strength essentially flat ([Bjork & Bjork, 1992; see Appendix G for the full framework](#)).

The student in the GPT Base group felt confident at the end of practice. The brain had not consolidated. Two weeks later, on the unannounced exam, the gap appeared. The student's confidence was an unreliable signal. It always was; AI just made the signal louder.

A teaching analogy that holds. A teacher hands a student a calculator before they understand division. The student gets the right answer on every problem in the worksheet. On the unannounced quiz two weeks later, the calculator is taken away. The student has produced a perfect worksheet and learned nothing. The worksheet is the artifact; the learning was the process; the calculator bypassed the process. AI is the calculator at scale, and the worksheet has gotten longer. The analogy breaks down at one place worth naming: calculators do not bullshit, and AI does. The verification burden the analogy hides is the new skill the curriculum has to teach.

### 3.2 Why detection fails — three modes, peer-reviewed

If you accept the Bastani finding, the question becomes: what is the right response? The instinct of many teachers and administrators in 2023 and 2024 was *catch them*. Buy a detector. Run student work through it. Discipline the flagged. The instinct was understandable. It does not work, on three independent grounds.

**Mode 1 — the tools are unreliable on their own terms.** Weber-Wulff et al. (2023), publishing in the peer-reviewed *International Journal for Educational Integrity*, tested twelve detection tools across 54 cases (756 total tests, March–May 2023) and concluded the tools "are neither accurate nor reliable" and exhibit a systematic bias toward classifying outputs as human-written when stressed by mild adversarial conditions (paraphrasing, translation, light editing) ([Weber-Wulff et al., IJEI 2023](https://link.springer.com/article/10.1007/s40979-023-00146-z); [arXiv preprint](https://arxiv.org/abs/2306.15666)). The strongest evidence for the unreliability problem came from OpenAI itself. The company launched its AI Text Classifier on January 31, 2023, and **withdrew it on July 20, 2023**, citing a "low rate of accuracy" — the classifier correctly identified AI-written content only 26% of the time and produced false positives on roughly 9% of human-written text ([OpenAI announcement, updated July 2023](https://openai.com/index/new-ai-classifier-for-indicating-ai-written-text/)). The company that *makes* GPT could not reliably detect GPT output produced by GPT. That is the strongest single signal about the technical limits of the problem.

**Mode 2 — the errors are biased.** Liang, Yuksekgonul, Mao, Wu, and Zou (2023), publishing in the peer-reviewed Cell Press journal *Patterns*, tested seven widely-used GPT detectors on TOEFL essays written by non-native English speakers and on essays written by U.S. 8th graders ([Liang et al., *Patterns* 2023](https://www.cell.com/patterns/fulltext/S2666-3899(23)00130-7); DOI [10.1016/j.patter.2023.100779](https://doi.org/10.1016/j.patter.2023.100779)). The detectors achieved near-perfect accuracy on the 8th-grade essays. They misclassified **more than 50% of the TOEFL essays as AI-generated.**

The mechanism, restated because the chapter cannot move past this point quickly: detectors flag text with low *perplexity* — text where the next word is highly predictable given the prior context — as AI-generated. Large language models produce low-perplexity text by construction. So do non-native English writers, for entirely different reasons: a narrower vocabulary, more conventional phrasings, less surprising word order. The detector cannot distinguish "writing the model produced" from "writing that does not surprise the model." Those are different things. The detector treats them as the same. The error is not random. It is systematically allocated to a protected category.

This is where the equity argument and the technical argument coincide. A detector that misclassifies the writing of multilingual students at five times the rate of native speakers is making a measurement error and a civil-rights problem in the same operation. The chapter is not going to soften that. It is the clearest evidence in the literature.

**Mode 3 — serious institutions are walking back.** Vanderbilt University disabled the Turnitin AI detector in August 2023 and published the reasoning ([Vanderbilt Brightspace announcement, Aug 16 2023](https://www.vanderbilt.edu/brightspace/2023/08/16/guidance-on-ai-detection-and-why-were-disabling-turnitins-ai-detector/)). The arithmetic was the load-bearing piece. Vanderbilt processed about 75,000 student papers through Turnitin in 2022. Turnitin's own published false-positive rate at launch was about 1%. One percent of 75,000 is 750. The Office of Student Accountability would not have the bandwidth to adjudicate 750 contested cases honestly; the inevitable triage would produce unjust outcomes and uneven enforcement. Vanderbilt's stated alternative was investing in pedagogy and assignment design.

The named harms are documented. **Louise Stivers**, a political-science major at UC Davis (2023), had a paper summarizing a Supreme Court case flagged as partially AI-generated by Turnitin and was referred to the Office of Student Support and Judicial Affairs ([Rolling Stone coverage](https://www.rollingstone.com/culture/culture-features/student-accused-ai-cheating-turnitin-1234747351/)). **William Quarterman**, a senior history major at the same institution the same year, had his work flagged by GPTZero, received a failing grade, and faced a referral on appeal ([Washington Post / NMLLP summary](https://nmllplaw.com/blog/when-ai-gets-you-accused-what-to-do-if-your-school-says-you-used-chatgpt/)). The litigation landscape has continued to expand as more cases proceed ([NBC News overview, 2025](https://www.nbcnews.com/tech/internet/college-students-ai-cheating-detectors-humanizers-rcna253878)). The pattern: the false-positive rate is not just a statistic. It is a person, named, with consequences.

The chapter's framing on detection vendor accuracy claims: do not litigate them. Vendor numbers age fast, are produced in controlled internal evaluation, and reliably exceed independent peer-reviewed estimates ([verify any specific vendor figure if you must cite one]). Cite the peer-reviewed evidence (Liang 2023, Weber-Wulff 2023) and the institutional retreat (OpenAI July 2023, Vanderbilt August 2023) as the durable signal. Both are on the public record. Neither will be revised by next quarter's marketing.

### 3.3 The AI-survivable assignment framework

If detection cannot work, what does? The answer this chapter offers: assignments designed so the artifact alone cannot stand as evidence of the learning. The artifact must come with the process that produced it, or be performed under conditions where the process is observable.

The five-question checklist (see §1) is the operational instrument. Each question maps to a specific limitation of AI capability as of 2026.

**1. Does the assignment require the student to defend claims in conversation?**

AI produces text. It cannot sit through an oral examination on a paper it did not write. The student who can defend the claims in real time has the mental model. The student who cannot does not. This is the move pre-AI doctoral defenses have always made. It generalizes downward to a high school history class as well as a graduate seminar. The cost is class time and emotional load — defenses are stressful, particularly for students with test anxiety or processing differences. The trade-off is real and the chapter will not pretend otherwise.

**2. Does the assignment require applying concepts to a situation that did not exist when the AI was trained?**

The model has a training cutoff. Apply the concept to a specific event from last month, to a dataset the class collected this week, to the local school board's decision two days ago, to a reading the AI has not absorbed, and the transfer cannot be pre-baked. This is not AI-proof — students can paste the new material into the prompt — but it raises the floor: the student must at least describe the new situation accurately to get useful help. The cognitive work of *encountering the situation and recognizing what is and is not analogous* is the work the assignment surfaces.

**3. Does the assignment require process documentation?**

The artifact used to be proof of the process. It no longer is. So the process must become its own proof. Drafts dated and submitted across weeks. Annotations on sources in the student's voice. A captured prompt log if AI was used. A short decision record — *I changed paragraph three because* — at each revision. The Medhavy GLP framework formalizes seven of these signals; the chapter's operational ask is simpler: collect enough of the process that a hostile reader could reconstruct the student's developmental path. This is the most-portable move across age bands. K-8 versions look like math journals and sticky-note revision logs; college versions look like annotated bibliographies and version-controlled drafts. The shape is the same. The artifact rests on the process record, not on itself.

**4. Does the assignment require real-time unassisted performance?**

In-class writing. Whiteboard problem-solving. Oral defenses. The phase gate enforced by the room. This is the highest-friction option and the most legally defensible — when the writing happens under your eye, the question of authorship does not arise. It is also the option that disadvantages students who think slowly under pressure or who have documented processing differences. A defensible regime uses real-time performance as one component, not the whole assessment.

**5. If a student used AI freely and produced a good artifact, would you know whether they learned anything?**

This is the diagnostic question, and the one to come back to. It is the question the professor in the opening case never asked. If the answer is no, the assessment is measuring artifact quality, not learning. Bastani's GPT Base students produced 48% better practice performance and learned 17 points less. An assignment that cannot distinguish the GPT Base student from the no-AI student is the assignment Bastani's intervention destroyed. Redesign so the answer is *yes*.

The framework is not *make assignments AI-proof.* Nothing is AI-proof at the artifact level — that is the structural lesson of the artifact decoupling described in the Preface. The framework is *make assessments that observe the learning, not just the artifact.*

### 3.4 Privacy — FERPA, COPPA, and the anonymization habit

The legal layer has to be present and principle-level. This chapter is not legal advice and cannot be. The specifics are state-variable, district-variable, contract-variable, and changing month by month. What the chapter can give you is the operational habits that keep most everyday teacher AI use legally defensible, and the moments to stop and call counsel.

**FERPA — the Family Educational Rights and Privacy Act (20 U.S.C. § 1232g)** protects "education records" containing personally identifiable information about students. Three principles the chapter can defensibly assert.

*Identifiable student data submitted to a consumer AI tool is a disclosure.* A free ChatGPT, Claude, or Gemini account that has no data-processing agreement with your school is, in FERPA terms, a third party with no authorization to receive the record. When you paste a student's name and grade into the prompt window, you have made the disclosure. The act is small. The legal frame is not.

*The "school official" exception requires a contract.* FERPA allows disclosure to a "school official with a legitimate educational interest," and the regulations extend this to external vendors *only when* the vendor is under the direct control of the school with respect to the use and maintenance of the records (34 CFR § 99.31(a)(1)(i)(B)). A signed Data Processing Agreement is what triggers the exception. A free consumer account does not. District-licensed Khan Academy, MagicSchool, or a Microsoft 365 account with the educational tenant typically has the DPA in place. A teacher's personal ChatGPT subscription does not.

*Anonymization is the operational fix.* The protocol from Chapter 6 — strip names, IDs, identifying details, replace with generic placeholders before any external AI interaction — is the practical move that removes FERPA exposure for routine AI-assisted tasks. The teacher who uses AI to generate differentiated practice problems does not need student names in the prompt; the teacher who uses AI to summarize a class roster does. The first task is routine; the second is the moment to stop. The U.S. Department of Education's Office of Educational Technology framed the same posture in its May 2023 *Artificial Intelligence and the Future of Teaching and Learning* report — "human in the loop" as the federal stance ([ed.gov PDF](https://www.ed.gov/sites/ed/files/documents/ai-report/ai-report.pdf)). The Department's 2025 FERPA FAQ refresh updated 37 questions, and a 2026 AI-specific FERPA publication is in preparation [verify on publication]. The federal frame is moving. The principles are not.

**COPPA — the Children's Online Privacy Protection Act (15 U.S.C. § 6501–6506)** restricts the collection of personal information from children under 13 by online services. The FTC finalized amendments in April 2025 that took effect June 23, 2025, and include the first explicit treatment of children's data used to train algorithms — operators cannot retain children's personal information indefinitely even when claimed as necessary for algorithm improvement ([FTC final rule](https://www.ftc.gov/system/files/ftc_gov/pdf/coppa_sbp_1.16_0.pdf)). The operational implication for elementary teachers is direct: default consumer AI tools require users to be at least 13. A 4th-grade teacher who sets up shared ChatGPT logins for the class is asking the students to violate the service's terms and exposing the school to COPPA risk. For students under 13, AI use should run through (a) education-specific products with COPPA-compliant data agreements (Khanmigo, MagicSchool's K-5 offerings, district-licensed products with signed DPAs) or (b) the teacher operating the AI on the students' behalf with anonymized inputs and reviewed outputs.

The chapter will say it once more, plainly: **FERPA and COPPA application to AI is legal-stakes, state-variable, and rapidly evolving. The principles above are the starting point. The specifics belong to your district counsel and privacy officer.** The Student Privacy Compass aggregates state guidance as it changes ([studentprivacycompass.org](https://studentprivacycompass.org/state-guidance-on-the-use-of-generative-ai-in-k-12-education/)). The TeachAI policy tracker ([teachai.org/policy-tracker](https://www.teachai.org/policy-tracker)) tracks state-level guidance and shows the trajectory toward design-and-disclosure frameworks rather than prohibition — by April 2025, at least 28 U.S. states had published K-12 AI guidance.

### 3.5 The equity dimension

The chapter has to hold a difficult finding: AI use among teens is not uniformly distributed, and the patterns matter for policy design. Pew Research (January 2025) reported that the share of U.S. teens aged 13–17 who have used ChatGPT for schoolwork rose from 13% in 2023 to 26% in 2024 ([Pew Research, Jan 15 2025](https://www.pewresearch.org/short-reads/2025/01/15/about-a-quarter-of-us-teens-have-used-chatgpt-for-schoolwork-double-the-share-in-2023/)). The cross-tabs are non-obvious: Black and Hispanic teens (31% each) report higher use than White teens (22%); higher-income families show higher rates than lower-income families; and teens themselves carry an implicit norm — 54% find AI use acceptable for research, 29% for math, only 18% for essays.

The equity argument cuts both directions. *Banning AI* in a context where roughly a quarter of students use it anyway produces a policy that punishes the students who follow rules and rewards those who do not — selective enforcement is the structural pattern. *Requiring AI* without addressing differential home access — broadband, device, paid-tier access to better models — widens the gap rather than closing it. The same logic the Trust Teacher framing applied to phone-ban policies applies here: facially neutral rules can produce unequal effects when underlying access patterns are unequal. A defensible policy names both directions and adjusts.

### 3.6 The teacher transparency question

The reflexive move. If you use AI to draft your feedback, generate practice problems, build your slides, and never tell the students, you are asking them to disclose what you conceal. That asymmetry is noticed. It corrodes the policy faster than any failure of enforcement.

The chapter's prescription has three layers.

*Disclose at the syllabus level.* One sentence near the top: *I use AI tools to help draft practice problems, generate slide outlines, and respond to routine emails. AI does not grade your work substantively, write the comments you receive on your papers, decide your final grade, or choose what we teach this week.* The point is not that AI was used. The point is what AI did and did not do — the boundary.

*Disclose at the artifact level.* When a handout or slide deck was AI-drafted and teacher-edited, note it on the artifact. A short footer is enough.

*Disclose the boundary, not just the tool.* The disclosure pattern the chapter recommends for student work — *what the AI did, what it did not, where the human judgment lives* — is the pattern the teacher should be modeling. That is the reflexive commitment in action: the rule you ask of others is the rule you live yourself.

---

## 4. Worked example — redesigning the research paper

The chapter has to land this concretely. Take one assignment most teachers reading this book have given some version of: a research paper. Watch what it looks like before, why it is AI-survivable-broken, what changes when the checklist is applied, and what policy paragraph goes with the redesign.

### 4.1 The original assignment

> **Research Paper.** Choose a topic from American history between 1865 and 1945. Write a 1,500–2,000-word research paper using at least five academic sources. Make an argument. Cite using Chicago style. Due in four weeks.

The prompt is clear, the standards are reasonable, the grading rubric is in the syllabus. This is a well-written assignment by every pre-2022 measure. Now apply the checklist.

1. *Does it require defending claims in conversation?* No.
2. *Does it require applying concepts to a situation that did not exist when the AI was trained?* No — 1865–1945 is well-trodden ground.
3. *Does it require process documentation?* No — only the final artifact is collected.
4. *Does it require real-time unassisted performance?* No.
5. *If a student used AI freely and produced a good artifact, would you know whether they learned anything?* No.

Five no's. The assignment is AI-survivable-broken. A student can produce a passable artifact through the AI pathway and the teacher cannot tell. The grade is then either too generous (if the student used AI and got an A) or grossly unjust (if the student wrote honestly and got the same grade as the student who did not). The integrity question is downstream of the design question. The artifact will not save you.

### 4.2 The redesign

> **Research Paper (Redesigned).** Choose a topic from American history between 1865 and 1945 that connects to one event or trend from the last twelve months in our local community, state, or national news. (A paper on the 1934 Reciprocal Trade Agreements Act might connect to a 2026 trade dispute we have discussed in class. A paper on the 1908 White House Conservation Conference might connect to a local land-use decision currently before the city council.) Write a 1,500–2,000-word research paper using at least five academic sources. Make an argument that explicitly links the historical material to the current event you chose.
>
> **Required process portfolio (submitted with final paper):**
> - **Topic memo** (one page, due Week 1): the historical topic you chose, the current event it connects to, and a one-paragraph explanation of the connection you intend to argue. Submitted in class on paper.
> - **Annotated bibliography** (due Week 2): each source listed with two sentences in your own voice — one summarizing the argument, one explaining how the source helps or complicates your developing argument.
> - **Draft 1** (due Week 3): full draft with a 200-word reflection memo identifying what you still do not know and what you plan to change.
> - **AI use disclosure**: a short paragraph naming any AI tool used, what you used it for (brainstorming, outlining, grammar review, source identification), what you did not use it for, and one prompt log entry showing a representative exchange.
> - **Defense conference** (Week 4, in office hours, 10 minutes): bring the final paper; be prepared to talk through your argument, your sources, and one place you changed your mind during drafting.

Apply the checklist to the redesign.

1. *Defending claims in conversation?* Yes — the 10-minute defense conference is the gate.
2. *Applying concepts to a situation that did not exist when the AI was trained?* Yes — the link to a current local event forces transfer the AI cannot pre-bake.
3. *Process documentation?* Yes — topic memo, annotated bibliography, draft with reflection memo, AI disclosure, prompt log.
4. *Real-time unassisted performance?* Yes — the topic memo is submitted in class on paper; the defense conference is live.
5. *If a student used AI freely, would you know whether they learned anything?* Yes — the in-class topic memo, the defense conference, and the reflection memo each provide an independent observation of the student's mental model.

Five yes's. The redesign costs you some assignment elegance (it has more parts now), some grading time (the bibliography and the reflection memo are short, but they exist), and ten minutes per student in office hours. It saves you the entire detection-and-discipline workflow the professor in §2 spent her semester on. The trade is good.

### 4.3 The policy paragraph that goes with it

> **AI Use in This Course.** You may use AI tools (ChatGPT, Claude, Gemini, or others) for brainstorming, outlining, source identification, and grammar review on the research paper. You may not use AI to write paragraphs you submit as your own writing. Your AI use disclosure paragraph and prompt log entry are required components of the assignment — incomplete or inaccurate disclosure is the integrity violation, not the AI use itself. The defense conference is the point at which I will see whether the paper represents your mental model of the historical-current connection you argued. If it does, the AI use that helped you get there is acknowledged and credited. If it does not, no detection software is needed; the conversation will show. I use AI tools to help me draft slide outlines, generate practice problems, and respond to routine course emails. I do not use AI to grade your work or write the substantive comments you receive on your drafts.

Three things to notice about that paragraph. *Specific* — it names tools, names permitted uses, names a forbidden use. *Enforceable* — the violations are observable through the disclosure and the defense, not through a detector. *Pedagogically motivated* — the rule cites the learning mechanism (the defense conference shows the mental model) rather than asserting a prohibition. And the last two sentences are the teacher transparency move: the disclosure pattern asked of students is the pattern the teacher lives.

### 4.4 The lesson and the limit

The redesign does one thing the original did not: it collects evidence of the process across time and culminates in a live conversation. That structure makes the GPT Base failure mode visible. A student who got 48% better at producing draft prose but learned 17 points less will not survive the topic memo (written in class, on paper), the annotated bibliography (in the student's own voice), the reflection memo (about their own thinking), and the defense conference. The original assignment had none of those filters. The artifact was the only signal. The artifact is no longer a reliable signal.

The limit is honest. The redesign costs class time. It will not work in a 300-student lecture course without restructuring how grading capacity is allocated. The defense conference is harder for some students than others, and a one-shot defense disadvantages students with documented anxiety or processing differences — defensible policy allows for an alternative format (written defense, asynchronous video). And process documentation can itself be gamed at the margin: a student could AI-generate the draft and then AI-generate the reflection memo. The framework raises the cost of bypassing the learning to something close to the cost of doing the learning. It does not eliminate the bypass entirely. As the Frictional appendix puts it: gaming all the friction signals simultaneously is approximately as expensive as performing the underlying cognitive work — at which point the gaming has become indistinguishable from learning in the only sense that matters.

---

## 5. Common misconceptions

Four worth working through carefully.

**Misconception 1: "Detection software works well enough; the false positives are rare."**

The peer-reviewed evidence does not support this. Liang 2023 found >50% misclassification on TOEFL essays — that is not a rare-event problem, that is a systematic-bias problem. Weber-Wulff 2023 found the class of tools "neither accurate nor reliable." OpenAI withdrew its own classifier in July 2023 citing 26% true-positive accuracy. Vendor numbers (e.g., a "below 1% false positive rate") have a documented gap with independent peer-reviewed estimates, and even taken at face value the institutional arithmetic is brutal: a 1% false positive rate at Vanderbilt's 2022 throughput produced approximately 750 wrongly-flagged papers in a single year. The institutional retreat from detection-first is not theoretical — Vanderbilt published its reasoning in August 2023 ([Brightspace announcement](https://www.vanderbilt.edu/brightspace/2023/08/16/guidance-on-ai-detection-and-why-were-disabling-turnitins-ai-detector/)) and a wave of other universities have followed since. The fix is not a better detector.

**Misconception 2: "Banning AI in the classroom solves the integrity problem."**

It does not, for three reasons. *First*, the Pew January 2025 data shows ~26% of teens use ChatGPT for schoolwork; the ban is counterfactual at the population level — it punishes the students who follow it and rewards the ones who do not. *Second*, the equity pattern is non-obvious: higher AI use among Black and Hispanic teens than White teens, higher use among higher-income families. A blanket ban interacts asymmetrically with what students have at home. *Third*, even a perfectly enforced ban during class hours does not address the assignment-level problem — students still write papers outside of class. The ban is a category error; it tries to enforce at the wrong layer.

**Misconception 3: "An honor code is enough."**

Honor codes signal values. They do not redesign the assessment. The Preface's argument is that the artifact is now decoupled from the process. The honor code can ask students to do the work; it cannot make the artifact prove they did. Vanderbilt has had an honor code since 1875. Vanderbilt disabled the AI detector in 2023. Both facts are compatible because the honor code addresses a different layer of the problem than detection or design does. The honor code is necessary; it is not sufficient.

**Misconception 4: "More policy enforcement equals more integrity."**

This is the misconception the opening case is built on. The professor enforced harder; her students learned less. The relationship between policy enforcement and integrity is not linear. Past a threshold, enforcement consumes the teaching time that would have produced the learning the policy was supposed to protect. The pattern is general: when the integrity workflow grows large enough to dominate the teaching workflow, both fail at once. The durable response is to lower the enforcement burden by raising the design floor.

---

## 6. Exercises

### Exercise 1 (Create) — Draft a student AI-use policy

Choose one course you teach. Write one paragraph (150–300 words) of an AI-use policy. Evaluate it against three criteria:

1. **Specific.** Does it name actual tools and specific permitted and forbidden uses? *"You may use ChatGPT for brainstorming"* is specific. *"AI use must be appropriate"* is not.
2. **Enforceable.** Are the violations observable without detection software? Could you tell whether a student violated the policy by looking at the work they submitted plus the process documentation, without running anything through a detector?
3. **Pedagogically motivated.** Does the rule cite the learning mechanism it protects? *"Drafting your own first draft is required because the writing struggle is where you build the argument"* is motivated. *"No AI on drafts"* is not.

Optional addition: include one sentence of your own AI-use disclosure (what you use AI for in your teaching; what you do not). Test it the same way.

### Exercise 2 (Apply) — Redesign one assignment for AI-survivability

Take one assignment from your current semester. Apply the five-question checklist. For each question scoring "no," write one specific redesign move that would change the answer to "yes." Do not redesign more than you have to — the goal is the minimum-viable redesign that gets to five yeses, not a wholesale overhaul.

Suggested format:

| Question | Current answer | Redesign move |
|---|---|---|
| 1. Defended in conversation? | No | Add a 5-minute defense in the next class meeting |
| 2. Novel application? | No | Require connecting to one event from the last six months |
| 3. Process documentation? | No | Require an annotated outline submitted one week before final |
| 4. Real-time performance? | No | First half of writing happens in class |
| 5. AI-bypass detectable? | No | Combination of above is enough |

If the redesign passes the checklist, also write the policy paragraph that goes with it (Exercise 1's format). Submit both as a single deliverable.

### Exercise 3 (Evaluate) — Audit three detection-tool accuracy claims

Find three publicly-stated accuracy claims from AI-detection-tool vendors. (Vendor websites, marketing materials, press releases, or independent reporting are all fair game.) For each claim, evaluate:

1. **The basis of the claim.** Is the evaluation independent and peer-reviewed, or is it the vendor's internal benchmark? Is the evaluation methodology public?
2. **The match to independent evidence.** How does the vendor's stated false-positive rate compare to Liang 2023's >50% TOEFL misclassification finding or Weber-Wulff 2023's broader reliability assessment?
3. **The fitness-for-discipline test.** If you applied the vendor's stated false-positive rate to one semester of student work in your course, how many wrongly-flagged students would you expect, and would your institution have the capacity to adjudicate the appeals honestly? (This is the Vanderbilt arithmetic, applied to your own throughput.)

Write a one-page summary of what the audit tells you about whether the tool can serve as primary evidence in an integrity case.

---

## 7. What would change my mind

A well-designed replication of Bastani et al. (2025) in a different context — different country, different subject, different age band — that *failed* to find the performance paradox in the unguarded AI condition, particularly if it found that students who used AI freely during practice performed *at or above* the no-AI control on a delayed unassisted test. That finding would substantially weaken the empirical case for design-over-detection by undermining the load-bearing reason design is necessary. The chapter's framework would still be defensible on the institutional-retreat and detector-bias grounds, but the central pedagogical argument would have to be rebuilt on a narrower base.

---

## 8. Still puzzling

A few things I do not yet fully understand.

- **The K-8 generalization.** Most of the AI-survivable framework's published evidence comes from college and late-secondary contexts. The "process documentation" and "novel application" moves clearly portable downward; the "defense in conversation" move is portable but slower; the calibration of the framework to a 5th-grade or 3rd-grade context is something the chapter does not have a confident answer for yet.
- **What process documentation actually costs at scale.** The redesign in §4 adds checkpoints to one assignment. A teacher with 150 students and four preps cannot do this for every assignment. The chapter has been honest that detection-first costs more — but the design-first response also has costs, and the equilibrium for a full teaching load has not been worked out in the published literature.
- **The teacher-transparency-as-mandatory question.** The reflexive argument says teachers should disclose their own AI use. Whether that disclosure should be required by policy at the institutional level, encouraged but not required, or left fully to instructor discretion is not settled. Different institutions are running different experiments and the evidence is not yet in.
- **Whether the framework holds as AI capability advances.** The five-question checklist works because of specific 2026 limits on AI capability — training cutoffs, inability to defend in conversation, inability to produce process records. If those limits move (and some are already moving), the checklist will need revision. The framework is robust to incremental capability increases; it is not robust to qualitative shifts the chapter cannot predict.

---

## Bridge to Chapter 14

Chapter 13 addressed what teachers do — the assessment design, the privacy habits, the policy paragraph, the disclosure pattern. Chapter 14 addresses what teachers *tell students* about all of this: why the rules exist, how the students themselves can use AI to learn rather than to bypass learning, and the capability-building-versus-capability-borrowing distinction that gives students a usable mental model for their own AI use. The Bastani finding presented in Chapter 13 in its technical form will appear in Chapter 14 in student-facing language. The same neurobiology; a different audience; the same point.

---

**Tags:** academic-integrity, AI-survivable-assessment, Bastani-2025, AI-detection, FERPA, COPPA, Liang-2023, Weber-Wulff-2023, Vanderbilt, equity-and-access, teacher-transparency, process-documentation

*Voice: feynman. Composite-illustrative opening labeled. Bastani 2025 numbers verified against PNAS publication and SSRN preprint; the August 2025 correction is affiliation-only per pantry crosscheck — substantive numbers stand. FERPA/COPPA treated principle-level; defer specifics to district counsel. Detection vendor accuracy figures cited only as institutional context (Vanderbilt arithmetic) and OpenAI withdrawal; not relied on as load-bearing.*
