# 01 — Project Brief, Design Logic & Deliverable Map

Everything here traces back to your *Master Execution Manual: MBA Capstone Research Guide — State-Owned Enterprise Governance in Caribbean SIDS*.

---

## 1. The research design in one page

**Title:** *Consequences without owners? Transferring private-sector performance and accountability practices to state-owned enterprises in Caribbean Small Island Developing States*

| Element | Specification |
|---|---|
| **Aim** | Evaluate the strength of performance-consequence mechanisms in Caribbean SIDS SOE governance frameworks, and recommend SIDS-appropriate private-sector practices |
| **Method** | Comparative multiple-case study, mixed methods |
| **Data** | **Secondary data only** — no interviews, no fieldwork, no primary collection |
| **Cases** | The Bahamas · Jamaica · Barbados · Trinidad and Tobago (4 countries) |
| **Benchmark** | OECD Guidelines on Corporate Governance of SOEs, 2024 revision |
| **Unit of analysis** | The national SOE governance framework, scored indicator by indicator |
| **Instrument** | Performance-Consequence Governance Index (PCGI), 21 indicators across 7 dimensions |
| **Propositions** | **P1** de jure > de facto in every country · **P2** D5 (Consequences) is the lowest-scoring dimension across the board |

**Why secondary-data-only is a strength, not a limitation:** four jurisdictions × 21 indicators × two measurement levels is already a large analytical load. Primary collection would collapse under a 28-day timeline and would trigger a much heavier ethics process. **Say this in your methodology chapter** — frame it as a deliberate design choice for comparability and replicability, not as a compromise.

---

## 2. The five phases

### Phase 1 — Data: build the Document Corpus
Two corpora that must **never** be merged:

- **Framework documents** = what the rules *require*. Statutes, regulations, monitoring manuals, the OECD benchmark itself.
- **Evidence documents** = what actually *happens*. Auditor General reports, PAC reports, IMF Article IVs, budget annexes, SOE annual reports.

**Deliverable:** the **Document Register** (`data/Document_Register.csv`) — mandated in Excel. Every document gets: type, country, exact name, year, URL, format, accessibility, reusability, whether downloaded, and a hash for integrity.

> **The single most useful habit in this project:** record *why* a document was opened and *which indicator* it feeds, in the register, at the moment you open it. Reconstructing that later from four countries' worth of PDFs is miserable.

### Phase 2 — Quantitative coding (De Jure): what the law says
- Method: **Directed Content Analysis** (Hsieh & Shannon) — you begin with the OECD-derived framework and code the law against it.
- Score each of the 21 indicators **0–3** (rubric in `05-Method-Rubric-and-PCGI.md`).
- **"Record the exact quotation and section number justifying every score… No quote means no score."**
- `Dk = mean of the 3 indicator scores` for dimension k.
- `Total PCGI (de jure) = (Σ si / 63) × 100`

### Phase 3 — Qualitative coding (De Facto): what actually happens
- Re-apply 0–3 to **reality** (see the different anchors below).
- **`Implementation Gap: Gapk = Dk(de jure) − Dk(de facto)`**
- Then **Reflexive Thematic Analysis** (Braun & Clarke): Step 1 initial coding — label every relevant sentence ("bailout without conditions", "reporting arrears"); Step 2 cluster codes into themes.
- Your manual's model theme, which is very good and worth earning: *"Accountability is legislated but not owned: monitoring duties are assigned to units that lack authority."*

### Phase 4 — SIDS constraints C1–C6 and the Transferability Matrix
Score **6–8 private-sector practices** on two axes, 1–5 each:
- **Axis 1 Governance Fit (Expected Impact)**
- **Axis 2 SIDS Feasibility**

High Fit + High Feasibility = **"Transfer Now"** · High Fit + Low Feasibility = **"Adapt First"** → plot the matrix → **answers RQ3**.

Pre-worked candidates with scores and justifications: `07-Private-Sector-Practices.md` and `data/Transferability_Matrix.csv`.

### Phase 5 — Writing: 28 days
See `10-28-Day-Roadmap.md`. The manual's instruction to write Introductions and Conclusions **last** is correct and worth obeying literally.

---

## 3. The six SIDS constraints (C1–C6) — your explanatory engine

These are what make your project more than a compliance audit. Each one explains *why* a gap exists, and each one drives the Feasibility axis. Tag every qualitative code to one or more of these; that tagging is what turns description into explanation.

