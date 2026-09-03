# `touch` - Create Empty Files and Update Timestamps

## 1. What is `touch`?

The `touch` command is commonly used to:

* Create empty files.
* Update file timestamps.

It is one of the simplest and most frequently used Linux commands.

---

## 2. Basic Syntax

```bash
touch FILE_NAME
```

Example:

```bash
touch notes.txt
```

If `notes.txt` does not exist, Linux creates an empty file.

---

## 3. Create Multiple Files

You can create multiple files at once:

```bash
touch file1.txt file2.txt file3.txt
```

---

## 4. Check the Created File

Use:

```bash
ls
```

Example:

```bash
touch example.txt
ls
```

You should see:

```text
example.txt
```

---

## 5. Update File Timestamp

If the file already exists:

```bash
touch notes.txt
```

does not normally erase its content.

Instead, it updates the file's access and modification timestamps.

You can check timestamps using:

```bash
ls -l
```

---

## 6. Create Files Using Brace Expansion

```bash
touch file{1,2,3}.txt
```

This creates:

```text
file1.txt
file2.txt
file3.txt
```

You can also create numbered files:

```bash
touch file{1..5}.txt
```

This creates:

```text
file1.txt
file2.txt
file3.txt
file4.txt
file5.txt
```

---

## 7. Important Options

### `-c` — Do Not Create a File

```bash
touch -c file.txt
```

If the file does not exist, it will not be created.

---

### `-a` — Update Access Time

```bash
touch -a file.txt
```

Updates the access time.

---

### `-m` — Update Modification Time

```bash
touch -m file.txt
```

Updates the modification time.

---

## 8. Real-World Examples

### Create a Python file

```bash
touch app.py
```

### Create project files

```bash
touch README.md requirements.txt .gitignore
```

### Create multiple source files

```bash
touch main.py config.py database.py
```

---

## 9. Common Mistakes

### Mistake 1: Thinking `touch` Creates Directories

This:

```bash
touch project
```

creates a file, not a directory.

To create a directory:

```bash
mkdir project
```

---

### Mistake 2: Thinking `touch` Deletes File Content

Running:

```bash
touch existing-file.txt
```

does not normally delete the file's contents.

It updates timestamps.

---

## 10. Related Commands

| Command | Purpose                        |
| ------- | ------------------------------ |
| `touch` | Create files/update timestamps |
| `mkdir` | Create directories             |
| `rm`    | Remove files                   |
| `cp`    | Copy files                     |
| `mv`    | Move or rename files           |

---

## 11. Practice Exercises

1. Create a file called `notes.txt`.
2. Create five files in one command.
3. Create files using brace expansion.
4. Check the files using `ls`.
5. Run `touch` on an existing file and check its timestamp using `ls -l`.

---

## 12. Quick Reference

```bash
touch file.txt
touch file1.txt file2.txt
touch file{1..5}.txt
touch -c file.txt
touch -a file.txt
touch -m file.txt
```

---

## Summary

`touch` is mainly used to create empty files and update file timestamps.

The most commonly used command is:

```bash
touch filename
```

