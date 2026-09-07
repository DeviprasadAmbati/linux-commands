# `git pull` - Download and Integrate Remote Changes

## 1. What is `git pull`?

`git pull` retrieves changes from a remote repository and integrates them into the current local branch.

Conceptually, it performs:

```text
git fetch
   +
git merge
```

in the common case.

---

## 2. Basic Syntax

```bash
git pull
```

---

## 3. Pull from a Specific Remote Branch

```bash
git pull origin main
```

---

## 4. Why Use `git pull`?

Use it when changes have been pushed to GitHub and you want to update your local repository.

---

## 5. Typical Workflow

```bash
git status
git pull origin main
```

Then continue working.

---

## 6. Important Note

If you have local changes that conflict with incoming changes, Git may stop and require you to resolve the situation.

Always check:

```bash
git status
```

---

## Summary

`git pull` downloads remote changes and integrates them into your current branch.

