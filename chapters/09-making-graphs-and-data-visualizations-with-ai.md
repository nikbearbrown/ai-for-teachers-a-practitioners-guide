# Chapter 9 — Making Graphs and Data Visualizations with AI

<!-- FACT-CHECK FLAG: MIXED — see factchecks/09-making-graphs-and-data-visualizations-with-ai-assertions.md -->

**Suggested titles:**
- Chapter 9 — Making Graphs and Data Visualizations with AI
- Chapter 9 — The Department Chair's Spreadsheet: A Chart Honesty Checklist
- Chapter 9 — Why the Mean Bar Chart Is the Wrong Tool for Your Equity Question

**TL;DR:** AI can produce a publication-quality chart from a plain-language description in seconds, and most of those charts will quietly lie — truncated y-axes, topic-label titles, decorative color, mean bars that hide the distribution where the equity story actually lives. The fix is not a better tool but a five-question chart checklist, anchored to Cairo's "compared with what?" and Tufte's proportional ink, that the teacher runs on every chart before it leaves the building.

---

## Learning objectives

By the end of this chapter you will be able to:

1. **(Understand)** Identify the five functional categories most useful for teacher data — comparison, change over time, distribution, relationship, part-to-whole — and explain which category each question requires.
2. **(Apply)** Write a plain-language chart request prompt that specifies what the chart is trying to show, what the data contains, and what the reader should understand in five seconds.
3. **(Apply)** Identify the three most common chart errors in education data: truncated y-axes, overcrowded pie charts, and mean bar charts where distribution is the question.
4. **(Analyze)** Apply Cairo's "compared with what?" check — every quantitative claim a chart makes requires an explicit reference.
5. **(Evaluate)** Run Tufte's proportional-ink check and the honest-title check on any chart in under five minutes.
6. **(Create)** Produce a chart of real assessment data using the AI prompting workflow, then audit and rewrite it against the five-question checklist.

**Prerequisites:** Chapter 3 (the four-component prompt structure — role, context, task, constraints) and basic numeracy (mean, median, quartile, percentile). Familiarity with a spreadsheet tool is assumed; D3 or programming experience is not.

**Phase gate:** Teacher runs the five-question chart checklist on every AI-generated chart before using it in a presentation, report, or parent communication. AI generates; teacher audits and authorizes.

---

## 1. The department chair with three years of data

It is a Saturday in March. Maya Okonkwo, math department chair at a 1,400-student public high school, is sitting at her kitchen table with three years of student performance data open in Excel. The file has 4,200 rows. Each row is one student, one unit, one assessment — score, teacher, period, race/ethnicity, English-learner status, IEP status, free-and-reduced lunch eligibility. The principal has asked for a five-slide presentation by Wednesday on "where the program is and where it's going."

Maya knows the data contains a story. She can feel it the way you can feel a draft in an old house without finding the window. The freshman scores have moved over three years. The sophomore scores have not, but she thinks the distribution has shifted. There is something in the Algebra II numbers that does not match what teachers say in department meetings. She does not have words for these patterns yet. She has Excel. She has, sitting on her phone, the same AI tools her students use. What she does not have is the next thirty hours that learning a real data-visualization stack — Tableau, R, Python, D3 — would require, and she has a class of juniors on Monday morning.

So she does what any teacher in 2026 with a deadline and a laptop does. She opens her AI tool of choice and types: *Make me a chart of these scores by teacher.*

What comes back is a six-color bar chart with a y-axis starting at 62, a title that reads "Average Score by Teacher," and a legend in a font too small to read at projection distance. The chart looks professional. It also makes Mr. Sandoval's class look like it is failing — the bars create a visual gap of roughly 4× between his bar and the highest one, and his class's mean is 71.4 against the highest class's 78.2. The data difference is 9.5%. The visual difference is dramatic. The chart claimed a story the data did not support.

Maya does not catch this. Most teachers won't. The chart looks like the charts she has seen in board presentations for fifteen years. *That* is the failure mode. AI did not invent the truncated y-axis. AI scaled it. The chart looks done. It looks professional. It is wrong.

This chapter is about catching what Maya almost missed. It is about a five-question audit, anchored in three names that matter — **Cairo**, **Tufte**, **Knaflic** — that any teacher can run on any chart in under five minutes. By the end of the chapter you will know what the AI gets right (production speed, breadth of options, decent first drafts), what it gets wrong (axis defaults, title defaults, color defaults, the choice of chart type itself), and what you have to keep in your own head.

The principle to carry through: **AI accelerates production. AI does not accelerate decision.** The decision step *is* the work, and it is the work that protects the chart from lying to its reader.

---

## 2. Concept I — Five functional categories: pick the chart by question, not by data type

The most common chart mistake teachers make — and the one AI tools cheerfully amplify — is picking a chart type by what the data *is* instead of by what the question *asks*. "I have percentages" produces a pie chart. "I have scores over time" produces a line chart. "I have two columns of numbers" produces a scatterplot. The data type drives the visual.

