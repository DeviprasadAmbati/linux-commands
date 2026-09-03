# `du` - Display Directory Disk Usage

## 1. What is `du`?

`du` stands for **Disk Usage**.

The `du` command calculates how much disk space is used by files and directories.

While `df` shows filesystem-level disk usage, `du` helps identify which directories are using space.

---

## 2. Basic Syntax

```bash
du directory
```

Example:

```bash
du /home
```

---

## 3. Human-Readable Output

Use:

```bash
du -h directory
```

Example:

```bash
du -h /var/log
```

---

## 4. Display Only the Total Size

Use:

```bash
du -sh directory
```

Example:

```bash
du -sh /home/deviprasad
```

Explanation:

```text
-s → Summary
-h → Human-readable format
```

---

## 5. Check All Directories in the Current Location

```bash
du -sh *
```

This is useful for finding large directories.

---

## 6. Sort Directories by Size

You can combine `du` with `sort`:

```bash
du -sh * | sort -h
```

This displays directories ordered by size.

---

## 7. Real-World Example

If your disk is almost full:

First check:

```bash
df -h
```

Then identify large directories:

```bash
du -sh /var/*
```

---

## 8. Quick Reference

```bash
du directory
du -h directory
du -sh directory
du -sh *
du -sh * | sort -h
```

---

## Summary

`du` helps you identify how much disk space files and directories are using.

The most commonly used command is:

```bash
du -sh directory
```

