# Book Back Questions & Quiz Workflow — Common Rules (Classes 1–12)

> **நோக்கம்:** Class 1–12, எல்லா பாடங்கள், மொழிகள், Medium-கள் மற்றும் Term / Annual books-க்கும் ஒரே Step 1 → Step 2 → Step 3 செயல்வரிசை.

## தொடங்குவதற்கு முன் — Edition Gate

1. Class + Subject + Medium + Term / Annual + Volume-ஐ அடையாளம் காண்க.
2. `docs/BOOK_EDITION_VERIFICATION_RULES_TA.md`-ஐப் பின்பற்றி official listing, PDF, imprint, TOC மற்றும் Book Back பக்கங்களைச் சரிபார்க்கவும்.
3. Edition உறுதியாகாவிட்டால் இறுதி Answers / Quiz வெளியிட வேண்டாம். `CURRENT_VALIDITY_UNVERIFIED` அல்லது பொருத்தமான status-ஐப் பதிவு செய்து blocker-ஐக் குறிப்பிடவும்.
4. Edition Gate முடிந்த பிறகே Step 1 தொடங்க வேண்டும்.

---

## STEP 1 — `answers.md`: முழுக் கேள்விப் பட்டியல் + விடை ஆதாரம்

1. Unit-இன் `questions.md` முழுவதையும் படிக்கவும்.
2. அதே Book Back / Evaluation பகுதிகளை பாடநூல் PDF-இல் பார்த்து wording, section, numbering, order ஆகியவற்றை ஒப்பிடவும்.
3. `answers.md`-ல் கேள்விகளை அதே வரிசையில் முழுமையாகப் பதிவு செய்யவும்; கேள்வியைச் சுருக்கவோ விடவோ கூடாது.
4. One-mark / One-word / Objective வினாக்களுக்கு சரியான விடை, சுருக்க விளக்கம், திறந்து சரிபார்த்த Direct Source URL, தேவையான PDF page மற்றும் verification status சேர்க்கவும்.
5. விடை உறுதியாகாவிட்டால் ஊகிக்க வேண்டாம்; `ANSWER_NOT_FOUND` அல்லது `REVIEW_REQUIRED` எனக் குறிக்கவும்.
6. குறு / சிறு / நெடு / திறந்தநிலை வினாக்களுக்கு முழு விடை எழுத வேண்டாம். கீழே உள்ள placeholders மற்றும் source link மட்டும் வைக்கவும்:
   - `விடைக்குறிப்பு`
   - `சாதாரண விடை`
   - `விரிவான விடை`
   - `Source: [Unit question source](./questions.md)`
7. படம் / வரைபடம் / அட்டவணை சார்ந்தவற்றை source page பார்த்த பிறகே வகைப்படுத்தவும்.

**Step 1 QA:** எல்லா கேள்விகளும் அதே order-ல் உள்ளனவா? Objective விடைகளுக்கு answer + explanation + direct source + status உள்ளதா? பெரிய வினாக்களுக்கு placeholders மட்டும் உள்ளனவா? unresolved / image-dependent பதிவுகள் குறிக்கப்பட்டுள்ளனவா?

**Step 1 முடிந்த பிறகே Step 2.**

---

## STEP 2 — `quiz.md`: அசல் பாடநூல் Objective / MCQ

1. Step 1-ல் சரிபார்க்கப்பட்ட கேள்விகளில் பாடநூலிலேயே நான்கு options உடன் உள்ள MCQ-களை மட்டும் தேர்ந்தெடுக்கவும்.
2. கேள்வி wording, நான்கு options, option order, answer key ஆகியவை அசல் புத்தகத்துடன் பொருந்த வேண்டும்.
3. பாடநூலில் நான்கு options இல்லாததை Original MCQ என்று காட்டக்கூடாது.
4. ஒவ்வொரு வினாவுக்கும் நான்கு options, சரியான விடை, சுருக்க விளக்கம் மற்றும் source link சேர்க்கவும்.
5. உருவாக்கிய distractors-ஐ original textbook options என்று காட்டக்கூடாது.

