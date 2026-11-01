---
name: apple-design-skill
description: Review an existing UI against Apple design principles; use after implementation, not for UI generation.
---
# Apple Design Skill

## Purpose
Review an already-built UI against Apple design principles and patterns. This skill is for critique and refinement, not for generating a new interface from scratch.

## Install command
```bash
npx skills add dickwu/apple-design-skill
```

## When to use
Use this skill after the UI has been implemented and there is something concrete to review, such as:
- A running app or accessible preview
- Screenshots of the implemented interface
- Existing UI code or a design artifact that can be inspected

Do not activate it as the primary skill when the user is asking to generate a first draft or create a new UI.

## Workflow
1. Confirm that the UI already exists and identify the review target.
2. Inspect the implementation or provided screenshots.
3. Apply the installed skill's review criteria and Apple design guidance.
4. Report specific usability, hierarchy, layout, interaction, and visual consistency issues.
5. Prioritize actionable fixes; avoid vague feedback such as “make it cleaner.”
6. Do not rewrite or regenerate the entire interface unless the user separately requests implementation changes.

## Output expectations
A useful review should include:
- Issue and affected screen/component
- Why it matters to users
- Severity or priority
- Concrete recommended correction

## Scope note
This is a review/critique skill. It does not replace a UI generation or implementation workflow. Only claim that it was run if its instructions were actually loaded and the review was performed.
