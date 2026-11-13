# ResistInsight — development journal

**By:** Babuni

## November 2026 — a small addon that taught me something

Resistances caught my attention while playing a warrior on a private World of Warcraft server. Their importance in play appealed to me, but the character panel never explained enough about what a resistance rating actually meant. Making BuxbrewResist gave me both an answer and a useful tool: by working through the calculations, the mechanics became clearer, and the tooltip could finally show the estimated chances and damage reduction rather than another unexplained number.

Seeing those results in the game was satisfying. A small audience may care about resistance statistics in this much detail, but that never made the project less worthwhile to me. The same idea eventually became the foundation of [ResistForever](https://github.com/babunidev/ResistForever), a port for a newer game environment. Some players have downloaded that successor; its continuing development belongs to its own repository.

With the old repository renamed **ResistInsight**, this original version feels complete. There are no plans to add more features, although problems reported by Turtle WoW / Octo WoW players can still be addressed. At my direction, AI updated the documentation and corrected the earlier, ambiguous "on hold" description. No gameplay code was changed or retested in this session.

## Retrospective evidence

The implementation history is partly reconstructed from source and commit metadata, not from a complete record of the original design conversations. Lua appeared in September 2025; identifiable September 2026 changes include character-panel tooltip support, negative-resistance presentation and combined spell-miss estimates. The dated evidence is preserved in [CHANGELOG.md](../CHANGELOG.md).

An October 2026 documentation review inspected source, tests and selected diffs without running the game or tests. The November revision adds my personal recollection of why the project began and clarifies its maintenance policy. AI helped review, structure and write these records; the original creative motivation was mine. Earlier coding assistance cannot be reconstructed confidently from generic commit names.

## 2026-11-13 — Giving the repository clear permissions

Public source alone did not explain what others could reuse, so I approved MIT for original addon code. AI assistance added the license and brought the project notes into agreement, without changing how the application runs. Other people's content retains its own terms.
