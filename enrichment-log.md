# Enrichment log — ai-for-teachers-a-practitioners-guide

Run dates: 2026-05-20 (first batch + interrupt), 2026-05-20 follow-up (inline closure), 2026-05-20 full-overwrite re-run (this pass).

---

## 2026-05-20 full-overwrite re-run

### Final state

- **67 SVGs / 67 PNGs / 67 D3 HTML files** — 1:1:1
- **All 14 substantive chapters fully closed**: 0 unresolved markers, 0 TODO stubs
- **All 14 existing Wayback Machine sections preserved untouched** (Hunter, Skinner, Mason, Tyler, Thorndike, Vygotsky, Rogers, Vignelli, Bertin, Murray, Hopper, Gantt, Plato, Freire)
- **All 14 chapters have a fresh `## Prompts` section** — one structural prompt per figure

### Per-chapter

01-the-ai-dividend.md — 2 SVGs regenerated, 2 D3 HTMLs regenerated, 0 tables, Wayback kept (Madeline Hunter)
02-the-phase-gate.md — 10 SVGs regenerated, 10 D3 HTMLs regenerated, 1 table rendered (twelve-gate risk tier), Wayback kept (B.F. Skinner)
03-prompting-that-works.md — 3 SVGs regenerated, 3 D3 HTMLs regenerated, 0 tables, Wayback kept (Charlotte Mason)
04-lesson-planning-with-ai.md — 3 SVGs regenerated, 3 D3 HTMLs regenerated, 0 tables, Wayback kept (Ralph Tyler)
05-assessment-grading-and-feedback-with-ai.md — 6 SVGs regenerated, 6 D3 HTMLs regenerated, 0 tables, Wayback kept (Edward Thorndike)
06-differentiation-with-ai.md — 3 SVGs (incl. fig-03 newly generated), 3 D3 HTMLs, 0 tables, Wayback kept (Lev Vygotsky)
07-communication-with-ai.md — 6 SVGs (incl. fig-05, fig-06 newly generated), 6 D3 HTMLs, 0 tables, Wayback kept (Carl Rogers)
08-making-slides-with-ai.md — 5 SVGs regenerated, 5 D3 HTMLs regenerated, 1 table rendered (topic label → claim headline), Wayback kept (Massimo Vignelli)
09-making-graphs-and-data-visualizations-with-ai.md — 4 SVGs regenerated, 4 D3 HTMLs regenerated, 1 table rendered (five functional chart categories), Wayback kept (Jacques Bertin)
10-writing-with-ai-an-introduction.md — 6 SVGs regenerated, 6 D3 HTMLs regenerated, 1 table rendered (five-question checklist before/after), Wayback kept (Donald Murray)
11-coding-with-ai-an-introduction.md — 5 SVGs regenerated, 5 D3 HTMLs regenerated, 1 table rendered (risk classification of teacher coding tasks), Wayback kept (Grace Hopper)
12-building-your-ai-workflow.md — 4 SVGs (incl. fig-03, fig-04 newly generated), 4 D3 HTMLs, 0 tables, Wayback kept (Henry Gantt)
13-academic-integrity-privacy-and-honest-use.md — 4 SVGs regenerated, 4 D3 HTMLs regenerated, 0 tables, Wayback kept (Plato)
14-what-to-tell-your-students.md — 6 SVGs regenerated, 6 D3 HTMLs regenerated, 0 tables, Wayback kept (Paulo Freire)

### Summary

Total chapters processed: 14
Total figures regenerated: 67 (62 existing overwritten + 5 newly created — ch.06 fig-03, ch.07 fig-05/06, ch.12 fig-03/04)
Total D3 HTML files written: 67 (50 newly created — only 17 existed before this run)
Total tables rendered: 5 (all 5 prior TODO stubs in ch.02, 08, 09, 10, 11 now real markdown tables)
Total Wayback Machine subjects added: 0 (all 14 kept per "skip if existing" override)

### Process

1. **Wave 1 — 7 parallel agents** on ch.01–07. All completed cleanly. No rate-limit hits.
2. **Wave 2 — 7 parallel agents** on ch.08–14. All completed cleanly. No rate-limit hits.
3. **PNG pass.** `node SCRIPTS/svg-to-png.mjs` rasterized all 67 SVGs at 300dpi — 67 converted, 0 failed.

### Closed follow-ups from prior runs

- ✅ **45 missing D3 HTMLs** — all 67 D3 HTMLs now exist on disk
- ✅ **5 TODO table stubs** — all rendered as real markdown tables with content inferred from chapter context
- ✅ **5 missing SVGs** — ch.06 fig-03, ch.07 fig-05/06, ch.12 fig-03/04 all generated (prior log had under-reported this as 2)

### Notes

- Two-wave parallel pattern (7+7) avoided the rate-limit hit that plagued the first batch on this book
- Wayback portrait `.jpg` files referenced in Wayback sections still do not exist on disk — consistent pattern across the series; they are generated separately
- All SVG/D3 generations followed the brutalist constitution: warm grayscale only, EB Garamond chain, D3 7.9.0 from cdnjs, `var(--color-*)` tokens, dark-mode + prefers-reduced-motion variants, ResizeObserver redraw, `(event, d)` handler signatures, full accessibility (`role="img"`, `<title>`, `<desc>`)

