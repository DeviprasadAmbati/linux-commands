# `git add` - Stage Changes

## 1. What is `git add`?

`git add` moves changes from the working directory into the staging area.

Git has three important areas:

```text
Working Directory
       ↓
    git add
       ↓
Staging Area
       ↓
  git commit
       ↓
Repository
```

---

## 2. Add a Specific File

```bash
git add README.md
```

---

## 3. Add a Directory

```bash
git add 15-git/
```

---

## 4. Add All Changes

```bash
git add .
```

This stages changes under the current directory.

---

## 5. Check Staged Changes

```bash
git status
```

---

## 6. Unstage a File

```bash
git restore --staged README.md
```

This removes the file from staging without deleting its changes.

---

## Quick Reference

```bash
git add file
git add directory/
git add .
git restore --staged file
```

---

## Summary

`git add` prepares changes for the next commit by placing them in the staging area.

