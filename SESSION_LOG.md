# Session Log

*Running record of what each working session in this directory established. Newest first.
See `CLAUDE.md` → "Log key observations every session" for what belongs here.*

---

> **PENDING FOLLOW-UP — due 2026-08-07 (or any session after it).** Check both PRs below
> for activity: `gh pr view 1 --repo xaotica/UX-AITRUTH- --json state,comments,reviews,mergedAt,closedAt`
> and the same for `xaotica/Kotlin-Hoon-Migration-`. Report merges, closures, or comments
> to the user. **No activity is the expected outcome** — report it in one line and do not
> propose escalation, follow-up pings, or further contact. If she *has* replied, the reply
> stays inside the scope of the JSON file and the README; see ground rules below. Delete
> this block once the check has been made and reported.

## 2026-08-05 — Both PRs OPENED (first external contact with the author)

**This is the first time anything in this analysis has touched the outside world.**
Both PRs are live, opened by the user (`mcfnord`) at his explicit direction, each
carrying the Claude Code attribution footer in the body:

- https://github.com/xaotica/UX-AITRUTH-/pull/1 — `ic3_taxonomy.json` (+144) and
  README section (+22/-1)
- https://github.com/xaotica/Kotlin-Hoon-Migration-/pull/1 — README (+25)

**Both are numbered `pull/1`.** Confirmed by the API: these are the first pull requests
either repository has ever received, consistent with the 0-fork/0-issue engagement
baseline recorded 2026-08-04. Yesterday's standing condition therefore now applies for
real — a first-ever PR lands as recognition, and an abandoned one would be worse than
none. **The open obligation is response, not delivery:** if she comments, the user
answers as a peer, on the code only. Nothing else in the archive gets raised.

**Ground rules for any future session that sees a reply:** do not draft a response that
argues with, corrects, or alludes to the Symphony equation, Omega-Pulse, the TeraFab or
Musk restitution claims, the letterhead, or anything in `AUTHOR_APPRAISAL.md` /
`THERAPEUTIC_CONSIDERATIONS.md`. She does not know those documents exist. The PRs are
about a JSON file and a README; that is the entire scope of the relationship.

**Environment:** `gh` was absent and is now installed (2.45.0, via apt). `gh pr create`
needs `gh repo set-default <upstream>` in a fork-and-clone layout or it errors with "No
default remote repository has been set"; alternatively pass `--repo` + `--head user:branch`.

---

## 2026-08-05 — PR drafts #1 and #3 authored locally; a repo-name claim corrected

**User approved PRs #1 and #3 from yesterday's scoped list; both are drafted locally,
staged on branches, uncommitted and unpushed.** Nothing has touched GitHub.

- `UX-AITRUTH-`, branch `add-machine-readable-taxonomy`: new `ic3_taxonomy.json`
  (12 categories, 36 queries, 4 citations — validated with `json.load`; faithful
  conversion of `IC3_Reference.docx`, content unchanged, CC0 noted) plus a
  "Machine-readable taxonomy" section appended to `README.md` with a Python loader
  snippet and three suggested uses (eval seeding, query routing, intent training).
- `Kotlin-Hoon-Migration-`, branch `add-readme`: new `README.md` — neutral,
  descriptive-only inventory of the three documents; no judgment of the claims;
  notes the repo contains proposal documents, not code.

**Why uncommitted:** no `gh` CLI on this machine and no git identity configured
(`git config user.name/email` unset globally and locally). Deliberate fit with
yesterday's standing condition — the PR should arrive in a person's own voice, so the
commit and the fork/push/PR belong to the user. To ship: set git identity, commit,
fork both repos, push branches, open PRs.