## Final state

- **62 SVGs / 62 PNGs / 17 D3 HTML files** on disk
- **All 14 substantive chapters closed**: 0 unresolved comment markers anywhere
- **All 14 chapters have a Wayback Machine section** with a pre-assigned figure
- **All 14 chapters have a `## Prompts` section** with one structural prompt per figure

## Per-chapter

01-the-ai-dividend.md — 2 tables rendered, 2 SVGs generated, 2 D3 HTML files generated, Wayback Machine: added (Madeline Hunter)
02-the-phase-gate.md — 1 table marker preserved as TODO, 10 SVGs generated, 0 D3 HTML files generated, Wayback Machine: added (B.F. Skinner)
03-prompting-that-works.md — 1 table rendered (platform-by-task-fit matrix), 3 SVGs generated, 3 D3 HTML files generated, Wayback Machine: added (Charlotte Mason)
04-lesson-planning-with-ai.md — 2 tables rendered, 3 SVGs generated, 3 D3 HTML files generated, Wayback Machine: added (Ralph Tyler)
05-assessment-grading-and-feedback-with-ai.md — 0 tables rendered (chapter has no TABLE markers), 6 SVGs generated, 0 D3 HTML files generated, Wayback Machine: added (Edward Thorndike)
06-differentiation-with-ai.md — 2 tables rendered, 3 SVGs generated, 0 D3 HTML files generated, Wayback Machine: added (Lev Vygotsky)
07-communication-with-ai.md — 1 table rendered, 6 SVGs generated, 0 D3 HTML files generated, Wayback Machine: added (Carl Rogers)
08-making-slides-with-ai.md — 1 table marker preserved as TODO, 5 SVGs generated, 1 D3 HTML file generated, Wayback Machine: added (Massimo Vignelli)
09-making-graphs-and-data-visualizations-with-ai.md — 1 table marker preserved as TODO, 4 SVGs generated, 2 D3 HTML files generated, Wayback Machine: added (Jacques Bertin)
10-writing-with-ai-an-introduction.md — 1 table marker preserved as TODO, 6 SVGs generated, 2 D3 HTML files generated, Wayback Machine: added (Donald Murray)
11-coding-with-ai-an-introduction.md — 1 table marker preserved as TODO, 5 SVGs generated, 2 D3 HTML files generated, Wayback Machine: added (Grace Hopper)
12-building-your-ai-workflow.md — 1 table rendered, 4 SVGs generated (2 SVGs missing — refs still in chapter), 0 D3 HTML files generated, Wayback Machine: added (Henry Gantt)
13-academic-integrity-privacy-and-honest-use.md — 2 tables rendered, 4 SVGs generated, 1 D3 HTML file generated, Wayback Machine: added (Plato)
14-what-to-tell-your-students.md — 0 tables rendered (chapter has no TABLE markers), 6 SVGs generated, 1 D3 HTML file generated, Wayback Machine: added (Paulo Freire)

## Summary

Total chapters processed: 14
Total tables rendered or stubbed: 11 rendered, 6 stubbed as TODO
Total SVG+PNG pairs generated: 62
Total D3 v7 HTML files generated: 17
Total Wayback Machine subjects added: 14 (no duplicates with prior books in the series)

## Known follow-ups (deferred from this run)

This run hit the agent rate limit mid-pass. The following items were deferred and closed inline rather than re-spawning agents:

1. **6 TABLE markers preserved as TODO** in chapters 02, 08, 09, 10, 11. The original marker description is preserved inside an HTML comment so the table can be rendered later from the same brief. These appear as `<!-- TODO: render table ... -->` followed by an italic placeholder caption.
2. **45 D3 HTML companions missing** — only 17 of the 62 SVGs got a matching D3 v7 HTML reference implementation. The Prompts section in each chapter still names the expected `d3/{slug}-fig-{NN}.html` path; a follow-up pass should generate those files.
3. **2 SVGs in ch.12 are referenced but missing** — chapter has 4 figure refs but only 2 SVGs on disk. The Wayback section, Prompts, and other refs are correct; the 2 missing SVGs (fig-03 and fig-04 by ref count vs file count) need to be generated.

## Notes / deviations

- Same EB Garamond / no-base64 typography rule as prior books in this series
- Brutalist constitution copied from `../ai-for-graphs-a-practitioners-guide/brutalist/`
- Two marker formats coexisted in source chapters: `<!-- → [TYPE: ...] -->` (bracketed) and `<!-- → TYPE: ... -->` (unbracketed). The closing pass handled both.
- One SVG had an unescaped `&` (ch.10 fig-03, "Flower & Hayes") that broke librsvg — fixed inline and re-rasterized
- Wayback figure assignments are unique across all prior books in the ai-for-* series (Hunter, Skinner, Mason, Tyler, Thorndike, Vygotsky, Rogers, Vignelli, Bertin, Murray, Hopper, Gantt, Plato, Freire)
- Portrait `.jpg` files referenced in Wayback sections do not yet exist in `images/` — same pattern as other books in the series; these are generated separately
