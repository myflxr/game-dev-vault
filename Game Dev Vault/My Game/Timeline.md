---
tags: [log]
updated: 2026-01-01
---

# Timeline

Back to [[My Game]]

What was done, newest at the bottom. One entry per task: **what you asked → what was built → how it was tested → what's left.** Link the pages involved.

> ✏️ *Example entries. Your AI adds one after every task.*

## 2026-01-01
- **Daily rewards** ([[Spec - Daily rewards]] → [[Daily rewards]])
  - Asked: a 7-day login streak, prize grows each day, resets if you miss a day.
  - Built: `DailyRewards` (server) checks time on the server, `DailyRewardsUI` popup, data key `Daily`.
  - Tested: Play test with the clock moved forward 1, 2 and 9 days; old saves without `Daily` load fine; phone layout checked.
  - Backup: `_Backup_DailyRewards` ([[Backups and tools]]).
  - Open: prize amounts for days 5–7 ([[Open questions]]).
