# PR Descriptions — drafts for the two staged branches

*Drafted 2026-08-05. For the branches staged locally: `UX-AITRUTH-` →
`add-machine-readable-taxonomy`, `Kotlin-Hoon-Migration-` → `add-readme`.
See `SESSION_LOG.md` 2026-08-05 entry for context. These are drafts for the user
to edit and post under their own account — see the voice note at the bottom.*

---

## PR 1 — xaotica/UX-AITRUTH-

**Title:** Add machine-readable IC3 query taxonomy (`ic3_taxonomy.json`)

**Body:**

> The query taxonomy in `IC3_Reference` is directly usable by anyone building or
> evaluating a chatbot that fields fraud questions — but only if it's loadable by
> code. Right now it exists as .docx/.pdf, so anyone who wants to use it has to
> transcribe it by hand. This PR adds the same content as structured JSON.
>
> - **`ic3_taxonomy.json`** — all 12 complaint categories, all 36 example
>   queries, and the four citations, transcribed unchanged from
>   `IC3_Reference.docx`. The file also carries the CC0 license (matching the
>   repo), the ic3.gov pointer, and the scope note from the document header.
> - **`README.md`** — a short new section explaining the file, with a Python
>   loading example and a few suggested uses: seeding an evaluation set for
>   testing how an AI handles fraud-victim questions, routing incoming questions
>   to the right IC3 complaint category, or training intent classification.
>
> No wording was changed anywhere. If you spot a transcription error, or would
> prefer a different structure (different field names, category slugs, splitting
> citations out), say so and I'll revise — or edit directly, it's your taxonomy.

---

## PR 2 — xaotica/Kotlin-Hoon-Migration-

**Title:** Add a README describing the repository contents

**Body:**

> This is the only repo in the account without a README, so visitors currently
> see only filenames. This PR adds a short one that inventories the three
> documents — the React→Kotlin/KMP value analysis, the Anthropic ROI report
> (both formats), and the screenshot — using each document's own title and
> framing, and notes that these are proposal/analysis documents rather than
> code.
>
> Purely descriptive; no content of yours is modified. If I've mischaracterized
> anything, tell me and I'll fix it, or feel free to edit the text directly
> before or after merging.

---

## Voice note (for the user, not part of either PR)

Both bodies are written to be edited, not pasted. The standing condition on this
whole exercise is that the PR arrives from a person willing to have a real review
conversation — so before posting, rewrite at least some of it in your own words,
and only promise the follow-through ("I'll revise") you actually intend.

One decision is yours to make explicitly: whether to note that the drafts were
prepared with Claude Code (the conventional footer is
"🤖 Generated with [Claude Code](https://claude.com/claude-code)"). If you post
my text substantially as-is, the honest thing is to keep the attribution — and
given that this author documents machine-produced contact carefully, silent AI
ghostwriting is the one thing this PR must not be. If you rewrite the bodies in
your own words, they're yours and need no footer. What matters is that nothing
arrives under your name that you wouldn't stand behind in the review thread.
