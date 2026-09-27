# 10 — The 28-Day Roadmap, Made Operational

Your manual's roadmap, with the sequencing traps flagged. The manual's phases and this plan interlock — Week 1 = Phase 1, Week 2 = Phase 2, Week 3 = Phases 3–4, Week 4 = Phase 5.

---

## The one thing that will actually sink this project

**Not the analysis. The data collection.**

Four countries × (1 framework document + AG reports + PAC reports + IMF Article IVs + budget annexes) is roughly **40–60 documents**, most of them PDFs of 50–300 pages, several behind sites that block automated access, and some simply not online.

If you spend Week 2 hunting for documents, you will not code them, and you will not write Chapters 3, 4 or 5.

**So: collect everything in Week 1, while scoring nothing.** Download aggressively, name files systematically, and log them as you go. Days 5–7 of Week 1 and all of Week 2 must be pure reading and scoring.

---

## Before Day 1 — three things to lock

- [ ] **Submit the ethics form.** It is the manual's Week 1 item and it blocks collection. Content: `09-Ethics-Access-and-Sharing.md` Part 3.
- [ ] **Freeze the 21-indicator architecture.** Adopt, adapt or replace the proposal in `02-OECD-2024-Benchmark-Map.md` Part D. **Changing indicators after you have scored invalidates every score you have taken** — this is the single most expensive mistake available to you.
- [ ] **Get employer permission** for the employer artifact if you intend to use it (`08-Insider-Practice-Note-WITHHELD.md`).

---

## WEEK 1 — Data (Phase 1)

**Goal: every document downloaded, named, logged. Zero scoring.**

| Day | Task | Output |
|---|---|---|
| 1 | Set up `Document_Register.csv`, the folder structure, and the two-corpus separation (`_FRAMEWORK/`, `_EVIDENCE/`) | Working register |
| 1 | Download the OECD Guidelines 2024 (cite by DOI, not the mirror) | BENCH-01 |
| 2 | Download the 4 national framework documents — see `03-Framework-Documents.md` for URLs and access workarounds | BHS/JAM/BRB/TTO-FW-01 |
| 3–4 | Download the evidence corpus: AG reports (last 5 years each), PAC reports, IMF Article IVs, budget/Fiscal Strategy Reports — see `04-Evidence-Documents.md` | 20–40 rows in the register |
| 5 | Log every document: country, type, year, URL, format, accessibility, **shareability ruling**, `Framework or Evidence` | Register complete |
| 5 | **Run the Disclosure Audit** (top ~20 SOE websites — see `04-Evidence-Documents.md` §5) | Audit table |
| 6–7 | **Start Chapter 2 (Literature Review)** using `06-Academic-Reference-Library.md` | Lit review draft |

> **Naming convention — adopt it on Day 1, not Day 5.** 
> `{ISO3}-{FRAMEWORK|EVIDENCE}-{AG|PAC|IMF|BUDGET|STATUTE}-{YYYY}.pdf` 
> e.g. `BHS-EVIDENCE-AG-2023.pdf`, `TTO-FRAMEWORK-STATUTE-2011.pdf`. 
> With 50 documents you will not remember what `report_final_v2.pdf` was, and you will not be able to tell framework from evidence — which is the one distinction your whole methodology rests on.

**Week 1 deliverable:** Document Register + Lit Review draft + Disclosure Audit.

---

## WEEK 2 — Coding (Phase 2)

**Goal: all 84 de jure cells scored, with a quotation in every one.**

| Day | Task |
|---|---|
| 8–9 | Read the **framework** documents. Score de jure. Use `data/PCGI_Scoring_Sheet.csv` |
| 8–9 | Apply the **2-vs-3 test** mechanically — *named actor + defined trigger + specified outcome* (`05-Method-Rubric-and-PCGI.md` §2) |
| 10–11 | Start reading **Auditor General** reports. This is the highest-value evidence source and the slowest — start early |
| 12–13 | Score de facto. Fill `Evidence_Doc_Used_De_Facto` and `De_Facto_Quotation` |
| 14 | Compute `Dk` for each dimension, each level, each country. Compute PCGI. Compute `Gapk` |

**Discipline rules for this week:**
- **One country at a time, all 21 indicators.** Do not score indicator-by-indicator across countries — you will lose the local legal vocabulary and start pattern-matching.
- **Fill `Why_Not_One_Higher` for every single cell.** It forces the judgement to be explicit and gives you Chapter 4's text almost for free.
- **When a de facto score is hard, that difficulty is itself data.** "No evidence either way is located" is a finding about transparency, not a gap in your work — record it and move on.
- **Expect to overshoot.** Scoring 84 cells against a fresh rubric takes longer than it looks. If you are behind at Day 11, drop to scoring de facto at dimension level for the weakest-evidence country and **disclose the reduced granularity.**

