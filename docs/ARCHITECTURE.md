# ResistInsight — architecture

**By:** Babuni  
**Runtime:** WoW 1.12 addon, installed as `BuxbrewResist`

This records the original implementation. The later [ResistForever](https://github.com/babunidev/ResistForever) port must not inherit these assumptions without separate verification. The November 2026 revision changed documentation only.

## Resistance estimates

`BuxbrewResist.lua` maps magic schools and reads the total resistance from the second return value of `UnitResistance`. For nonnegative values, `computeAverageResist` clamps `R / (5 * max(level, 20)) * 0.75` to 0–0.75. `buildBuckets` samples eleven points with triangular weights, normalizes and groups them into 0%, 25%, 50%, 75% and 100% resist outcomes. `expectedReduction` weights those outcomes, so the result need not equal the initial clamped figure.

Negative resistance follows a separate `R / (5 * max(playerLevel, 20))` vulnerability approximation, without the positive model's 0.75 multiplier. `totalReduction` calculates `miss + (1 - miss) * average` with an assumed 4% same-level base miss and 1% for the level+3 comparison. The binary rejection explanation uses a different, capped additive reference formula. None of these calculations is a verified universal probability model for private servers.

## Interface and commands

Tooltips hook `MagicResFrame1..5`, preserve the previous `OnEnter` handler and use legacy global `this`. School identity comes from `frame:GetID()`, not visible order. Checks for ownership and missing values protect some edge cases; a per-frame flag guards against repeated hooks. Hook installation runs immediately and on `ADDON_LOADED` / `PLAYER_LOGIN`. Values are refreshed on hover.

`/buxres` accepts school names and unambiguous prefixes; Physical and Holy use separate summaries. The TOC declares interface `11200`, version `1.2` and a saved variable named `BuxResDB`; the inspected Lua does not use that variable.

## Evidence and verification

The source audit dated **2026-10-26** examined the Lua, TOC, README, test harness and selected commits at [0691901](https://github.com/babunidev/ResistInsight/commit/06919016c8e0e11041fb633920b507a91058dd97). The November documentation revision rechecked the current source and metadata; neither audit established live gameplay compatibility or measured server behavior. The Python/Lupa test harness exists but was not executed in this pass.