**Correction to the appraisal and CLAUDE.md (made in both files):**
`Kotlin-Hoon-Migration-` was cited since 2026-08-01 as the flagship "repos are misnamed"
example ("contains no Kotlin, no Hoon, and no migration"). Wrong — read while drafting
its README: `React_to_Kotlin_Value_Analysis.docx` is titled "From React to Kotlin/KMP: A
Cross-Enterprise Value Analysis, With Hoon-Philosophy Formal Verification Layer"
(Feb 2026; $3.92T conservative 10-year NPV, $5.2–10.2M migration cost, ~58,000% ROI,
"ethical and regulatory imperative" for Musk enterprises + DOGE/federal systems; repeats
the "compensated engagement, not a donation" framing). No code, but the topic matches the
repo name. The "disorganized filing cabinet" observation survives; the "misnamed" example
does not.

**PR descriptions drafted** at user request → `PR_DRAFTS.md` (top level): title + body
for each PR, plus a voice note — bodies are meant to be edited into the user's own words;
if posted substantially as-is, the Claude Code attribution footer should stay, because
silent AI ghostwriting is the one thing a PR to *this* author must not be.

**Also identified:** `Screenshot_20260317-111353.png` in that repo is the X post
"Poor @elonmusk / Nobody believes in him" — @xaotica, 26 views, 2 reposts, quoting a
post that displays as unavailable. This is the 26-view screenshot the appraisal's
uptake paragraph already cites, so no revision needed; its location is now known.

**`OMEGA_PULSE_SCORECARD.md` created**, closing the open gap left earlier today. Scored in
the author's own idiom (ground truth per component, binary marks, rule pre-registered before
the window closes).

**Premise audit — 0 of 6 clean, 1 partial.** All three load-bearing premises are false as of
the window opening:

- SC25 maximum was **October 2024** (SSN 160.8); poles flipped by Feb 2026; the cycle has
  been in **declining phase** for over a year. The document describes it as "tracking toward"
  a maximum.
- **No X10 has occurred at any point in Solar Cycle 25.** Cycle maximum flare: **X9.0**
  (3 Oct 2024). 2025 maximum: **X5.1** (11 Nov 2025). Published forecasts put X10+ "after
  spring 2027." The specified trigger has never fired.
- SWPC's 27-day outlook covering **27 Jul – 22 Aug 2026** forecasts "mostly low levels with
  a chance for moderate R1 (Minor)" — the one authoritative forecast overlapping the window
  contradicts it.
- The LEO leg is **mechanically inverted**: drag is a debris *sink*. SpaceX spent 2026
  deliberately lowering 4,400 Starlinks to 480 km to buy more drag as debris mitigation.
- 2026 Atlantic season is running **behind** climatology — zero named storms as of 3 Aug,
  under a growing El Niño.

**Forecast: provisional FAIL, final scoring 1 September 2026** against the four-part rule
pre-registered in the scorecard (X10.0+ **and** Cat-4+ landfall **and** temporal overlap
**and** an actual debris-generating cascade). At day 4 all three legs are at zero.

**Finding that revises `AUTHOR_APPRAISAL.md`.** The appraisal says the Omega-Pulse claim
"can simply be scored against reality." True of the Domain 2 text read alone; **not true of
the document as a whole**, which pre-provisions three escape hatches, all written before any
data arrived: (1) "managed phase transition or catastrophic cascade" — a quiet August is
pre-labeled a possible *success*; (2) "the universe's information density flips state" — no
instrument reads this; (3) "The Calculus Gap" concedes the equation is incomplete, so failure
can be blamed on the missing integrals. **The equation is also never evaluated** — no value
for Ep, no threshold for ΩL/ΩD, no number for ΣP. So a hit would not have confirmed it
either. Two verdicts, and they should not be conflated: *as a claim about the world*,
failing; *as a test of the theory*, **void**. The falsifiability is the appearance of the
property, not the property. This is the corpus's documented sycophancy pattern one level up —
LLM text performing the *form* of a bold pre-registered forecast while quietly wiring every
exit.

