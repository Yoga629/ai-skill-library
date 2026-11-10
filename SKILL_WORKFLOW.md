# Global Skill Usage Rules

These rules govern how skills in this repository are selected and used across tasks.

## Required order

### 1. Find Skills first
Start each substantial task by using **Find Skills** to identify skills relevant to the user's goal and context.

- Match skills to the actual task, stack, and deliverable.
- Prefer a small set of relevant skills over loading the entire library.
- If Find Skills cannot be executed in the current environment, disclose that limitation and use the catalog manually; do not claim the search was run.

### 2. Ponytail for code
When writing, editing, debugging, or refactoring code, apply **Ponytail** as the coding discipline.

- Prefer the smallest complete solution.
- Reuse existing project patterns and dependencies where reasonable.
- Avoid unnecessary abstractions, dependencies, boilerplate, and speculative features.
- Do not sacrifice correctness, security, validation, accessibility, or maintainability for fewer lines.

### 3. Design skills for UI/UX
For interface design and frontend presentation, select relevant design skills from the library to guide the work and avoid generic AI-generated design (“AI slop”).

- Use **UI/UX Pro Max**, **Taste Skill**, **Impeccable**, and/or **UX/UI Agent Skills** when their documented scope fits the task.
- Do not blindly apply every design skill. Resolve overlap and conflicts in favor of the user's requirements, the existing design system, accessibility, and a coherent visual direction.
- Apply design guidance during generation/implementation when appropriate.
- Use **Apple Design Skill only after a UI exists**, as a review/critique skill; it is not a UI generator.
- Use **AntiSlop AI** as an additional quality filter when installed and relevant. Do not claim it is active unless its instructions were actually loaded.

## Task-specific skills

After Find Skills, select additional skills only when they materially help the task.

- **Graphify:** For large or unfamiliar codebases, architecture questions, cross-file relationships, or repeated queries over the same project corpus, check for an existing `graphify-out/graph.json` first. Query an existing graph before rebuilding. For a simple one-off lookup, use targeted search/read instead of building a graph.
- **CodeGraph:** Use when its project code-relationship analysis fits the repository and task.
- **BrowserAct:** Use for user-requested local browser automation, JavaScript-rendered page inspection, or browser interaction where the user has authorized access. Load its skill before running BrowserAct commands; install the CLI only when needed and with the user's awareness.
- **BrowserAct Skill Forge:** Use when the user asks to create a reusable, website-specific Skill. It depends on BrowserAct. Do not use it for a one-off page lookup.
- **Other specialized skills:** Use only when their documented scope fits, such as retrieving a design-system specification or running a post-implementation UI review.

For BrowserAct tasks, do not bypass authentication, access controls, paywalls, CAPTCHAs, rate limits, or other technical restrictions. Require confirmation before consequential browser actions (form submissions, messages, uploads, purchases, account changes, or deletions). Do not expose credentials, cookies, or session tokens.

When coding is involved, apply Ponytail to the implementation after the relevant discovery and inspection steps.

## Execution and honesty
- A documented command is not the same as an installed or executed skill.
- Never claim a skill was loaded, installed, run, or verified unless that actually happened.
- If a skill or terminal is unavailable, state the limitation briefly and provide a practical fallback.
- Confirm the target project directory before commands that modify files or configuration.
- Keep the final output focused on the user's requested deliverable and meaningful findings.