This is backwards. The question drives the visual. The data type is a constraint, not a recommendation.

Andy Kirk, in *Data Visualisation: A Handbook for Data Driven Design* (SAGE, 2nd ed. 2019), and the Financial Times' open-source [Visual Vocabulary](https://github.com/Financial-Times/chart-doctor/tree/main/visual-vocabulary) (FT Visual Journalism Team, lead designer Alan Smith) name nine functional categories of chart question — Deviation, Correlation, Ranking, Distribution, Change over Time, Part-to-Whole, Magnitude, Spatial, and Flow. For teacher data, five of them carry almost everything you'll need.

**Comparison — *which is bigger?*** Across categories — teachers, sections, schools, demographic groups. The default form is a sorted bar chart, ranked by value rather than alphabetically. *Sorted* is load-bearing: an unsorted bar chart asks the reader to do the comparison work that the chart was supposed to do.

**Change over time — *which way is it moving?*** Across periods — weeks, units, terms, years. Line charts when the time axis is continuous and the shape of the trend is the message. Bar charts when the periods are discrete and the magnitude in each period is the message.

**Distribution — *what does the spread look like?*** Across students within a group. Histograms, box plots, violin plots, strip plots, jittered dot plots. This is the category teachers most often skip and the category where most equity stories actually live. We will return to it in §4.

**Relationship — *do these two variables move together?*** Scatterplots when both are quantitative. Bubble charts when a third quantitative variable enters. Useful for attendance-vs-grade, formative-vs-summative, time-on-task-vs-mastery.

**Part-to-whole — *what fraction of the total?*** Stacked bars when there are more than three parts. Pies, donuts, waffle charts only when there are three parts or fewer *and* the part-to-whole gestalt is the point, not the comparison among parts. (More on pies in §5 — they are the most overused chart in education reporting.)

Here is the move. Before you open the AI tool, write the question in one sentence. Then name the category. Then ask for the chart. Watch what happens when you do this in the Maya scene:

- Vague request: *Make me a chart of these scores by teacher.* (AI produces the truncated bar chart.)
- Question-first request: *Compare mean scores across six teachers in the same course, sorted by mean, with the y-axis at zero, no decorative color, title stating the finding rather than the topic.*

Same data. Different chart. Different reader experience. Different professional judgment.

A misconception worth naming. *Choosing by question* is sometimes mistaken for *choosing by personal preference*. It is not. The question is constrained by the data and by what the reader needs to do with the chart. "I want to compare 19% to 21%" is a comparison question. A pie chart cannot show a 2-point difference; the wedges look identical. A side-by-side bar can. The pie is *wrong for this question*, not wrong as personal taste.

Cole Nussbaumer Knaflic, in *Storytelling with Data: A Data Visualization Guide for Business Professionals* (Wiley, 2015), titles her Chapter 2 "Choosing an Effective Visual." Her instruction is simple: name the audience, name the single takeaway, then pick the form. Stephen Few, in *Show Me the Numbers* (Analytics Press, 2nd ed. 2012), gives a fuller decision tree built on the same move. The instruction translates to the AI context cleanly: the prompt that names the question and the takeaway produces a better chart than the prompt that describes the data.

---

## 3. Concept II — Cairo's "compared with what?" and Tufte's proportional ink

Two instruments do most of the work in chart honesty. Both are decades old. Both apply directly to AI output. Neither is hard to run.

### Cairo: every claim has a reference

Alberto Cairo, in *The Truthful Art: Data, Charts, and Maps for Communication* (New Riders, 2016) and *How Charts Lie* (W. W. Norton, 2019), names the single most useful diagnostic for chart honesty: *compared with what?* Every quantitative claim a chart makes — *this is high, this is low, this rose, this fell* — must be set against an explicit reference. A chart that fails the check makes a claim without a reference and gives the reader a meaningless number.

Four ways the check exposes a chart that lies:

1. **Absolute counts where ratios are needed.** *30 students proficient in Mr. Smith's class, 22 in Mrs. Jones's.* Compared with what? With class size. Smith's class has 32 students; Jones's has 24. The rates are 94% and 92%. The raw count chart told the wrong story by a wide margin.
2. **Time series without baseline.** *Scores rose from 72 to 78 this year.* Compared with what? With the previous trajectory. If the three prior years were 70 → 73 → 76, then 78 is the slope continuing, not a new effect attributable to a new principal or program.
3. **Cross-sectional comparison without controls.** Comparing AP students to non-AP students on any outcome ignores selection into the groups. The honest answer to "compared with what?" requires matched controls or an explicit footnote saying no honest comparison is available.
4. **Single-value claims.** A chart that shows one number — *76% proficient* — and implies it is good or bad. Compared with what? The state average, the prior year's value, the district target — one of these has to anchor the number, or the reader has nothing to do with it.

