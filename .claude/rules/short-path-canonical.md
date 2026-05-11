# AI Portfolio Helper — Short-Path Canonical Pin

You are inside the **canonical** AI Portfolio Helper entity. This is NOT a launchpad/mirror; this IS the source of truth. Edits go here.

## Canonical (this directory)

```
/home/dawson/dawson-workspace/code/0_layer_universal/layer_1/layer_1_projects/short_ai_portfolio_helper/
```

UUID: `ada4ecf2-3202-4a30-a896-3d85d7f46be0`

## Conceptual parent (also canonical, peer at the same shallow level)

```
/home/dawson/dawson-workspace/code/0_layer_universal/layer_1/layer_1_projects/short_ai_workspace_example/
```

UUID: `cf4d9dcb-a345-4e6f-8272-9a0b1d2c722f`

This entity is a **sub-feature of AI Workspace Example** — pedagogically nested under AI Workspace Example's teaching charter. Inherited rules cascade from AI Workspace Example (and from the school hierarchy via AI Workspace Example's own breadcrumb chain). See this entity's `0AGNOSTIC.md` "Inherited Rules" section.

## Deep-tree breadcrumb (navigation marker, NOT a write target)

```
/home/dawson/dawson-workspace/code/0_layer_universal/layer_1/layer_1_projects/layer_1_project_school/.../layer_4_subx3_feature_ai_workspace_example_breadcrumb/layer_5/layer_5_subx4_features/layer_5_subx4_feature_ai_portfolio_helper_breadcrumb/breadcrumb_0AGNOSTIC.md
```

The breadcrumb is **nested inside the AI Workspace Example breadcrumb**, marking it as a child feature. This makes the conceptual hierarchy visible to anyone browsing the deep school tree: `school → academic_societies → AI Society → AI Workspace Example → AI Portfolio Helper`. Never edit the breadcrumb as if it were canonical.

## Architecture pattern: short-path canonical (experimental)

This entity uses the **short-path entity pattern**, sibling of `short_ai_workspace_example` and `short_sandbox_program`:

| Pattern | Source of truth | Mirror / pointer |
|---------|----------------|------------------|
| **Short-path (this entity)** | **Shallow path here** | **Deep breadcrumb under AI Workspace Example's breadcrumb in the school submodule** (read-only) |

## Repo / commit mechanics

- This canonical lives in the **root repo** (`0_layer_universal`). All canonical edits commit to the root repo.
- The deep-tree breadcrumb lives in the **school submodule** (`Dawson2025/1-school`). Breadcrumb refreshes commit to the school submodule first, then the root repo bumps the submodule pointer.
- Per the **Submodule Integrity Protocol** (root `0AGNOSTIC.md`): commit/push order is bottom-up — school submodule first, then root.
