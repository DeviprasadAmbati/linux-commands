# `head` - Display the Beginning of a File

## 1. What is `head`?

The `head` command displays the first lines of a file.

By default, it displays the first **10 lines**.

---

## 2. Basic Syntax

```bash
head FILE_NAME
```

Example:

```bash
head notes.txt
```

---

## 3. Display Specific Number of Lines

```bash
head -n 5 notes.txt
```

Displays the first 5 lines.

---

## 4. Display Multiple Files

```bash
head file1.txt file2.txt
```

---

## 5. Real-World Examples

### View the first lines of a log

```bash
head application.log
```

### View the first 20 lines

```bash
head -n 20 application.log
```

### Check a CSV file header

```bash
head data.csv
```

---

## 6. Related Commands

| Command | Purpose           |
| ------- | ----------------- |
| `head`  | Beginning of file |
| `tail`  | End of file       |
| `cat`   | Entire file       |
| `less`  | Paginated view    |

---

## Practice Exercises

1. Create a file with more than 10 lines.
2. Run `head file.txt`.
3. Run `head -n 5 file.txt`.
4. Compare the output with `tail`.

---

## Quick Reference

```bash
head file.txt
head -n 5 file.txt
head -n 20 file.txt
```

---

## Summary

`head` displays the beginning of a file.

Default:

```bash
head file.txt
```

shows the first 10 lines.

