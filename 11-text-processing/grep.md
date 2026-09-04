# `grep` - Search Text Using Patterns

## 1. What is `grep`?

`grep` is a Linux command used to search for specific text or patterns inside files or command output.

The name comes from the historical `ed` command:

```text
g/re/p
```

which means:

```text
Globally search for a Regular Expression and Print matching lines.
```

`grep` is one of the most commonly used Linux commands.

---

## 2. Basic Syntax

```bash
grep pattern filename
```

Example:

```bash
grep error application.log
```

This displays lines containing the word `error`.

---

## 3. Search Case Insensitively

Use:

```bash
grep -i error application.log
```

This matches:

```text
error
ERROR
Error
```

---

## 4. Search Recursively

Use:

```bash
grep -r "error" directory/
```

This searches through files inside the directory and its subdirectories.

---

## 5. Show Line Numbers

Use:

```bash
grep -n error application.log
```

Example output:

```text
15:error occurred
27:another error
```

---

## 6. Invert the Search

Use:

```bash
grep -v error application.log
```

This displays lines that do **not** contain `error`.

---

## 7. Combine Options

Example:

```bash
grep -rin "error" .
```

Explanation:

```text
-r → Recursive search
-i → Ignore case
-n → Show line numbers
```

---

## 8. Use `grep` with Pipes

Example:

```bash
ps aux | grep python
```

This searches running processes for `python`.

Another example:

```bash
ls -l | grep ".txt"
```

---

## 9. Common Options

| Option | Purpose                 |
| ------ | ----------------------- |
| `-i`   | Ignore case             |
| `-r`   | Search recursively      |
| `-n`   | Show line numbers       |
| `-v`   | Show non-matching lines |
| `-l`   | Show filenames only     |
| `-c`   | Count matching lines    |

---

## 10. Quick Reference

```bash
grep pattern file
grep -i pattern file
grep -r pattern directory/
grep -n pattern file
grep -v pattern file
grep -rin pattern .
```

---

## Summary

`grep` is used to search for text and patterns in files and command output.

One of the most commonly used commands is:

```bash
grep -rin "pattern" .
```

