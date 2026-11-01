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
