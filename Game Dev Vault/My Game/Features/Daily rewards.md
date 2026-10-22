---
tags: [feature]
updated: 2026-01-01
---

# Daily rewards

Back to [[My Game]] · Spec: [[Spec - Daily rewards]]

> ✏️ *Example of a feature page: written by the AI after building. It's the manual for future you (and future AI).*

## What it does
A 7-day login streak. One claim per day; the prize grows each day; missing a day resets the streak to day 1.

## How it works
| Part | Where | Job |
|---|---|---|
| `DailyRewards` | ServerScriptService | Checks `os.time()` against `lastClaim`, pays the prize, saves `Daily` |
| `DailyRewardsUI` | StarterGui | The calendar popup and the red dot |
| `ClaimDaily` | ReplicatedStorage remote | Client asks, server decides |

## Prizes (change them here)
| Day | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
|---|---|---|---|---|---|---|---|
| Cash | 100 | 150 | 200 | 300 | 500 | 750 | 1500 |

Edit `DailyRewards.Prizes` to change them.

## Saved data
`Daily = {streak = 1..7, lastClaim = unix time}`. Old saves without it start at day 1.

## Tested
- Clock +1 day → day 2 ✔ · +9 days → reset to day 1 ✔
- Old save without `Daily` ✔ · Phone layout ✔ · Claim spam (10 clicks) → paid once ✔
