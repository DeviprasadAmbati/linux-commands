# `who` - Display Logged-In Users

## 1. What is `who`?

The `who` command displays information about users currently logged into the system.

---

## 2. Basic Syntax

```bash
who
```

Example output:

```text
deviprasad tty1 2026-09-04 10:00
user2      pts/0 2026-09-04 11:30
```

---

## 3. Understanding the Output

The output may contain:

| Information | Meaning                 |
| ----------- | ----------------------- |
| Username    | Logged-in user          |
| Terminal    | Terminal session        |
| Login time  | When the user logged in |

---

## 4. Display Additional Information

Use:

```bash
who -a
```

This displays more detailed information.

---

## 5. Check Current User

If you only want your current username, use:

```bash
whoami
```

---

## Quick Reference

```bash
who
who -a
whoami
```

---

## Summary

`who` displays information about users currently logged into the Linux system.

