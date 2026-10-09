# Complementary Database Searches – Search Guide

**Review:** Accuracy and Safety-Related Limitations of General-Purpose LLM Chatbots for Dental Patient Information: A Systematic Review Across Specialties
**Purpose:** Complement the API-based search of 2 October 2026 (PubMed/MEDLINE, Europe PMC incl. preprints, Semantic Scholar, Crossref, DOAJ, arXiv, AI search connectors) with licensed and supplementary sources.
**Sources covered in this guide:** Scopus · Web of Science Core Collection · EBSCO Dentistry & Oral Sciences Source · IEEE Xplore · Google Scholar
**Reporting standard:** PRISMA 2020 and PRISMA-S
**Version:** 1.0 – 2026-10-09

---

## 1. Search principles (identical to the original search)

| Principle | Rule |
|---|---|
| Concept logic | **C1 (LLM / chatbot) AND C2 (dentistry)**. No patient or outcome block (exception: Google Scholar, see §7). Patient-facing focus and outcomes are judged during screening. |
| Fields | Title, abstract, keywords (incl. indexer keywords where the platform searches them by default). |
| Publication period | 2022–2026 (publication year). |
| Limits | **None**: no language, document-type or subject-area filters. |
| Ambiguous product names | Gemini, Bard, Claude, Llama, Copilot, Mistral, Grok are kept for sensitivity. They produce some noise (e.g. "Gemini twins", llama dentition), which is removed at screening. |
| Search date | Run all sources within the same week if possible and record the exact date per source. Before submission, all sources (including the original ones) are updated together to one common cut-off date. |

### 1.1 Concept block C1 – LLM / chatbot (free text)

```
"large language model*" OR LLM OR LLMs OR chatbot* OR "chat bot*" OR ChatGPT OR "Chat GPT"
OR "GPT-3*" OR "GPT-4*" OR "GPT-5*" OR "generative pre-trained transformer*"
OR "generative pretrained transformer*" OR "generative artificial intelligence" OR "generative AI"
OR "conversational agent*" OR "conversational AI" OR "conversational artificial intelligence"
OR Gemini OR Bard OR Copilot OR "Bing Chat" OR Claude OR Llama OR DeepSeek OR Perplexity
OR Mistral OR Grok OR "ERNIE Bot" OR Qwen
```

### 1.2 Concept block C2 – Dentistry (free text)

```
dental* OR dentist* OR "oral health" OR "oral surgery" OR "oral medicine" OR "oral cancer"
OR "oral lesion*" OR maxillofacial OR orthodont* OR endodont* OR periodont* OR prosthodont*
OR implantolog* OR pedodont* OR "pediatric dentistry" OR "paediatric dentistry" OR caries
OR carious OR tooth OR teeth OR "third molar*" OR "root canal*" OR gingiv* OR temporomandibular
OR "cleft lip" OR "cleft palate" OR malocclusion OR denture* OR xerostomia OR "dry mouth"
OR halitosis OR "oral hygiene" OR avulsion
```

---

## 2. Before running the searches

1. **Peer review of the strategy (PRESS):** ask a librarian of the JLU Giessen University Library to check the strings with the PRESS 2015 checklist; document the date and reviewer.
2. **Check licence coverage:** note which editions/indexes are included in the JLU licence (especially for Web of Science; see §4).
3. **Create a search log** (template in §8) before starting, and fill it in while searching.

---

## 3. Scopus

**Interface:** scopus.com → *Advanced document search*

```
TITLE-ABS-KEY ( "large language model*" OR llm OR llms OR chatbot* OR "chat bot*" OR chatgpt OR "chat gpt" OR "gpt-3*" OR "gpt-4*" OR "gpt-5*" OR "generative pre-trained transformer*" OR "generative pretrained transformer*" OR "generative artificial intelligence" OR "generative ai" OR "conversational agent*" OR "conversational ai" OR "conversational artificial intelligence" OR gemini OR bard OR copilot OR "bing chat" OR claude OR llama OR deepseek OR perplexity OR mistral OR grok OR "ernie bot" OR qwen )
AND TITLE-ABS-KEY ( dental* OR dentist* OR "oral health" OR "oral surgery" OR "oral medicine" OR "oral cancer" OR "oral lesion*" OR maxillofacial OR orthodont* OR endodont* OR periodont* OR prosthodont* OR implantolog* OR pedodont* OR "pediatric dentistry" OR "paediatric dentistry" OR caries OR carious OR tooth OR teeth OR "third molar*" OR "root canal*" OR gingiv* OR temporomandibular OR "cleft lip" OR "cleft palate" OR malocclusion OR denture* OR xerostomia OR "dry mouth" OR halitosis OR "oral hygiene" OR avulsion )
AND PUBYEAR > 2021
```

