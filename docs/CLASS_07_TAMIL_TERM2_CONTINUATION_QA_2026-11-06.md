# Class 07 Tamil — Term 2 — Continuation QA (2026-11-06)

**Repository:** https://github.com/Eaglesiva/tn-class-07  
**Branch:** `main`  
**Status:** `PARTIAL_MASTER_SYNC — NOT TERM COMPLETE`  
**Edition:** `CURRENT_VALIDITY_UNVERIFIED` (2025 third-party text mirror and repository PDFs are references; current official edition / page-image comparison is not certified).

## Current verified unit quiz inventory

| Unit folder | Quiz records | Current disposition |
|---|---:|---|
| `02_azhiyaa_selvam` | 3 | Three one-mark answers included; two source conflicts held back |
| `02_poothodutthal` | 14 | Four-option records present; this folder currently carries three assessment groups and must retain its source/page mapping |
| `03_tamil_olir_idangal` | 0 | One open-ended visitor-guide prompt; correctly not converted |
| `04_palli_maruthirappu` | 0 | One long/open-ended summary prompt; correctly not converted |
| `04_tholirperayar` | 1 | One original MCQ accepted; one MCQ and a matching item held for answer conflict |
| `05_thirukkural` | 5 | Five original MCQs included |

**Current synced records: 23** (3 + 14 + 1 + 5). The 0-record arrays are not omitted from the audit; they contain no eligible four-option questions.

## Master sync

- Master path: `tamil/term2/book_back_questions/quiz.json`.
- The file is a live partial master: records are flattened from the four existing non-empty unit JSON files above.
- Total records: 23.
- Duplicate IDs: 0.
- Exactly four distinct options per record: yes.
- `correctOptionIndex` valid (0–3): yes.
- `sourceUrl` present: yes.
- JSON parses successfully.
- This file is **not** a completion claim for Term 2. It must be regenerated from all unit JSON files after missing units are processed.

## Incomplete / extraction issues

1. `01_kalai_vannam/questions.md` exists but includes mismatched / concatenated OCR content. Its first three MCQs do not match the Term 2 text mirror's assessment section for `ஒரு வேண்டுகோள்`. Do not invent answers or transfer records from another lesson. Re-extract the correct Book Back block from the PDF / page source before creating `answers.md`, `quiz.md`, and `quiz.json`.
2. `01_othuvathu_ozhiyal`, `03_thayirlai_thottapattu`, and `05_ilakkiya_vagai_sollgal` have page PDFs but no unit-level `questions.md` in the current tree. Extract Book Back questions from their corresponding PDF pages before proceeding.
3. Repository Term 2 contains combined / overlapping page extraction and some legacy folder slugs. Split question blocks only after matching them to actual lesson titles and PDF pages. Do not rename or move existing material based on folder names alone.
4. Open-ended / long-answer items remain placeholders only; no model answers have been written.

## Next execution order

1. Resolve the malformed `01_kalai_vannam` question extraction from page 31 and its correct assessment block.
2. Extract the missing question lists from pages 11, 14–21, and 25–30, identifying the exact lesson boundaries.
3. Complete Steps 1–3 for every applicable Term 2 unit, keeping source conflicts excluded.
4. Rebuild the Term 2 Master Quiz and perform full duplicate / options / correct-index / source validation.
5. Only then mark Term 2 complete and proceed to final all-term aggregation.

**Conclusion:** Term 2 has a valid 23-record partial Master Quiz now. The overall Term 2 unit inventory is still incomplete; this report explicitly preserves that status.
