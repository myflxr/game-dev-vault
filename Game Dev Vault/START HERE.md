---
tags: [guide]
---

# 👋 Start here

This vault is a **shared memory for you and your AI** while you build a game.

AI assistants (Claude, ChatGPT, Copilot…) forget everything between chats. This vault fixes that: every decision, plan and change lives here, and the AI reads it before it works. Result: it stops asking the same questions, stops undoing your choices, and builds things *your* way.

Made by **Doom Studio**. Free to use, change and share.

---

## How to use it (5 minutes)

1. **Install Obsidian** (free): https://obsidian.md
2. Open Obsidian → **Open folder as vault** → pick this `Game Dev Vault` folder.
3. Rename the example game folder **`My Game`** to your game's name (Obsidian fixes the links for you).
4. Fill in three pages first:
   - [[My Game|Home page]]: what your game is, in a few lines
   - [[How you think]]: what you're aiming for and how you like to work
   - [[Working rules]]: rules the AI must always follow
5. Give your AI access to the vault (see below) and paste the start prompt from [[AI prompt - start of a session]].

> The example pages are filled in for a made-up Roblox game, **Pizza Rush**, so you can see what "good" looks like. Replace them with your own, or keep them as a guide.

---

## Giving the AI access

| AI tool | How it reads the vault |
|---|---|
| **Claude Code** (desktop app or terminal) | Best option. It can read and write files directly. Add the vault folder to the session, and put [[CLAUDE.md example]] in your project so it reads the vault every time. |
| **Claude / ChatGPT in the browser** | Paste the important pages ([[How you think]], [[Working rules]], the spec) into the chat, or attach them as files. Copy its summary back into [[Timeline]] yourself. |
| **Cursor / VS Code with AI** | Open the vault folder in the editor next to your game code. |

---

## The loop (how a feature gets built)

1. **Write a spec** in `Specs/` using [[_Spec template]] (or ask the AI to draft one with [[AI prompt - write a spec]]).
2. **AI reads the vault, then plans.** It explains the cause / plan in plain words before building.
3. **You say OK** (or let it go for small jobs, your choice in [[Working rules]]).
4. **AI builds and tests**, then reports: what changed, how it was tested, what's still open.
5. **AI updates the vault:** a [[Timeline]] entry, the feature page, [[Open questions]], and [[How you think]] if you decided something new.

That last step is the magic. Every session makes the next one smarter.

---

## What's in here

| Folder / page | What it's for |
|---|---|
| `My Game/` | Everything about one game. Make a copy of the folder for each new game. |
| [[How you think]] | Your taste and habits, with real quotes. The AI reads this first. |
| [[Working rules]] | Hard rules: backups, testing, what needs your OK. |
| [[Game overview]] | Every system in the game and where its scripts are. |
| [[Timeline]] | What was done, day by day. |
| [[Open questions]] | Decisions waiting for you (checkboxes). |
| [[Backups and tools]] | Backups the AI made and helper tools, so nothing gets lost. |
| `Specs/` | One page per feature request. |
| `Features/` | One page per finished system: how it works, how to change it. |
| `AI/` | Copy-paste prompts and the `CLAUDE.md` example. |
| `Templates/` | Blank pages for Obsidian's Templates plugin (Ctrl+P → "Insert template"). |

Questions? Join the Doom Studio Discord and ask in `#ai-workflow`.
