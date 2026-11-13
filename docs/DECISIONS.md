# ResistInsight — decisions

**By:** Babuni

## Confirmed creative decisions

| Decision | Rationale and boundary |
| --- | --- |
| Explain resistance values in tooltips | The default WoW 1.12 character panel did not explain enough; making the addon also helped me learn the mechanics |
| Retain the historical installed addon identity | GitHub is named `ResistInsight`, but the addon still installs as `BuxbrewResist` and uses `/buxres` |
| Consider the original addon finished | Further features are not planned; "on hold" applies to new development |
| Accept maintenance reports | Players can contact `babunigaming@gmail.com` with reproducible issues, without an implied release schedule |
| Keep ResistForever separate | The later port has its own client target, implementation history and mathematical assumptions |

These decisions were clarified directly in November 2026. They do not imply that all earlier implementation choices were documented as explicit personal approvals.

## Observed implementation choices

| Source behavior | Evidence | Limit |
| --- | --- | --- |
| Weighted partial-resist outcomes | `buildBuckets`, `expectedReduction` | Approximate distribution, not measured server probabilities |
| Multiplicative combination of misses and resistance | `totalReduction` | Assumed direct-damage scenario |
| Separate negative-resistance vulnerability path | Negative resistance calculations | Actual server behavior unverified |
| Preserve existing hover handlers | Tooltip hook wrapper and guard | Coexistence with all addons untested |
| Mocked Lua verification harness | `tests/test_tooltips.py` | Not an in-client compatibility test |

## Deferred investigations, not approved work

Client compatibility, level edge cases, negative resistance, tooltip interactions, DoT/binary exceptions and model accuracy warrant investigation **only if maintenance requires it**. The November documentation pass made no gameplay change and ran no tests. See [ROADMAP.md](../ROADMAP.md) for the maintenance boundary.

## 2026-11-13 — Licensing decision

To make the reuse terms explicit, I approved MIT for original addon software. This applies only to material for which the relevant rights can be granted; third-party contributors keep their own credits and licenses. AI assistance committed the license notice and updated project-facing documentation. This was a legal/documentation change, not a runtime feature or test.
