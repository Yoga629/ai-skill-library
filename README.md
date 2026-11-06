# AI Skill Library

A modular, Markdown-based library of reusable instructions for AI assistants.

## Purpose

This repository contains focused skills that an AI assistant can consult and apply when a task calls for them. Each skill should be self-contained, practical, and explicit about its scope and limitations.

> This repository provides instructions. It does not guarantee that every AI platform will automatically load, execute, or permanently remember them.

## Repository structure

```text
ai-skill-library/
├── README.md
├── SKILL_TEMPLATE.md
├── SKILLS.md
├── CONTRIBUTING.md
├── LICENSE
└── skills/
    └── <skill-name>/
        └── SKILL.md
```

## How to use

1. Browse `SKILLS.md` to find a skill.
2. Open the skill's `SKILL.md`.
3. Provide the file or repository link to an AI assistant that can access it.
4. State the task and explain whether the skill should be applied, adapted, or used as a reference.
5. Review the output. Skills are guidance, not a substitute for judgment or verification.

## Installation

You can install skills from this repository using the [Skills CLI](https://github.com/vercel-labs/skills).

### Install all available skills

```bash
npx skills add Yoga629/ai-skill-library
```

### List available skills

```bash
npx skills add Yoga629/ai-skill-library --list
```

### Install a specific skill

Use the `--skill` option followed by the skill name:

```bash
npx skills add Yoga629/ai-skill-library --skill ponytail
```

For example, to install the UI/UX Pro Max skill:

```bash
npx skills add Yoga629/ai-skill-library --skill ui-ux-pro-max
```

### Installation notes

- Run the command in the project directory where you want to use the skill.
- The Skills CLI may ask you to select an AI coding agent and an installation scope.
- Restart your agent session if necessary so it can load the newly installed skill.
- Not every skill is suitable for every task. Use skills according to their documented purpose and activation conditions.
- Installing a skill does not mean that its instructions have been executed or that its tools have been installed.

For more information, see the [Skills CLI documentation](https://github.com/vercel-labs/skills).

## Design principles

- **Modular:** one skill should solve one recognizable class of tasks.
- **Explicit:** define when to use it and when not to.
- **Actionable:** provide a workflow, not just broad advice.
- **Verifiable:** include quality checks and expected outputs.
- **Portable:** use Markdown and avoid platform-specific assumptions unless documented.
- **Safe:** never include secrets, credentials, or instructions to bypass safeguards.

## Adding a skill

Create a folder under `skills/` and add a `SKILL.md` using `SKILL_TEMPLATE.md`. Then add an entry to `SKILLS.md`.

## Versioning

Use Git history and release tags to track changes. Add a version and changelog to individual skills when their behavior changes substantially.

### UX/UI Agent Skills

Commands and workflow are documented in [`skills/ux-ui-agent-skills/SKILL.md`](skills/ux-ui-agent-skills/SKILL.md).

### Apple Design Skill

A post-implementation UI review skill. See [`skills/apple-design-skill/SKILL.md`](skills/apple-design-skill/SKILL.md).

### AntiSlop AI

A quality filter for AI-generated UI, copy, and code. See [`skills/antislop-ai/SKILL.md`](skills/antislop-ai/SKILL.md).

### Ponytail

A minimal-code / anti-overengineering coding skill. See [`skills/ponytail/SKILL.md`](skills/ponytail/SKILL.md).

## Global skill workflow

Use [`SKILL_WORKFLOW.md`](SKILL_WORKFLOW.md) as the top-level rule for selecting and applying skills. In brief: Find Skills first, Ponytail for code, and relevant design skills for UI/UX quality and avoiding generic AI output.


### Graphify

Graphify provides a Codex-targeted skill and supporting reference files for building and querying persistent knowledge graphs for complex codebases and project corpora. See [`skills/graphify/SKILL.md`](skills/graphify/SKILL.md). The upstream Apache-2.0 license and attribution notice are included in the skill folder.

Install only this skill:

```bash
npx skills add Yoga629/ai-skill-library --skill graphify
```

The skill's workflow may install the Graphify CLI package (`graphifyy`) when needed. Review its instructions before running setup commands. Upstream: https://github.com/Graphify-Labs/graphify (branch `v8`).
