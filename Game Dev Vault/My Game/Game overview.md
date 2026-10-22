---
tags: [reference]
updated: 2026-01-01
---

# Game overview

Back to [[My Game]]

Every system in the game, where its scripts live, and which page explains it. The AI keeps this up to date so it never has to "search the whole game" again.

> ✏️ *Example for Pizza Rush. Ask your AI: "look through my game and fill in Game overview".*

| System | Where | Scripts | Notes |
|---|---|---|---|
| Player data (saving) | ServerScriptService | `PlayerData` | DataStore `PizzaRush_v2`. Cash, rebirths, streak. **Careful: saved data.** |
| Shop / ovens | Workspace.Tycoons | `TycoonServer`, `ButtonHandler` | One tycoon per player, 6 plots |
| Delivery riders | ServerScriptService | `RiderAI` | Pathfinding to houses, pays on arrival |
| Daily rewards | ServerScriptService + StarterGui | `DailyRewards`, `DailyRewardsUI` | See [[Daily rewards]] |
| UI kit | ReplicatedStorage | `UIKit` | Shared buttons / colours. Use it for new UI. |
| Settings | StarterPlayerScripts | `SettingsClient` | Music, SFX, graphics |

## Remotes
| Remote | From → to | What |
|---|---|---|
| `ClaimDaily` | client → server | Claim today's reward (server checks the time) |
| `BuyButton` | client → server | Buy a tycoon button (server checks cash) |

## Data keys
| Key | Type | Used by |
|---|---|---|
| `Cash` | number | everything |
| `Rebirths` | number | `TycoonServer` |
| `Daily` | `{streak, lastClaim}` | [[Daily rewards]] |
