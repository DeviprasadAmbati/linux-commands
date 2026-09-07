# `git clone` - Copy a Remote Repository

## 1. What is `git clone`?

`git clone` creates a local copy of a remote Git repository.

It downloads:

* Repository files
* Commit history
* Branch information
* Remote configuration

---

## 2. Basic Syntax

```bash
git clone repository-url
```

---

## 3. Example

```bash
git clone https://github.com/user/project.git
```

Git creates:

```text
project/
```

and downloads the repository into it.

---

## 4. Clone into a Specific Directory

```bash
git clone https://github.com/user/project.git my-project
```

The repository will be placed inside:

```text
my-project/
```

---

## 5. Clone a Specific Branch

```bash
git clone -b branch-name repository-url
```

Example:

```bash
git clone -b develop https://github.com/user/project.git
```

---

## 6. Verify the Remote

After cloning:

```bash
cd project
git remote -v
```

---

## Quick Reference

```bash
git clone URL
git clone URL directory
git clone -b branch-name URL
git remote -v
```

---

## Summary

`git clone` downloads a remote Git repository and creates a local working copy.

