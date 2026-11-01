# Skill Catalog

This catalog lists the skills available in the repository.

## Available skills

- **Find Skills** — Mandatory context-sensitive discovery of relevant skills before starting project work.
  - **Use when:** Before substantive work on a new project, after identifying the user's project context.
  - **File:** `skills/find-skills/SKILL.md`
  - **Source:** `vercel-labs/skills@find-skills`

- **Antigravity Skills Manager** — Install and verify the manager, inspect diagnostics, and list installed skills.
  - **Use when:** Before substantive project implementation in the relevant environment.
  - **File:** `skills/antigravity-skills-manager/SKILL.md`
  - **Package:** `@rmyndharis/antigravity-skills`

- **CodeGraph** — Set up CodeGraph and use the project code graph to inspect code relationships before editing.
  - **Use when:** Before substantive work on an existing codebase.
  - **File:** `skills/codegraph/SKILL.md`
  - **Package:** `@colbymchenry/codegraph`

- **Superpowers** — Install the correct Superpowers plugin for Claude or Antigravity and review its workflow instructions.
  - **Use when:** Before substantive project implementation, after identifying the active coding agent.
  - **File:** `skills/superpowers/SKILL.md`
  - **Upstream:** `obra/superpowers`

- **UI/UX Pro Max** — Install and apply UI/UX Pro Max guidance and existing design-system rules for interface work.
  - **Use when:** Projects involving UI/UX design or frontend interface implementation.
  - **File:** `skills/ui-ux-pro-max/SKILL.md`
  - **Package:** `ui-ux-pro-max-cli`

- **Taste Skill** — Improve frontend art direction, visual design, and interface review with context-sensitive guidance.
  - **Use when:** Projects involving UI/UX or frontend interface implementation.
  - **File:** `skills/taste-skill/SKILL.md`
  - **Source:** `Leonxlnx/taste-skill`

- **Impeccable** — Install and use interface-design guidance for UI construction and refinement.
  - **Use when:** Projects involving UI/UX design or frontend interface work.
  - **File:** `skills/impeccable/SKILL.md`
  - **Install command:** `npx impeccable install`

## Catalog entry format

- **Skill name** — Short description of the capability.
  - **Use when:** situations where this skill is relevant.
  - **File:** `skills/<skill-name>/SKILL.md`
- **UX/UI Agent Skills** (`skills/ux-ui-agent-skills/SKILL.md`): initialize the full UX/UI toolkit, add selected areas, list available areas, or fetch a design-system spec such as Stripe.
- **Apple Design Skill** (`skills/apple-design-skill/SKILL.md`): review an already-implemented UI against Apple design guidance; use after the UI exists, not to generate a new UI.
- **AntiSlop AI** (`skills/antislop-ai/SKILL.md`): filter generic AI-generated UI, copy, and code; can guide work during implementation or audit existing output afterward.
- **Ponytail** (`skills/ponytail/SKILL.md`): minimize unnecessary code while maintaining completeness, validation, security, and quality; includes install guidance and agent-specific notes.
