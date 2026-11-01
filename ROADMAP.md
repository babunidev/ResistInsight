# ResistInsight — roadmap and maintenance status

**By:** Babuni

## Status: complete, maintenance only

ResistInsight (originally **BuxbrewResist**) is finished in its intended scope. New features and proactive development are **not planned**. The earlier phrase "on hold" refers to new development, not abandonment of players who already use the addon.

The addon remains available for compatible WoW 1.12 private-server clients. Bugs or breakages reported by Turtle WoW / Octo WoW players may be fixed when reported to **babunigaming@gmail.com**. A report should include the client/server version, reproduction steps and any visible error. There is no promised release schedule, and this documentation pass did not establish current client compatibility.

The newer port is [ResistForever](https://github.com/babunidev/ResistForever). Its future development is separate from this repository.

## Existing scope

- Show explanatory mitigation estimates and resistance outcomes in five magic-resistance tooltips.
- Provide detailed school summaries and examples through `/buxres`.
- Preserve the historic `BuxbrewResist` installation names and slash commands.

## Deferred technical checks

These are **maintenance investigation notes**, not a planned feature roadmap or evidence of a current defect.

- Run `tests/test_tooltips.py` with a suitable Python/Lupa Lua 5.1 environment, recording the command and results; a mocked harness is not an in-game test.
- Check tooltip hooking, repeated initialization, frame ownership and interaction with other addons in the target client.
- Validate negative resistance, caps, low-level behavior and missing stats if a relevant bug is reported.
- Treat the legacy bucket distribution, spell-miss assumptions and binary/DoT examples as approximations until verified against actual server behavior.
- Review screenshots and the unused `BuxResDB` declaration only when maintenance requires it.

No addon code or gameplay tests were changed or run during the November 2026 documentation revision.
