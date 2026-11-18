# Git Tutor

A concise educational guide to Git and GitHub workflows.

## Covered concepts

- Creating and cloning repositories
- Tracking and committing changes
- Push and pull
- Branches
- Forks and pull requests
- Basic collaboration practices

## Status

Completed learning project retained for reference.

## Git learning route: from commands to collaboration

The goal is to understand four states: **working tree → staging area → local commit → remote branch**. Commands operate on different states; this is why `git add`, `git commit` and `git push` are separate actions.

### Everyday commands

| Task | Command | Important distinction |
|---|---|---|
| Inspect | `git status` | First step before any change |
| Stage a reviewed file | `git add README.md` | Does not create a commit |
| See staged differences | `git diff --cached` | Review exactly what will be committed |
| Commit | `git commit -m "docs: explain workflow"` | Local history only |
| Publish branch | `git push -u origin my-branch` | Remote branch, not a merge |
| Inspect history | `git log --oneline` | Read-only exploration |
| Recover safely | `git restore path` | Discards uncommitted edits; preview first |

### Collaboration exercise

On a toy repository, create two branches that modify the same harmless Markdown paragraph. Open a pull request, inspect the conflict and resolve it by preserving both intended meanings. Record what was checked; do not force-push shared history without an explicit team decision.

### How it connects to analytics

A Python reporting script, a synthetic CSV fixture, a QA test and a methodology note should be updated together in a reviewable PR. Never put actual business extracts or credentials in Git.

**RU:** этот репозиторий — введение в модель Git и командный workflow. Для более глубокого обучения и актуальных рекомендаций переходите в основное [Git Collaboration Guide](https://github.com/KonstantinOreshnikov/git-instruction-workshop).

Resources: [Pro Git](https://git-scm.com/book/en/v2) · [GitHub Flow](https://docs.github.com/en/get-started/using-github/github-flow).
