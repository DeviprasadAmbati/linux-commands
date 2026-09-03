# `who` - Display Logged-In Users

## 1. What is `who`?

The `who` command displays information about users currently logged into the system.

---

## 2. Basic Syntax

```bash
who
```

---

## 3. Example Output

Example:

```text
deviprasad pts/0 2026-09-03 10:30
```

This can include:

* Username.
* Terminal.
* Login time.

---

## 4. Useful Options

### Display Current Runlevel

```bash
who -r
```

### Display All Available Information

```bash
who -a
```

---

## 5. Related Commands

| Command  | Purpose                   |
| -------- | ------------------------- |
| `who`    | Logged-in users           |
| `whoami` | Current user              |
| `w`      | Users and activity        |
| `id`     | User identity information |

---

## Practice Exercises

```bash
who
who -a
whoami
```

---

## Summary

`who` shows users currently logged into the system.

