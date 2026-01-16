---
name: git-commit
description: Write git commit messages following the Conventional Commits specification
license: MIT
compatibility: opencode
metadata:
  category: git
  workflow: version-control
---

## What I do

- Format commit messages using Conventional Commits syntax
- Select the appropriate commit type for each change
- Write clear, imperative subject lines

## Commit format

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

## Allowed types

| Type | Purpose |
|------|---------|
| feat | New feature |
| fix | Bug fix |
| docs | Documentation only |
| style | Formatting, no code change |
| refactor | Code change that neither fixes nor adds |
| test | Adding or updating tests |
| chore | Maintenance, dependencies, config |

## Rules

- Subject line must be 72 characters or less
- Use imperative mood: "add" not "added" or "adds"
- No period at the end of the subject line
- Separate subject from body with a blank line
- Wrap body at 72 characters

## Breaking changes


Indicate breaking changes by adding `!` after the type/scope:

```
feat(api)!: change authentication response format
```

Include `BREAKING CHANGE:` in the footer.

## Examples

```
feat(auth): add OAuth2 login support

fix(parser): handle empty input gracefully

docs: update installation instructions

refactor(api)!: rename user endpoints

BREAKING CHANGE: /users/:id is now /user/:id
```

## When to use me

Use this skill when committing changes to ensure consistent, meaningful commit history that supports automated changelogs and semantic versioning.
