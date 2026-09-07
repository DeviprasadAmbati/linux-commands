# `git commit` - Save Changes to Git History

## 1. What is `git commit`?

`git commit` records staged changes in the Git repository history.

A commit represents a logical checkpoint in your project.

---

## 2. Basic Syntax

```bash
git commit -m "commit message"
```

Example:

```bash
git commit -m "Add networking command documentation"
```

---

## 3. Why Commit Messages Matter

A good commit message explains what changed.

Good:

```text
Add detailed documentation for networking commands
```

Bad:

```text
changes
```

---

## 4. View Commit History

```bash
git log
```

---

## 5. Commit Workflow

```bash
git status
git add file.md
git commit -m "Add file documentation"
```

---

## Quick Reference

```bash
git add .
git commit -m "Describe the change"
git log
```

---

## Summary

`git commit` creates a permanent checkpoint containing staged changes.

