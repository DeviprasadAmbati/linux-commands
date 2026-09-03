# `cp` - Copy Files and Directories

## 1. What is `cp`?

`cp` stands for **copy**.

The `cp` command is used to copy files and directories from one location to another.

Unlike the `mv` command, `cp` keeps the original file or directory unchanged and creates a duplicate at the destination.

---

## 2. Basic Syntax

```bash
cp SOURCE DESTINATION
```

Example:

```bash
cp file.txt backup.txt
```

This creates a copy of `file.txt` named `backup.txt`.

The original file still exists.

---

## 3. Copy a File

Suppose you have:

```text
file.txt
```

Run:

```bash
cp file.txt copy.txt
```

Now:

```text
file.txt
copy.txt
```

Both files exist.

---

## 4. Copy a File to Another Directory

```bash
cp file.txt Documents/
```

This copies `file.txt` into the `Documents` directory.

The file keeps its original name.

---

## 5. Copy Multiple Files

```bash
cp file1.txt file2.txt file3.txt Documents/
```

This copies all three files into the `Documents` directory.

---

## 6. Copy a Directory

To copy a directory, use the `-r` option:

```bash
cp -r project backup/
```

`-r` means **recursive**.

It copies the directory and everything inside it.

Example:

```text
project/
├── main.py
└── config.py
```

After:

```bash
cp -r project backup/
```

You will have:

```text
backup/
└── project/
    ├── main.py
    └── config.py
```

---

## 7. Important Options

### `-r` - Recursive Copy

```bash
cp -r source_directory destination_directory
```

Used for copying directories and their contents.

---

### `-i` - Interactive Mode

```bash
cp -i file.txt backup.txt
```

If the destination file already exists, Linux asks for confirmation before overwriting it.

---

### `-v` - Verbose Output

```bash
cp -v file.txt backup.txt
```

Displays information about what is being copied.

---

### `-n` - Do Not Overwrite

```bash
cp -n file.txt backup.txt
```

Prevents overwriting an existing destination file.

---

### `-p` - Preserve File Attributes

```bash
cp -p file.txt backup.txt
```

Attempts to preserve attributes such as timestamps and permissions.

---

## 8. Real-World Examples

### Backup a configuration file

```bash
cp config.conf config.conf.backup
```

### Copy a project

```bash
cp -r my-project my-project-backup
```

### Copy files into a backup directory

```bash
cp *.txt backup/
```

### Copy with confirmation

```bash
cp -i important.txt backup/
```

---

## 9. Common Mistakes

### Mistake 1: Forgetting `-r` for Directories

This may fail:

```bash
cp project backup/
```

Use:

```bash
cp -r project backup/
```

---

### Mistake 2: Accidentally Overwriting Files

This command can overwrite an existing file:

```bash
cp file.txt backup.txt
```

Use interactive mode when necessary:

```bash
cp -i file.txt backup.txt
```

---

## 10. Related Commands

| Command | Purpose                    |
| ------- | -------------------------- |
| `cp`    | Copy files and directories |
| `mv`    | Move or rename files       |
| `rm`    | Remove files               |
| `mkdir` | Create directories         |

---

## 11. Practice Exercises

1. Create a file named `file1.txt`.
2. Copy it to `file2.txt`.
3. Create a directory named `backup`.
4. Copy `file1.txt` into `backup`.
5. Create a directory containing files.
6. Copy the directory using `cp -r`.
7. Try `cp -i` with an existing destination file.
8. Use `cp -v` and observe the output.

---

## 12. Quick Reference

```bash
# Copy a file
cp source.txt destination.txt

# Copy into a directory
cp file.txt directory/

# Copy multiple files
cp file1.txt file2.txt directory/

# Copy a directory
cp -r source_directory destination/

# Interactive copy
cp -i source.txt destination.txt

# Verbose output
cp -v source.txt destination.txt

# Do not overwrite
cp -n source.txt destination.txt
```

---

## Summary

The `cp` command is used to copy files and directories.

The original data remains unchanged.

The most important commands are:

```bash
cp source destination
cp file directory/
cp -r directory destination/
cp -i source destination
```

