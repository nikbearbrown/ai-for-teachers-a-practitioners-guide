# Chapter 7 — Communication with AI: Parents, Admin, and Documentation

**TL;DR.** Most teacher communication is form-rendering of judgments the teacher already has — and that is exactly where AI earns its keep, by writing the prose while you keep the substance. The chapter's whole skill is sorting which messages can be drafted-then-reviewed and which must be drafted-by-you-then-tone-adjusted, because the failure mode for getting that sort wrong is invisible until it isn't.

---

## Learning objectives

By the end of this chapter, you should be able to:

1. **Apply.** Use AI to draft a parent communication from rough bullet notes, specifying tone and relationship context.
2. **Apply.** Use AI to produce a meeting summary or action-items document from rough notes.
3. **Apply.** Write a prompt for a behavioral report that includes a factual record, family-appropriate tone, and a district-template format.
4. **Analyze.** Apply the communication phase gate: routine communications — AI drafts, teacher reviews and sends; sensitive communications — teacher drafts core message, AI adjusts tone only.
5. **Evaluate.** Identify the communications AI should not draft at all — those where the teacher's authentic, specific noticing is the primary value the family is reading the message for.

---

## 1. Opening case — the Sunday progress-report shift

*This case is composite-illustrative. The teacher is not a single documented person. The arithmetic of 600 comments per year and the 72-to-16-hour reduction is a plausible-shape example drawn from the IEP-and-progress-report AI-adoption literature ([EdWeek 2025](https://www.edweek.org/teaching-learning/teachers-are-using-ai-to-help-write-ieps-advocates-have-concerns/2025/10)); it is not measured for any specific teacher. The 50% / 2.5-hour weekly reduction projected by the book's overall time model has not been independently validated in a teacher-week time-use study and is presented as an estimate, not a finding. [verify against any future workload audit that breaks out communication-task time separately.]*

It is 7:42 on a Sunday evening in late October. A middle-school English teacher — call her Ms. Patel — has 150 students across five sections. Progress reports go home Friday. 150 individual comments. Last year, comments took her about seven minutes each — pull up the gradebook, scan six weeks, find a way to say *quiet but improving, watch the homework, please reach out if you want to talk about Wednesdays*, do it again 149 times. Eighteen hours per cycle. Four cycles a year. Seventy-two hours every year on the form of observations she had already made.

This Sunday is different. Across the quarter she has been adding two-or-three-line bullets to a private notes document for each student. *Sept 12 — strong on the Sandra Cisneros essay, great answer in discussion. Sept 19 — late on vocab quiz. Oct 17 — homework holding, parent emailed about a soccer tournament Wednesday, said she might be tired.* Five lines per student, accumulated across six weeks instead of conjured at the deadline.

She opens Claude, pastes her bullets for the first student into a prompt template she has been refining since August — three sentences in the school's required register, warm and specific, opens with something concrete, names one growth target, invites contact. The model returns a draft. She reads it against her bullets. Every claim traces. She edits one word and pastes into the gradebook. Ninety seconds. She does it 149 more times.

Five hours, not eighteen. The fifty-six hours she did not spend writing comments this year, she spent in parent conferences and on three phone calls she had been putting off — the part of the job nobody else could do. The comment-rendering was what she had been doing instead, because the deadline was Friday and the conferences were "later."

Three things to name. First, the AI did not "write the comments"; it rendered observations Ms. Patel had already made. Second, the savings came from substitution — *form-rendering time* moved out, *relational time* moved in. Third, the workflow only works because she did the boring discipline of writing bullets across the quarter. Without the bullets, the model would have invented plausible-sounding comments about students it had never met. That is the failure mode this chapter is built around.

---

## 2. The core concept — sorting messages before drafting them

A teacher's communication week is not one task. It is four or five tasks bundled under one label, sitting at very different places on the AI gate. The chapter rests on a sort.

### 2.1 The routine / sensitive split — a risk distinction, not a content distinction

The first move is not *what is this message about?* It is *what happens if this message is partly wrong?* Three operational tests sort to the right bucket:

1. **School-board-readable test.** Would you be comfortable if this message were read aloud in a school-board meeting six months from now?
2. **Informational-versus-relational test.** Is the parent reading this for the information it contains, or for evidence that *you know their kid*? Field-trip permission slips are informational. *I noticed Maya solved the volume problem in an unusual way today* is relational.
3. **Factual-error-risk test.** Could a small drift produce harm — disciplinary exposure, custody complication, medical implication, professional liability? Behavioral incidents, allegations, references to other students — these tolerate zero drift. Field-trip dates do.

The third test is load-bearing. The routine/sensitive split is a *risk* distinction, not a *topic* distinction. A parent email that *looks* routine becomes sensitive the moment it names another student, references a custody arrangement, or contains a claim a parent might forward to the district.

A common misreading: *parent emails are routine; IEP narratives are sensitive*. The gate is risk, not genre. Some IEP narratives are routine (progress monitoring on a stable goal). Some parent emails are sensitive (a quiet escalation about a peer-conflict incident).

### 2.2 The tone-adjustment use case — where AI earns its keep

The highest-leverage move in this chapter, stated plainly:

> **AI converts rough teacher notes into appropriately-toned professional prose. The teacher supplies the content. The model supplies the register. The teacher reviews the prose against the content.**

This is not "AI writing for the teacher." It is *AI doing the register conversion the teacher would otherwise do by hand*. You already had the observation. You already had the judgment about how the family will hear it. What you don't always have, at 6:47 on a Thursday evening, is the energy to render the observation in three sentences that land warmly without sliding into bureaucratic stiffness or over-intimacy. Register conversion is form-work. The model is good at form-work — what Ethan Mollick in *Co-Intelligence* (2024) calls the "co-pilot" pattern.

The phase-gate placement is three-step: teacher writes bullets (the **what**); model writes prose (the **how**); teacher reads the prose against the bullets (the **did it preserve what I meant**). Step three is what gets skipped under time pressure. Step three is what catches the failures.

A misconception to flag in advance: teachers sometimes prompt the model *without bullets* — "write a parent email about Jamie's behavior this week." The model fabricates a plausible behavioral narrative. The fabricated specifics are the legal and relational exposure the chapter is most worried about. **AI tone-adjustment requires teacher-supplied content. If the bullets do not exist, the prompt is not ready.**

### 2.3 Translation — what works, what doesn't, and the accuracy you cannot see

Translation is the use case where the failure mode is invisible to the teacher deploying it. A teacher who does not speak Vietnamese cannot tell whether the model's Vietnamese rendering of *"your daughter is struggling with fractions"* communicates concern, blame, indifference, or accidentally something else. The teacher trusts the artifact precisely because they cannot evaluate it.

A peer-reviewed evaluation of Google Translate for English-to-Spanish teacher-to-parent email communication with Latino ELL families rated translations at roughly **75% accuracy**, with documented errors in literal translation, register, and punctuation — while overall meaning was usually preserved ([Castro Ponce et al. 2022](https://www.tandfonline.com/doi/abs/10.1080/15348431.2022.2104849)). General estimates for high-resource European language pairs cluster in the 80–90% range on routine prose. That is a usable floor for routine messages.

The picture changes substantially for low-resource languages — including languages widely spoken by U.S. immigrant families: Karen, Burmese, Somali, Haitian Creole, several indigenous languages. The model's *fluency* on a low-resource output is not evidence of its *accuracy*; the system can produce grammatically-shaped output that is semantically wrong. [contested] — there is no comprehensive education-specific benchmark across these languages; the inference is from general MT literature. Mechanism: a translation system is good at a language pair in proportion to how much parallel text was in its training data, and Karen-English does not have what Spanish-English has.

Three operational rules:

1. **Round-trip translate** any non-routine message. English to target, then target back to English, ideally through a different model. If the round-trip preserves your meaning, the forward translation likely did too. If it distorts, do not send.
2. **Disclose machine assistance** with a footer — *"This message was translated with AI assistance. Please contact me if anything is unclear."* That converts residual error from hidden hazard to flagged uncertainty.
3. **Never use machine translation for high-stakes communications.** IEP meetings, disciplinary communications, custody-sensitive scheduling, medical-adjacent messages, procedural-rights notices. These require qualified human translators.

The Individuals with Disabilities Education Act (IDEA) generally requires meaningful native-language access for parents in special-education communications; Section 504 carries related expectations. Whether machine translation can satisfy specific requirements in your district is a question for your district's counsel and language-access coordinator. **The principle: in any communication where a translation error could affect a student's procedural rights or the family's ability to participate meaningfully, machine translation is not sufficient. Defer specifics to your district.** [contested] — IDEA / Section 504 native-language standards as applied to machine translation are an active area without settled case law.

The equity edge: AI translation democratizes access for high-resource languages. It does not close the gap for low-resource ones and may quietly widen it, because the teacher cannot detect the gap. A district that adopts AI translation without maintaining qualified human interpreters for low-resource languages has made the situation better for some families and worse for others.

### 2.4 Administrative documentation — IEPs, meeting notes, incident reports

Administrative documentation includes meeting notes (IEP, 504, parent-teacher conferences), compliance forms, behavioral incident reports, and the broader write-it-down-or-it-didn't-happen layer of school work. The cognitive shape — *form-rendering of observations the teacher already made* — is one of the cleanest fits for AI assistance.

The workflow has three pieces. *Teacher supplies:* dated, specific notes captured during or immediately after the event. *Model produces:* the polished narrative in district-template language. *Teacher reviews:* every factual claim against the original notes, corrects drift, signs. The third step is non-negotiable.

Adoption is moving fast. A 2025 industry survey reported nearly 60% of special-education teachers used AI to develop an IEP or Section 504 plan during 2024–25, up 18 points from the previous year — 15% drafting in full, 31% identifying progress trends, 30% summarizing existing plans ([EdWeek 2025](https://www.edweek.org/teaching-learning/teachers-are-using-ai-to-help-write-ieps-advocates-have-concerns/2025/10)). Advocate concerns track the same fault line: AI-drafted plans built on thin student input may fail IDEA's individualization requirement ([K-12 Dive 2025](https://www.k12dive.com/news/artificial-intelligence-special-education-Section-504-benefits-risks-privacy-IDEA-IEP/804535/)). The pattern is settled. The legal exposure is not.

The most concrete near-term constraint is FERPA (20 U.S.C. § 1232g), which treats records containing personally identifiable student information as education records. Pasting student names, IDs, behavioral specifics, or assessment data into a *non-enterprise* AI tool — a personal ChatGPT account, a free-tier chatbot, a model without a district "school official" agreement — creates an education record outside school control and likely violates FERPA ([Future of Privacy Forum 2024](https://fpf.org/wp-content/uploads/2024/10/Ed_AI_legal_compliance.pdf_FInal_OCT24.pdf)). [contested] — specific FERPA application to AI tooling varies by state DPA implementation; defer to district policy.

The operational rule: **use only AI tools your district has vetted under a school-official agreement, OR de-identify before pasting.** *Student A, grade 7, ELL Level 3, IEP for reading* is workable. *Maya Reyes, period 4, IEP signed 9/12, last assessment 78%* is a FERPA problem waiting to be filed.

### 2.5 The sensitive-communication gate — when you draft the substance

The phase gate is sharper than in any earlier chapter:

> **For any communication with legal, behavioral, family-conflict, or relational-trust implications, the teacher writes the core message first. AI may adjust register. AI may not invent substance.**

The reason is mechanism, not policy. Three failure modes accumulate when AI drafts a sensitive communication from a thin prompt.

**Fabricated specificity.** Asked to draft a behavioral email without bullets, the model produces a confident narrative with details the teacher never provided. The teacher skims and sends. The parent reads details that don't match what the student reports. The student is correct; the model invented. The documentation now contains claims the teacher cannot substantiate.

**Smoothed-over substance.** The model's default register is professional warmth. A communication that needs to convey *concern* gets rendered as *reassurance*. The family does not understand the seriousness; the record does not show the seriousness was conveyed.

**Legal drift.** The model produces phrasings — *we will look into this matter*, *out of an abundance of caution* — that carry institutional implications the teacher did not intend and the district has not authorized. The teacher who signs the message is the one who published it.

That last failure mode connects to a broader legal point. The publisher-liability principle in U.S. defamation doctrine — *the party who publishes a defamatory statement is the responsible party, regardless of who composed the underlying text* — extends, in the controlling reading, to AI-drafted content the user signs and sends ([Tenzer 2024](https://annualsurveyofamericanlaw.org/wp-content/uploads/2024/09/02_NYS_80_2_Tenzer.pdf)). **The teacher who signs an AI-drafted statement is the one who published it.** [contested] — defamation case law for AI-drafted communications is actively developing; specific outcomes in the school-records context are not yet settled. Defer specifics to district counsel.

The deeper argument — *Frictional* in Appendix G — is that the cognitive work of *deciding what to say* in a sensitive moment is precisely the work that must remain human, because it constitutes the professional judgment the family is paying for. The form can be delegated. The substance cannot.

### 2.6 The Dual Capacity Framework, and the relationship as the irreducible

The U.S. Department of Education's *Dual Capacity-Building Framework for Family–School Partnerships* ([Mapp & Kuttner 2013](https://www.ed.gov/media/document/41-dual-capacity-building-framework-family-school-partnerships-109231.pdf)) treats family-school communication not as information transmission but as **relationship infrastructure** — *trustful relationships* are a process condition for effective partnership. Every communication is a deposit or withdrawal from the trust account. [Kraft & Rogers (2015)](https://scholar.harvard.edu/files/todd_rogers/files/empirical_in_press.kraft_rogers.pdf) showed in a field experiment that brief positive teacher-to-parent messages produce measurable changes in student behavior.

The teacher-student-family relationship is, in John Hattie's *Visible Learning* synthesis, among the higher-impact influences on student outcomes — direction well-supported across literatures, though specific effect-size magnitudes are methodologically contested ([effect-size list](https://visible-learning.org/hattie-ranking-influences-effect-sizes-learning-achievement/)). [contested] — the precise d-value is debated; the direction is robust. The CLASS framework from Hamre and Pianta operationalizes relationship quality through emotional support, classroom organization, and instructional support, with stronger effects for higher-risk students ([Pianta 2016](https://journals.sagepub.com/doi/abs/10.1177/2372732215622457)).

What this means for the chapter: when a parent senses that the teacher *knows their kid* — the specific thing this specific child did this specific week — the relational signal is doing work the information content is not. A model-drafted message cannot produce that signal because the model does not know the child. It can only produce generic-warmth-shaped prose. The parent who expected specific noticing and got generic warmth reads the *absence* — not consciously, but reliably.

This is why the final classification — *communications AI should not draft at all* — is not about content sensitivity. It is about **what the recipient is reading the message for**. If for information, AI can draft. If for evidence-that-you-know-my-kid, only you can.

### 2.7 The gate, stated

> **Routine communications: AI drafts, teacher reviews and sends. Sensitive communications: teacher drafts the core, AI adjusts only register, teacher reviews and sends. The teacher's signature is the moment of accountability — the teacher signs only what the teacher can defend.**

That is the chapter.

---

## 3. The worked example — two emails, same teacher, same Friday afternoon

The cleanest way to see the gate work is to put two communications side by side. Same teacher. Same parent. Same Friday afternoon. Different drafting workflow.

### 3.1 The routine case — a parent note about a struggling-with-homework week

*Scenario.* Ms. Patel's seventh-grade student, Maria Reyes, has turned in her lab report late for the third time this quarter — though the work, when she submits, is strong. Maria has been quiet in class, not disruptive, just disengaged. Mrs. Reyes speaks Spanish at home; her English is functional but not fluent. Ms. Patel wants a quick phone call.

**Step 1 — bullets.** Ms. Patel writes the substance herself:

```
- Maria — lab report late, third time this quarter
- Work quality when she does it is strong (esp. last narrative essay)
- Quiet in class lately, not disruptive, just disengaged
- Would like a short phone call, not a formal meeting
- Mom prefers Spanish at home, English functional
- Tone: warm but honest; name strong work first; don't catastrophize
```

The teacher has named what is true, what she wants, and what register the message needs.

**Step 2 — the prompt.**

```
ROLE: Seventh-grade English teacher writing a warm, brief, honest
note to a parent. Plain English, short sentences, no idioms.

TASK: Three-to-four-sentence email to Mrs. Reyes from the bullets
below. Open with the strong work. Name the late pattern honestly.
Invite a short phone call. Then produce a Spanish translation as a
separate block with a footer noting AI translation assistance.

CONSTRAINTS:
- Do not invent facts beyond the bullets.
- Do not catastrophize. Do not soften the late-work pattern out.
- No jargon ("engagement," "academic progress").

BULLETS: [paste above]
```

**Step 3 — what the AI produces.**

> *Hi Mrs. Reyes — I wanted to share something good first: Maria's last narrative essay was really strong, and her writing this quarter has had moments I want to make sure you know about. I also want to be honest that her lab report came in late again this week — the third time this quarter — and I've noticed she's been a bit quieter in class lately. Could we set up a short phone call this week, just to check in? Nothing formal, fifteen minutes at most. — Ms. Patel*
>
> *Hola Sra. Reyes — Quería compartir algo bueno primero: el último ensayo narrativo de Maria fue muy bueno... ¿Podemos tener una llamada corta esta semana? Nada formal, quince minutos como máximo. — Ms. Patel*
>
> *(Este mensaje fue traducido con la ayuda de inteligencia artificial. Por favor avíseme si algo no se entiende.)*

**Step 4 — the teacher review.**

Ms. Patel reads the English draft against her bullets. *Really strong* matches. *Late again this week, third time this quarter* matches. *Quieter in class lately* matches. Nothing was invented. She does the round-trip on the Spanish — pastes it back through the model with *translate to English* and reads against her original draft. Meaning is preserved. She edits one word and sends. Total elapsed time: four minutes, including the round-trip.

**What the model did:** rendered her bullets in the right register, in two languages.
**What the model did not do:** decide what to say.

The PCK move here — equivalent to Chapter 4's "I know this class will hit this misconception" — is *Ms. Patel knew to lead with the strong work*. The model did not invent that framing; she specified it. Without the bullets, the model would have produced something else, possibly something that read as concerned before it read as appreciative. That is the exact case where a model can be confidently wrong about register because it does not know the relationship.

### 3.2 The sensitive case — a behavioral incident note

*Scenario.* Same Friday afternoon. A seventh-grader, Devon, raised his voice at another student during group work, used a phrase Ms. Patel needs to document, refused two redirects, and was sent to the assistant principal's office. Ms. Patel needs both a behavioral incident report and a parent notification.

**The wrong workflow.** She prompts: *Write a behavioral incident report and parent notification for a 7th-grade student who was disruptive in class today.* She provided no details. The model produces a confident narrative with manufactured specificity — *raised his voice repeatedly, refused multiple redirects, used profanity directed at another student, left the classroom without permission.* Some happened. Some did not. The model invented the missing specifics, pattern-matching to typical middle-school disruption reports.

Three things go wrong at once. The behavioral report becomes part of Devon's disciplinary file; if challenged in a due-process hearing, it contains claims Ms. Patel cannot substantiate, and publisher liability survives authorship pathway ([Tenzer 2024](https://annualsurveyofamericanlaw.org/wp-content/uploads/2024/09/02_NYS_80_2_Tenzer.pdf)). The parent reads details Devon denies — Devon is correct — and family trust does not survive. The intervention team gets bad data; the PBIS Behavior Incident Report protocol ([NCPMI 2018](https://cfrmorris.org/wp-content/uploads/2019/04/NCPMI_BIR_v2_Training-Instructions-Definitions_10-18.pdf)) requires *objective, specific, observable* language. Fabricated specifics are the opposite.

**The right workflow.** Ms. Patel writes the substance herself, while the events are fresh:

```
Third period, ~1:42 p.m. Group work on persuasive essay.
Devon raised voice at S during disagreement about who would
present. Exact phrase: [X]. I redirected verbally, asked him to
take a break at desk near door. He remained at group table.
Redirected again, asked him to step to hallway. He did not step
out. Continued arguing. Called office; AP came down ~1:48 p.m.,
Devon walked out without further incident.
Prior pattern: two raised-voice incidents 9/19 and 10/3, both
deescalated without office referral.
```

Then the model is invited in with a tight scope:

```
ROLE: Experienced teacher writing two documents from a factual
incident record.

TASK 1: Rewrite the record below as a behavioral incident report
in district format. Preserve every fact. Do not add details. Do
not soften or sharpen. Do not introduce institutional phrasings
("out of an abundance of caution"). Quote the student's exact
phrase verbatim.

TASK 2: Brief parent notification referencing the incident, the
redirect sequence, the office referral, and a request to speak
Monday. Do not characterize intent. Do not predict consequences
beyond what occurred.

CONSTRAINTS:
- Every fact must trace to the record.
- If anything is ambiguous, ask before generating.

INCIDENT RECORD: [paste above]
```

**The teacher review.** Ms. Patel reads each sentence against her record. Every claim must trace. Anything that doesn't trace gets struck. Anything that softens the seriousness gets sharpened; anything sharpened beyond observation gets softened. The exact phrase is preserved verbatim. For the parent notification she reads against a different test: *would I be comfortable if this were forwarded to district counsel?*

Three things to notice. The model never decided anything; it rendered. The right workflow takes maybe twenty minutes; the wrong took five — but the five-minute version produces the documentation crisis. And the institutional phrasings never appeared because she told the model not to use them. The prompt itself is a phase-gate enforcement mechanism.

### 3.3 The lesson and the limit

AI is genuinely useful for tone-rendering teacher-supplied substance. The dividend is largest on routine communications where the substance is well-defined and the register cost is the bottleneck. It is smaller on sensitive communications where the substance must be teacher-authored — but not zero, because tone-rendering and format-translation still earn their keep.

The limit: there is a class of communication where the value to the recipient is not the information but *the evidence that you know their kid*. AI cannot manufacture that evidence. A model-drafted *I noticed Maya solved the volume problem in an unusual way today* is generic praise dressed up as specific noticing. Parents read the absence.

---

## 4. The three prompt templates

These three templates are the chapter's take-home artifact. They specialize the Chapter 3 four-component structure (role / context / task / constraints) for the three communication shapes a teacher hits most often. Save them. Edit them in place. They are starting points, not commandments.

### 4.1 Template — parent progress note from teacher bullets

```
ROLE: Experienced [grade] [subject] teacher writing a [warm /
professional / formal] note to a parent.

CONTEXT:
- Student identifier: [redact PII for non-vetted tools]
- Parent name and preferred mode of address
- Family communication preferences (language, phone vs. email)
- Relationship history (first contact, ongoing, prior concerns)

TASK: Write an [N]-sentence email from the bullets below. Open with
[specific move]. Name the [concern / pattern / request] honestly.
Close with [specific invitation]. Sign as [signature].

CONSTRAINTS:
- Do not invent facts beyond the bullets.
- Do not catastrophize. Do not soften out of existence.
- No jargon ("engagement," "stakeholders," "interventions").

BULLETS: [paste 4–8 lines: what's true, what you want, what
register the family needs]
```

### 4.2 Template — meeting summary or action-items document

```
ROLE: Experienced teacher producing a clear meeting summary in
[district template / action-items format].

CONTEXT: Meeting type [parent-teacher / IEP / 504 / team]. Attendees
[role-only for non-vetted tools]. Date, duration, purpose in one
sentence.

TASK: Structured summary with markdown headers:
- Topics discussed (bulleted)
- Decisions made (with decision-maker by role)
- Action items (with owner-role and due date)
- Open questions for next meeting

CONSTRAINTS:
- Every claim must trace to the notes.
- Do not soften disagreements; if attendees disagreed, name that.
- Do not infer intent or attribute motives.
- No PII beyond what notes already include.

NOTES: [paste dated, rough meeting notes]
```

### 4.3 Template — class newsletter or announcement

```
ROLE: Experienced [grade] teacher writing a [weekly newsletter /
one-off announcement] for families reading on phones.

CONTEXT: Audience [grade] families. Tone [warm / informative /
urgent]. Languages [English / English + Spanish / etc.].

TASK: [N]-word announcement with sections:
- One-line opening with the most important thing
- This week's learning (2–3 bullets, plain English)
- Reminders (dates, deadlines, what students bring)
- One "ask" if there is one
If multiple languages, each in a labeled block, AI-translation footer
on non-English versions.

CONSTRAINTS:
- No "we are excited to share" or corporate openers.
- No PII for individual students.
- Specific dates and times, not "next week."
- Sentences capped at 20 words for phone readability.

CONTENT BULLETS: [paste 5–10 lines]
```

---

## 5. Common misconceptions

Four worth naming explicitly. Each is a place where the chapter's gate fails quietly under time pressure.

**Misconception 1: "AI handles parent communication."** It does not. AI handles the *register conversion* of parent communication you have already substantively composed. The substance — what is true about this child, what the family needs to hear, what the relationship can carry — comes from you. A workflow where AI generates parent communications from thin prompts produces fabricated specificity, smoothed-over substance, or institutional drift, and the teacher who signs is the publisher. The dividend is real precisely where you do the substantive work and the model does the form-rendering.

**Misconception 2: "Translation is solved."** It is not. Translation is usable for routine prose in high-resource language pairs at roughly 80–90% meaning preservation — useful, real, worth deploying with a round-trip check and an honesty footer. It is not solved for low-resource languages (Karen, Burmese, Somali, Haitian Creole, indigenous languages), where the model can be confidently wrong and the teacher cannot detect the error. And it is not appropriate, as a substitute for qualified human translators, for any communication involving procedural rights, medical content, custody scheduling, or formal disciplinary proceedings. Defer specifics to your district.

**Misconception 3: "Tone is window dressing."** It is not. The Dual Capacity Framework treats family-school communications as relationship infrastructure ([Mapp & Kuttner 2013](https://www.ed.gov/media/document/41-dual-capacity-building-framework-family-school-partnerships-109231.pdf)). Kraft and Rogers showed that even brief positive-content messages from teacher to parent produced measurable changes in student behavior ([Kraft & Rogers 2015](https://scholar.harvard.edu/files/todd_rogers/files/empirical_in_press.kraft_rogers.pdf)). Tone is what determines whether the message lands as *concerned partner* or *bureaucratic functionary*. A communication whose register is wrong has done its damage before the recipient finishes reading.

**Misconception 4: "Use AI for the hard messages too — it's better at staying calm."** This is the most dangerous of the four, because it is true on the surface and wrong underneath. A model will produce calmer prose than a tired teacher at 9:47 p.m. on a Thursday. The problem is not the calm. The problem is that the model has no judgment about *what should be said*. It will be calm about details that did not happen. It will be calm about a softened version of a serious incident that needed to land seriously. It will be calm with corporate-tone phrasings the teacher did not intend. Calm is the register the model defaults to. *Right* is the register you are responsible for.

---

## 6. Exercises

Three exercises, graduated. Do them in order.

### 6.1 Classify a week's communications (warm-up)

Pull every parent, administrative, and family-facing message you sent in the last full school week — email, LMS message, phone-call notes, progress notes, incident reports, newsletters. At least 10 messages; do not exclude routine ones.

For each, apply the three operational tests from §2.1: school-board-readable, informational-vs-relational, factual-error-risk. Sort into a 2x2: *routine vs. sensitive* on one axis, *AI-appropriate (with review) vs. teacher-drafted-substance (AI tone-adjusts only)* on the other. Most teachers will be surprised by where some "routine-looking" messages land. The exercise's value is in the surprises.

Write one paragraph: what proportion of your week's communications are sensitive in the chapter's sense? Were any drafted in a way that didn't match where they land on the gate? What would you change about Monday's workflow?

### 6.2 Tone-shift comparison (apply)

Pick a recent routine communication you drafted manually. Write the bullets you would have used. Run them through the §4.1 progress-note template. Compare the AI draft to your original. Where did the model *add value* (register, brevity, structure)? Where did it *drift* (overstatement, understatement, fabricated specifics, missing nuance)? What does the comparison reveal about your prompt — what would you add to your next bullets to close the gap? Save the refined prompt as the first entry in your communication prompt library.

### 6.3 Create a sensitive-communication workflow (create)

Take one sensitive communication you drafted in the last month — a behavioral note, an academic-concern email, a family-difficulty follow-up. Don't pick the hardest one; pick a typical one. Build out the §3.2 workflow: (1) write the substance in your own voice — dated, specific, observable, in the format you would want under cross-examination; (2) write a tightly-scoped prompt asking the model only to *render in district format* and *adjust register*, with explicit *do not invent / do not soften / do not introduce institutional phrasings* constraints; (3) run the model; (4) review every sentence against your record — strike anything that does not trace; (5) compare to what you actually sent at the time.

Write one paragraph: what would have changed? Save the workflow as a second entry in your prompt library, tagged *sensitive*.

---

## 7. What would change my mind

A rigorous parent-perception study — one that randomized parents to receive AI-drafted versus teacher-drafted communications of equivalent substantive content, measured their sense of *the teacher knows my child*, and showed no detectable difference under blind review — would substantially weaken the chapter's strongest claim. The relational-signal argument in §2.6 rests on the inference that recipients can tell the difference between specific noticing and pattern-matched warmth. If parents cannot tell — at scale, across diverse family populations — then the gate's location in §2.5 needs to move. The mechanism would still apply to high-stakes documentation (defamation, FERPA, IDEA), but the everyday relational case for teacher-drafted substance would be weaker than the chapter currently treats it.

---

## 8. Still puzzling

Four things I do not yet know how to settle.

**The parent-perception gap.** Industry surveys exist; rigorous parent-side evaluation of AI-drafted versus teacher-drafted communications does not, as of early 2026. The chapter's argument that *parents read the absence of specific noticing* is grounded in the Hamre-Pianta and Mapp-Kuttner literatures, but the specific empirical question has not been studied at scale.

**Translation equity over time.** If AI translation continues to improve for high-resource languages while improving slowly for low-resource ones, does the gap between families served well and families served poorly widen or narrow over five years? Mechanism stories run both directions; the longitudinal study does not exist.

**Long-run relational drift.** If a teacher uses AI tone-adjustment for routine messages across a full school year — properly, with bullets, with review — does the family's sense of the teacher-as-relational-presence shift? The mechanism argument predicts yes at some level. The empirical study is not done.

**Defamation in school records.** The publisher-liability principle is settled. The case law applying it to AI-drafted school records is not. The first appellate decision will tell us a great deal about which workflows survive.

---

## 9. Bridge to Chapter 8

Chapters 4 through 7 cover the four text-heavy categories of a teacher's week. Each rests on the same insight — AI is a strong form-renderer for human-supplied substance, and the phase gate is the boundary. Chapter 8 turns from text to visual output. Slides have their own version of the same problem: a structurally correct deck the model can produce in minutes, and a teaching-correct deck that requires a vocabulary for what makes a slide *teach* rather than *display*. The gate moves. The principle does not.

---

**Tags:** parent communication; family-school partnership; FERPA; IDEA; machine translation; Dual Capacity Framework; behavioral documentation; phase gate; tone adjustment; defamation
