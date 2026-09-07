# `git stash` - Temporarily Save Changes

## 1. What is `git stash`?

`git stash` temporarily saves uncommitted changes so that you can work on a clean working directory.

It is useful when you need to switch branches without committing unfinished work.

---

## 2. Save Current Changes

```bash
git stash
```

---

## 3. View Stashed Changes

```bash
git stash list
```

---

## 4. Apply the Latest Stash

```bash
git stash apply
```

This restores the changes but keeps the stash entry.

---

## 5. Apply and Remove the Stash

```bash
git stash pop
```

This applies the latest stash and removes it if the operation succeeds.

---

## 6. Create a Named Stash

```bash
git stash push -m "Work in progress"
```

---

## 7. Delete a Stash

```bash
git stash drop
```

---

## 8. Example Workflow

You are working on a feature:

```bash
git status
```

You need to switch branches:

```bash
git stash
git switch main
```

Later:

```bash
git switch feature-login
git stash pop
```

---

## Quick Reference

```bash
git stash
git stash list
git stash apply
git stash pop
git stash push -m "message"
git stash drop
```

---

## Summary

`git stash` temporarily stores uncommitted changes so you can work with a clean working directory.

