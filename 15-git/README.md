# Git Commands

A quick reference for commonly used Git commands.

| Command                                    | Short Description                                       |
| ------------------------------------------ | ------------------------------------------------------- |
| `git init`                                 | Initialize a new Git repository                         |
| `git clone <url>`                          | Clone a remote repository                               |
| `git status`                               | Show the current repository status                      |
| `git add <file>`                           | Stage a specific file                                   |
| `git add .`                                | Stage changes in the current directory                  |
| `git add -A`                               | Stage all changes in the repository                     |
| `git commit -m "message"`                  | Create a commit with a message                          |
| `git push`                                 | Push local commits to a remote repository               |
| `git pull`                                 | Fetch and integrate changes from a remote repository    |
| `git fetch`                                | Download changes from a remote without integrating them |
| `git branch`                               | List or manage branches                                 |
| `git branch <name>`                        | Create a new branch                                     |
| `git branch -d <name>`                     | Delete a local branch                                   |
| `git checkout <branch>`                    | Switch to another branch                                |
| `git checkout -b <name>`                   | Create and switch to a new branch                       |
| `git switch <branch>`                      | Switch to another branch                                |
| `git switch -c <name>`                     | Create and switch to a new branch                       |
| `git merge <branch>`                       | Merge another branch into the current branch            |
| `git log`                                  | Show commit history                                     |
| `git log --oneline`                        | Show compact commit history                             |
| `git diff`                                 | Show unstaged changes                                   |
| `git diff --staged`                        | Show staged changes                                     |
| `git remote -v`                            | Show configured remote repositories                     |
| `git remote add origin <url>`              | Add a remote repository                                 |
| `git remote remove <name>`                 | Remove a remote repository                              |
| `git remote rename <old> <new>`            | Rename a remote repository                              |
| `git reset <file>`                         | Unstage a file                                          |
| `git reset --soft HEAD~1`                  | Undo the last commit but keep changes staged            |
| `git reset --mixed HEAD~1`                 | Undo the last commit and unstage changes                |
| `git reset --hard HEAD~1`                  | Undo the last commit and discard changes                |
| `git stash`                                | Temporarily save uncommitted changes                    |
| `git stash list`                           | List saved stashes                                      |
| `git stash pop`                            | Apply and remove the latest stash                       |
| `git stash apply`                          | Apply a stash without removing it                       |
| `git stash drop`                           | Delete a stash                                          |
| `git show`                                 | Show details of a commit                                |
| `git tag`                                  | List Git tags                                           |
| `git tag <name>`                           | Create a Git tag                                        |
| `git rm <file>`                            | Remove a file and stage the deletion                    |
| `git mv <old> <new>`                       | Move or rename a file and stage the change              |
| `git restore <file>`                       | Restore a file from the last commit                     |
| `git restore --staged <file>`              | Unstage a file                                          |
| `git config --list`                        | Show Git configuration                                  |
| `git config --global user.name "<name>"`   | Set global Git username                                 |
| `git config --global user.email "<email>"` | Set global Git email                                    |
| `git help <command>`                       | Show help for a Git command                             |

## Common Git Workflow

```bash
git status
git add .
git commit -m "Your commit message"
git push origin main
```

## Branch Workflow

```bash
git branch
git switch -c feature-name
git add .
git commit -m "Add feature"
git switch main
git merge feature-name
git push origin main
```

## Remote Workflow

```bash
git remote -v
git fetch
git pull
git push
```

