# Skill Catalog

This repository contains reusable AI skills for software development, UI/UX design, and quality review.

## Global skill workflow

1. **Find Skills first:** Discover relevant skills based on the user's context and task before starting substantive work.
2. **Ponytail for code:** Apply minimal, complete, maintainable coding practices when writing, editing, debugging, or refactoring code.
3. **Design skills for UI/UX:** Select relevant design skills to guide interface work and reduce generic AI-generated design patterns.
4. **Use skills selectively:** Do not activate every skill blindly. Choose only those relevant to the task.
5. **Apple Design Skill is for review:** Use it after a UI exists. It is not a UI-generation skill.

## Available skills

- **Find Skills** — Discover relevant skills based on the user's task and context.
  - **Use when:** Before substantive project work.
  - **File:** `skills/find-skills/SKILL.md`
  - **Source:** `vercel-labs/skills@find-skills`

- **Antigravity Skills Manager** — Install, diagnose, and inspect skills managed by Antigravity.
  - **Use when:** Working in an Antigravity environment.
  - **File:** `skills/antigravity-skills-manager/SKILL.md`
  - **Package:** `@rmyndharis/antigravity-skills`

- **Graphify** — Build and query persistent knowledge graphs for complex codebases and project corpora.
  - **Use when:** Architecture, cross-file relationships, documentation-to-code links, or repeated structural questions make a graph worthwhile.
  - **File:** `skills/graphify/SKILL.md`
  - **Upstream:** `Graphify-Labs/graphify` (branch `v8`, Apache-2.0).

- **CodeGraph** — Inspect code relationships and project structure.
  - **Use when:** Working on an existing codebase where understanding dependencies matters.
  - **File:** `skills/codegraph/SKILL.md`
  - **Package:** `@colbymchenry/codegraph`

- **Superpowers** — Apply structured software development workflows.
  - **Use when:** Substantive implementation tasks in a supported coding agent.
  - **File:** `skills/superpowers/SKILL.md`
  - **Upstream:** `obra/superpowers`

- **UI/UX Pro Max** — Apply UI/UX guidance and design-system rules.
  - **Use when:** UI/UX design or frontend interface implementation.
  - **File:** `skills/ui-ux-pro-max/SKILL.md`
  - **Package:** `ui-ux-pro-max-cli`

- **Taste Skill** — Improve art direction, visual design, and interface review.
  - **Use when:** UI/UX or frontend work.
  - **File:** `skills/taste-skill/SKILL.md`
  - **Source:** `Leonxlnx/taste-skill`

- **Impeccable** — Refine interface design and frontend implementation.
  - **Use when:** UI/UX design or frontend work.
  - **File:** `skills/impeccable/SKILL.md`
  - **Install command:** `npx impeccable install`

- **UX/UI Agent Skills** — Initialize UX/UI skill areas, list areas, or retrieve design-system specifications.
  - **Use when:** UI/UX workflows requiring reusable design guidance.
  - **File:** `skills/ux-ui-agent-skills/SKILL.md`

- **Apple Design Skill** — Review an existing UI against Apple design guidance.
  - **Use when:** After UI implementation, during review and refinement.
  - **File:** `skills/apple-design-skill/SKILL.md`
  - **Source:** `dickwu/apple-design-skill`

- **AntiSlop AI** — Reduce generic AI-generated UI, copy, and code patterns.
  - **Use when:** During implementation or when auditing existing output.
  - **File:** `skills/antislop-ai/SKILL.md`
  - **Command:** `npx antislop-ai`

- **Ponytail** — Prefer minimal, complete, maintainable code without unnecessary complexity.
  - **Use when:** Writing, editing, debugging, or refactoring code.
  - **File:** `skills/ponytail/SKILL.md`
  - **Source:** `DietrichGebert/ponytail`

## Skill catalog entry format

- **Skill name** — Short description of the capability.
  - **Use when:** Situations where the skill is relevant.
  - **File:** `skills/<skill-name>/SKILL.md`

## Skill authoring template

`SKILL_TEMPLATE.md` is a reusable blueprint for creating new skills. Copy and adapt it into a new skill folder as `SKILL.md`. The template itself is documentation for skill authors, not an automatically activated skill.

## Installation

Install skills from this repository using the Skills CLI:

```bash
npx skills add Yoga629/ai-skill-library
```

List available skills:

```bash
npx skills add Yoga629/ai-skill-library --list
```

Install one specific skill:

```bash
npx skills add Yoga629/ai-skill-library --skill ponytail
```

Each installable `SKILL.md` must contain valid YAML frontmatter with a `name` and `description` at the top of the file.
