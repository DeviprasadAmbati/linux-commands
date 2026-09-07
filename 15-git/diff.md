# `git diff` - Compare Changes

## 1. What is `git diff`?

`git diff` displays differences between versions of files.

It is useful for reviewing changes before committing.

---

## 2. Check Unstaged Changes

```bash
git diff
```

This compares your working directory with the staging area.

---

## 3. Check Staged Changes

```bash
git diff --staged
```

This shows changes that will be included in the next commit.

---

## 4. Compare Two Commits

```bash
git diff commit1 commit2
```

---

## 5. Why Use `git diff`?

Before committing, you can run:

```bash
git diff
git diff --staged
```

to verify that you are committing the intended changes.

---

## Quick Reference

```bash
git diff
git diff --staged
git diff commit1 commit2
```

---

## Summary

`git diff` helps you inspect differences between working files, staged changes, commits, and branches.

