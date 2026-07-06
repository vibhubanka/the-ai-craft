<!--
Copy the contents of this file into your local or global AGENTS.md (or CLAUDE.md) file.
I am using this as a global AGENTS.md file with opencode.
-->

# Agent Instructions

## 1. Commit Messages — Conventional Commits

### Format:

- type = feat, fix, build, chore, ci, docs, style, perf, or revert
- scope = file or module if applicable
- description = short description about the change

#### Short format - Regular use for all commits
`<type>[optional scope]: <description>`
Example: `feat(form-update): adds validator functions to MyAppForm`

#### Full format: Use this to verify PR merge commits and when specified.
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

| Type | SemVer Impact |
| :--- | :--- |
| `feat` | `MINOR` |
| `fix` | `PATCH` |
| Any + `!` or `BREAKING CHANGE` footer | `MAJOR` |

## 2. GitHub Work — Use `gh` CLI

Use the `gh` CLI (not raw git remote commands or the web UI) for all GitHub-related work: PRs, issues, repo/workflow status, CI checks, etc.
