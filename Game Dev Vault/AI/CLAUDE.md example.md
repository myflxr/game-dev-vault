---
tags: [ai, claude-code]
---

# CLAUDE.md example

Back to [[START HERE]]

**Claude Code** reads a file called `CLAUDE.md` automatically at the start of every session. Put one in your project folder (next to your game files) so Claude always uses the vault, without you pasting a prompt.

1. Create a file named `CLAUDE.md` in your project folder.
2. Paste the text below and change the path to where your vault is.

```markdown
# My game

## Vault (read first)
My notes for this game are in an Obsidian vault:
C:\Users\<you>\Documents\Game Dev Vault\My Game

Before deciding anything, read:
- How you think.md  (how I decide; it beats your defaults)
- Working rules.md  (always apply)
- Game overview.md  (systems and scripts)
- Open questions.md

## After every task
1. Report: cause -> fix -> how you tested (numbers / screenshots).
2. Update the vault: Timeline entry, the feature page in Features/,
   Open questions, and How you think if I decided or corrected something.

## Always ask first
Robux / players' money, saved data changes, deleting my work.
```

> 💡 With Claude Code you can also say *"remember that"* and it saves the fact to its own memory. The vault is still better for anything you want to **see and edit yourself**.