**Notes**
- Double quotes = loose phrase (wildcards inside are allowed); `TITLE-ABS-KEY` covers title, abstract, author keywords and indexed keywords.
- Do not apply the left-hand filters (document type, subject area, language).

**Export**
- Select all → *Export* → **RIS**.
- Tick: *Citation information*, *Bibliographical information*, *Abstract & keywords* (at minimum).
- Scopus limits the number of records per export (check the limit shown in the export dialog); if the result set is larger, split by year (`PUBYEAR = 2022` … `PUBYEAR = 2026`) and export each part.
- File name: `Scopus_2026-10-XX.ris` (or `_part1`, `_part2`, …).

---

## 4. Web of Science Core Collection

**Interface:** webofscience.com → select database **Web of Science Core Collection** → *Advanced Search*

```
TS=("large language model*" OR LLM OR LLMs OR chatbot* OR "chat bot*" OR ChatGPT OR "Chat GPT" OR "GPT-3*" OR "GPT-4*" OR "GPT-5*" OR "generative pre-trained transformer*" OR "generative pretrained transformer*" OR "generative artificial intelligence" OR "generative AI" OR "conversational agent*" OR "conversational AI" OR "conversational artificial intelligence" OR Gemini OR Bard OR Copilot OR "Bing Chat" OR Claude OR Llama OR DeepSeek OR Perplexity OR Mistral OR Grok OR "ERNIE Bot" OR Qwen)
AND TS=(dental* OR dentist* OR "oral health" OR "oral surgery" OR "oral medicine" OR "oral cancer" OR "oral lesion*" OR maxillofacial OR orthodont* OR endodont* OR periodont* OR prosthodont* OR implantolog* OR pedodont* OR "pediatric dentistry" OR "paediatric dentistry" OR caries OR carious OR tooth OR teeth OR "third molar*" OR "root canal*" OR gingiv* OR temporomandibular OR "cleft lip" OR "cleft palate" OR malocclusion OR denture* OR xerostomia OR "dry mouth" OR halitosis OR "oral hygiene" OR avulsion)
AND PY=(2022-2026)
```

**Notes**
- `TS=` searches title, abstract, author keywords and Keywords Plus.
- **Record the editions/indexes** searched (e.g. SCI-EXPANDED, SSCI, ESCI, CPCI-S) and their coverage years as shown under *Editions* – required by PRISMA-S.
- No document-type or language refinement.

**Export**
- *Export* → **RIS (other reference software)** → Record content: **Full Record**.
- Maximum 1,000 records per export: export records 1–1000, 1001–2000, … as separate files.
- File names: `WoS_2026-10-XX_part1.ris`, `WoS_2026-10-XX_part2.ris`, …

---

## 5. EBSCO – Dentistry & Oral Sciences Source (DOSS)

**Interface:** EBSCOhost → select database **Dentistry & Oral Sciences Source** → *Advanced Search*

Because DOSS is a dental database, **only block C1 is applied** (C2 would reduce sensitivity without adding precision).

Enter in three rows combined with **OR**, field selector as indicated:

| Row | Field | Search terms |
|---|---|---|
| 1 | TI Title | block C1 (below) |
| 2 | AB Abstract | block C1 |
| 3 | KW Author-Supplied Keywords | block C1 |

Block C1 in EBSCO syntax:

```
"large language model*" OR LLM OR LLMs OR chatbot* OR "chat bot*" OR ChatGPT OR "Chat GPT" OR GPT-3* OR GPT-4* OR GPT-5* OR "generative pre-trained transformer*" OR "generative pretrained transformer*" OR "generative artificial intelligence" OR "generative AI" OR "conversational agent*" OR "conversational AI" OR "conversational artificial intelligence" OR Gemini OR Bard OR Copilot OR "Bing Chat" OR Claude OR Llama OR DeepSeek OR Perplexity OR Mistral OR Grok OR "ERNIE Bot" OR Qwen
```

Equivalent single-line command:

```
TI ( <C1> ) OR AB ( <C1> ) OR KW ( <C1> )
```

**Limits:** *Publication Date* 2022-01 to 2026-12. No other limiters. Leave the expanders (e.g. *Apply equivalent subjects*) at their defaults and record their settings in the search log.

**Notes**
- If JLU has no DOSS licence, record this in the search log and skip; alternatively use **CINAHL** with the full C1 AND C2 logic (same syntax, rows TI/AB/KW).

**Export**
- Add all results to *Folder* (in pages) → *Export* → **Direct Export in RIS Format**.
- EBSCO exports a limited number of records per batch (check the on-screen limit); export in parts if needed.
- File name: `EBSCO-DOSS_2026-10-XX.ris`.

---

## 6. IEEE Xplore

**Interface:** ieeexplore.ieee.org → *Advanced Search* → **Command Search**

