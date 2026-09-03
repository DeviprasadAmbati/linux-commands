# `cat` - Display and Combine File Contents

## 1. What is `cat`?

`cat` stands for **concatenate**.

The `cat` command is used to:

* Display file contents.
* Combine multiple files.
* Create simple files using redirection.
* View multiple files together.

---

## 2. Basic Syntax

```bash
cat FILE_NAME
```

Example:

```bash
cat notes.txt
```

This displays the contents of `notes.txt`.

---

## 3. Display Multiple Files

```bash
cat file1.txt file2.txt
```

The contents of both files are displayed one after another.

---

## 4. Create a File Using `cat`

```bash
cat > notes.txt
```

Type your content and press:

```text
CTRL + D
```

to save and finish input.

---

## 5. Append Content to a File

```bash
cat >> notes.txt
```

Type additional content and press:

```text
CTRL + D
```

The new content is added to the existing file.

---

## 6. Important Options

### `-n` - Show Line Numbers

```bash
cat -n notes.txt
```

Displays line numbers for all lines.

---

### `-b` - Number Non-Empty Lines

```bash
cat -b notes.txt
```

Numbers only non-empty lines.

---

### `-s` - Remove Repeated Empty Lines

```bash
cat -s notes.txt
```

Combines multiple consecutive empty lines into one.

---

## 7. Real-World Examples

### View a configuration file

```bash
cat config.conf
```

### Combine files

```bash
cat file1.txt file2.txt > combined.txt
```

### Add content to a log file

```bash
cat new-log.txt >> application.log
```

---

## 8. Common Mistakes

### Mistake 1: Using `cat` for Very Large Files

`cat` prints the entire file at once.

For large files, prefer:

```bash
less large-file.txt
```

---

### Mistake 2: Accidentally Overwriting a File

This command:

```bash
cat > file.txt
```

can overwrite existing content.

Use:

```bash
cat >> file.txt
```

when you want to append.

---

## 9. Related Commands

| Command | Purpose                     |
| ------- | --------------------------- |
| `cat`   | Display file contents       |
| `less`  | View large files            |
| `head`  | Display beginning of a file |
| `tail`  | Display end of a file       |

---

## 10. Practice Exercises

1. Create a file using `cat`.
2. Display the file contents.
3. Create two files and display both together.
4. Use `cat -n` to show line numbers.
5. Combine two files into a third file.

---

## Quick Reference

```bash
cat file.txt
cat file1.txt file2.txt
cat -n file.txt
cat > file.txt
cat >> file.txt
```

---

## Summary

`cat` is used to display and combine file contents.

For small files:

```bash
cat file.txt
```

is quick and convenient.

