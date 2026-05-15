# baimiao-skill

A reusable AI text generation skill encoding the principles of Chinese **plain description** (白描, *báimiáo*) — a writing style that withholds explicit naming of emotions, judgments, and causal links, leaving the work of interpretation to the reader.

> 中文版本：[README-zh.md](README-zh.md)

## What this is

`SKILL.md` is a Markdown skill file compatible with [Claude Code](https://docs.claude.com/en/docs/claude-code), the [Claude Agent SDK](https://docs.claude.com/en/api/agent-sdk), and Claude.ai. It encodes the philosophy, requirements, mechanisms, boundaries, and self-checks of 白描 as a constraint set for AI text generation.

The skill is **language-style-only** — it makes no assumption about application context (novels, screenplays, RPG dialogue, journalism, etc.). For CRPG dialogue graph node-level use, see the companion repo [baimiao-rpg-node-skill](https://github.com/outsiderrr/baimiao-rpg-node-skill).

## How to use

**In Claude Code**: place `SKILL.md` in `.claude/skills/baimiao/` of your project, then invoke when generating text.

**In Claude Agent SDK or API**: include the content of `SKILL.md` as a system prompt prefix when calling the model.

**In Claude.ai**: paste the content into a project's system prompt, or upload as a project file.

## Content overview

1. **Essence** (本质定义) — 4 keywords: low intervention, facts, withholding the naming right, judgment left to the reader
2. **5 requirements** (构成要件) — perceivability, physical adjectives, concrete-object metaphors, no summary endings, implicit causality
3. **5 implementation mechanisms** (W-B.1–5) — differential, materialization, third-party reflection, key-word loadbearing, action-chain accumulation
4. **3 operational principles** (运作机制) — name dissipation, inverse density law, prior-knowledge dependency
5. **4 boundary conditions** (边界条件) — when not to use 白描
6. **5 adjacent concept distinctions** (相邻概念辨析) — what 白描 is *not* (≠ brevity, ≠ objectivity, ≠ minimalism, ≠ non-lyrical, ≠ show-don't-tell)
7. **7-point self-check** for finished text

## Note on language

The skill content itself is written in Chinese (白描 is a Chinese aesthetic concept with established Chinese-language references — Lu Xun, Wang Zengqi, etc.). The skill can still be used to generate text in any language whose 白描 principles transfer.

This README is in English by default; a Chinese version is available at [README-zh.md](README-zh.md).

## License

[CC BY 4.0](LICENSE)

You are free to share and adapt this work for any purpose, including commercially. Attribution is required — please link back to this repository.
