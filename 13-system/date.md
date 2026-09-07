# `date` - Display or Format Date and Time

## 1. What is `date`?

The `date` command displays the current system date and time.

It can also format date and time output.

---

## 2. Display Current Date and Time

Run:

```bash
date
```

Example output:

```text
Fri Sep 4 18:00:00 IST 2026
```

---

## 3. Display Date in a Custom Format

Example:

```bash
date +"%Y-%m-%d"
```

Example output:

```text
2026-09-04
```

---

## 4. Common Format Options

| Format | Meaning         |
| ------ | --------------- |
| `%Y`   | Four-digit year |
| `%m`   | Month           |
| `%d`   | Day             |
| `%H`   | Hour            |
| `%M`   | Minutes         |
| `%S`   | Seconds         |

---

## 5. Example Custom Format

```bash
date +"%Y-%m-%d %H:%M:%S"
```

Example:

```text
2026-09-04 18:00:00
```

---

## 6. Display UTC Time

Use:

```bash
date -u
```

This displays the current time in UTC.

---

## Quick Reference

```bash
date
date -u
date +"%Y-%m-%d"
date +"%Y-%m-%d %H:%M:%S"
```

---

## Summary

`date` displays and formats the current system date and time.

