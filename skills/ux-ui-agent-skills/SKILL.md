---
name: ux-ui-agent-skills
description: Initialize UX/UI skill areas, inspect available areas, and retrieve design-system specifications.
---
# UX/UI Agent Skills

## Purpose
Use the `ux-ui-agent-skills` toolkit to bootstrap UX/UI skill areas, inspect available areas, or retrieve a specific design-system specification.

## Source commands
```bash
npx ux-ui-agent-skills init
npx ux-ui-agent-skills add tokens taste design-systems
npx ux-ui-agent-skills list
npx ux-ui-agent-skills library get stripe
```

## When to use
- Use `init` when the user explicitly wants the full kit initialized in the current folder.
- Use `add` when the user wants only selected areas, such as `tokens`, `taste`, or `design-systems`.
- Use `list` to inspect which areas are available.
- Use `library get <name>` to retrieve a particular design-system specification, such as `stripe`.

## Workflow
1. Identify whether the user wants the full kit, selected areas, a catalog listing, or a single design-system spec.
2. Confirm the intended working directory before running initialization or installation commands.
3. Execute only the command matching the user's request, unless they explicitly ask for multiple actions.
4. Inspect command output and use the resulting skill/spec content in the design task.
5. Do not claim installation or retrieval succeeded unless the command actually ran and its output supports that claim.

## Safety and scope
- These commands can modify the current project folder or retrieve external content. Confirm the target folder before `init` or `add`.
- Do not install the full kit when the user requested only selected areas.
- Treat retrieved design-system specs as reference material; adapt them to the project rather than blindly overwriting existing design decisions.
- If terminal access is unavailable, provide the exact command and state that it has not been executed.

## Examples
- Full toolkit: `npx ux-ui-agent-skills init`
- Selected areas: `npx ux-ui-agent-skills add tokens taste design-systems`
- Inspect available areas: `npx ux-ui-agent-skills list`
- Retrieve Stripe spec: `npx ux-ui-agent-skills library get stripe`
