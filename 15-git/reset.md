# `git reset` - Move HEAD and Manage Staged Changes

## 1. What is `git reset`?

`git reset` is a powerful command used to move the current branch pointer and modify the staging state.

It has several modes and should be used carefully.

---

## 2. Unstage a File

```bash
git reset HEAD file.md
```

This removes the file from the staging area while keeping the working-file changes.

Modern Git also supports:

```bash
git restore --staged file.md
```

---

## 3. Soft Reset

```bash
git reset --soft HEAD~1
```

This moves `HEAD` back one commit while keeping the changes staged.

---

## 4. Mixed Reset

```bash
git reset HEAD~1
```

This moves `HEAD` back and typically leaves the changes in the working directory unstaged.

---

## 5. Hard Reset

```bash
git reset --hard HEAD~1
```

This moves `HEAD` back and discards tracked working-tree and staging changes that are overwritten by the reset.

⚠️ Use this carefully.

---

## 6. Check Before Resetting

Always inspect:

```bash
git status
git log --oneline
```

---

## Quick Reference

```bash
git reset HEAD file.md
git reset --soft HEAD~1
git reset HEAD~1
git reset --hard HEAD~1
```

---

## Summary

`git reset` is a powerful history and staging-management command. Use destructive modes carefully.

