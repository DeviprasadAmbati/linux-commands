# `git init` - Initialize a Git Repository

## 1. What is `git init`?

`git init` creates a new Git repository inside a directory.

It creates a hidden `.git` directory that stores:

* Git configuration
* Commit history
* Branch information
* Staging information
* Repository metadata

---

## 2. Basic Syntax

```bash
git init
```

---

## 3. Example

Create a project:

```bash
mkdir my-project
cd my-project
```

Initialize Git:

```bash
git init
```

Git will create:

```text
.git/
```

---

## 4. Check Repository Status

After initialization:

```bash
git status
```

---

## 5. Initialize a Repository with a Specific Branch

Modern Git allows:

```bash
git init -b main
```

This initializes the repository with `main` as the initial branch.

---

## 6. Important Note

Do not run `git init` repeatedly inside subdirectories of an existing repository unless you intentionally want a separate repository.

You can check the repository root using:

```bash
git rev-parse --show-toplevel
```

---

## Quick Reference

```bash
git init
git init -b main
git status
git rev-parse --show-toplevel
```

---

## Summary

`git init` converts a normal directory into a Git repository.

