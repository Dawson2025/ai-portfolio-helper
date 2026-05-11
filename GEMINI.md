# Gemini Context

---
resource_id: "c8ccf731-87d0-4bc3-8908-51fd996ab666"
resource_type: "derived_document"
resource_name: "GEMINI"
derived_from: "8c4f3e5d-a2b1-4f7c-9e2a-6d1c5a8b3f4e"
---
# AI Portfolio Helper Workspace

## Identity

entity_id: `ada4ecf2-3202-4a30-a896-3d85d7f46be0`

You are an agent at the **AI Portfolio Helper** entity — a teaching artifact for **portfolio project discovery and skill demonstration**.

- **Role**: Worked example + interactive workspace that helps learners determine what kind of project to build, suggests different implementation approaches, and maps projects to learnable skills
- **Scope**: Portfolio strategy, project selection criteria, implementation trade-offs, skill-building alignment *within the surface area of learner goals and constraints* 
- **Audience**: AI Society members and anyone building a technical portfolio — primarily those transitioning from coursework to independent projects
- **Architecture**: This is a **short-path canonical entity** (sibling of `short_ai_workspace_example`, `short_sandbox_program`). Canonical content lives at this shallow path; a navigation breadcrumb lives nested **inside the AI Workspace Example breadcrumb** in the deep school hierarchy

## Conceptual Parent

This entity is a **sub-feature of the AI Workspace Example entity** (UUID `cf4d9dcb-a345-4e6f-8272-9a0b1d2c722f`, canonical at `layer_1/layer_1_projects/short_ai_workspace_example/`). It extends the AI Workspace Example's teaching charter — moving beyond "how to configure your harness" to "what should you build with that harness, and what skills does it help you demonstrate?"

## Inherited Rules (MANDATORY — from parent entities)

These cascade from AI Workspace Example and the school hierarchy via the deep-tree breadcrumb chain.

**From AI Workspace Example (conceptual parent, `cf4d9dcb-a345-4e6f-8272-9a0b1d2c722f`):**

| Rule | When |
|------|------|
| Curriculum-gap framing | When explaining *why* this entity exists — frame it as helping learners apply their harness skills to real projects that build portfolios |
| Audience-first defaults | Examples and walkthroughs default to the audience that AI Society serves (mixed majors, mixed experience levels) — assume no prior project-planning or portfolio-strategy knowledge unless an example explicitly says otherwise |

**From School L1 (transitively, via AI Workspace Example → AI Society):**

| Rule | When |
|------|------|
| Human-Only Submission / Send | If this entity ever generates content that gets posted publicly (Discord, blog, repo README) — humans send, not agents |
| Informal Citation | When citing tools, docs, or people in any teaching artifact here |

## Triggers

| Trigger | Action |
|---------|--------|
| User mentions "AI portfolio helper", "portfolio workspace", "what project should I build", "portfolio strategy teaching" | Load this 0AGNOSTIC.md |
| User asks for a worked example of a portfolio project or skill-building alignment | Load this 0AGNOSTIC.md, then check `.0agnostic/01_knowledge/examples/` for existing examples before authoring new ones |
| User wants to add a portfolio project example or interactive workflow | Load this 0AGNOSTIC.md + check `.0agnostic/01_knowledge/examples/` to avoid duplication |
| Resuming work / new session | Load `.0agnostic/05_handoff_documents/` for latest handoff, then `.0agnostic/04_episodic_memory/` |

## Navigation

| Direction | Path |
|-----------|------|
| Conceptual parent (canonical) | `layer_1/layer_1_projects/short_ai_workspace_example/` (UUID `cf4d9dcb-a345-4e6f-8272-9a0b1d2c722f`) |
| Deep-tree breadcrumb (navigation marker) | nested inside AI Workspace Example's breadcrumb in the school submodule |

## .0agnostic/ Resources

This entity is freshly created. Resources will be added as portfolio examples and selection tools are developed.

| Resource | Purpose | When to Read |
|----------|---------|--------------|
| `.0agnostic/01_knowledge/examples/` | (planned) Portfolio project case studies, skill-alignment analysis, decision trees | When designing new projects or looking for precedent |
| `.0agnostic/01_knowledge/skills_mapping/` | (planned) How different project types teach which skills | When aligning project choice to learning goals |
| `.0agnostic/02_rules/` | (planned) Entity-specific rules as patterns emerge | TBD as content develops |
| `.0agnostic/05_handoff_documents/` | Cross-session handoffs | Resuming work or onboarding contributors |

## Current Status

**Just created (2026-05-07)**. No content yet. First content priorities (suggestion):

1. A **project selection framework** — decision tree for choosing portfolio projects based on skill gaps, time, and audience
2. **Portfolio project examples** — 3-5 worked examples from AI Society members showing real project choices and why they succeeded
3. **Skill mapping reference** — which skills does each type of project teach (ML projects, systems projects, tools projects, etc.)
4. **Implementation trade-off guide** — for a given portfolio goal, what are 2-3 different implementation approaches and their trade-offs

---

*This is the source of truth for the AI Portfolio Helper entity. Tool-specific files (CLAUDE.md, GEMINI.md, AGENTS.md) are generated from this.*

*Architecture note: this entity uses the **short-path canonical** pattern. Edits go HERE, at the shallow path. The deep-tree breadcrumb is a navigation marker, not a write target.*

## Claude-Specific Rules

### UUID Path Resolution
Paths in this file are resolved at sync time. If a path doesn't exist (entity was renamed/moved since last sync), check the **UUID Reference Index** table in this file for the source UUID. Resolve it to the current path:
```
Grep pattern="THE-UUID" path=".uuid-index.tsv"
```

### MANDATORY: Entity Lookup
For entity discovery, Grep `.entity-lookup.tsv` at the repo root. Each line has: name, UUID, path, parent_UUID (tab-separated). Example: `Grep pattern="portfolio" path=".entity-lookup.tsv"`. Use UUIDs for stable references, paths for file access.

### CLAUDE.md Integration
This file is auto-generated from 0AGNOSTIC.md. Edit 0AGNOSTIC.md to make changes.

---
*Auto-generated tool files (CLAUDE.md, AGENTS.md, GEMINI.md, OPENAI.md) to be created via agnostic-sync.sh*

## Gemini-Specific Notes

### Context Loading
Load detailed resources from .0agnostic/ when needed:
- rules/ - Behavioral constraints
- prompts/ - Task-specific prompts
- knowledge/ - Reference information
- agents/ - Agent definitions

### UUID Path Resolution
Paths in this file are resolved at sync time. If a path doesn't exist (entity was renamed/moved since last sync), check the **UUID Reference Index** table in this file for the source UUID. Resolve it to the current path:
```
Grep pattern="THE-UUID" path=".uuid-index.tsv"
```
The 4th column of the result is the current relative path.

### Session Continuity
Maintain episodic memory in .0agnostic/episodic_memory/:
- sessions/ - Timestamped session records
- changes/ - Divergence and conflict logs
- index.md - Searchable session index

---
*Auto-generated from 0AGNOSTIC.md via agnostic-sync.sh*
*Do not edit directly - edit 0AGNOSTIC.md instead*
