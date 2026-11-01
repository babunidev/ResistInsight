# ResistInsight — experience design

**By:** Babuni

## Making a number meaningful

The resistance stats on my warrior were interesting precisely because they could affect combat, yet the character panel left their meaning obscure. ResistInsight was conceived to answer the question at the point of use: **what might this resistance value actually do?** Working on those explanations also helped me understand the mechanic.

Instead of adding a separate interface, the addon extends the existing five magic-resistance tooltips. They show an estimated long-run average, possible partial-resist outcomes, the effect of another 10 resistance and a comparison against a higher-level caster. A compact total sits at the end; `/buxres` provides longer examples in chat. Negative resistance is shown as a red vulnerability estimate, without a misleading probability table.

## Boundaries of the presentation

The visuals express estimates, not guarantees: one cast can behave differently from the displayed average. Red/green emphasis is accompanied by labels and signs. Base spell-miss assumptions, DoT ticks and binary spells require careful qualification because the addon does not verify every server's rules.

Screenshots in the [README](../README.md#screenshots) illustrate the existing UI; they are not evidence of current runtime compatibility. The original interface is a completed design, not a proposal for additional features. Bug-related presentation changes remain possible.
