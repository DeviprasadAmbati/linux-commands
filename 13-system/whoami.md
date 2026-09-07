# `whoami` - Display the Current User

## 1. What is `whoami`?

The `whoami` command displays the username of the current effective user.

---

## 2. Basic Syntax

```bash
whoami
```

Example output:

```text
deviprasad
```

---

## 3. Why Use `whoami`?

It is useful when you want to confirm:

* Which user is currently active
* Whether you are running as `root`
* Which account is executing a script

---

## 4. Example with `sudo`

Normally:

```bash
whoami
```

might display:

```text
deviprasad
```

But inside a root shell, it may display:

```text
root
```

---

## 5. Related Commands

You can also use:

```bash
id -un
```

to display the effective username.

---

## Quick Reference

```bash
whoami
id -un
```

---

## Summary

`whoami` displays the username of the current effective user.

