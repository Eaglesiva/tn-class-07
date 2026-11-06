# Class 07 Tamil — Term 1 — Step 1/2/3 QA Report

**Audit date:** 2026-11-06  
**Repository:** [Eaglesiva/tn-class-07](https://github.com/Eaglesiva/tn-class-07)  
**Branch:** `main`  
**Status:** `PARTIAL — 11 UNITS HAVE STEP ARTIFACTS; 5 TERM 1 UNITS REMAIN`

## Scope and evidence

The existing repository question files and unit page manifests were inspected. Missing questions for 1.1, 1.3 and 1.5 were added using the repository page references, the 2025 Term 1 text mirror, and opened third-party Guide answer pages. The mirror and Guides are **not official Government answer keys**.

The repository PDFs are preserved as the primary page references. In this pass the PDF page images could not be independently rendered for visual comparison; therefore exact visual transcription and the current official edition remain unconfirmed.

- Text mirror: https://huggingface.co/datasets/Joemn/TamilNadu-State-board-books-2025-Tamil-and-english-versions/blob/main/7th-standard/Tamil/Class_7_Tamil_Tamil_Tamil_-_Term_1_-_2025_Edition.md
- Edition status for all processed units: `CURRENT_VALIDITY_UNVERIFIED`.
- Do not treat this report as an official 2026–27 edition certification.

## Unit-level status

| Unit | Step 1 answer / review status | Step 2 original MCQ | Step 3 transformed MCQ | Placeholder count |
|---|---|---:|---:|---:|
| 1.1 எங்கள் தமிழ் | 3 objective answers | 3 | 0 | 4 |
| 1.2 ஒன்றல்ல இரண்டல்ல | 5 objective answers | 5 | 0 | 6 |
| 1.3 பேச்சுமொழியும் எழுத்துமொழியும் | 4 MCQ + 5 சரி/தவறு answers | 4 | 0 | 6 |
| 1.4 ஆளுக்கு ஒரு வேலை | Open / activity prompts only | 0 | 0 | 3 |
| 1.5 குற்றியலுகரம், குற்றியலிகரம் | 5 odd-word answers; classification held for review | 0 | 5 | 2 |
| 2.1 காடு | 3 objective answers | 3 | 0 | 7 |
| 2.2 அப்படியே நிற்கட்டும் அந்த மரம் | 5 objective answers | 5 | 0 | 7 |
| 2.5 நால்வகைக் குறுக்கங்கள் | 2 confirmed original MCQ; 1 source conflict held; 2 riddles transformed | 2 | 2 | 9 |
| 2.6 திருக்குறள் | 7 MCQ + 1 prose-to-Kural answer (not quiz) | 7 | 0 | 4 |
| 3 விடுதலைத் திருநாள் | 6 objective answers | 6 | 0 | 5 |
| ஓரெழுத்து ஒருமொழி, பகுபதம், பகாப்பதம் | 4 original MCQ + 13 transformed objective items | 4 | 13 | 16 |
| **TOTAL** |  | **39** | **20** | **69** |

## Issues intentionally held back

1. **1.5 குற்றியலுகரம் classification:** the opened Guide classifies ‘ஆறு’ as உயிர்த்தொடர், while the textbook text mirror lists ‘ஆறு’ as an example of நெடில்தொடர். This is marked `REVIEW_REQUIRED_SOURCE_CONFLICT`; no generated Quiz item was created from that disputed table.
2. **2.5 நால்வகைக் குறுக்கங்கள்:** one original MCQ remains excluded due to a source conflict; it must not be guessed.
3. **2.6 திருக்குறள்:** the prose-to-Kural question is answered in `answers.md` but excluded from Quiz because a unique correct option was not established.
4. **ஓரெழுத்து ஒருமொழி:** an image-dependent grid/activity remains outside the Quiz; the Guide page title has a Term 2 label although the repository content is in Term 1, so it is only a secondary answer reference.
5. **1.3 பேச்சுமொழியும் எழுத்துமொழியும்:** true/false and media-classification answers are recorded in Step 1 but not relabelled as original four-option MCQs or force-converted into four-option items.

## Technical QA

- All 11 processed unit `quiz.json` files parsed successfully.
- Unit Quiz records: **59**.
- Term 1 Master Quiz: `tamil/term1/book_back_questions/quiz.json` — updated to 59 records.
- Master order matches the explicit unit JSON flattening order listed below.
- Duplicate Quiz IDs: **0**.
- Records without exactly four distinct options: **0**.
- Records with invalid `correctOptionIndex` (outside 0–3): **0**.
- Records missing `sourceUrl`: **0**.
- All 11 processed units have `questions.md`, `answers.md`, `quiz.md`, and `quiz.json`.
- Long / open-ended responses are placeholders only; no long model answers were added.

### Master Quiz order

1. 1.1 எங்கள் தமிழ்
2. 1.2 ஒன்றல்ல இரண்டல்ல
3. 1.3 பேச்சுமொழியும் எழுத்துமொழியும்
4. 1.4 ஆளுக்கு ஒரு வேலை
5. 1.5 குற்றியலுகரம், குற்றியலிகரம்
6. 2.1 காடு
7. 2.2 அப்படியே நிற்கட்டும் அந்த மரம்
8. 2.5 நால்வகைக் குறுக்கங்கள்
9. 2.6 திருக்குறள்
10. விடுதலைத் திருநாள்
11. ஓரெழுத்து ஒருமொழி, பகுபதம், பகாப்பதம்

## Remaining Term 1 units

The manifest contains further unit folders that still need the four book-back files:

- `03_tamilarin_kappalottiya_kadal`
- `04_vilangugal_ulagam`
- `01_naadu_arasu_naadu`
- `03_kappaloattiya_tamilar`
- `05_thirukkural_2`

These are still pending; do not mark Term 1 complete.

## Next batches

1. Finish the five remaining Term 1 units and rebuild / QA the Term 1 Master Quiz.
2. Process all Term 2 units; the current repository has some `questions.md` files, including files explicitly stating no separate book-back evaluation.
3. Process all Term 3 units; distinguish true evaluation questions from lesson-body text and lessons with no separate evaluation.
4. Create and verify the full Tamil Master Quiz at `tamil/book_back_questions/quiz.json` only after all three Term Masters are ready.
5. Keep the official edition status visible as unverified until the relevant official textbook PDF / imprint / contents / Book Back pages are compared.

**Conclusion:** Class 7 Tamil Term 1 is still PARTIAL. Eleven units now have Step 1–3 artifacts, 59 quiz records are synced, and five units remain. Structural Quiz QA passed; official current-edition and PDF image verification remain outstanding.
