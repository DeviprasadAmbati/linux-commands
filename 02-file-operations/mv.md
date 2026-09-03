# `mv` - Move and Rename Files

## 1. What is `mv`?

`mv` stands for **move**.

The `mv` command is used to:

* Move files from one location to another.
* Move directories.
* Rename files.
* Rename directories.

Unlike `cp`, the `mv` command does not normally create a duplicate. The item is moved or renamed.

---

## 2. Basic Syntax

```bash
mv SOURCE DESTINATION
```

---

## 3. Rename a File

```bash
mv oldname.txt newname.txt
```

This renames:

```text
oldname.txt
```

to:

```text
newname.txt
```

---

## 4. Move a File

```bash
mv file.txt Documents/
```

This moves `file.txt` into the `Documents` directory.

---

## 5. Move Multiple Files

```bash
mv file1.txt file2.txt file3.txt Documents/
```

All files are moved into `Documents`.

---

## 6. Rename a Directory

```bash
mv old-project new-project
```

This renames the directory.

---

## 7. Important Options

### `-i` - Interactive Mode

```bash
mv -i old.txt new.txt
```

Asks for confirmation before overwriting an existing file.

---

### `-v` - Verbose Mode

```bash
mv -v old.txt new.txt
```

Displays information about the operation.

---

### `-n` - Do Not Overwrite

```bash
mv -n source.txt destination.txt
```

Prevents overwriting an existing file.

---

## 8. Real-World Examples

### Rename a file

```bash
mv app.py main.py
```

### Move a file

```bash
mv report.pdf Documents/
```

### Organize log files

```bash
mv *.log logs/
```

### Rename a project

```bash
mv old-project new-project
```

---

## 9. Common Mistakes

### Mistake 1: Accidentally Overwriting a File

```bash
mv source.txt destination.txt
```

can replace the destination file.

Use:

```bash
mv -i source.txt destination.txt
```

when you want confirmation.

---

### Mistake 2: Confusing Move and Copy

`cp`:

```text
Creates a copy
```

`mv`:

```text
Moves or renames the original
```

---

## 10. Related Commands

| Command | Purpose            |
| ------- | ------------------ |
| `mv`    | Move or rename     |
| `cp`    | Copy               |
| `rm`    | Remove             |
| `mkdir` | Create directories |

---

## 11. Practice Exercises

1. Create `old.txt`.
2. Rename it to `new.txt`.
3. Create a directory named `documents`.
4. Move `new.txt` into `documents`.
5. Move multiple files into one directory.
6. Rename a directory.
7. Try `mv -i`.
8. Try `mv -v`.

---

## 12. Quick Reference

```bash
# Rename a file
mv old.txt new.txt

# Move a file
mv file.txt directory/

# Move multiple files
mv file1.txt file2.txt directory/

# Rename a directory
mv old-directory new-directory

# Interactive mode
mv -i source destination

# Verbose mode
mv -v source destination
```

---

## Summary

`mv` is used to move and rename files and directories.

Remember:

```text
cp = Copy

mv = Move / Rename
```

