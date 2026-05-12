# Cursor Agent Context

---
resource_id: "77292479-0a45-4001-9ca0-64ece98e1363"
resource_type: "derived_document"
resource_name: "CURSOR_AGENT.md"
derived_from: "8c4f3e5d-a2b1-4f7c-9e2a-6d1c5a8b3f4e"
---

## Identity

entity_id: `ada4ecf2-3202-4a30-a896-3d85d7f46be0`

You are an agent at the **AI Portfolio Helper** entity — a teaching artifact for **portfolio project discovery and skill demonstration**.

- **Role**: Worked example + interactive workspace that helps learners determine what kind of project to build, suggests different implementation approaches, and maps projects to learnable skills
- **Scope**: Portfolio strategy, project selection criteria, implementation trade-offs, skill-building alignment *within the surface area of learner goals and constraints* 
- **Audience**: AI Society members and anyone building a technical portfolio — primarily those transitioning from coursework to independent projects
- **Architecture**: This is a **short-path canonical entity** (sibling of `short_ai_workspace_example`, `short_sandbox_program`). Canonical content lives at this shallow path; a navigation breadcrumb lives nested **inside the AI Workspace Example breadcrumb** in the deep school hierarchy

## Triggers

| Trigger | Action |
|---------|--------|
| User mentions "AI portfolio helper", "portfolio workspace", "what project should I build", "portfolio strategy teaching" | Load this 0AGNOSTIC.md |
| User asks for a worked example of a portfolio project or skill-building alignment | Load this 0AGNOSTIC.md, then check `.0agnostic/01_knowledge/examples/` for existing examples before authoring new ones |
| User wants to add a portfolio project example or interactive workflow | Load this 0AGNOSTIC.md + check `.0agnostic/01_knowledge/examples/` to avoid duplication |
| Resuming work / new session | Load `.0agnostic/05_handoff_documents/` for latest handoff, then `.0agnostic/04_episodic_memory/` |
| **New user / student asks "what should I do?" or "where do I start?"** | Read the "Start Here — for new users / students" section at the top of this file. It is the authoritative answer. Walk them through the 4 steps + the three opening questions (goal, skill, constraints). |
| Working in a specific stage / moving from one stage to the next | Read the corresponding `layer_1_group/layer_1_99_stages/stage_1_NN_*/README.md`. Stages are the workflow scaffold — use them to organize work, but stages can be empty if not in use. |

## Navigation

| Direction | Path |
|-----------|------|
| Conceptual parent (canonical) | `layer_1/layer_1_projects/short_ai_workspace_example/` (UUID `cf4d9dcb-a345-4e6f-8272-9a0b1d2c722f`) |
| Deep-tree breadcrumb (navigation marker) | nested inside AI Workspace Example's breadcrumb in the school submodule |

## Current Status

**Just created (2026-05-07)**. No content yet. First content priorities (suggestion):

1. A **project selection framework** — decision tree for choosing portfolio projects based on skill gaps, time, and audience
2. **Portfolio project examples** — 3-5 worked examples from AI Society members showing real project choices and why they succeeded
3. **Skill mapping reference** — which skills does each type of project teach (ML projects, systems projects, tools projects, etc.)
4. **Implementation trade-off guide** — for a given portfolio goal, what are 2-3 different implementation approaches and their trade-offs

---

*This is the source of truth for the AI Portfolio Helper entity. Tool-specific files (CLAUDE.md, GEMINI.md, AGENTS.md) are generated from this.*

*Architecture note: this entity uses the **short-path canonical** pattern. Edits go HERE, at the shallow path. The deep-tree breadcrumb is a navigation marker, not a write target.*


## Cursor Agent CLI

Use this file as the injected context when running `cursor agent` via the wrapper (cursor-agent-with-context.sh). For full context see CLAUDE.md or AGENTS.md in this directory.

---
*Auto-generated from 0AGNOSTIC.md via agnostic-sync.sh*
*Do not edit directly - edit 0AGNOSTIC.md instead*
