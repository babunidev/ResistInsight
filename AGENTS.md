# ResistInsight — contribution and documentation rules

**Creative:** Babuni
**Repository:** `babunidev/ResistInsight`
**Installed addon:** `BuxbrewResist`
**Status:** Finished; maintenance only

## Boundaries

- The project originated from Babuni's interest in resistance mechanics while playing a warrior on a private World of Warcraft server. The addon made tooltip values easier to understand; creating it also helped Babuni learn the mechanics.
- No proactive feature roadmap is planned. Player-reported bugs or compatibility problems may receive fixes, coordinated via **babunigaming@gmail.com**.
- The audience includes compatible WoW 1.12 private-server clients, notably Turtle WoW / Octo WoW. Do not promise untested current compatibility.
- [ResistForever](https://github.com/babunidev/ResistForever) is the later port, not the same runtime or necessarily the same resistance model. Keep the projects distinct.
- Retain `BuxbrewResist.lua`, `BuxbrewResist.toc`, the addon folder, manifest identity and `/buxres` unless a separate technical decision explicitly changes them.

## Authorship and writing

- Use **Babuni** for human attribution; **babuni.dev** is the portfolio platform. Use **creative**, not **creator**, as the role label.
- Public-facing accounts of motivation, decisions and development belong in Babuni's **first-person perspective**. Do **not** begin a narrative sentence with `I` or `My`; integrate first-person language naturally.
- Identify the human creative's direction separately from AI drafting, research or coding. Do not imply that Babuni wrote code AI generated, that AI conceived the project, or that any AI proposal was approved without evidence.
- Keep journal entries brief, specific and human-readable; preserve meaningful history without reproducing redundant archival snapshots. Mark retrospective reconstruction where needed.
- Keep source-observed behavior, personal recollection, proposals and tests distinct. Never make up conversations, implementations, compatibility results or historical approval.

## Technical integrity

- Check `BuxbrewResist.lua`, the TOC, tests, relevant diffs and current branch before making behavioral claims.
- This is a legacy approximate model, not verified server probability data. Do not conflate partial resist, full spell failure, binary mechanics and DoT behavior.
- A passing mocked Lupa/Lua 5.1 test is not confirmation that the addon works in a current 1.12 client.
- On a reported defect, investigate tooltip hooks, frame IDs, level-dependent calculations, caps and other addons as relevant. Record the test command, environment and result rather than claiming verification from source alone.
- For substantial maintenance, update README, CHANGELOG, docs/DEVLOG and affected technical docs alongside code. For documentation-only changes, leave Lua, TOC, tests and screenshots untouched. Verify links and changed paths.

## Documentation layout

`README.md` describes installation and usage; `CONCEPT.md` captures the creative origin; `ROADMAP.md` defines maintenance status; `CHANGELOG.md` records changes. The `docs/` directory holds development history, decisions, design, architecture, content and AI attribution.

## Repository-local documentation standard

Follow [the documentation standard](docs/DOCUMENTATION.md) for first-person author voice throughout project documentation, factual changelogs, and naming the AI tool and verified model for each contribution. These rules travel with this repository and do not depend on the babuni.dev ChatGPT Project. Preserve all project-specific technical, creative, canon, safety, licensing, and historical rules in this file; follow the linked standard for public first-person narrative, human–AI attribution, concise development journals, decision records, and evidence-based verification. **Babuni** is the human creative; **babuni.dev** is the website/portfolio, not the person. Preserve third-party credits and historical legal notices. References above to a dated “documentation-only audit” describe that past task, not a permanent ban on later authorized implementation.
