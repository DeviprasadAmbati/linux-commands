# `uniq` - Filter Repeated Lines

## 1. What is `uniq`?

The `uniq` command removes or reports repeated adjacent lines.

An important point is that `uniq` works best with sorted input because duplicate lines must normally be next to each other.

---

## 2. Basic Syntax

```bash
uniq file.txt
```

---

## 3. Remove Duplicate Lines

A common approach is:

```bash
sort file.txt | uniq
```

Or simply:

```bash
sort -u file.txt
```

---

## 4. Count Duplicate Lines

Use:

```bash
uniq -c file.txt
```

Example:

```text
2 Apple
3 Banana
1 Orange
```

---

## 5. Display Only Duplicate Lines

Use:

```bash
uniq -d file.txt
```

---

## 6. Display Only Unique Lines

Use:

```bash
uniq -u file.txt
```

---

## Quick Reference

```bash
uniq file.txt
sort file.txt | uniq
uniq -c file.txt
uniq -d file.txt
uniq -u file.txt
```

---

## Summary

`uniq` is used to identify or remove repeated adjacent lines.

