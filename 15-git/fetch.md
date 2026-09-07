# `git fetch` - Download Remote Changes Without Merging

## 1. What is `git fetch`?

`git fetch` downloads information from a remote repository without changing your current working files.

It updates your remote-tracking branches.

---

## 2. Basic Syntax

```bash
git fetch
```

---

## 3. Fetch from a Specific Remote

```bash
git fetch origin
```

---

## 4. `fetch` vs `pull`

### `git fetch`

```text
Remote
  ↓
Local remote-tracking information
```

It does not automatically merge changes.

### `git pull`

```text
Remote
  ↓
Fetch
  ↓
Merge/Integrate
```

---

## 5. Useful Workflow

```bash
git fetch origin
git log origin/main
```

You can inspect remote changes before deciding how to integrate them.

---

## Summary

`git fetch` downloads remote repository information without automatically merging it into your current branch.

