# Class 7 Tamil — Term 3 Completion & Full Master Quiz QA
**Audit date:** 2026-11-06  
**Repository:** [Eaglesiva/tn-class-07](https://github.com/Eaglesiva/tn-class-07)  
**Branch:** main

## Executive result

- **Term 3 scope:** COMPLETE — all 17 lesson titles across all three units have the four required lesson artifacts: `questions.md`, `answers.md`, `quiz.md`, and `quiz.json`.
- **Term 3 Master Quiz:** 65 records.
- **Consolidated Class 7 Tamil Master Quiz:** 184 records, combining Term 1 (69), Term 2 (50), and Term 3 (65).
- **JSON QA:** zero duplicate IDs; every quiz item has exactly four distinct options, a valid `correctOptionIndex` from 0 to 3, and a non-empty `sourceUrl`.
- **Scope limitation:** textbook edition certification is not complete. Current official 2026–27 imprint and page-image comparison have not been verified. Every Term 3 lesson retains `CURRENT_VALIDITY_UNVERIFIED`.

## Term 3 lesson inventory

| Unit | Lesson | Records in unit quiz |
|---|---|---:|
| 1.1 | விருந்தோம்பல் | 3 |
| 1.2 | வயலும் வாழ்வும் | 8 |
| 1.3 | திக்கெல்லாம் புகழுறும் திருநெல்வேலி | 7 |
| 1.4 | திருநெல்வேலிச் சீமையும் கவிகளும் | 0 |
| 1.5 | அணி இலக்கணம் | 0 |
| 2.1 | புதுமை விளக்கு | 7 |
| 2.2 | அறம் என்னும் கதிர் | 8 |
| 2.3 | ஒப்புரவு நெறி | 7 |
| 2.4 | உண்மை ஒளி | 0 |
| 2.5 | அணி இலக்கணம் | 0 |
| 2.6 | திருக்குறள் | 4 |
| 3.1 | மலைப்பொழிவு | 9 |
| 3.2 | தன்னை அறிதல் | 2 |
| 3.3 | கண்ணியமிகு தலைவர் | 6 |
| 3.4 | பயணம் | 0 |
| 3.5 | ஆகுபெயர் | 4 |
| 3.6 | திருக்குறள் | 0 |
| **Total** | **17 lessons** | **65** |

All 17 lesson directories passed the repository tree check for all four required files. Empty `quiz.json` files contain `[]` and are intentional where the textbook assessment did not contain an eligible four-option question.

## Lessons intentionally containing zero quiz records

- **1.4 திருநெல்வேலிச் சீமையும் கவிகளும்:** the assessment is a descriptive compilation prompt.
- **1.5 அணி இலக்கணம்:** two explanatory questions; no eligible MCQ or matching task.
- **2.4 உண்மை ஒளி:** one picture-story summary prompt; no MCQ.
- **2.5 அணி இலக்கணம்:** two descriptive questions; no MCQ.
- **3.4 பயணம்:** one story-summary prompt; no MCQ.
- **3.6 திருக்குறள்:** the source text contains selected Kural chapters but no separate Book Back assessment section. The existing placeholder inventory was clarified and no Kural-based questions were invented.

These were not forced into synthetic MCQs. The original descriptive prompts remain in `questions.md` and each has its own answer placeholders in `answers.md`, where applicable.

## Step implementation and review notes

1. Original textbook multiple-choice items are kept in the Step 2 section of each `quiz.md`.
2. Questions transformed from matching items, where used, are separately labeled Step 3. Generated distractors are not represented as original textbook choices.
3. Written, descriptive, image-dependent, and story-summary prompts are not converted into quiz records.
4. In Unit 2.3, an additional MCQ found in a third-party guide was not included because it was absent from the repository's source question inventory.
5. Some extracted matching sequences were out of reading order. The reconciled keys are explicitly documented in the relevant `answers.md` files; they are based on the poem/glossary meaning and are not presented as a verbatim official answer key.
6. Historical folder slugs and source PDFs were not moved or renamed. Where the lesson's canonical title did not match a legacy folder name, the question artifacts were placed in a separate lesson-specific directory and the mapping/source note is included in that lesson's `questions.md`.

## Source and edition caveat

The Term 3 question inventory was checked against a third-party text mirror of the 2025 Term 3 book:

[Class 7 Tamil Term 3 — 2025 text mirror](https://huggingface.co/datasets/Joemn/TamilNadu-State-board-books-2025-Tamil-and-english-versions/blob/main/7th-standard/Tamil/Class_7_Tamil_Tamil_Tamil_-_Term_3_-_2025_Edition.md)

Answer keys were cross-checked against the guide links cited inside the relevant lesson files. This is suitable for completing the current repository workflow, but **it does not certify that the repository PDFs are the official 2026–27 edition**. Official source verification and a visual page-by-page comparison remain pending. Do not mark the edition status as verified until that separate check is performed.

## Master files

- [Term 3 Master Quiz](../tamil/term3/book_back_questions/quiz.json)
- [Term 1 Master Quiz](../tamil/term1/book_back_questions/quiz.json)
- [Term 2 Master Quiz](../tamil/term2/book_back_questions/quiz.json)
- [Consolidated Class 7 Tamil Master Quiz](../tamil/book_back_questions/quiz.json)

## Consolidated Master QA

| Dataset | Record count | Duplicate IDs | Invalid records |
|---|---:|---:|---:|
| Term 1 | 69 | 0 | 0 |
| Term 2 | 50 | 0 | 0 |
| Term 3 | 65 | 0 | 0 |
| **Class 7 combined** | **184** | **0** | **0** |

Cross-term ID comparison found no collisions between Term 1, Term 2, and Term 3. The merged file preserves each term's existing records and their source metadata.

**Workflow status:** Term 3 complete; Term 1 + Term 2 + Term 3 consolidated into the Class 7 Tamil Master Quiz.  
**Edition status:** `CURRENT_VALIDITY_UNVERIFIED` pending official 2026–27 source/PDF verification.
