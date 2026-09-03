# `rm` - Remove Files and Directories

## 1. What is `rm`?

`rm` stands for **remove**.

The `rm` command is used to permanently remove files and directories.

Unlike a graphical desktop recycle bin, files removed using `rm` may not be easily recoverable.

Always verify the file or directory before removing it.

---

## 2. Basic Syntax

```bash
rm FILE
```

Example:

```bash
rm file.txt
```

This removes `file.txt`.

---

## 3. Remove Multiple Files

```bash
rm file1.txt file2.txt file3.txt
```

This removes all specified files.

---

## 4. Remove a Directory

To remove a directory and its contents:

```bash
rm -r directory_name
```

The `-r` option means recursive.

---

## 5. Important Options

### `-r` - Recursive Removal

```bash
rm -r directory
```

Removes the directory and its contents.

⚠️ Be very careful with this command.

---

### `-i` - Interactive Mode

```bash
rm -i file.txt
```

Asks for confirmation before removing the file.

This is useful when deleting important files.

---

### `-v` - Verbose Output

```bash
rm -v file.txt
```

Displays information about what is being removed.

---

### `-f` - Force Removal

```bash
rm -f file.txt
```

Attempts to remove files without asking for confirmation.

⚠️ Use this carefully.

---

## 6. Real-World Examples

### Remove a temporary file

```bash
rm temp.txt
```

### Remove multiple log files

```bash
rm *.log
```

### Remove an empty project directory

```bash
rm -r old-project
```

### Remove with confirmation

```bash
rm -i important.txt
```

---

## 7. Safety Tips

Before using `rm`, check your current directory:

```bash
pwd
```

Check the files:

```bash
ls
```

Then remove only the intended file.

For important files, prefer:

```bash
rm -i filename
```

---

## 8. Common Mistakes

### Mistake 1: Using `rm` in the Wrong Directory

Always check:

```bash
pwd
```

before removing files.

---

### Mistake 2: Using Wildcards Carelessly

This command:

```bash
rm *.txt
```

removes all `.txt` files in the current directory.

Always run:

```bash
ls *.txt
```

first to see which files match.

---

### Mistake 3: Using Recursive Removal Carelessly

```bash
rm -r directory
```

removes the directory and everything inside it.

Double-check the directory name before pressing Enter.

---

## 9. Related Commands

| Command | Purpose                  |
| ------- | ------------------------ |
| `rm`    | Remove files             |
| `rmdir` | Remove empty directories |
| `cp`    | Copy files               |
| `mv`    | Move or rename files     |

---

## 10. Practice Exercises

⚠️ Create a safe practice directory first.

```bash
mkdir rm-practice
cd rm-practice
```

Then:

1. Create three test files.
2. Remove one file.
3. Use `rm -i` on another file.
4. Create a subdirectory.
5. Add test files inside it.
6. Remove the practice directory using `rm -r`.

Never practice destructive commands on important files.

---

## 11. Quick Reference

```bash
# Remove a file
rm file.txt

# Remove multiple files
rm file1.txt file2.txt

# Remove with confirmation
rm -i file.txt

# Remove a directory recursively
rm -r directory

# Verbose removal
rm -v file.txt
```

---

## Summary

`rm` is used to remove files and directories.

The most important commands are:

```bash
rm file.txt
rm -i file.txt
rm -r directory
```

⚠️ Always check your current directory and target files before removing anything.

