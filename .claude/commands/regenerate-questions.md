---
description: Regenerate questions.json from questions.raw with English and German translations
---

Read `questions.raw` where each line contains a question in any language, generate both English and German translations for each question, and write the results to `questions.json` in the following format:

```json
[
  {
    "de": "German translation",
    "en": "English translation"
  }
]
```

Important workflow:
1. Check if questions.raw or questions.json have uncommitted changes and notify the user
2. As a first step, wipe the existing questions.json
3. Read all questions from questions.raw (each line is one question)
4. Generate accurate English and German translations for each question
5. Write to questions.json following the exact format with "de" and "en" keys
6. Commit when done with message "chore: regenerate questions"

Notes:
- Questions in questions.raw can be in any language
- Maintain the order of questions
- Ensure natural and accurate translations
- Do nothing but tell the user when either questions.raw or questions.json have uncommitted changes
