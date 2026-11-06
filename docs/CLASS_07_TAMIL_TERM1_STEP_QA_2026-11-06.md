# Class 7 Tamil — Term 1 — Step Workflow QA Report

- Audit date: 2026-11-06
- Repository: https://github.com/Eaglesiva/tn-class-07
- Scope processed: Term 1 — `ஒன்றல்ல இரண்டல்ல`, `காடு`, `அப்படியே நிற்கட்டும் அந்த மரம்`, `நால்வகைக் குறுக்கங்கள்`, `திருக்குறள்`
- Overall status: **IN PROGRESS — NOT COMPLETE**

## Repository baseline

- Tamil `questions.md` files present at baseline: 21.
- Tamil `answers.md`, `quiz.md`, `quiz.json` files at baseline: 0.
- Term page manifests contain 85 / 64 / 83 referenced PDF pages for Terms 1 / 2 / 3; all referenced paths checked in the repository tree were present.
- Class 7 has term-based books. The Master Quiz path used here is `tamil/term1/book_back_questions/quiz.json`.

## Common workflow

- Added `docs/BOOK_BACK_QUIZ_WORKFLOW_TA.md` to this repository.
- It specifies Edition Gate followed by STEP 1 (`answers.md`), STEP 2 (original textbook MCQs in `quiz.md`), STEP 3 (eligible transformed one-mark items in `quiz.md` + `quiz.json`), and final QA.
- Large-answer writing is out of scope; the three requested placeholders and `questions.md` source links are retained.

## Edition Gate

- Tamil Nadu Textbook and Educational Services Corporation (Government of Tamil Nadu) lists Class 4–7 Term 1 and Class 1–7 Term 2 textbook sales for academic year 2026–27. Official listing: https://textbookcorp.in/
- The repository stores chapter page PDFs, including the local page files linked from the five unit folders.
- The PDF bytes / cover / imprint / contents / Book Back pages have **not** been visually checked against the official 2026–27 distribution edition in this audit.
- An accessible 2025 edition textbook-text transcription mirror was used only as a secondary text cross-check: https://huggingface.co/datasets/Joemn/TamilNadu-State-board-books-2025-Tamil-and-english-versions/blob/main/7th-standard/Tamil/Class_7_Tamil_Tamil_Tamil_-_Term_1_-_2025_Edition.md
- Objective answer keys were checked against third-party chapter Guide pages:
  - ஒன்றல்ல இரண்டல்ல: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-ondralla-irandalla-question-answer/
  - காடு: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-kaadu-question-answer/
  - அப்படியே நிற்கட்டும் அந்த மரம்: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-appadiye-nirkattum-antha-maram-question-answer/
  - நால்வகைக் குறுக்கங்கள்: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-naalvagai-kurukkangal-question-answer/
  - திருக்குறள்: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-thirukkural-2-question-answer/
- Neither the third-party Guide nor the text mirror is an official Government answer key.
- Edition status: `OFFICIAL_LISTING_FOUND_PDF_UNVERIFIED`. Final publication is blocked until the relevant 2026–27 PDF pages are opened and compared.

## Unit-level deliverables

| Chapter | Step 1 prompts | Verified / reviewable answer entries | Step 2 original MCQs published | Step 3 transformed MCQs | Placeholder prompts |
|---|---:|---:|---:|---:|---:|
| ஒன்றல்ல இரண்டல்ல (இயல் 1.2) | 11 | 5 | 5 | 0 | 6 |
| காடு (இயல் 2.1) | 10 | 3 | 3 | 0 | 7 |
| அப்படியே நிற்கட்டும் அந்த மரம் (இயல் 2.2) | 12 | 5 | 5 | 0 | 7 |
| நால்வகைக் குறுக்கங்கள் (இயல் 2.5) | 14 | 2 confirmed + 1 review + 2 riddle answers | 2 | 2 | 9 |
| திருக்குறள் (இயல் 2.6) | 12 | 7 + 1 prose-to-Kural answer | 7 | 0 | 4 |
| **Processed total** | **59** | **25 confirmed + 2 review / exclusion notes** | **22** | **2** | **33** |