**Step 2 QA:** தகுதியான அனைத்து original MCQ-களும் உள்ளனவா? நான்கு options / order / answer key சரியா? Step 3-ல் மாற்றப்படும் வினாக்களிலிருந்து தெளிவாக வேறுபட்டுள்ளனவா?

**Step 2 முடிந்த பிறகே Step 3.**

---

## STEP 3 — `quiz.md` + `quiz.json`: மாற்றத்தகுதியான One-mark வினாக்கள்

1. Step 1-ல் உள்ள மற்ற one-mark / one-word / short objective வினாக்களில் ஒரே ஒரு விடையை ஆதாரத்துடன் உறுதிப்படுத்தக்கூடியவற்றை மட்டும் நான்கு-option MCQ-ஆக மாற்றவும்.
2. Fill-in-the-blank, one-word, matching, grammar, name, date, number போன்றவை தகுதியானால் சேர்க்கலாம்.
3. ஒவ்வொரு item-க்கும் நான்கு distinct options; ஒரு correct answer; பொருத்தமான தவறான distractors; concise explanation; direct source இருக்க வேண்டும்.
4. குறுவினா / சிறுவினா / நெடுவினா / கட்டுரை / திறந்தநிலை / படைப்பாற்றல் / unresolved / image-dependent வினாக்களை Quiz-ஆக மாற்ற வேண்டாம்.
5. Generated options-ஐ generated distractors என்று தெளிவாக அறியக்கூடிய வகையில் பராமரிக்கவும்.
6. `quiz.md` மற்றும் `quiz.json` ஒரே பதிவுகள், ஒரே order, ஒரே options, answer, explanation, source metadata உடன் இருக்க வேண்டும்.
7. Unit JSON-களை repository-யின் term / subject-level Master Quiz-இல் sync செய்யவும்.

**Step 3 QA:** எல்லா தகுதியான one-mark வினாக்களும் பரிசீலிக்கப்பட்டனவா? JSON parse ஆகிறதா? Duplicate IDs இல்லையா? ஒவ்வொரு item-க்கும் நான்கு unique options, correct index 0–3, source உள்ளதா? Markdown / JSON / Master sync ஆகிறதா?

---

## Unit Completion Gate

ஒவ்வொரு Unit முடிவிலும் கீழ்கண்ட வடிவில் அறிக்கை எழுதவும்:

- STEP 1: DONE / BLOCKED + கேள்வி எண்ணிக்கை
- STEP 2: DONE / BLOCKED + Original MCQ எண்ணிக்கை
- STEP 3: DONE / BLOCKED + Transformed MCQ எண்ணிக்கை
- Excluded: long-answer / open-ended / image-dependent / unresolved எண்ணிக்கை மற்றும் காரணம்
- QA: question order / markdown-json sync / JSON validation / master sync
- Edition Gate: status + evidence
- Remaining: blocker / மீதமுள்ள பணி

மூன்று Steps-ல் ஏதேனும் ஒன்று BLOCKED என்றால் Unit COMPLETE அல்ல. எல்லா Units-க்கும் QA முடிந்த பிறகே Subject COMPLETE என்று அறிவிக்க வேண்டும்.

## பொதுவான விதிகள்

- பெரிய வினாக்களுக்கு முழு விடைகள் எழுதுவது இந்த workflow-இன் scope அல்ல.
- எந்த விடையையும் ஆதாரமின்றி `VERIFIED` என்று குறிக்கக்கூடாது.
- கேள்வி, PDF அல்லது ஏற்கெனவே உள்ள கோப்புகளை ஆதாரமின்றி delete / rename / move / overwrite செய்யக்கூடாது.
- Class 1–12 அனைத்திற்கும் Step 1–3 ஒரே மாதிரி; Term, Medium, புத்தக வடிவமைப்பு மற்றும் lesson எண்ணிக்கை மட்டும் மாறலாம்.
