The query taxonomy in `IC3_Reference` is directly usable by anyone building or evaluating a chatbot that fields fraud questions — but only if it's loadable by code. Right now it exists as .docx/.pdf, so anyone who wants to use it has to transcribe it by hand. This PR adds the same content as structured JSON.

- **`ic3_taxonomy.json`** — all 12 complaint categories, all 36 example queries, and the four citations, transcribed unchanged from `IC3_Reference.docx`. The file also carries the CC0 license (matching the repo), the ic3.gov pointer, and the scope note from the document header.
- **`README.md`** — a short new section explaining the file, with a Python loading example and a few suggested uses: seeding an evaluation set for testing how an AI handles fraud-victim questions, routing incoming questions to the right IC3 complaint category, or training intent classification.

No wording was changed anywhere. If you spot a transcription error, or would prefer a different structure (different field names, category slugs, splitting citations out), say so and I'll revise — or edit directly, it's your taxonomy.

🤖 Generated with [Claude Code](https://claude.com/claude-code)