```
("All Metadata":"large language model*" OR "All Metadata":LLM* OR "All Metadata":ChatGPT OR "All Metadata":chatbot* OR "All Metadata":"generative AI" OR "All Metadata":"conversational agent*")
AND ("All Metadata":dental OR "All Metadata":dentistry OR "All Metadata":dentist* OR "All Metadata":orthodont* OR "All Metadata":periodont* OR "All Metadata":"oral health" OR "All Metadata":tooth OR "All Metadata":teeth OR "All Metadata":maxillofacial)
```

**Filters:** Year 2022–2026 (slider on the results page). No content-type filter.

**Notes**
- IEEE Xplore limits the number of search terms and wildcards per query. If the query is rejected, split it into two runs with the same C2 block:
  - Run A: C1 = `"large language model*" OR LLM* OR ChatGPT`
  - Run B: C1 = `chatbot* OR "generative AI" OR "conversational agent*"`
- Record each run separately in the search log (hits per run); duplicates between runs are removed during deduplication.

**Export**
- Select all results (per page) → *Export* → **Citations** → Format **RIS**, *Citation & Abstract*.
- IEEE exports up to 1,000 records per batch.
- File name: `IEEE_2026-10-XX.ris` (or `_runA`, `_runB`).

---

## 7. Google Scholar (via Publish or Perish)

Google Scholar does not support truncation, limits queries to 256 characters and shows at most 1,000 results; results are not fully reproducible. It is therefore used as a **supplementary source with a fixed number of screened records**.

**Tool:** Publish or Perish (Harzing; free desktop app) → *Google Scholar* search
(Alternative: manual search on scholar.google.com and export via a reference manager.)

**Query** (patient block added here on purpose to improve precision of the first 200 hits):

```
(ChatGPT OR "large language model" OR chatbot OR "generative AI" OR Gemini OR Copilot OR DeepSeek) (dental OR dentistry OR orthodontic OR periodontal OR endodontic OR "oral surgery") (patient OR patients)
```

**Settings in Publish or Perish**
- Field: *Keywords*
- Years: 2022 – 2026
- Maximum number of results: **200**
- Sort: relevance (Google Scholar default)

**Export**
- *Save Results* → **RIS** (or CSV).
- File name: `GoogleScholar_PoP_2026-10-XX.ris`.
- Save a screenshot of the query settings and the result count.

---

## 8. Search log (fill in for every source – PRISMA-S)

| Field | Scopus | Web of Science CC | EBSCO DOSS | IEEE Xplore | Google Scholar |
|---|---|---|---|---|---|
| Platform / interface | Elsevier Scopus | Clarivate WoS | EBSCOhost | IEEE Xplore | Publish or Perish 8.x |
| Database / editions searched | Scopus | [e.g. SCI-EXPANDED 1900–present; ESCI 2005–present …] | Dentistry & Oral Sciences Source | IEEE Xplore Digital Library | Google Scholar |
| Date of search (YYYY-MM-DD) | | | | | |
| Searcher (initials) | | | | | |
| Exact string used (copy/paste) | | | | | |
| Limits applied | PUBYEAR > 2021 | PY 2022–2026 | 2022–2026 | 2022–2026 | 2022–2026; first 200 |
| Number of hits | | | | | |
| Number of records exported | | | | | |
| Export file name(s) | | | | | |
| Deviations / problems | | | | | |

Additionally save, per source: the search history (screenshot or PDF), and the export files unchanged (do not edit them in a reference manager before handing them over).

---

## 9. Quality checks

1. **Sensitivity test with known relevant records:** after export, the records retrieved are checked against the 21 benchmark studies included at title/abstract stage (Zhang et al. 2025) and further title/abstract-included records indexed in the respective database. A known record that is indexed but not retrieved indicates a gap in the string → adapt and re-run (document the change).
2. **Plausibility of hit counts:** compare the hit counts of Scopus and Web of Science; an extreme difference suggests a syntax error (e.g. missing parentheses).
3. **Spot check of noise:** look at 20 random hits; if a single ambiguous term (e.g. `Llama`, `Gemini`) dominates the noise, note it – it is not removed from the string, but explained in the methods.

---

## 10. Hand-over and further processing

Upload all export files (RIS/CSV) together with the completed search log. Processing then follows the documented pipeline:

1. Import and normalisation of all files; record counts per source.
2. Deduplication against each other **and** against all 3,055 existing unique records (including those removed before screening).
3. New unique records → title/abstract screening with the same three-reviewer procedure (R1 and R2 independent, R3 arbitration) and screening guide v1.2, followed by the ASReview quality check.
4. Update of the PRISMA 2020 flow diagram ("Identification via other methods / complementary searches"), Supplementary Table S1, the search workbook and the methods text (§2.3).

**Not part of this step:** backward/forward citation searching of included studies – this follows after full-text screening. Reference lists of the related systematic reviews (workbook sheet `Related_Reviews`) may already be checked now.
