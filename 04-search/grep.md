# `grep` - Search Text Using Patterns

## 1. What is `grep`?

`grep` is used to search for text patterns inside files or command output.

It is one of the most important Linux commands for searching logs, files, and text.

---

## 2. Basic Syntax

```bash
grep "PATTERN" FILE_NAME
```

Example:

```bash
grep "error" application.log
```

This displays lines containing the word `error`.

---

## 3. Important Options

### `-i` - Ignore Case

```bash
grep -i "error" application.log
```

Matches:

```text
error
ERROR
Error
```

---

### `-n` - Show Line Numbers

```bash
grep -n "error" application.log
```

---

### `-v` - Show Non-Matching Lines

```bash
grep -v "error" application.log
```

---

### `-r` - Recursive Search

```bash
grep -r "password" .
```

Searches through files inside the current directory and subdirectories.

---

### `-c` - Count Matching Lines

```bash
grep -c "error" application.log
```

---

## 4. Search Command Output

```bash
ls -la | grep ".txt"
```

This filters output to show lines containing `.txt`.

---

## 5. Real-World Examples

### Search application errors

```bash
grep "ERROR" application.log
```

### Search case-insensitively

```bash
grep -i "error" application.log
```

### Search recursively

```bash
grep -r "database_url" .
```

### Count errors

```bash
grep -c "ERROR" application.log
```

---

## 6. Common Mistakes

### Mistake: Case Sensitivity

```bash
grep "error" file.txt
```

does not necessarily match:

```text
ERROR
```

Use:

```bash
grep -i "error" file.txt
```

---

## 7. Related Commands

| Command  | Purpose            |
| -------- | ------------------ |
| `grep`   | Search text        |
| `find`   | Search files       |
| `locate` | Find indexed files |
| `wc`     | Count lines        |

---

## Practice Exercises

1. Create a file containing different words.
2. Search for a word.
3. Use `-i`.
4. Use `-n`.
5. Use `-v`.
6. Search recursively.

---

## Quick Reference

```bash
grep "word" file.txt
grep -i "word" file.txt
grep -n "word" file.txt
grep -v "word" file.txt
grep -r "word" .
grep -c "word" file.txt
```

---

## Summary

`grep` searches for patterns in text.

One of the most useful commands is:

```bash
grep -r "pattern" .
```