Notes:
- In Naalvagai Kurukkangal, the first MCQ is excluded from Quiz because the third-party Guide says “அரை” while the textbook's own rule says an AI at the end of a word has one māttirai; `வேட்கை` has AI at the end. The repository answer file marks it `REVIEW_REQUIRED_SOURCE_CONFLICT`, rather than silently overriding either source.
- In Thirukkural, the prose-to-Kural selection is answered in `answers.md` but excluded from Quiz because two printed Kural options are thematically related and a safe unique conversion was not established.
- Naalvagai's two riddles are transformed into MCQ only in STEP 3 and are explicitly labelled as transformed, not original textbook MCQ.

Each processed unit now has:
- `book_back_questions/questions.md` — cleaned question transcription with a repository PDF link and a clearly labelled secondary text-mirror reference.
- `book_back_questions/answers.md` — prompts in source order; one-mark answers + explanations + direct Guide/text references; open / long prompts have placeholders only; unresolved conflicts are labelled.
- `book_back_questions/quiz.md` — original MCQs and eligible transformed one-word items, clearly separated.
- `book_back_questions/quiz.json` — structured records corresponding to the unit Markdown quiz.

## Step results

### ஒன்றல்ல இரண்டல்ல (இயல் 1.2)
- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 11 prompts; 5 objective answers; 6 open/activity placeholders.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 5 original MCQs.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items.

### காடு (இயல் 2.1)
- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 10 prompts; 3 objective answers; 7 placeholders.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 3 original MCQs.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items.

### அப்படியே நிற்கட்டும் அந்த மரம் (இயல் 2.2)
- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 12 prompts; 5 objective answers; 7 placeholders.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 5 original MCQs.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items.

### நால்வகைக் குறுக்கங்கள் (இயல் 2.5)
- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 14 prompts; 2 objective answers confirmed; 1 source conflict held as `REVIEW_REQUIRED`; 2 riddles answered; 9 open / explanatory / activity prompts have placeholders.
- STEP 2: **PROVISIONAL / PARTIAL** — 2 original MCQs published; 1 original MCQ excluded pending source conflict resolution.
- STEP 3: **PROVISIONAL / DONE FOR ELIGIBLE ITEMS** — 2 one-word riddles transformed to MCQs; both are labelled as transformed items.

### திருக்குறள் (இயல் 2.6)
- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 12 prompts; 7 objective answers; 4 short-answer placeholders; one prose-to-Kural question answered separately.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 7 original MCQs.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items.

## Technical QA performed

- All five unit `quiz.json` files parsed successfully.
- Unit records: 5 + 3 + 5 + 4 + 7 = 24.
- Term 1 Master Quiz records: 24.
- Master Quiz exactly matches the ordered concatenation of the five unit JSON files in processed chapter order: **PASS**.
- IDs unique across all 24 records: **PASS**.
- Every record has exactly four unique options: **PASS**.
- Every `correctOptionIndex` is an integer from 0 through 3: **PASS**.
- Unit Markdown quiz counts are aligned to the corresponding JSON records; Naalvagai separates its two original MCQs from its two transformed riddles.
- External source links in the five processed question / answer / quiz folders were checked for malformed spacing.
- Local source references were changed from non-portable `file:///...` paths to repository PDF links in the five processed question files.
- Step 1 answers and quizzes have not been certified against official 2026–27 PDFs. No Unit or Subject is labelled COMPLETE.

## Remaining work

1. Verify the official 2026–27 Term 1 Tamil PDF pages / imprint against the local repository PDFs.
2. Resolve Naalvagai Q1 against the printed 2026–27 textbook edition / official material before publishing its answer.
3. Process the remaining Term 1 Tamil chapters (including `விடுதலைத் திருநாள்`, `ஆளுக்கு ஒரு வேலை`, `ஓரெழுத்து ஒருமொழி`, and the other question files / missing sub-lessons) and rebuild the Master Quiz from every eligible unit.
4. Process Tamil Terms 2 and 3.
5. Process English, Maths TM / EM, Science TM / EM, and Social Science TM / EM.
6. Run subject / term-wide final QA before marking any subject complete.

**Conclusion:** Five Class 7 Tamil Term 1 chapters now have Step 1–3 artifacts and 24 structured Quiz items (22 original + 2 transformed), with the Naalvagai conflict explicitly held for review. Structural JSON / Master sync passed. The official edition gate and the remaining chapters / subjects are still pending. Do not report Class 7 complete.
