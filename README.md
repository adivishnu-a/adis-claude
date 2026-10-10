# adis-claude

My global `CLAUDE.md` for Claude Code: always-on behavioral guidelines that apply to every project.

## What's in it

`CLAUDE.md` has five parts:

1. **Coding discipline** — think before coding, simplicity first, surgical changes, goal-driven execution. Includes a note to check current docs on the web for key technical decisions instead of relying on stale training data.
2. **Frontend & UI design** — decide before drawing, commit to a direction, craft-floor checks, operate-mode rules, hardening, copy, and a list of defaults to refuse.
3. **UX psychology & conversion** — ask easy questions, be specific, safety nets over sales pitches, reduce decisions, give before you ask, frame honestly, the action area, meet users where they are, fit the control to the task, recognition over recall.
4. **Interface patterns** — rank then style, filters as decision support, content over banners, polish where it's felt.
5. **Mobile & touch UI** — rebuild for mobile instead of shrinking, one screen one job, gestures, the bottom bar.

`skills/audit/` is an on-demand `/audit` skill: an independent, read-only pre-launch audit with a weighted score and launch verdict. It runs in a forked subagent with file-editing tools removed, and audits against `CLAUDE.md` as the house standard, which outranks the audit's own criteria. Install by symlinking it into `~/.claude/skills/audit`.

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

Install the audit skill by symlinking its folder (it then appears as `/audit`):

```bash
mkdir -p ~/.claude/skills && ln -sfn "$(pwd)/skills/audit" ~/.claude/skills/audit
```
