# 09 — Ethics, Access & Shareability Rulings

You asked specifically about **whether the data can be shared**. This file gives a plain ruling for every source type in your corpus, plus the ethics form your manual requires in Week 1.

> ⚠️ **Not legal advice.** These are working research rulings based on the licence and access position of each source type, correct as at the retrieval dates in the Document Register. **Verify the licence notice on any document you intend to reproduce at length** — one line at the front of a PDF settles it, and it takes ten seconds.

---

## PART 1 — Shareability rulings by source type

Legend: **✅ Reproduce freely** · **🟡 Link, or quote briefly with attribution** · **🔴 Cite only** · **⛔ Do not use**

| # | Source type | Ruling | What you may actually do | What you must not do |
|---|---|---|---|---|
| 1 | **OECD Guidelines on Corporate Governance of SOEs 2024** | ✅ | **CC BY 4.0.** Reproduce figures, tables and extended quotations in your dissertation, in slides, in a handout, and share the PDF with your supervisor. The publication carries an explicit permission statement | Claim authorship of OECD text; represent an altered version as the official Guidelines. Translations must cite the original and identify any changes |
| 2 | **National statutes** (PFM Acts, Public Bodies Management & Accountability Act, etc.) | 🟡 | Statutes and their official texts are published public documents. **Quote sections at length** — you must, for the rubric. Share the **link** liberally | Redistribute a commercial annotated edition, a paid legal-database version (LexisNexis etc.), or a purchased consolidated PDF. Also note: **many government sites are not actually licensed for open reuse** — so *quote the law, link to it, do not republish the whole PDF* |
| 3 | **Auditor General reports** | 🟡 | Public documents, tabled in Parliament. Quote findings and cite page/paragraph numbers. Share the link | Republish in bulk. AG reports are a primary accountability record — treat with care, and **quote accurately**; misquoting an AG finding is a serious error |
| 4 | **PAC reports / Parliament hansard** | 🟡 | Public record. Quote, cite, link | Bulk reproduction |
| 5 | **IMF Article IV staff reports** | 🟡 | IMF publications are generally available for reuse with attribution; the IMF copyright policy permits quotation. Safest: quote briefly, cite fully, link | Assume blanket redistribution of a full report without checking the copyright notice on the specific document |
| 6 | **Government budget documents & Fiscal Strategy Reports** | 🟡 | Public documents. **Extract and reproduce tables and figures in your own charts** with attribution | Redistribute full PDFs in bulk |
| 7 | **Statutory bodies' / SOEs' annual reports** | 🟡 | Publicly filed. Quote results, cite page numbers, link to the posting | Treat as freely licensed |
| 8 | **Peer-reviewed journal articles** | 🔴 | Cite in full (Harvard + DOI). Quote a sentence or two within fair dealing / fair use limits. **Link to the publisher version or, better, to an open-access or repository copy** | Extract substantial portions, reproduce figures, or distribute the PDF. Do not post a paywalled PDF anywhere |
| 9 | **Books & textbooks** | 🔴 | Cite chapters and page numbers. Short quotations only | Scan, upload, or circulate chapters |
| 10 | **Working papers & preprints** (World Bank, IDB, CDB, ECLAC, *SSRN*, *RePEc* — often under CC licences) | ✅ / 🟡 | Many are CC-licensed or explicitly open access — **check the notice on each**, then quote and share accordingly. Always cite | Assume openness; verify per document. Where the notice is silent, treat as 🟡 |
| 11 | **News media** | 🔴 | Use to **locate** official documents; cite as background only | **Never as the basis of a de facto score.** Prevent republication of substantial article text |
| 12 | **The End-of-Shift Report app** (`Capstone-Christain.html`) | ⚠️ **Conditional** | May be reproduced in an appendix **with employer permission and after redaction** of operational specifics and personal data | **Never attach a real submitted report** — it contains crew names and flags named individuals. Never publish security- or operation-sensitive procedure detail. See `08-Insider-Practice-Note-WITHHELD.md` for a sanitised substitute |
| 13 | **Online corporate/agency material** | 🔴 | Cite with URL and retrieval date | Copy substantial text or logos |

### The 3 rules of thumb that cover almost everything

1. **A government is not automatically an open licensor.** "Publicly available" ≠ "freely reusable." **Quoting a statute to justify a score is always fine. Republishing the statute PDF is not.** Link it.
2. **The OECD is the one source you can lean on.** CC BY 4.0 — quote it generously, reproduce its structure, and build your instrument openly on it. Cite it every single time.
3. **Never share a paywalled PDF, even with a classmate.** Share the DOI or an open-access mirror. This is the most common way students accidentally breach policy, and it is entirely avoidable.

### Practical discipline

Keep two folders, and never mix them:

```
_CAN-SHARE/      → OECD PDF, your own charts, your own CSVs, open-licence working papers
_LINK-ONLY/      → statutes, AG reports, IMF reports, budget docs, journal PDFs
```

