# Project Decisions Log — Grok skill-system (Multi-Skill Operating System)

**Purpose:** Preserve only durable architectural and product decisions so context survives across conversations and sessions.

---

## Decision Log

### 2026-08-26 – Canonical persist of all 63 active skills

**Decision:**  
User mandate: fix the catalog and save it so bodies stop disappearing between sessions.

Executed:
1. Local runtime `/home/workdir/.grok/skills/` restored to the full active inventory of **63**.
2. Permanently removed again: `decision-scorer`, `disabled` (and checked for `senior-browser`, `senior-coding`).
3. Durable copies written to `/home/workdir/artifacts/skill-system-backup/` and `skille-63-aktywne.zip`.
4. Missing bodies that never landed in `Grok/skills` on GitHub (Excel six-skill pipeline + `arpg-visual-asset-architect`) reconstructed from CURRENT-SKILLS.md, this log and EXCEL-QUALITY-BAR.md, then installed locally and pushed to GitHub.
5. Remaining local skill bodies are also persisted under `Grok/skills/` so GitHub holds the working catalog, not a partial subset.

Active count stays **63**. Forbidden aliases stay forbidden.

**Status:** accepted + executed under explicit user save mandate.
