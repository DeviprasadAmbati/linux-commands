# `git push` - Upload Local Commits

## 1. What is `git push`?

`git push` uploads local commits to a remote Git repository.

For example, GitHub is commonly used as a remote repository.

---

## 2. Basic Syntax

```bash
git push remote branch
```

Example:

```bash
git push origin main
```

---

## 3. Understand `origin`

`origin` is commonly the default name assigned to the remote repository when using `git clone`.

Check it with:

```bash
git remote -v
```

---

## 4. Push a New Branch

```bash
git push -u origin feature-branch
```

The `-u` option sets the upstream branch.

After that, you can often use:

```bash
git push
```

---

## 5. Typical Workflow

```bash
git status
git add .
git commit -m "Add documentation"
git push origin main
```

---

## Summary

`git push` uploads local commits to a remote repository.