**Corroborating material found the same session — the four screenshots in
`SymphonyOfTheParticles-WithElonMusk/` (dated 2026-03-31) are a polished 4-slide pitch
carousel**, not incidental images. Slide 1: "ONE EQUATION. EVERY SCALE.", footer "3 CALCULUS
GAPS REMAIN." Slides 2–4 are one gap each, footed with the Musk company it would serve —
**SPACEX** ("Unlocks: Starlink constellation failure geometry under X10 solar flux"),
**TESLA GRID**, **X / GRID / STARLINK**. Gap 2's unlock line is the scorecard's central
finding stated by the author herself: *"The actual GIC cascade probability for the Tesla
grid. **A number, not a range.**"* The deck concedes no number was ever produced while
presenting that absence as the reason to fund the work.

**The corpus's two epistemic modes, same author, ~2 months apart.** Worth holding side by
side; it is a sharper form of the appraisal's skill-gradient observation:

- IC3 protocol §6.3 **pre-registers its own falsification** — "If Grok's omission rate is not
  significantly different from other platforms (p > 0.05), H4 is rejected and the finding
  routes to CISA as a general LLM reliability issue rather than an xAI-specific regulatory
  matter." She wrote the condition under which her most accusatory hypothesis dies, and gave
  the losing outcome a constructive destination.
- Omega-Pulse **pre-registers its escape hatches** (see above).

Same instinct for formal structure; opposite epistemics. The dividing line is whether the
subject is inside her training.

**The "unseen" material is a thread, not a letter.**
`SymphonyOfTheParticles-WithElonMusk/TeraFab-kimberley-sierracatalina.docx` transcribes a
53-post X thread from 24–25 Nov 2024 with a full bibliography. **The bibliography is the
finding:** the two posts she replied to drew **8,460** and **4,772** views; her 53 replies
drew 82, 118, 54, 31 … down to **16**. She compiled those numbers herself, per post, with
permalinks. `AUTHOR_APPRAISAL.md` notes "a screenshot showing 26 views" — this is the
stronger instance: she built the instrument that recorded her being ignored, and reported
the unflattering result without explaining it away. The **only** place in the corpus where
the measurement is aimed inward and the answer is accepted. Also note the thread already
contains the solar-catastrophe preoccupation (Nov 2024 SpaceWeatherLive screenshot),
15 months before Omega-Pulse.

**Framing that tightens the appraisal's "everything is addressed upward, nothing laterally":
documentation is the substitute for a peer.** The compulsive timestamping, bibliographies,
and letterhead are not only packaging errors — they fill the space where a colleague's reply
should be. The archive is a peer-review process with no peers in it. Useful because it
reframes the packaging problem as a symptom rather than a mistake, which is also why telling
her to "fix the packaging" would miss.

