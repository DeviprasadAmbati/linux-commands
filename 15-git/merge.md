# `git merge` - Combine Branches

## 1. What is `git merge`?

`git merge` combines the changes from one branch into another branch.

---

## 2. Basic Workflow

Suppose you have:

```text
main
feature-login
```

Switch to `main`:

```bash
git switch main
```

Merge the feature:

```bash
git merge feature-login
```

---

## 3. Example

```bash
git switch main
git merge feature-login
```

Git attempts to combine the histories.

---

## 4. Merge Conflicts

A conflict can occur when Git cannot automatically combine changes.

Check:

```bash
git status
```

Git will identify conflicted files.

After resolving the conflict:

```bash
git add resolved-file
git commit
```

---

## 5. Abort a Merge

If you want to cancel an in-progress merge:

```bash
git merge --abort
```

---

## Quick Reference

```bash
git switch main
git merge feature-branch
git merge --abort
```

---

## Summary

`git merge` combines the history and changes of one branch into another.

