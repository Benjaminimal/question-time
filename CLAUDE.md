# Question Time

## What it is

A mobile first, frontend only, web app that can be used to get interesting conversations started through simple questions.
It's multilingual and currently supports German and English.

## Guidelines

- Keep all the application logic, structure, and styling in one single `index.html` file.
- Questions are read from `questions.json` which uses the following format for translations.

```json
[
  {
    "de": "Ist das eine Frage?",
    "en": "Is this a question?"
  }
]
```

- New questions must be appended to `questions.raw`.
- Never edit `questions.json` unless explicitly instructed.