**Week 2 deliverable:** De Jure / De Facto scores + gap table.

---

## WEEK 3 — Analysis (Phases 3–4)

**Goal: themes, charts, and the matrix.**

| Day | Task |
|---|---|
| 15–16 | **Reflexive thematic analysis.** Step 1 initial coding — log every code in `data/Reflexive_Coding_Log.csv`. Keep codes ugly and specific |
| 17 | Step 2: cluster codes into themes. **Test each theme against the standard** — does it make a claim, name a mechanism, and stay falsifiable? (`05-…Rubric.md` §6) |
| 17 | Map every theme to C1–C6. A theme mapping to no constraint goes to Chapter 4 as description |
| 18 | Build **radar charts** (7 dimensions × 4 countries) and **gap tables** |
| 19–20 | Score the **Transferability Matrix** (`data/Transferability_Matrix.csv`) and plot it |
| 21 | Draft **Chapter 3 (Methods)** and **Chapter 4 (Findings)** |

**The trap in this week:** the temptation to start with the Transferability Matrix because it is the most visibly productive task. Don't. The matrix is an *interpretation* of your scores — build the scores' story first, or the matrix will be unanchored.

**Week 3 deliverable:** Charts, matrices, Ch. 3 and Ch. 4 drafts.

---

## WEEK 4 — Writing (Phase 5)

| Day | Task |
|---|---|
| 22–23 | **Chapter 5 (Discussion).** This is where C1–C6 do their work and where the matrix becomes recommendations |
| 24 | **Chapter 1 (Introduction) and Chapter 6 (Conclusion) — write these LAST.** The manual is right: you cannot introduce a study you have not finished, and writing the intro first guarantees a rewrite |
| 25 | **Fact-check every legal reference.** Act name, year, section number, jurisdiction. Open each document and verify each citation against the source. **This is where a day of checking prevents the most damaging class of error** |
| 26 | Consistency pass: dimensions, indicator IDs, scores, totals, figure numbering, table numbering |
| 27 | Proof, format, reference list, appendices |
| 28 | **Submit** |

**Days 22–24 are the ones people lose.** Writing 3 chapters in 6 days is achievable only if Ch. 3 and Ch. 4 exist by Day 21. If you are behind, the right cut is **granularity, not chapters** — score de facto at dimension level, say so, and finish.

---

## Risk register

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Documents not obtainable for one country | **High** | High | Start Day 3. Log as `NOT OBTAINED` with reason. Disclose as a limitation. Do not silently drop the country |
| Site blocks automated access (403s observed) | High | Low | Use a browser, not a script |
| Ethics form takes longer than expected | Medium | High | Submit Day 1. Begin only document *location*, not collection, until it clears |
| Rubric 2-vs-3 ambiguity slows scoring | **High** | Medium | Apply the mechanical test. Log your reasoning in `Why_Not_One_Higher`. Accept that some calls are judgement |
| Baseline literature is thin on Caribbean SOEs | High | Medium | Widen to SIDS economics, small-state public administration, and Commonwealth Caribbean public finance. Never pad with irrelevant sources |
| The app distracts from the dissertation | Medium | Medium | One appendix, one Chapter 5 paragraph. It is evidence, not the subject |
| P1 or P2 not supported by the data | Medium | **Low — this is fine** | Report it. A partial refutation defended with evidence scores better than a forced confirmation. If D5 is *not* the lowest dimension, that is a genuine finding and needs explaining |

---

## The argument to protect, in one paragraph

Keep this visible above your desk from Day 1. Every chapter either supports it or qualifies it:

> Caribbean SIDS have largely adopted the **form** of private-sector performance management for their state-owned enterprises — targets, reporting, boards, audits — but not the **consequences** for failing to meet them. The reasons are structural to small states: there are too few people to staff independent oversight (C1), everyone is socially and politically close enough that sanctioning is personally costly (C2), the fixed costs of scrutiny cannot be spread across a small portfolio (C3), natural monopolies leave nothing to benchmark against (C4), external shocks supply legitimate excuses for missing targets (C5), and governments cannot let essential enterprises fail (C6). The OECD benchmark itself is thin on consequences and concedes that no one size fits all. Transfer is therefore possible — but it has to be **adapted to the small state, not copied from the large one.** The mechanisms that survive are those that manufacture accountability **procedurally**, through information, roles and pre-commitment, rather than relying on independent actors, competitive markets, or the credible threat of failure.