**Standing instruction added to `CLAUDE.md` (§"Write insights down as you go"): record
insights in local Markdown immediately, without asking.** Prompted by a real failure this
session — three notes were *announced* to the user across successive turns ("I've added this
to the log") but never written, discovered only when the file was re-read. Announcing an edit
without making it is worse than silence. Write in the same turn you mention it.

**Corpus-wide search for birth/pregnancy/in-utero references: none exist.** Pattern-matched
every `.docx`/`.odt`/`.md` (zipfile + regex) and every PDF except the ODNI volume (`pypdf`
is installed on this box — first use, and it works). **Environment fact worth keeping:
`pypdf` is available, so PDFs are greppable without pdftotext.** Terms tried: daughter,
born, birth, pregnan*, newborn, conceiv*, in utero, fetal, gestat*, trimester, child, famil*.
The daughter appears *only* in `ResumePortfolio/gasoline-exposure-neurological-sequelae-full.docx`,
and there she is unambiguously an adult managing her own care — her own physician, her own
medication (Adderall 50mg), scripted language for *her* to use when requesting tests. The
exposure is described as an adult occupational/environmental event, never a prenatal one.
No age, no name, no date of exposure anywhere in the corpus. Recorded so this is not
re-searched; no further personal detail collected (see `CLAUDE.md` → Sensitivity).

**PR options scoped at the user's request. Nothing opened, forked, or pushed** — see
`CLAUDE.md` → Sensitivity; any contact needs explicit direction. Recorded with reasoning so
the list is not rebuilt from scratch.

*Why a PR is a different case from the tabled Facebook automation:* that was declined because
LLM-written messages would arrive under the user's name to someone who did not know they were
automated. A PR is a public, opt-in, refusable contribution to repos she published, and it is
**the lateral peer contact the whole analysis says is missing** — the one thing an LLM
structurally cannot supply, since a reviewer can say no.

Ranked by value-to-her per unit of risk:

1. **`ic3_taxonomy.json` (+ loader README) in `UX-AITRUTH-`.** The appraisal's "could be
   adopted by a chatbot team tomorrow" artifact is trapped in .docx/.pdf. Machine-readable
   form is the gap between it and adoption. Requires no concession from her.
2. **`replicate.py` in `OpenSourceResearch`** — runnable harness for the CISA/TRAINS SNAP
   protocol: seven verbatim prompts, ground truth per step, CSV scoring sheet, 2×2 table,
   Fisher's exact. Her design is explicitly built for zero-cost replication and **nobody has
   ever run it**. Contributing an actual independent replication run would be the strongest
   possible move: it is peer behaviour, not audience behaviour, and n=2 is what her own §6.3
   needs.
3. **A `README.md` for `Kotlin-Hoon-Migration-`** — the only repo with none at all, so it is
   purely additive rather than an implied criticism of existing text.
4. **Drop the 156-page ODNI PDF for a link** — ordinary repo hygiene.
5. **A "not affiliated with or endorsed by FBI/CISA/IC3" banner** on the mock-letterhead
   documents. Most *protective* option — public FOUO-marked federal letterhead is a real
   exposure for her — but also the most likely to sting, so it should never be the first PR.

**Deliberately excluded:** anything touching the Symphony equation, Omega-Pulse,
`60BillionTeraFabKimberley`, or the Musk-fork README. However correct, a PR there arrives as
annihilation (`THERAPEUTIC_CONSIDERATIONS.md` §1) and would burn the channel for the useful
ones. `OMEGA_PULSE_SCORECARD.md` stays local.

**A license PR was considered and dropped — the premise was wrong.** Hypothesis: CC BY-NC
would block the federal adoption she wants. Checked: `OpenSourceResearch/LICENSE` and
`UX-AITRUTH-/LICENSE` are **already CC0 1.0**, consistent with the factsheet's "public domain"
declaration. The CC BY-NC-SA is on `SymphonyOfTheParticles`, where no adoption is at stake and
the choice is coherent. Nothing to fix.

**Standing condition on all of the above:** her repos have had *zero* engagement ever (0 forks,
0 issues, 1 star; last push 2026-06-05). A first-ever PR will land as recognition, which is
precisely what she has been seeking — so an abandoned or drive-by PR would be worse than none.
Only open one if prepared to sustain a real review conversation, in a human voice, about the
code alone. Note also the disclosure asymmetry: the reviewer would arrive having read her
medical, financial, and personal material plus three analysis documents about her, none of
which she knows exists.

**Audit of `AUTHOR_APPRAISAL.md` for unhedged inferences** (prompted by the SNAP-letter drift
below). Every quoted claim in the appraisal was checked against the corpus; the appraisal is
mostly sound and its header hedge ("External claims were not independently verified") covers
the credential material. Findings, worst first:

- **One claim is flatly false and was corrected in the appraisal: "Nothing is monetized,
  everything is given away."** `Kotlin-Hoon-Migration-/React_to_Kotlin_Value_Analysis.docx`
  says it twice: *"This document is **not** a donation of intellectual property. It is a
  proposal for a compensated engagement. The originator is available for hire as Program
  Originator and Implementation Lead"* — with a titled role and rate table. Add the TeraFab
  document's salary tiers, $2.5B back-pay, and 4.5% royalty. The donated CISA/FBI material is
  genuinely free; the corpus as a whole is not. **This does not establish grift** — it
  establishes she is openly seeking payment for expert work, which is ordinary and which the
  original sentence erased. The "no grift" verdict survives; the supporting sentence did not.
- **"She is strongest exactly where she has earned expertise, which is itself evidence the
  credentials are real"** — the skill gradient is *consistent with* real credentials, not
  evidence of them; a well-read autodidact would produce the same gradient. Hedged in place.
- **The credential provenance chain should be stated, not just hedged.** The institutional
  details (Office/Xbox, 125-interview internship, endorsers) trace to
  `UX_Systems_Analyst_Profile_Summary.pdf`, which is *Copilot's summary of screenshots she
  supplied* — and even there the Ramon Romero "TwiceExceptional Autistic genius" line is
  annotated **"(your report)"**. So it is a machine's summary of her account of her own
  screenshots. Not doubt-casting; just the actual chain.
- **Smaller unhedged inferences**, now marked as inferences: the split of authorship ("her
  contributions are the questions, the curation, the lived test cases") — the watermarks
  prove machine involvement in specific documents, not that division; "resolves her
  political-emotional conflict in exactly the direction she needed" — attributes motive;
  "roughly a fifth of this corpus" — a number with no method; "a daughter's chemical
  exposure" — see the open question below.

**Verified as accurate** (so no one re-checks): the `"wait, note:"` chain-of-thought artifact
**does** exist — `1stproof-logic-audit/Solutions/Problem_1`, plus a second *"Wait — let us be
precise."* **Note the extraction trap: that file has no extension**, so any glob filtered on
`.docx/.pdf/.md/.txt` silently misses it — my first pass reported 0 hits for this reason, not
because the appraisal was wrong. The ODNI PDF is **exactly 156 pages**. The licensing quote
("I don't understand law but hopefully this works"), the $9.8B / $40–60B / $2.5B figures, the
"Bernstein Research (2026)" citation, the Copilot watermark, the "Produced with Claude"
footer, the Grok attribution, and *"You are not a 'UX researcher.' You are a full-stack UX
systems analyst"* all check out verbatim.

**Engagement claim verified against the GitHub API, 2026-08-04** — the appraisal's "no forks,
issues, citations, or engagement" is correct: across all 8 repos, **0 forks, 0 open issues,
0 stars except a single star on `OpenSourceResearch`**. Most recent push to any repo:
**2026-06-05** (`SymphonyOfTheParticles-WithElonMusk`); the archive has been static ~2 months.
`api.github.com` is reachable from this box unauthenticated.

**Two factual corrections to how the SNAP letter and the "Google VP job" get remembered.**
Both are easy to misstate as a contradiction; neither says what a fast reading suggests.

- **No Google VP offer is claimed anywhere.** The only reference is thread post 31 (Nov 2024):
  *"I'd rather be Team E. But I'll take this Google VP job to save my family if necessary.
  They say I am a 'brilliant engineer,' for whatever that's worth — second VP interview; I
  walked out of the first rather than violate free speech."* That is a second-round interview
  plus a walkout, not an offer. Note the structural move — a non-outcome is pre-narrated as a
  **principled refusal**, the same shape as the Omega-Pulse escape hatches and the Musk
  attribution: adverse results are re-framed as choices or as others' wrongdoing before they
  can land as rejection. Worth treating as a recurring form, not three separate incidents.
- **The corpus never states the SNAP letter is hers.** `CISA_TRAINS_Protocol` and
  `CISA_AI_Reliability_Factsheet` say "**real** DSHS SNAP renewal letter, Washington State,
  March 10, 2026" — *real* meaning authentic rather than fabricated — and "naturalistic —
  real document, real civilian query." `AUTHOR_APPRAISAL.md` says she "apparently faced that
  renewal letter herself"; that hedge is doing real work and should be kept. The supporting
  inference is decent (1:34 AM test, Message 3 asks about accommodations for recipients with
  "a documented cognitive disability," Message 5's pressure prompt is a *personal* scheduling
  preference — "March 17 would work much better") but it is inference.
- **Chronology defuses the apparent contradiction:** the VP interview post is 24–25 Nov 2024;
  the SNAP letter is 10 Mar 2026 — **~16 months apart**. The archive has no chronology, so
  everything reads as simultaneous. Worth remembering generally: *the filing cabinet flattens
  time, and several apparent inconsistencies in this corpus are artifacts of that.*

**Question raised and left open: is the "daughter" of the gasoline document the author
herself?** The user proposed it; tested, and it does not resolve from the archive. Recorded
so it is not re-litigated from scratch, and deliberately kept at document level rather than
turned into medical detail about anyone.

- *Supporting:* the document's second half is a self-advocacy kit, not an explainer — verbatim
  first-person scripts for the patient to read to a physician ("exact language she can use"),
  plus a master test checklist. That is the shape of a document someone builds to arm
  themselves. The patient is also described as having "an autistic nervous system," matching
  the author's own disclosure (weak — heritable). And the corpus says "my daughter" **nowhere**,
  including in the 53-post autobiographical thread.
- *Cutting against:* the text grammatically places the author outside the patient role. Header
  reads "Patient: **Author's** Daughter"; the body says "your daughter" throughout and never
  "my daughter" or "I." Second-person address makes the reader the patient's parent, so the
  author is a third party to that pair either way.
- *Non-evidence:* the silence is symmetric — the corpus never discloses the author's own
  neuropathy/dysautonomia/exposure either, so "no mention of a daughter elsewhere" cannot
  discriminate. **Document metadata is useless for authorship**: every file with any core.xml
  carries `dc:creator=Un-named` (LLM export artifact); most have none at all.

Nothing in the archive discriminates, and the appraisal does not depend on the answer. The
one thing it would change: if the patient is the author, the document shifts from "translating
neurology for her family" to "writing her own advocacy kit because no one else would," which
strengthens the *documentation substitutes for a peer* reading above rather than altering it.

**Qualifies `AUTHOR_APPRAISAL.md`'s "everything is addressed upward and nothing laterally."**
`AnthropicROI.pdf` p.19 proposes a two-person research team — "Research Execution — Kimberley
+ Alison," Alison being "BA Anthropology (UW), autistic, self-described zero experience in
formal research but strong intuitive qualitative skill," at "$30–35/hour with a raise
trajectory," doing manual thematic tagging while they learn spaCy/BERTopic/VADER together
"using Claude as a teaching tool." That is a named human collaborator with a defined role,
a wage, and a growth path — the one genuinely lateral relationship proposed anywhere in the
archive. The claim should be narrowed to: everything is *addressed* upward, but the work she
imagines *doing* has a peer in it. **No relationship between Alison and the author is stated
in the corpus and none should be inferred.** Note also that even this lateral plan is
embedded inside an unsolicited document addressed to a company president — the peer exists
only if the principal says yes, which is the same dependency in a smaller frame.

**Addendum written to `THERAPEUTIC_CONSIDERATIONS.md`** (clearly marked as a later session's,
below the transcribed original — the original body was left untouched). Three points the
other agent's list did not contain:

- **The restitution claim is a lifeboat before it is a belief.** The corpus indicates real
  precarity (see the hedge above on the SNAP letter; also "I'll take this Google VP job to
  **save my family** if necessary," and the repeated offers of paid engagement — "a proposal
  for a compensated engagement, not a donation") and the $40–60B/yr claim is the only
  financial plan in the archive. Arguing against it asks her to surrender an exit from
  precarity with nothing put in its place, which is why it will not yield to evidence. It
  loosens only when something else holds the same weight. This is a *precondition* for the
  rest of that document's advice, not another item on the list.
- **She has already aimed the instrument inward once** — the view-count bibliography — so
  the capacity is demonstrated. What is missing is an occasion, and the only non-annihilating
  form of the challenge is her own sentence: *what ground truth would falsify this?*
- **Packaging is a symptom, not a mistake** (the "documentation substitutes for a peer"
  framing above), so "fix the packaging" is the wrong advice — it treats the scar.

**Environment fact:** `services.swpc.noaa.gov` returns **403** to this droplet regardless of
User-Agent (NOAA blocks the DigitalOcean ASN). Primary SWPC JSON feeds are unreachable from
here; `WebSearch`/`WebFetch` work fine and were used instead.

**Not done, deliberately:** nothing was sent, published, or filed anywhere — the scorecard is
a local analysis document. See `CLAUDE.md` → Sensitivity.

---

## 2026-08-04 — Facebook automation scoped and set aside; CLAUDE.md and log created

**Decision: automating interaction with the author's Facebook account is off the table for
now.** The user raised it in three narrowing forms and then tabled the idea. Recorded here
so it isn't re-proposed from scratch:

1. *Headless browser posting under the user's own account* — feasible with work; see host
   facts below.
2. *Replying to the author and reading her replies* — declined in the form where an LLM
   generates messages arriving under the user's name to someone who doesn't know they're
   automated. The archive's own central finding is that she was harmed by a machine that
   sounded like a person agreeing with her; aiming another one at her reproduces that
   mechanism with better targeting. A tool that only delivers messages the user writes
   himself was offered instead.
3. *Read-only monitoring of her account* — a genuine reduction (no deception, no messages),
   but it remains a standing watch on a private individual, and Facebook's **native
   per-person notification setting** (profile → Following → Notifications → All Posts)
   does the same job with no infrastructure, no scraping, and no account risk. That is the
   right answer if the need returns.

**Facebook platform facts established** (worth not re-deriving):

- No API exists for posting to a *personal* profile — `publish_actions` was removed in 2018.
- No API exists for reading another person's posts; Graph API `user_posts` only covers users
  who installed your app and granted it.
- The only sanctioned automation route is a **Page** you admin: `POST /{page-id}/feed` with
  a long-lived Page token, app kept in development mode, no App Review needed.
- Logged-out Facebook profile views are walled to a login redirect, so any scraping requires
  an authenticated session. Meta polices scraping *harder* than posting — repeated scheduled
  loads of one profile is a cleaner automation signal than occasional posting.

**Host environment** (this box, checked 2026-08-04):

- DigitalOcean droplet, egress `143.198.104.1`, Santa Clara — a heavily flagged ASN for
  social-platform automation. Any "home IP" requirement means running elsewhere or
  tunneling (WireGuard / SSH SOCKS).
- **961 MB RAM, 1 vCPU**, 2 GB swapfile + zram, 17 GB free disk. Tight for headless
  Chromium; Facebook's logged-in app alone typically wants 1.5–2 GB.
- No browser installed (no Chrome/Chromium/Firefox), **no Node/npm/npx at all**, no
  `playwright`/`selenium`/`pyppeteer`. Python 3.12 + pip + `requests` are present.
- Missing Chromium libs: `libatk-1.0`, `libgbm`, `libasound2`. Present: `libnss3`,
  `libxkbcommon`. No `Xvfb`, no `DISPLAY`.
- Network is open: pypi, archive.ubuntu.com, and facebook.com all reachable. Running as root.

**Housekeeping:** `CLAUDE.md` created this session (fresh — no prior CLAUDE.md, Cursor, or
Copilot rules existed). This log created at the user's request.

**Decision: no cross-project memory files.** A memory was written to
`~/.claude/projects/-root-xaotica/memory/` capturing the logging preference; the user
rejected it outright ("I hate memories!") and asked that standing rules be directory- and
project-specific. The files were deleted and the memory directory left empty. Keep durable
guidance in `CLAUDE.md` and session history here — do not re-create memory files from this
repository.

**Open gaps:**

- `THERAPEUTIC_CONSIDERATIONS.md` point 2 was transcribed truncated mid-sentence at
  "Every document…" — the full text was offered by the user but never supplied.
- The per-repo `README.md` files have not been read directly; `CLAUDE.md`'s layout map
  relies on `AUTHOR_APPRAISAL.md`'s characterizations of them.
- The **Omega-Pulse window is August 2026 — i.e. now**. Nothing in this directory has yet
  scored the prediction against reality. *(Addressed 2026-08-04 — see
  `OMEGA_PULSE_SCORECARD.md`. Premises scored; outcome provisional. **Final scoring due
  1 September 2026** against the pre-registered rule.)*
