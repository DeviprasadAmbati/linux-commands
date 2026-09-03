# `whoami` - Display the Current User

## 1. What is `whoami`?

The `whoami` command displays the username of the user currently running the command.

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

It is useful when:

* Working with multiple users.
* Using `sudo`.
* Working on remote servers.
* Checking which account is currently active.

---

## 4. Example with `sudo`

You may run:

```bash
whoami
```

and see:

```text
deviprasad
```

But:

```bash
sudo whoami
```

may output:

```text
root
```

This shows that the command is running with elevated privileges.

---

## 5. Related Commands

| Command  | Purpose                    |
| -------- | -------------------------- |
| `whoami` | Current username           |
| `who`    | Logged-in users            |
| `id`     | User and group information |
| `groups` | User groups                |

---

## Practice Exercises

1. Run:

```bash
whoami
```

2. Run:

```bash
id
```

3. Compare the results.

---

## Quick Reference

```bash
whoami
sudo whoami
```

---

## Summary

Use:

```bash
whoami
```

to quickly identify the current user.

