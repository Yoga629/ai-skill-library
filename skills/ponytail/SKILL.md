# Ponytail

## Purpose
A coding skill/plugin that encourages the smallest complete implementation: reuse existing patterns, avoid unnecessary code and dependencies, and preserve validation, security, and tests.

## Install command
For the Skills CLI:
```bash
npx skills add DietrichGebert/ponytail
```

## When to use
Use for coding tasks where scope control and avoiding over-engineering matter: implementation, bug fixes, refactoring, code review, or dependency decisions.

## Workflow
1. Choose installation for the user's agent. The Skills CLI is one option; the upstream repository also documents agent-specific plugin installation.
2. For Skills CLI installation, run:
   ```bash
   npx skills add DietrichGebert/ponytail
   ```
3. If the agent is already running, start a new session so it can load the added skills.
4. Use the main Ponytail skill for implementation guidance, or invoke the repository's relevant review/audit skills where supported.
5. Keep security, trust-boundary validation, data-loss handling, and accessibility intact. “Less code” is not permission to be negligent.

## Important notes
- The repository includes multiple skills, not only one. The Skills CLI can install the collection; specify `--skill` if only one named skill is desired.
- The install command adds skills; it does not necessarily enable the plugin's always-on rules or lifecycle hooks. Agent-specific plugin installation may be needed for those.
- Review the official install instructions for the target agent before choosing a plugin-specific command.
- Do not claim installation succeeded unless it was actually run and verified.

## Official references
- Repository: https://github.com/DietrichGebert/ponytail
- Install guide: https://github.com/DietrichGebert/ponytail/blob/main/INSTALL.md
