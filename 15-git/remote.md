# `git remote` - Manage Remote Repositories

## 1. What is `git remote`?

`git remote` manages connections between your local repository and remote repositories such as GitHub.

---

## 2. Display Remotes

```bash
git remote
```

---

## 3. Display Remote URLs

```bash
git remote -v
```

Example:

```text
origin  https://github.com/user/project.git (fetch)
origin  https://github.com/user/project.git (push)
```

---

## 4. Add a Remote

```bash
git remote add origin https://github.com/user/project.git
```

---

## 5. Remove a Remote

```bash
git remote remove origin
```

---

## 6. Change a Remote URL

```bash
git remote set-url origin https://github.com/user/new-project.git
```

---

## Quick Reference

```bash
git remote
git remote -v
git remote add origin URL
git remote remove origin
git remote set-url origin URL
```

---

## Summary

`git remote` manages the connection between a local Git repository and remote repositories.

