# `tail` - Display the End of a File

## 1. What is `tail`?

The `tail` command displays the last part of a file.

By default, it displays the last 10 lines.

---

## 2. Basic Syntax

```bash
tail file.txt
```

---

## 3. Display a Specific Number of Lines

```bash
tail -n 5 file.txt
```

---

## 4. Follow a File in Real Time

Use:

```bash
tail -f application.log
```

This is extremely useful for monitoring log files.

As new lines are added, they appear in the terminal.

Stop with:

```text
Ctrl + C
```

---

## 5. Real-World Example

Monitor a web server log:

```bash
tail -f /var/log/nginx/access.log
```

---

## Quick Reference

```bash
tail file.txt
tail -n 5 file.txt
tail -f application.log
```

---

## Summary

`tail` displays the end of a file and can monitor files in real time.

