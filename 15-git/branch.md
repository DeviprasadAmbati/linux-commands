# `git branch` - Manage Branches

## 1. What is a Git Branch?

A branch is an independent line of development.

It allows developers to work on features without directly modifying another branch.

---

## 2. List Branches

```bash
git branch
```

---

## 3. Create a Branch

```bash
git branch feature-login
```

---

## 4. Delete a Local Branch

```bash
git branch -d feature-login
```

---

## 5. Force Delete a Branch

```bash
git branch -D feature-login
```

Use this carefully because it can delete a branch containing commits that have not been merged.

---

## 6. List Remote Branches

```bash
git branch -r
```

---

## 7. List All Branches

```bash
git branch -a
```

---

## Quick Reference

```bash
git branch
git branch feature-name
git branch -d feature-name
git branch -D feature-name
git branch -a
```

---

## Summary

`git branch` is used to create, inspect, and delete Git branches.

