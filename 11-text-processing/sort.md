# `sort` - Sort Lines of Text

## 1. What is `sort`?

The `sort` command arranges lines of text in a specific order.

By default, it sorts alphabetically.

---

## 2. Basic Syntax

```bash
sort file.txt
```

---

## 3. Sort in Reverse Order

```bash
sort -r file.txt
```

---

## 4. Sort Numerically

```bash
sort -n numbers.txt
```

Without `-n`, numbers may be sorted alphabetically instead of numerically.

---

## 5. Sort and Remove Duplicates

Use:

```bash
sort -u file.txt
```

---

## 6. Sort by a Specific Column

Example:

```bash
sort -k 2 file.txt
```

This sorts based on the second field.

---

## 7. Human-Readable Number Sorting

For values such as:

```text
1K
20M
2G
```

Use:

```bash
sort -h file.txt
```

---

## Quick Reference

```bash
sort file.txt
sort -r file.txt
sort -n numbers.txt
sort -u file.txt
sort -k 2 file.txt
sort -h file.txt
```

---

## Summary

`sort` organizes text lines alphabetically, numerically, or based on specific fields.

