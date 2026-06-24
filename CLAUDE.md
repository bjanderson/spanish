# CLAUDE.md

## About

This project is an interactive website for learning and practicing Spanish. All project requirements are specified in PRD.md

## English Language

- All English language in this project should focus on American English. Do not include examples of European English.

## Spanish Language

- All Spanish language in this project should focus on Latin American Spanish. Do not include examples of European Spanish.
- Follow typical Spanish norms with subject pronouns. For example, do not include subject pronouns (yo, tú, etc...) before verbs if the verb conjugation implies them.
- All generated sentences should use the following contexts:
  - Bible (non-denominational Christian)
  - Bible study (non-denominational Christian)
  - Bible stories (non-denominational Christian)
  - church (non-denominational Christian)
  - travel
  - restaurant
  - food
  - home
  - family
  - friends
  - pets
  - school and education
  - health
  - work
  - music

## Anki Text File Format

```
#separator:tab
#html:true
#notetype column:1
#deck column:2
#front column:3
#back column:4
#tags column:5
Basic	Spanish Practice	all, every	todo	100_Most_Common_Words_-_Adjectives
```

- English text goes in front (column:3)
- Spanish text goes in back (column:4)
- Name the deck (column:2) with the same name as the file it's being saved in

## Token efficiency

- **Never read `node_modules/`** — generated/vendor content, not editable source.
- **Prefer `grep` over sequential reads** when locating a specific heading, tag, wikilink, or passage across content files.
- **`attachments/` are binary.** Don't attempt to read PDFs, images, or SVGs unless the task explicitly requires it.
- Do not generate a summary after the action is complete.
- Do not re-read files you just wrote or edited — trust that writes succeeded.
- Do not summarize what you just did at the end of a response.
- Do not add commentary between tool calls — just run the tools.
- Batch independent tool calls in parallel (searches, reads) rather than sequentially.
- Warn me when my token usage reaches 90%.
