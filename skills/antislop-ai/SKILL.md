---
name: antislop-ai
description: Reduce generic AI-generated UI, copy, and code patterns during implementation or review.
---
# AntiSlop AI

## Purpose
Filter generic AI-generated UI, copy, and code patterns. This is a quality filter, not a replacement for the project's visual direction or design system.

## Install command
```bash
npx antislop-ai
```

## When to use
- While building a website, web app, or interface to guide the work away from generic AI output.
- After implementation to audit existing UI, text, or code and produce actionable findings.

## Workflow
1. Run the installer in the intended project directory and choose the relevant agent, install scope, and optional skill areas.
2. Start a new agent session after installation so the rules can load.
3. Resolve the usage mode:
   - **During:** guide implementation and conclude with a delivery-gate report.
   - **After:** audit existing work, list findings, let the user choose what to fix, then report results.
4. Apply only relevant rules and preserve intentional project-specific design decisions.
5. Report what changed or what was found; never claim the filter was active unless it was actually loaded.

## Optional commands
```bash
npx antislop-ai --mode during
npx antislop-ai --mode after
npx antislop-ai --mode ask
npx antislop-ai --update
```

## Safety and scope
- Installation can write skill folders and a pointer into the current project or user-level configuration. Confirm scope and target directory first.
- Do not choose or install optional skill areas without user authorization.
- Treat this as a filter, not a substitute for an authored design system, accessibility review, or product requirements.
- If terminal execution is unavailable, give the user the command and clearly state it has not been run.

## References
- Project repository: https://github.com/miqdadbadjuber/anti-slop
- Usage modes and install behavior: https://github.com/miqdadbadjuber/anti-slop/blob/main/GUIDE.md
