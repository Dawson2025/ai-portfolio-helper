# AI Portfolio Helper

A teaching artifact for **portfolio project discovery and skill alignment** — helps learners decide what to build, suggests different implementation approaches, and maps projects to demonstrable skills.

## What this teaches

Portfolio strategy *within the surface area of learner goals and constraints*:

- Project selection frameworks (decision trees for what to build)
- Skill-building alignment (which projects teach which skills)
- Implementation trade-off analysis (multiple approaches for a given goal)
- Portfolio narrative (how projects fit together as a story)

## Who this is for

Students transitioning from coursework to independent projects, early-career engineers building a public portfolio, anyone aligning project choices to specific learning goals or audience signals.

## Companion to AI Workspace Example

This entity is a **sub-feature** of [AI Workspace Example](https://github.com/Dawson2025/ai-workspace-example). The workspace example teaches *how* to configure your AI coding harness; this entity teaches *what* to build with it.

## Repository structure

This repository follows an entity-system pattern:

| Path | Purpose |
|------|---------|
| `0AGNOSTIC.md` | Source of truth for entity identity, scope, rules |
| `.0agnostic/` | On-demand resources (knowledge, rules, protocols, episodic memory) |
| `CLAUDE.md`, `AGENTS.md`, `GEMINI.md`, `CURSOR_AGENT.md` | Auto-generated tool-specific context files — do not edit directly |
| `.claude/`, `.cursor/`, `.github/` | Tool-specific configuration |

Edit `0AGNOSTIC.md`; tool-specific files regenerate via `agnostic-sync.sh` (upstream tooling).

## Status

Newly scaffolded — content (project frameworks, case studies, skill mappings) will be added over time.

## License

[PolyForm Noncommercial License 1.0.0](LICENSE.md) — source-available, free for non-commercial use.

| Use case | OK? |
|---|---|
| Personal study, hobby projects | Yes |
| Educational institutions, public research, non-profits, government | Yes |
| Internal use at a for-profit company | No — requires permission |
| Building a commercial product on top | No — requires permission |
| Republishing as your own | No |
| Using as training data for AI models | No — requires permission |

**Required Notice** (must be preserved in any redistribution):

> Required Notice: Copyright (c) 2026 Dawson

For commercial licensing, contact the copyright holder.

## Attribution

If you build on this work in any context where attribution is appropriate, please credit:

> Based on the AI Portfolio Helper by Dawson (https://github.com/Dawson2025/ai-portfolio-helper)
