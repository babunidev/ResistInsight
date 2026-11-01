# ResistInsight — concept

**By:** Babuni  
**Status:** Finished; maintenance only

## Where the idea came from

While playing a warrior on a private World of Warcraft server, resistances became a mechanic I particularly enjoyed. They felt valuable in play, but the game's character panel gave me little help understanding what the numbers actually did. Building a way to explain those numbers became a learning exercise as much as an addon project. By working through the resistance model, the mechanics became clearer to me too.

The result was **BuxbrewResist**, now presented on GitHub as **ResistInsight**. Seeing estimated mitigation and possible resist outcomes directly in the tooltips made those stats more meaningful and made the project personally rewarding, even though resistance mechanics are a niche interest.

## What the addon does

For the original WoW 1.12 client, the addon supplements five magic-resistance tooltips with estimated average reduction, partial-resist outcomes, changes from adding 10 resistance and a comparison against a higher-level attacker. Detailed chat explanations are available through `/buxres`. The installed addon keeps its historical `BuxbrewResist` identifiers.

The design explains **possible outcomes and long-run averages**, not a guarantee for the next spell. The legacy probability buckets and spell-miss assumptions are approximations rather than server-verified measurements. Binary spells and damage-over-time effects have special cases that this addon cannot universally resolve.

## What remains

The original addon is a **finished project**, with new development paused. Players on compatible private-server clients, including Turtle WoW / Octo WoW environments, may continue to use it. Compatibility with current client builds has not been retested here. Reported problems can be sent to **babunigaming@gmail.com** for maintenance.

[ResistForever](https://github.com/babunidev/ResistForever) is the later port, maintained as a separate project with its own rules and development history.

This account reflects my newly supplied recollection of the original motivation, alongside source-observed behavior. It does not invent a lost design discussion or claim the original code was written unaided.
