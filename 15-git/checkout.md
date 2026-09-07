# `git checkout` - Switch Branches and Restore Files

## 1. What is `git checkout`?

`git checkout` is an older, multi-purpose Git command.

It can be used to:

* Switch branches
* Create and switch branches
* Restore files from previous commits

---

## 2. Switch Branch

```bash
git checkout main
```

---

## 3. Create and Switch to a Branch

```bash
git checkout -b feature-login
```

---

## 4. Restore a File

Older Git workflows may use:

```bash
git checkout -- README.md
```

Modern Git provides clearer commands such as:

```bash
git restore README.md
```

---

## 5. Why Learn `checkout`?

You will encounter it frequently in existing Git documentation and repositories.

However, modern Git separates its responsibilities between:

```bash
git switch
git restore
```

---

## Summary

`git checkout` can switch branches and restore files, but modern Git provides more specialized commands.