| ID | Constraint | Mechanism | Where it bites hardest |
|---|---|---|---|
| **C1** | **Small talent pool** | Too few qualified people to fill all board, audit and oversight roles; the same individuals recur across public and private bodies | D6 (board independence), D7 (audit capacity) |
| **C2** | **Social/political proximity** | Everyone knows everyone; personalism makes sanctioning socially and politically costly; anonymity is fragile | D5 (consequences) — the deepest constraint |
| **C3** | **Diseconomies of scale** | High fixed costs of regulators, auditors and oversight units spread across a tiny SOE portfolio | D3, D7 — argues *against* creating new bodies |
| **C4** | **Natural monopolies** | No competitors to benchmark against; "efficiency" has no domestic reference point | D2, D3 — forces absolute, self-referential measures |
| **C5** | **Exposure to shocks** | Hurricanes and external shocks provide legitimate-sounding excuses for missing targets | D2 → D5 — erodes the credibility of every target |
| **C6** | **Fiscal constraint / soft-budget trap** | Government cannot let an essential SOE fail, so the ultimate sanction in private-sector governance is unavailable | D5 — removes the terminal consequence |

> **Note the shape of the argument this produces.** C2 and C6 are not *implementation* failures — they are **structural attributes of small states**. That is exactly why the manual's argument lands: the missing consequences are not there because officials are incompetent, but because in a state of 100,000–1.4 million people, the private sector's two ultimate disciplines are unavailable. **C1 and C4 are also directly conceded by the OECD itself** — it acknowledges "no one size fits all" and acknowledges the "no comparable entity" benchmarking problem. Cite that. It is much stronger than asserting it.

---

## 4. Deliverable map — what you produce, and where the raw material is

| Manual deliverable | Raw material in this pack |
|---|---|
| Document Register (Excel) | `data/Document_Register.csv` |
| De Jure / De Facto scores | `data/PCGI_Scoring_Sheet.csv` (84 pre-labelled rows) |
| Quotation bank | `Exact_Quotation` + `Section_Reference` columns — fill both or the score is void |
| Disclosure Audit of top 20 SOE websites | `04-Evidence-Documents.md` §5 |
| Reflexive coding log → themes | `data/Reflexive_Coding_Log.csv` |
| Radar charts + gap tables | From the dimension means in the scoring sheet |
| Transferability Matrix | `data/Transferability_Matrix.csv` + `07-Private-Sector-Practices.md` |
| Chapter 2 Literature Review | `06-Academic-Reference-Library.md` |
| Chapter 3 Methods | `05-Method-Rubric-and-PCGI.md` + `02-OECD-2024-Benchmark-Map.md` Part D |
| Chapter 4 Findings | Your own scored data |
| Chapter 5 Discussion & recommendations | `07-Private-Sector-Practices.md` + C1–C6 tagging |
| Appendix: the employer artifact (optional) | `08-Insider-Practice-Note-WITHHELD.md` |
| Ethics form | `09-Ethics-Access-and-Sharing.md` |

---

## 5. Two design decisions you must make explicit in Chapter 3

1. **Why these four countries?** The manual fixes them, but say *why*: all four are Commonwealth Caribbean SIDS with a British-derived public-finance and audit tradition, comparable legal forms, and public reporting in English. The Bahamas and Barbados are high-income SIDS; Jamaica and Trinidad and Tobago are larger, and T&T is energy-rich. **That variation is a feature** — it lets you test whether the Consequence Gap persists across fiscal capacity. If D5 is low in oil-rich Trinidad *and* in hurricane-exposed Bahamas, the gap is structural, not fiscal.
2. **Why the national legal framework as the unit, rather than individual SOEs?** Because your propositions are about *regimes*, not firms, and because a framework-level unit is what makes four-country comparison tractable in 28 days. Restrict firm-level analysis to the Disclosure Audit.

---

## 6. Threats to validity — name them before someone else does

| Threat | Why it is real here | Mitigation to state in Chapter 3 |
|---|---|---|
| **Coder subjectivity** | A single coder applying a 0–3 rubric across four jurisdictions | Publish the rubric and the quotation for every score; state your positionality; consider a small second-coder check on a 10% sample (a supervisor or peer can do this cheaply) |
| **Benchmark anaemia (D5)** | The OECD attaches few consequence provisions, so low D5 may reflect the benchmark, not the country | Explicitly separate the *drafting* gap from the *enforcement* gap — see `02-…Benchmark-Map.md` Part B |
| **De facto evidence is uneven** | Some countries publish AG reports promptly; others are years behind | Report the *latency* itself as a de facto finding — a five-year audit backlog **is** a D7/D5 data point, not a data problem |
| **Legal-text fetishism** | Scoring only what is written on the statute book misses unwritten practice | The whole point of Phase 3; triangulate every de jure score against at least one evidence document |
| **Recency asymmetry** | PFM Acts of 2001, 2019 and 2023 are not contemporaries | Score against each country's *current* framework and footnote the commencement date |