Put the ruling for every document in the `Reusable_Shareable` column of `data/Document_Register.csv`. Ten seconds at download time saves a rescoring exercise later.

---

## PART 2 — Access problems and how to work around them

Verified during research for this pack. Real statuses, real workarounds.

| Source | Status observed | What to do |
|---|---|---|
| **`laws.bahamas.gov.bs`** | **403 Forbidden** to automated requests | Site blocks programmatic access. **Open in a normal browser** and download manually, or use the mirrored copy of the Act (a full-text PDF of the **PFM Act 2023** was found live on `frcbahamas.gov.bs`). Do not treat the 403 as "unavailable" — it is a bot block, not a paywall |
| **`oecd.org` publication pages** | **403 Forbidden** to automated requests | Same: bot protection. Open in a browser. The **full 2024 Guidelines PDF is available via a mirror** — but for citation, always cite the **DOI** (`10.1787/18a24f43-en`), never the mirror |
| **`legalinstruments.oecd.org`** | Transport/DNS failure in testing; and the instrument number circulating in secondary sources was wrong | **The correct instrument is OECD/LEGAL/0414** (2015, reinforced 2024) — *not* 0419. Verify from the OECD Legal Instruments site or the Guidelines themselves |
| **Paywalled journals** | Expected | Use your **UniAthena / Abertay library access**. Failing that: Google Scholar → "All versions" → look for a repository copy; or email the author (researchers almost always send PDFs) |
| **Caribbean-authored literature** (SALISES, UWI, *Caribbean Journal of Public Sector Management* / *Social and Economic Studies*) | Often poorly indexed, thin open access | Go to **UWI St Augustine / Mona / Cave Hill institutional repositories**, SALISES working paper series, and the **Caribbean Development Bank** publications library directly. Expect to have to hunt. See `06-Academic-Reference-Library.md` |
| **AG reports more than ~5 years old** | Patchy online; often only physical or on request | Request directly from the Audit Office. If unobtainable for one country, **state the limitation** rather than dropping the country |

**Rule for your methodology chapter:** where a required document could not be obtained, record it in the register with status `NOT OBTAINED` and the reason, and disclose the resulting limitation. **An honest gap is methodologically stronger than a silent omission** — and a marker will look for exactly this.

---

## PART 3 — The ethics form (your Week 1 requirement)

Your manual lists the ethics form in Week 1. Your project is **secondary data only**, which puts you in the lightest category — but "secondary data" does not automatically mean "exempt." Address these six points:

### 1. State the basis plainly
> *This study uses only publicly available secondary data. No human participants are recruited, no personal data are collected, and no interviews, surveys or observations are conducted. No data are obtained under conditions of confidentiality or restricted access.*

### 2. Personal data — the one real risk
Even though you collect nothing, **published documents can contain personal data**: AG reports may name officers; SOE annual reports name directors; your own artifact captures crew names and flags individuals. Address it:
> *Where published documents identify individuals, no personal data will be extracted, and the study will not make or imply findings about identifiable individuals. Named individuals appearing in primary documents will be referred to by role rather than by name in the dissertation text.*

**Then actually do that.** Say "the General Manager," not the actual name.

### 3. The insider artifact — declare it, don't hide it
This is the item most likely to generate a question, so answer it before it is asked:
> *The researcher is employed within a Bahamian state-owned enterprise. A working operational reporting instrument developed for that enterprise is considered for inclusion as an illustrative appendix, subject to written employer permission and redaction of operational and personal content. The instrument is used to demonstrate technical feasibility only; no outcome or efficacy data are available or claimed. The researcher's professional position has been disclosed as a reflexive consideration in the methodology chapter.*

### 4. Permission (if you use the artifact)
Get a **short written confirmation** that the app may be described and reproduced for academic purposes. A single email is enough. Keep it. Do not rely on a verbal yes.

### 5. Data security and retention
> *All downloaded documents and working files are stored on a password-protected personal device. No data are stored in cloud services without access controls. Files will be retained until [date] to permit examination, then deleted.*

### 6. Conflict of interest
One sentence: state that you have no financial or governance interest in any SOE examined, and that your employment relationship is disclosed. **Disclosing it is the protection.** Concealing it is the exposure.

---

## PART 4 — Pre-submission compliance checklist

- [ ] Every source in the Document Register has a `Reusable_Shareable` ruling filled in
- [ ] No paywalled PDF is stored in a shareable folder or attached to any submission
- [ ] OECD is cited by **DOI**, not by mirror URL
- [ ] The correct legal instrument number (**OECD/LEGAL/0414**) is used
- [ ] No real shift report is attached; the app is redacted and permission is on file
- [ ] Named individuals in quoted material are de-identified to role
- [ ] Documents that could not be obtained are logged as `NOT OBTAINED` with reasons, and disclosed as limitations
- [ ] Ethics form submitted **before** document collection begins, not after
- [ ] Insider positionality is declared in the methodology chapter
- [ ] CC BY attribution notice present wherever OECD content is reproduced
