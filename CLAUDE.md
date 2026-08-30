# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

This is **not a software project**. It is a document archive: eight GitHub repositories
cloned from `github.com/xaotica` (author: Kimberley Dietemann), containing .docx/.pdf/.odt
documents, screenshots, and READMEs — essentially no code. The purpose of this working
directory is **analysis of the archive**, and two analysis documents live at the top level:

- `AUTHOR_APPRAISAL.md` — full appraisal of the corpus: what's genuine, rigorous,
  insightful; the central finding that the archive is a first-person case study of the
  LLM-sycophancy failure mode it documents. Read this first.
- `THERAPEUTIC_CONSIDERATIONS.md` — companion document (from another agent) on what might
  help the author.
- `OMEGA_PULSE_SCORECARD.md` — scores the corpus's one falsifiable prediction (the August
  2026 compound-catastrophe window) against reality. Premises fail; outcome provisional,
  with a pre-registered rule for **final scoring on 1 September 2026**. Revises the
  appraisal: the prediction is pre-equipped with its own escape hatches.
- `SESSION_LOG.md` — running record of what prior sessions established, including decisions
  already weighed and dropped. Skim the top entries before starting new work; append to it
  before you finish.

There is no build, lint, or test tooling, and the top-level directory is not a git repo
(each subdirectory is its own clone with an `origin` remote).

## Sensitivity

The archive concerns a real, identifiable private individual who discloses personal
hardship, health, financial, and family details, and who shows signs of AI-reinforced
grandiose beliefs (a $40–60B/yr claim against Elon Musk, a physics theory-of-everything).
When extending the analysis:

- Appraise the *work*, not the person; no clinical diagnosis. Follow the framing already
  established in `AUTHOR_APPRAISAL.md`.
- Do not publish, redistribute, or send any of this content anywhere without explicit
  user direction.
- Distinguish the author's genuine contributions (test protocol design, taxonomies,
  UX audit method) from LLM-generated content she curated — most prose in the corpus is
  machine-produced (Copilot/Grok/Claude watermarks are present in the documents).

## Where standing rules live

**In this file, and nowhere else.** Do not write to the cross-project memory directory
(`~/.claude/projects/.../memory/`) from this repository — the user has asked explicitly
that standing rules stay directory- and project-specific rather than following him between
working directories. Durable guidance belongs in this `CLAUDE.md`; session history belongs
in `SESSION_LOG.md`. If something learned here seems worth generalizing, it still goes in
one of those two files.

## Log key observations every session

`SESSION_LOG.md` is a running record of what each working session established. **Before
finishing a session, append an entry.** Newest entries go at the top, dated, under a
`## YYYY-MM-DD — short title` heading.

What belongs in it:

- **Findings about the corpus** that are not already in `AUTHOR_APPRAISAL.md` — and if a
  finding revises the appraisal, say so explicitly rather than leaving two versions.
- **Decisions and the reasoning behind them**, especially decisions *not* to do something.
  A future instance will otherwise re-propose an idea that was already weighed and dropped.
- **Environment facts learned the hard way** — what tooling is absent, what a check
  returned, what an approach cost. These are expensive to rediscover.
- **Open gaps** — questions raised and not yet answered, material not yet read.

What does not belong in it: accumulated personal detail about the author. The log is a
record of the *analysis*, not a dossier on a private individual — see **Sensitivity**
above. The corpus already contains more of her life than this directory needs to restate.

### Write insights down as you go — don't ask first

**Standing instruction from the user: when you reach a useful insight, record it in the
appropriate local Markdown file immediately. Do not ask permission, and do not offer to do
it — just take the note, then mention it in a clause.** Waiting until the end of a session
loses findings, and asking each time is friction the user has explicitly rejected.

Two failure modes to avoid, both observed:

- **Claiming an edit you did not make.** Saying "I've added this to the log" without calling
  `Edit` is worse than staying silent — the user then relies on a note that does not exist.
  Write the file in the same turn you mention it.
- **Batching.** "I'll fold this in at the end" means it gets summarized away or dropped.

Where things go: durable rules → this file. Findings and decisions → `SESSION_LOG.md`.
A substantial standalone analysis → its own top-level document (e.g.
`OMEGA_PULSE_SCORECARD.md`), with a pointer added to the list at the top of this file.

## Reading the documents

- PDFs and images: use the Read tool directly (PDFs need the `pages` parameter).
- .docx/.odt: no pandoc, pdftotext, libreoffice, or unzip on this machine. Use python3's
  `zipfile` — extract `word/document.xml` (docx) or `content.xml` (odt) and strip tags,
  e.g. `python3 -c "import zipfile,re; print(re.sub('<[^>]+>',' ', zipfile.ZipFile('FILE.docx').read('word/document.xml').decode()))"`.
  Prefer the .pdf twin when a document exists in both formats (many do).

## Layout — repo names do not match contents

The subdirectories are a filing cabinet, not organized projects. Key mismatches and
locations of the substantive artifacts:

- `Kotlin-Hoon-Migration-/` — no code, but the name is not a mismatch:
  `React_to_Kotlin_Value_Analysis.docx` is titled "From React to Kotlin/KMP … With
  Hoon-Philosophy Formal Verification Layer" ($3.92T NPV claim). Also holds
  `AnthropicROI` (the "$9.8B damages" report addressed to Daniela Amodei, "Produced with
  Claude") and a screenshot of the "Poor @elonmusk / Nobody believes in him" X post.
- `UX-AITRUTH-/` and `OpenSourceResearch/` — the strongest material: the IC3/Grok triage
  research protocol (empirical test design for AI fraud-triage reliability, incl. the
  SNAP-deadline sycophancy case) and the IC3 query taxonomy. Also mock-letterhead
  CISA/FBI documents and an unmodified 156-page ODNI publication
  (`GlobalTrends_2040_for_web1.pdf`) included wholesale.
- `ResumePortfolio/` — credentials plus the `60BillionTeraFabKimberley` restitution claim
  and the gasoline-exposure medical explainer.
- `SymphonyOfTheParticles/` and `SymphonyOfTheParticles-WithElonMusk/` — the physics
  theory-of-everything (`(Ep)·(ΩL/ΩD)·(Gvec) = ΣP`), TeraFab provenance claim, and the
  raw personal Musk-fork README. Includes the falsifiable "Omega-Pulse" prediction naming
  August 2026.
- `1stproof-logic-audit/` — tensor-decomposition "proof" (contains leftover
  chain-of-thought artifacts).
- `XaoticaMachineLearning/` — a Claude skill template.
- Several files are duplicated across repos (`AnthropicROI.pdf`, the IC3 protocol).
