# `sort` - Sort Lines of Text

## 1. What is `sort`?

The `sort` command is used to arrange lines of text in a specific order.

By default, it sorts alphabetically.

---

## 2. Basic Syntax

```bash
sort FILE_NAME
```

Example:

```bash
sort names.txt
```

---

## 3. Sort in Reverse Order

```bash
sort -r names.txt
```

---

## 4. Sort Numbers

```bash
sort -n numbers.txt
```

Without `-n`, numbers may be sorted alphabetically.

Example:

```text
1
10
2
```

With numeric sorting:

```text
1
2
10
```

---

## 5. Remove Duplicate Lines

```bash
sort -u names.txt
```

The `-u` option sorts and removes duplicate lines.

---

## 6. Sort by a Specific Column

For structured data:

```bash
sort -k 2 data.txt
```

This sorts based on the second column.

---

## 7. Real-World Examples

### Sort names

```bash
sort names.txt
```

### Sort numbers

```bash
sort -n numbers.txt
```

### Sort in reverse

```bash
sort -r names.txt
```

### Find unique sorted values

```bash
sort -u data.txt
```

---

## 8. Save Sorted Output

```bash
sort names.txt > sorted-names.txt
```

This saves the sorted result into a new file.

---

## 9. Related Commands

| Command | Purpose                |
| ------- | ---------------------- |
| `sort`  | Sort lines             |
| `uniq`  | Handle duplicate lines |
| `grep`  | Search text            |
| `wc`    | Count lines            |

---

## Practice Exercises

1. Create a file containing names.
2. Sort the names alphabetically.
3. Sort in reverse order.
4. Create a file containing numbers.
5. Sort using `-n`.
6. Remove duplicates using `-u`.

---

## Quick Reference

```bash
sort file.txt
sort -r file.txt
sort -n numbers.txt
sort -u file.txt
sort -k 2 data.txt
```

---

## Summary

`sort` arranges lines of text.

Most useful options:

```bash
sort file.txt
sort -n numbers.txt
sort -r file.txt
sort -u file.txt
```

