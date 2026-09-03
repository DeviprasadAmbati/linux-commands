# `find` - Search for Files and Directories

## 1. What is `find`?

The `find` command searches for files and directories.

Unlike `grep`, which searches inside file contents, `find` searches for files based on properties such as:

* Name.
* Type.
* Size.
* Permissions.
* Modification time.

---

## 2. Basic Syntax

```bash
find PATH OPTIONS
```

Example:

```bash
find . -name "file.txt"
```

This searches the current directory and subdirectories.

---

## 3. Search by File Name

```bash
find . -name "notes.txt"
```

---

## 4. Case-Insensitive Search

```bash
find . -iname "notes.txt"
```

This can match different letter cases.

---

## 5. Find Directories

```bash
find . -type d
```

---

## 6. Find Files

```bash
find . -type f
```

---

## 7. Find Files by Extension

```bash
find . -name "*.txt"
```

The quotes prevent the shell from expanding the wildcard before `find` receives it.

---

## 8. Find Files by Size

```bash
find . -size +100M
```

Finds files larger than 100 MB.

---

## 9. Find Recently Modified Files

```bash
find . -mtime -7
```

Finds files modified within approximately the last 7 days.

---

## 10. Real-World Examples

### Find Python files

```bash
find . -name "*.py"
```

### Find directories

```bash
find . -type d
```

### Find large files

```bash
find /home -size +500M
```

Permission errors may occur depending on your access rights.

---

## 11. Common Mistakes

### Mistake: Confusing `find` and `grep`

```text
find → Searches for files and directories

grep → Searches inside text
```

---

## Practice Exercises

1. Find all `.txt` files.
2. Find all `.py` files.
3. Find directories.
4. Find regular files.
5. Find files larger than a chosen size.
6. Find recently modified files.

---

## Quick Reference

```bash
find . -name "file.txt"
find . -iname "FILE.TXT"
find . -type f
find . -type d
find . -name "*.txt"
find . -size +100M
find . -mtime -7
```

---

## Summary

`find` is a powerful command for searching files and directories based on different conditions.