Cairo's frame is the load-bearing one for this chapter. He treats chart choice not as an aesthetic decision but as an **ethical** one. A chart that misleads its reader is not a stylistic misstep; it is a professional failure with consequences for whoever acts on the chart. A board that allocates resources based on a truncated-y-axis bar chart of teacher scores has been deceived by the chart. The chart is testimony. The witness has an obligation.

This frame should not be softened. It is the strongest single instrument in this domain, and it changes the way a teacher reads charts permanently.

### Tufte: proportional ink and the lie factor

Edward Tufte's *The Visual Display of Quantitative Information* (Graphics Press, 1st ed. 1983; 2nd ed. 2001), Chapter 2 ("Graphical Integrity"), gives the mechanical version of Cairo's ethics. Two instruments matter.

**Lie factor** = (size of effect shown in graphic) / (size of effect in data). Tufte's rule: the lie factor should be 1.0, with an acceptable range of 0.95 to 1.05. His textbook example reports a lie factor of 14.8 — a 53% numerical change displayed as a 783% visual change. The chart claims 15× the effect the data supports.

**Proportional ink** (a refinement of his data-ink ratio): the visual magnitude of each mark on a chart should be proportional to the quantity it encodes. For a bar chart, this means the bar starts at zero and its length is the magnitude. A bar chart with a y-axis truncated at 60 breaks proportional ink — the bar's visible length encodes (score − 60), not score. The reader's eye does not correct for the truncation. The reader perceives the bar at face length.

