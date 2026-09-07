# `git status` - Check Repository State

## 1. What is `git status`?

`git status` shows the current state of your Git repository.

It tells you:

* Current branch
* Modified files
* New files
* Deleted files
* Staged files
* Untracked files

---

## 2. Basic Syntax

```bash
git status
```

---

## 3. Example

```bash
git status
```

Possible output:

```text
On branch main

Changes not staged for commit:
  modified: README.md

Untracked files:
  notes.md
```

---

## 4. Why Use `git status`?

It is one of the most important Git commands.

Before running:

```bash
git add
git commit
git push
```

you should usually check:

```bash
git status
```

---

## Quick Reference

```bash
git status
git status --short
```

---

## Summary

`git status` tells you what has changed in your working directory and staging area.

