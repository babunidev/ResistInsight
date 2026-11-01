# ResistInsight — change history

**By:** Babuni

## 2026-11-01 — project history and maintenance status

- Clarified my original reason for making the addon: playing a warrior on a private server, enjoying the resistance mechanic, and wanting tooltips that explain it. Learning the model through development was part of the experience.
- Clarified that **ResistInsight is finished**, with no new features planned, while player-reported bugs remain eligible for maintenance at **babunigaming@gmail.com**.
- Documented the intended Turtle WoW / Octo WoW audience without presenting current client compatibility as newly verified.
- Kept the distinction between the original `BuxbrewResist` addon and its port, [ResistForever](https://github.com/babunidev/ResistForever).
- AI revised and consolidated documentation to remove repeated historical snapshots and align narrative style. **No Lua, TOC, test or image files were changed or run.**

## 2026-11-01 — repository renamed

- At my direction, the GitHub repository was renamed from **BuxbrewResist** to **ResistInsight**.
- Documentation links were updated, while installed addon identifiers and `/buxres` remained unchanged.
- The original was previously described as "on hold"; the maintenance clarification above supersedes that ambiguous wording.
- Documentation-only change: [49445f0](https://github.com/babunidev/ResistInsight/commit/49445f01dae4b1feaba6426cb41c7dc983fb2999).

## 2026-10-26 — documentation expansion

Source-informed documentation was expanded to cover usage, concept, architecture, visual design, content, decisions, development history and contributor guidance. Only Markdown was changed; no runtime test was performed.

## Earlier commit evidence

- **2025-09-10:** [f29a611](https://github.com/babunidev/ResistInsight/commit/f29a611e292c9a3bddd1c1b491dd8b4dd1b45c40) — initial Lua addition; many generic "Update" commits followed, whose titles do not establish specific fixes.
- **2026-09-05:** [c421f1f](https://github.com/babunidev/ResistInsight/commit/c421f1f070e33437ea06e69b0cddf82fee5903d0) — inspected diff adds character-panel tooltip handling and a Python/Lupa test harness.
- **2026-09-05:** [7a20e4a](https://github.com/babunidev/ResistInsight/commit/7a20e4a7f599b31dc95a1d3150966886a5ee3b87) — commit metadata describes negative-resistance vulnerability estimates.
- **2026-09-07:** [53fc422](https://github.com/babunidev/ResistInsight/commit/53fc4220e5aa6fc4b08c7995573d1c3db2b57da6) — inspected diff combines base spell misses with total direct-damage estimates, puts explanations into chat and adjusts tests.

Dates are GitHub commit dates, not independently established release dates. Earlier documentation was partly retrospective; AI did not reconstruct undocumented discussions.
