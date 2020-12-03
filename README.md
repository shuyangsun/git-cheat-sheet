# Git Cheat Sheet

Alternative resources:
- [PDF version by Atlassian](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet).
- [PDF version by Githun](https://education.github.com/git-cheat-sheet-education.pdf)

## User Configuration

To configure global user:

```bash
$ git config --global user.name "your name"
$ git config --global user.email "your@email.com"
```

To configure user for specific repo, remove the `--global` flag.

## Diff
| Command | Description |
| - | - |
| `git show COMMIT` | Show diff in commit. |

## Stash

| Command | Description |
| - | - |
| `git stash push -m "message"` | Stash changes with name "message". |
| `git stash list` | List all stashes by index. |
| `git stash apply stash@{n}` | Apply stash at index `n` and keep it in the stash. |
| `git stash pop stash@{n}` | Apply stash at index `n` and remove it from the stash. |
| `git stash drop stash@{n}` | Drop stash at index `n`, remaining stashes' indices are shifted up by one. |
