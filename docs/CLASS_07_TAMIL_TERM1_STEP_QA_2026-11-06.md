# Class 7 Tamil — Term 1 — Step Workflow QA Report

- Audit date: 2026-11-06
- Repository: https://github.com/Eaglesiva/tn-class-07
- Scope processed: Term 1 — `ஒன்றல்ல இரண்டல்ல`, `காடு`, `அப்படியே நிற்கட்டும் அந்த மரம்`, `திருக்குறள்`
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
- The repository stores chapter page PDFs, including the local page files linked from the four unit folders.
- The PDF bytes / cover / imprint / contents / Book Back pages have **not** been visually checked against the official 2026–27 distribution edition in this audit.
- An accessible 2025 edition textbook-text transcription mirror was used only as a secondary text cross-check: https://huggingface.co/datasets/Joemn/TamilNadu-State-board-books-2025-Tamil-and-english-versions/blob/main/7th-standard/Tamil/Class_7_Tamil_Tamil_Tamil_-_Term_1_-_2025_Edition.md
- Objective answer keys were checked against third-party chapter Guide pages:
  - ஒன்றல்ல இரண்டல்ல: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-ondralla-irandalla-question-answer/
  - காடு: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-kaadu-question-answer/
  - அப்படியே நிற்கட்டும் அந்த மரம்: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-appadiye-nirkattum-antha-maram-question-answer/
  - திருக்குறள்: https://samacheerkalviguide.com/samacheer-kalvi-7th-tamil-guide-thirukkural-2-question-answer/
- Neither the third-party Guide nor the text mirror is an official Government answer key.
- Edition status: `OFFICIAL_LISTING_FOUND_PDF_UNVERIFIED`. Final publication is blocked until the relevant 2026–27 PDF pages are opened and compared.

## Unit-level deliverables

| Chapter | Step 1 prompts | Objective answers in answers.md | Step 2 original MCQs | Step 3 transformed MCQs | Placeholder prompts |
|---|---:|---:|---:|---:|---:|
| ஒன்றல்ல இரண்டல்ல (இயல் 1.2) | 11 | 5 | 5 | 0 | 6 |
| காடு (இயல் 2.1) | 10 | 3 | 3 | 0 | 7 |
| அப்படியே நிற்கட்டும் அந்த மரம் (இயல் 2.2) | 12 | 5 | 5 | 0 | 7 |
| திருக்குறள் (இயல் 2.6) | 12 | 7 | 7 | 0 | 4 |
| **Processed total** | **45** | **20** | **20** | **0** | **24** |

Additional note: the Thirukkural lesson has one prose-to-Kural selection activity with an answer recorded in `answers.md`; it is excluded from `quiz.md` / `quiz.json` because the printed options include two Kural statements relevant to the theme and a safe unique four-option conversion was not established.

Each processed unit now has:
- `book_back_questions/questions.md` — cleaned question transcription with a repository PDF link and a clearly labelled secondary text-mirror reference.
- `book_back_questions/answers.md` — all prompts in source order; one-mark answers + explanations + direct Guide/text references; open / long prompts have placeholders only.
- `book_back_questions/quiz.md` — original textbook MCQs with four options, answer, explanation and source.
- `book_back_questions/quiz.json` — structured records corresponding to the unit Markdown quiz.

## Step results

### ஒன்றல்ல இரண்டல்ல (இயல் 1.2)

- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 11 prompts; 5 objective answers sourced; 6 open/activity prompts have placeholders.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 5 original MCQs cross-checked against the 2025 text mirror and third-party Guide.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items; remaining prompts are open-ended / explanatory tasks, not objective one-mark candidates.

### காடு (இயல் 2.1)

- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 10 prompts; 3 objective answers sourced; 7 open/activity prompts have placeholders.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 3 original MCQs cross-checked against the 2025 text mirror and third-party Guide.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items; remaining prompts are recitation, prosody analysis, and explanatory questions.

### அப்படியே நிற்கட்டும் அந்த மரம் (இயல் 2.2)

- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 12 prompts; 5 objective answers sourced; 7 open/activity prompts have placeholders.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 5 original MCQs cross-checked against the 2025 text mirror and third-party Guide.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items; remaining prompts are open activities and explanatory questions.

### திருக்குறள் (இயல் 2.6)

- STEP 1: **PROVISIONAL / BLOCKED BY EDITION GATE** — 12 prompts; 7 objective answers recorded; 4 short-answer placeholders retained; one passage-to-Kural item answered but excluded from Quiz due answer ambiguity.
- STEP 2: **PROVISIONAL / BLOCKED BY EDITION GATE** — 7 original MCQs cross-checked with the 2025 text mirror and third-party Guide; the final முரண்தொடை key was derived from the Kural wording and grammar context.
- STEP 3: **DONE FOR CURRENT QUESTION SET** — 0 transformed items; no other one-mark items safely eligible for conversion.

## Technical QA performed

- All four unit `quiz.json` files parsed successfully.
- Unit records: 5 + 3 + 5 + 7 = 20.
- Term 1 Master Quiz records: 20.
- Master Quiz exactly matches the ordered concatenation of the four unit JSON files in the processed chapter order: **PASS**.
- IDs unique across all 20 records: **PASS**.
- Every record has exactly four unique options: **PASS**.
- Every `correctOptionIndex` is an integer from 0 through 3: **PASS**.
- `quiz.md` numbered question counts match unit JSON counts: 5 = 5, 3 = 3, 5 = 5, and 7 = 7.
- Checked Markdown external-source links in all processed question / answer / quiz files: no malformed spaced URLs found.
- Local source references were changed from non-portable `file:///...` paths to repository PDF links in the four processed question files.
- Step 1 answers and quizzes have not been certified against official 2026–27 PDFs. Accordingly, no Unit or Subject is labelled COMPLETE.

## Remaining work

1. Verify the official 2026–27 Term 1 Tamil PDF pages / imprint against the local repository PDFs.
2. If any text differs, synchronize corrections across `questions.md`, `answers.md`, `quiz.md`, and `quiz.json`.
3. Process the remaining Term 1 Tamil chapters (including `நால்வகைக் குறுக்கங்கள்`, `விடுதலைத் திருநாள்`, `ஆளுக்கு ஒரு வேலை`, `ஓரெழுத்து ஒருமொழி`) and rebuild the Master Quiz from every eligible unit.
4. Process Tamil Terms 2 and 3.
5. Process English, Maths TM / EM, Science TM / EM, and Social Science TM / EM.
6. Run subject / term-wide final QA before marking any subject complete.

**Conclusion:** Four Class 7 Tamil Term 1 chapters have provisional Step 1–3 artifacts and passing structural JSON / Master sync checks (20 original MCQs). The official edition gate and the remaining chapters / subjects are still pending. Do not report Class 7 complete.