The empirical case is settled. Anshul Pandey and colleagues, "How Deceptive Are Deceptive Visualizations? An Empirical Analysis of Common Distortion Techniques" (*CHI 2015*), measured systematic, large viewer-misperception effects from y-axis truncation. Yang and colleagues (2021) replicated across five studies; in some conditions 83.5% of participants overestimated the data effect when the y-axis was truncated. Michael Correll, Enrico Bertini, and Steven Franconeri, in "Truncating the Y-Axis: Threat or Menace?" ([*CHI 2020*, arXiv:1907.02035](https://arxiv.org/abs/1907.02035)), reviewed the field and confirmed the effect is robust even when the truncation is explicitly labeled. Putting a "scale break" mark on the axis does not save the chart.

This is the pedagogical point. AI tools — Excel's default behavior, ChatGPT's matplotlib output, Claude's Artifact charts, Julius.ai — almost all auto-fit the y-axis to the data range by default. They produce truncated bars unless you tell them not to. *Treat this as a known defect of the tool, not an occasional accident.* Every bar-chart prompt must specify zero baseline, or every output must be audited for one.

A contested edge worth naming. Tufte holds that line charts can start anywhere because they encode shape, not magnitude. Stephen Few argues line charts with non-zero baselines are nearly as dishonest as truncated bars when the visual is meant to communicate magnitude rather than trend shape. Cairo splits the difference: for change-over-time where magnitude is the message, zero baseline; for trend identification where shape is the message, the baseline can be data-fit with a clear label. The disagreement is real. The honest move is to know which message your line chart is carrying and to make the baseline decision deliberately rather than by default.

---

## 4. Concept III — Distributions over means: where the equity story lives

This is the chapter's load-bearing move. It connects directly to the running thread of the book.

The standard education report shows mean scores. *6th-grade ELA mean = 72. Algebra I unit 4 mean = 68. Period 3 mean = 76.* A bar chart of means by group is the default move in board presentations, parent newsletters, and district dashboards. AI tools default to it. Excel defaults to it. It feels like the responsible thing to show.

Watch what it hides.

A class with a mean of 72 could have produced that mean three different ways. **Tight cluster:** everyone scored between 70 and 74 — the class is uniformly near the mean. **Bimodal split:** half the class scored around 60, half around 84 — the mean is a number nobody achieved. **Long left tail:** most students scored 75–78, but eight students scored 45–55 and pulled the mean down. The bar chart shows the same height in all three cases. The teaching response should be different in each. In the bimodal case, two groups need different things; in the long-tail case, eight students need targeted intervention now; in the tight cluster, the class is moving together and the curriculum is doing its job.

A bar chart of means hides this. A **box plot** shows the median, the interquartile range, and the outliers. A **violin plot** adds the shape of the distribution. A **strip plot** or **jittered dot plot** shows every student as a single dot, so you can literally see who is where. All three reveal what the mean conceals.

Here is the equity claim, and it is direct. The research is explicit. Eli Holder and Cindy Xiong, in "Dispersion vs. Disparity: Hiding Variability Can Encourage Stereotyping When Visualizing Social Outcomes" ([arXiv:2208.04440](https://arxiv.org/abs/2208.04440), 2022; published in *IEEE Transactions on Visualization and Computer Graphics*, 2023), ran a series of experiments comparing bar-chart-of-means presentations of group differences against variance-revealing alternatives (jitter, box plots, violin plots). The finding: when subgroup differences are shown as bar charts of means, readers infer *larger, more essentialist* group differences than when the same data is shown with variability visible. Hiding the variance hardens the category in the reader's mind. A bar chart of means by demographic group does not merely fail to show the spread; it actively encourages stereotyping by making within-group variability invisible.

This is the connection to the *Frictional* argument that runs through this book. Genuine learning leaves traces — variation in error patterns, in pacing, in retrieval strength. Mean scores erase those traces. The classroom whose mean rose because the top quartile pulled away while the bottom quartile slid is a classroom with an equity story the mean obscures. The board sees improvement; the data shows that improvement came at the cost of widening the gap. A distribution chart surfaces it. A bar chart of means is, in design terms, the equivalent of removing the friction trace — the appearance of progress without the evidence of who progressed.

The single sentence to carry out of this section: **if your equity question is "who is being left behind?" and your chart is a bar of means, your chart cannot answer your question.**

This has direct prompting consequences. When the question is about subgroup performance, the AI tool's default is wrong. The prompt must specify the chart type — *box plot, faceted by demographic group* or *strip plot with median overlaid* — or the output will be a bar chart that hides the answer to your own question.

### Cleveland & McGill, briefly

While the box-plot move is the equity-critical one, it is worth knowing why some encodings are more accurate than others. William Cleveland and Robert McGill, in "Graphical Perception: Theory, Experimentation, and Application to the Development of Graphical Methods" (*Journal of the American Statistical Association* 79(387), 1984; [JSTOR](https://www.jstor.org/stable/2288400)), tested how accurately readers can decode quantitative information from different visual channels. The ranking, in decreasing order of accuracy:

**position on a common scale > position on non-aligned scales > length > angle > area > volume > color luminance > color hue.**

Bars use length on a common scale. Box plots and dot plots use position. Both are near the top of the accuracy ranking. Pies use angle — fourth on the ranking, and the reason a pie cannot distinguish 19% from 21% the way a bar can. Choropleth maps use color luminance — near the bottom, and the reason a population map shaded by total population mostly just shows where the people are, not whatever variable you meant to show. The ranking tells you, before you choose a chart, which forms preserve information accurately and which do not.

### Color: encoding, not decoration

Three rules for color in teacher charts, derived from Cleveland & McGill and from Cynthia Brewer's ColorBrewer work ([colorbrewer2.org](https://colorbrewer2.org); Harrower & Brewer, "ColorBrewer.org: An Online Tool for Selecting Colour Schemes for Maps," *The Cartographic Journal* 40(1), 2003):

1. **Color encodes when nothing else can.** If position or length can carry the data — and for almost all teacher data they can — let them. Color is the weakest perceptual channel.
2. **Hue is categorical; luminance is ordered.** Use distinct hues for distinct categories (girls/boys, ELL/non-ELL, intervention/control). Use luminance gradients (light-to-dark of one hue) for ordered categories (below grade level / approaching / on / above). A rainbow palette for proficiency levels is dishonest because hue carries no natural order.
3. **Decoration is not encoding.** A bar chart in which each bar is a different color but the color carries no information is cognitive load with no payoff. AI tools default to this almost universally — every category gets its own color whether the colors mean anything or not. Strip them out unless they encode.

A defensible default for AI-generated charts: ColorBrewer's *Set2* for categorical and *YlOrRd* or *Blues* for sequential, in colorblind-safe variants where available. Specify the palette by name in the prompt. The AI tool will use it.

---

## 5. The five-question chart checklist

The audit before any chart leaves the building.

> **CALLOUT: The five-question chart checklist (Appendix C)**
>
> 1. **What question does this chart answer?** State it in one sentence. If you cannot, the chart is not ready.
> 2. **Compared with what?** Cairo's check. Every quantitative claim must have an explicit reference — a baseline, a benchmark, a prior period, a peer group.
> 3. **Does the y-axis start at zero?** For a bar chart, always. For a line chart, when magnitude is the message — and the choice must be defended either way, not defaulted.
> 4. **Is the title a finding or a topic?** A finding states what the chart shows in a sentence with a verb. A topic states the subject of the chart. Knaflic's rule: write the verb.
> 5. **Did you check for hidden variance?** If the chart shows means, ask whether the distribution matters. If it does, replace or supplement with a distribution chart.

A sixth question lives below the surface and matters whenever AI is in the loop: **does the chart match the data I gave it?** AI tools hallucinate. Claude's Artifact charts will, under ambiguous prompts, occasionally invent tick values or relabel axes. ChatGPT's Advanced Data Analysis sometimes auto-rounds or auto-groups data in ways the prompt did not ask for. The 2025 FACTS benchmark on grounded reasoning reports hallucination rates of 3–10% on frontier models depending on task and reasoning mode [verify exact figure]. Three percent of charts is enough to embarrass you in a board meeting. Always verify chart values against the source spreadsheet.

A useful sequence: write the question, then run questions 1–5, then run question 6. Five questions take about three minutes per chart. Question 6 takes another two. Five minutes per chart. That is the audit. That is the work.

---

## 6. Worked example — Maya's chart, fixed

Back to Maya at the kitchen table. Six teachers, same course, three years of unit assessments. The data she has:

| Teacher | Mean | SD | n |
|---|---|---|---|
| Adams | 78.2 | 11.4 | 142 |
| Brennan | 76.8 | 14.2 | 138 |
| Connor | 75.3 | 8.9 | 145 |
| Diaz | 74.1 | 13.7 | 140 |
| Edelstein | 73.6 | 16.1 | 139 |
| Sandoval | 71.4 | 9.2 | 137 |

Numbers above are composite-illustrative — drawn from typical patterns in district reports, not from a real school.

### The AI default

She types: *Make me a chart of average scores by teacher.*

What comes back: a six-color bar chart with bars in alphabetical order, a y-axis running from 70 to 80, a title that reads *Average Score by Teacher*, a legend repeating the teacher names already on the x-axis, and decorative gridlines every 0.5 units.

Run the five questions.

**Q1 — What question does this chart answer?** Unclear. The chart shows that the bars are different heights. The question — *are there meaningful differences in mean outcomes across these six classrooms?* — is implied but not answered, because the chart does not tell the reader whether a 6.8-point difference matters.

**Q2 — Compared with what?** Nothing on the chart says. State average? Prior year? Department target? Within-class variance? None of it is visible. Cairo's check fails immediately.

**Q3 — Does the y-axis start at zero?** No. It starts at 70. The visible bar lengths encode (score − 70), not score. With Adams at 82.3 and Sandoval at 75.5, the visible-segment ratio is (82.3 − 70)/(75.5 − 70) = 12.3/5.5 ≈ 2.24× — so Adams's bar reads as more than twice Sandoval's. The actual score ratio is 82.3/75.5 ≈ 1.09× — about 9% higher. The lie factor — visual ratio over data ratio — is roughly 2.24/1.09 ≈ 2.05. The chart inflates a 9% difference into a 124% visual difference; the chart is misleading.

**Q4 — Is the title a finding or a topic?** A topic. *Average Score by Teacher* names the chart's subject. It says nothing about what the reader is supposed to take away.

**Q5 — Did you check for hidden variance?** No. Edelstein's standard deviation is 16.1; Connor's is 8.9. Edelstein's class is nearly twice as variable as Connor's. The mean bar chart does not show this. If the question is about teaching effectiveness or about which students are being served, the within-class variance is most of the story.

### The rewrite

Maya rewrites the prompt:

```
ROLE: You are a data visualization assistant trained on Cairo, Tufte,
and Knaflic.

CONTEXT: I have unit assessment data from six teachers teaching the
same course. Sample sizes range 137–145 students per teacher. I will
paste the full dataset below.

TASK: Produce two charts side by side.

Chart 1 — Comparison of class means with confidence:
- Horizontal bar chart, sorted descending by mean
- Y-axis starts at zero, full 0–100 score range
- Error bars showing 95% CI (use the standard deviation and n provided)
- Annotation marking the state proficiency benchmark at 70
- Title: state the finding about the spread of means
  ("Mean scores across six sections span 6.8 points; all classes
  cluster within one standard deviation of each other")

Chart 2 — Distribution view of the same data:
- Faceted box plot, one panel per teacher, sorted the same way
- Shows median, IQR, and outliers
- Same x-axis (0–100) across all panels
- Title: state the finding about within-class variance
  ("Within-class variance differs more than between-class means do")

CONSTRAINTS:
- No decorative color. Use a single color across all bars in Chart 1.
  Use the same color across all boxes in Chart 2.
- Sans-serif font, 14pt minimum.
- Use ColorBrewer Set2's first color (#66c2a5) or a colorblind-safe
  equivalent.
- Print the chart-generation code so I can verify the data binding.
- Restate what you understood before generating, and flag any defaults
  you chose to apply.
```

What the AI returns now is two charts that disagree with the original story. Chart 1 — bars at full scale — shows the six means as a tight cluster between 71.4 and 78.2, all within roughly one standard deviation of each other. The visual gap that made Sandoval's class look like it was failing collapses into what it actually is: small. Chart 2 — the box plots — shows that Edelstein's class has the widest distribution; her median is roughly at the middle of the pack, but her lower quartile reaches 55 and her upper quartile reaches 92. Three of Edelstein's students fall in the bottom 10% of all 841 students in the dataset. Sandoval's class is the second-tightest distribution; his low mean reflects a class that is performing uniformly, not a class with a long tail.

Maya's takeaway changes. The chart she was about to bring to the principal would have started a conversation about Sandoval. The chart she now has starts a conversation about the eight students in Edelstein's lower quartile — and about whether the district's intervention resources are reaching them. *The chart shifted the question.* That is what a chart is for.

### The lesson and the limit

What worked: specifying the question, specifying the form, specifying the constraints. The AI produced both charts in under a minute once the specification was complete. The decision step — *we need a distribution view here, not a comparison view* — was the work. The production step was nearly free.

What did not work, and would have if the prompt were thinner: the AI's default. Every default (axis range, title, color, chart type) was wrong for this question. None of them were wrong as defaults; they are reasonable defaults for the average request. They were wrong for *this* request, and only the teacher could know that.

What still requires Maya's eyes: did the AI compute the confidence intervals correctly? She has to spot-check at least two against a calculator. Did it use the right standard deviations? She has to verify against the spreadsheet. Did it round the medians? She has to compare the box-plot percentile labels against the underlying data. The AI hallucinates rarely on this scale of dataset, but rarely is not never. The verification is the second half of the audit.

---

## 7. Common misconceptions

Four worth naming, each a load-bearing failure mode in education chart-making.

### Misconception 1: "AI-generated charts are objective."

The chart looks professional. The chart was generated by a machine. Therefore the chart is neutral. None of these inferences follow. The chart inherits the defaults of the tool that produced it — and those defaults were chosen by humans, optimized for typical use, and tested mostly on business and finance data, not education data. The default y-axis behavior, default color palette, default chart type, default title style — all of these encode aesthetic and analytic choices that may be wrong for your data. The chart is not objective. It is the output of a pipeline whose defaults you did not configure. Auditing is not optional.

### Misconception 2: "Bar charts of means tell the story."

They tell *a* story — the story of central tendency. They hide every other story: distribution, outliers, within-group variance, the shape of the curve, who is in the lower quartile. For most education questions — especially equity questions — the hidden stories are the ones that matter. Holder & Xiong's finding makes the cost explicit: mean bar charts of group differences produce stronger essentialist inferences in readers than variance-revealing alternatives. Showing the spread is not a stylistic preference; it is a check against a specific, measurable failure of inference.

### Misconception 3: "Pie charts are fine for percentages."

Pie charts encode quantity in angle, which Cleveland & McGill ranked fourth in perceptual accuracy. Bars encode quantity in length, which ranked first. A pie cannot reliably distinguish 19% from 21%. A pie with more than three or four wedges asks the reader to compare angles whose perceptual difference is below threshold. The replacement — a sorted horizontal bar chart — is more accurate, easier to read, and works at any number of categories. Stephen Few argues to cut pies entirely. Cairo and Knaflic allow three or fewer parts when the part-to-whole gestalt is the point and comparison among parts is not. Neither would defend a five-wedge pie of district demographics in a school board slide. Replace it with a bar.

### Misconception 4: "Color makes a chart readable."

Six colors on a bar chart of three categorical variables make the chart busier, not clearer. Each color asks the reader's eye to look up something in the legend and remember it across the chart. If the data already has a position-on-common-scale encoding (the bars), the color is doing no work — except adding cognitive load and potentially excluding the 8% of male readers and 0.5% of female readers with color-vision deficiency. The defensible default is one color per chart unless color is encoding a categorical variable that is not already on an axis. AI tools default to rainbow palettes. Strip them.

---

## 8. Three prompt templates

These are starting points, not finished prompts. Each one assumes Chapter 3's four-component structure — role, context, task, constraints — and each one builds in the audit moves from this chapter.

### Template 1 — Chart type selector

Use when you have data but are not sure which chart form fits the question.

```
ROLE: You are a data visualization advisor trained on Cairo's
"compared with what?" framework, Cleveland & McGill's perceptual
ranking, and Knaflic's question-first chart selection.

CONTEXT: I have the following data: [paste 5-10 rows including
column headers and types]. My question is: [state in one sentence].
My audience is: [board / parents / staff / colleagues]. The reader
should understand [single takeaway] in five seconds.

TASK:
1. Restate the question and the takeaway in your own words.
2. Name the functional category (comparison, change over time,
   distribution, relationship, part-to-whole).
3. Recommend a chart form and name one alternative.
4. State what each form would let the reader see, and what each
   would hide.
5. Flag any reason the data is not yet ready to chart (missing
   reference, no controls for comparison, no measure of variance,
   confounded categories).

CONSTRAINTS:
- Do not produce a chart in this step. Recommend the form only.
- If a pie chart would be in the recommendation, justify it against
  a sorted bar alternative.
- If the question is about subgroup outcomes, default toward
  distribution rather than means.
```

### Template 2 — Bar chart from grade data

Use when you have aggregate data by category and want a sorted, honest bar chart.

```
ROLE: You are a chart generator following Tufte's proportional-ink
rule and Cairo's "compared with what?" check.

CONTEXT: I have aggregated data by category. The categories are
[teachers / sections / grade levels / demographic groups]. The
quantity is [scores / proficiency rate / attendance rate]. The
sample sizes per category are [list].

TASK: Produce a horizontal bar chart with the following
specifications. Print the chart-generation code so I can verify
data binding.

CONSTRAINTS:
- Y-axis (the value axis) starts at zero and runs the full natural
  range of the measure (0–100 for percentages or score-out-of-100;
  0 to maximum for counts).
- Bars sorted descending by value, not alphabetically.
- One color across all bars. No legend. Use #66c2a5 or specify a
  colorblind-safe alternative.
- Include error bars (95% CI) computed from the SD and n provided.
- Title states the finding as a sentence with a verb, not the
  topic. Example: "Three sections cluster within 4 points; one
  section's mean is 9 points lower" — not "Mean Scores by Section."
- Subtitle names the comparison anchor: state benchmark, prior
  year value, or department target.
- Annotate the relevant reference line (benchmark, target, prior).
- Restate what you understood before generating. Flag any default
  you applied that I did not specify.
```

### Template 3 — Trend chart for attendance or assessment over time

Use when you have a measure over time and want to show change.

```
ROLE: You are a chart generator following Cairo, Tufte, and
Knaflic's guidance for change-over-time visualization.

CONTEXT: I have [attendance / assessment / behavior] data by
[week / month / unit / term] over [duration]. The grouping
variable is [single overall trend / by section / by demographic
subgroup]. Sample sizes per period: [list or note if constant].

TASK: Produce a line chart of the trend. Print the chart-
generation code.

CONSTRAINTS:
- If the magnitude of the values matters (these are raw scores or
  percentages where "where the value sits" is the message), use a
  zero-baseline y-axis. If only the shape of the trend matters,
  use a data-fit y-axis with a clearly labeled axis range AND a
  one-sentence note explaining the baseline choice.
- If grouping by subgroup, show each group as a separate line. Use
  at most five lines on one chart; if more groups, facet into small
  multiples.
- Annotate any specific event the reader should associate with a
  visible inflection (curriculum change, policy change, calendar
  disruption). Without annotation, the reader will invent a
  reason for any change they see.
- Title states the finding ("Attendance dropped 6 points after
  February break and has not recovered" — not "Attendance by
  Month").
- Include the comparison anchor: prior year's trend on the same
  axes, or a benchmark target line.
- Restate what you understood before generating. Flag any default
  applied.
```

Three notes that apply across all three templates. **Restate before generating** forces the model to surface its interpretation of the request before it commits to code; if its restatement is wrong, you catch it before you spend time auditing wrong output. **Flag any default applied** turns silent decisions into visible ones; you can accept or reject them. **Print the code** lets you (or a colleague, or a student) verify that the chart binds to the right columns. AI tools do not always bind correctly. The code is the receipt.

A practical note on tool choice as of this writing. **ChatGPT Advanced Data Analysis** (OpenAI) ingests CSV/XLSX directly and produces matplotlib output you can download. **Claude Artifacts** (Anthropic) produces interactive HTML/D3 charts you can iterate on in the chat window. **Julius.ai** is a dedicated data-analyst platform built on frontier models; it connects directly to spreadsheets and exports the code (Julius.ai company materials; *TechCrunch*, July 2025 [verify exact date]). All three accelerate the production step. None of them replace the decision step. The five-question checklist is the same checklist regardless of which tool you use, and the checklist is what protects you against the parts of the chart the AI does not get right.

A caveat that matters: tools change quarterly. The list of platforms above will be incomplete or partially obsolete within a year of this book's publication. The principles — chart by question, zero baseline, finding as title, distribution over means, audit before sending — do not change quarterly. Anchor on the principles. Re-shop the tools annually.

---

## 9. Exercises

Three exercises. Run them in order. The chapter is not complete until you have done at least the first two.

### Exercise 1 — Chart real assessment data and write the finding

Take one set of assessment data from your current semester — a unit test by section, a benchmark by demographic group, attendance by week, anything where the data is real and the question is one you actually need to answer. Use Template 2 (for comparison) or Template 3 (for trend) as your starting prompt. Generate the chart. Run the five-question checklist. Iterate the prompt at least once based on what the checklist flags. Then write **one sentence** describing what the chart reveals about student learning that you did not see in the raw data.

The single-sentence finding is the deliverable. If you cannot write the sentence, the chart did not answer your question. Re-prompt.

### Exercise 2 — Cairo audit of an existing report chart

Find a chart in a current district report, board presentation, state DOE dashboard, EdTech vendor brochure, or news story about your school or district. Run Cairo's "compared with what?" check on it explicitly. Identify the most serious failure mode (truncated axis, missing reference, mean bar where distribution is the question, decorative color, topic-label title). Then write the AI prompt that would have produced a more honest version of the same chart. You do not need to actually generate the corrected chart — the prompt is the artifact, because the prompt is where the audit becomes a habit.

A note. You will find these charts everywhere. State DOE dashboards are full of them. So are board slides. So is much of the press coverage of K-12 outcomes. This is not because the people producing them are dishonest; it is because the defaults are dishonest, and the production speed has outpaced the audit habit. Your job, after this chapter, is to slow the next chart down by five minutes.

### Exercise 3 — Create a distribution chart for an equity question

Take a measure for which subgroup performance is the actual policy question — proficiency by race/ethnicity, growth by ELL status, discipline referrals by IEP status, AP enrollment by free-and-reduced-lunch eligibility, anything where the question is *who is being served and who is not*. Generate **two** versions of the same data using AI:

- **Version A:** a bar chart of subgroup means.
- **Version B:** a faceted box plot or strip plot showing the distribution within each subgroup.

Compare them side by side. Write a paragraph (200–400 words) on what each version shows, what each hides, and which one you would use in a board meeting if your goal were honest reporting. Then write a sentence on which version is the *standard* board-meeting move at your institution, and why. The gap between those two answers is the chapter, restated as a local question about your own practice.

---

## 10. What would change my mind

The chapter's strongest claim — *if your equity question is "who is being left behind?" and your chart is a bar of means, your chart cannot answer your question* — rests on Holder & Xiong (2023) and the broader perceptual literature on chart misperception (Pandey 2015, Correll 2020, Yang 2021). I would update if a well-powered replication showed that variance-revealing distribution charts did **not** reduce essentialist inference in readers — or that the inferential improvement comes at a comprehension cost that makes the charts less useful in practice for non-expert audiences (administrators, parents, board members). The current evidence runs in one direction. A clean reversal would change the recommendation.

I would also update the broader chapter if a controlled study of AI-assisted chart-making with teachers showed that the five-question checklist did *not* improve chart honesty in real workflows — that teachers either skipped it, ran it superficially, or that the bottleneck was elsewhere (data literacy, statistical numeracy, time). The chapter assumes the audit is the protective move; that assumption is currently unmeasured in the teacher-AI context.

## 11. Still puzzling

A few things I do not yet have a clean answer to:

- **Hallucination rate as a function of data size.** Frontier models hallucinate data labels and tick values at 3–10% on grounded chart tasks [verify FACTS 2025]. Does this rate scale with dataset size, prompt complexity, or chart type? The 2025 multimodal-perception literature suggests AI is also worse than humans at *reading* Cleveland & McGill's perceptual tasks (Evaluating Graphical Perception with Multimodal LLMs, [arXiv:2504.04221](https://arxiv.org/abs/2504.04221), 2025). If models cannot reliably audit charts, the audit habit has to remain entirely human. How long does that remain true?
- **When to break the zero-baseline rule.** Tufte and Few disagree. Cairo splits the difference. The honest rule for teachers is probably *always zero unless you can defend the alternative in one sentence*, but I have not seen a teacher-context study that measures the cost of zero baselines in trend identification against the cost of non-zero baselines in magnitude misperception.
- **Whether the proportional-ink rule survives the move to small multiples.** A faceted distribution chart with six panels and individual x-axis ranges per panel is more readable than a single panel with everyone smashed together. But the per-panel ranges break the strict reading of proportional ink across panels. Is the local readability gain worth the cross-panel comparison loss? My current intuition is yes; my evidence is thin.
- **The right way to teach this to students.** The chapter is about teacher chart-making, but the deeper question is whether students should learn the same audit before they leave high school. If a board can be deceived by a truncated y-axis, so can a citizen. Is graphicacy a 12th-grade civics requirement? It probably should be. That is a conversation Chapter 14 (What to Tell Your Students) will continue.

---

## 12. Chapter summary and connection forward

This chapter named five functional categories — comparison, change over time, distribution, relationship, part-to-whole — and made one move with each: pick by question, not by data type. It introduced three instruments that catch most chart dishonesty: Cairo's "compared with what?", Tufte's proportional ink, and Knaflic's finding-as-title rule. It made one load-bearing equity move — *distributions over means* — and connected it directly to the running *Frictional* argument: a chart that hides the variance is the design equivalent of hiding the friction trace. It named the AI tools' systematic defaults (truncated axes, topic-label titles, decorative color, mean bars) and treated them as defects to audit, not occasional accidents. It gave a five-question checklist that takes five minutes per chart and protects you against the part of chart-making AI does not yet do well.

The teacher who runs this checklist on every chart will not produce flawless visualizations. They will produce charts that fail honestly when they fail — charts whose limits are visible, whose comparisons are anchored, whose claims have references. That is enough. That is the work.

**Bridge to Chapter 10.** Charts and slides are visual deliverables. Chapter 10 turns toward writing — both the writing you do as a teacher (syllabi, recommendation letters, departmental memos) and the writing your students do. The phase-gate question gets sharper there because writing is more entangled with the cognitive work of learning. A bar chart of means hides the equity story; an AI-generated essay can hide whether the student learned at all. Same family of problem; higher stakes.

---

**Tags:** data-visualization, charts, Cairo, Tufte, Knaflic, Cleveland-McGill, proportional-ink, distribution-vs-mean, equity-reporting, education-data, chart-honesty, AI-prompting

---

*Chapter 9 draft for review. Voice anchored to root style/ and book voice notes. Worked example is composite-illustrative; the underlying data shape is realistic for a public high-school math department, not drawn from a specific school. The truncated-y-axis failure-case search in research notes (find a real, named, citable public-facing chart with a truncated baseline) is still open and should be added before publication if a strong primary source can be located.*
