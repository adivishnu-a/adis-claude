# adis-claude

My global `CLAUDE.md` for Claude Code: always-on behavioral guidelines that apply to every project.

## What's in it

`CLAUDE.md` has three parts:

1. **Coding discipline** — think before coding, simplicity first, surgical changes, goal-driven execution. Includes a note to check current docs on the web for key technical decisions instead of relying on stale training data.
2. **Frontend & UI design** — decide before drawing, commit to a direction, craft-floor checks, operate-mode rules, hardening, copy, and a list of defaults to refuse.
3. **UX psychology & conversion** — ask easy questions, be specific, safety nets over sales pitches, reduce decisions, give before you ask, frame honestly, the action area.

`AGENTS.md` is the same content for tools that read the AGENTS.md convention (Cursor, Codex, Copilot, etc.). `CLAUDE.md` is the source of truth; if you edit one, mirror the change in the other.

Sources are credited in the header comment of `CLAUDE.md`.

## Install

Copy it to the global Claude Code config location:

```bash
cp CLAUDE.md ~/.claude/CLAUDE.md
```

Or symlink it so edits in this repo apply immediately:

```bash
ln -sf "$(pwd)/CLAUDE.md" ~/.claude/CLAUDE.md
```

Project-level `CLAUDE.md` files add to these; they don't replace them.
