# `git log` - View Commit History

## 1. What is `git log`?

`git log` displays the commit history of a Git repository.

---

## 2. Basic Syntax

```bash
git log
```

---

## 3. Compact History

Use:

```bash
git log --oneline
```

Example:

```text
a8f32ab Add networking documentation
2c7a8d1 Add shell documentation
```

---

## 4. Display Branch Graph

```bash
git log --oneline --graph --all
```

This provides a visual representation of branches and merges.

---

## 5. Show a Specific Number of Commits

```bash
git log -5
```

This displays the latest five commits.

---

## Quick Reference

```bash
git log
git log --oneline
git log --oneline --graph --all
git log -5
```

---

## Summary

`git log` is used to inspect the history of commits in a repository.

