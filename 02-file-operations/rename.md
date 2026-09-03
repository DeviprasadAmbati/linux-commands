# Renaming Files and Directories in Linux

## 1. How Do You Rename Files in Linux?

The most common Linux command used to rename files and directories is:

```bash
mv
```

Basic syntax:

```bash
mv OLD_NAME NEW_NAME
```

Example:

```bash
mv old-file.txt new-file.txt
```

---

## 2. Rename a File

Suppose you have:

```text
report.txt
```

Run:

```bash
mv report.txt final-report.txt
```

Now the file becomes:

```text
final-report.txt
```

---

## 3. Rename a Directory

```bash
mv old-project new-project
```

This renames the directory.

---

## 4. Rename Files Safely

Use interactive mode:

```bash
mv -i old.txt new.txt
```

If `new.txt` already exists, Linux asks for confirmation before overwriting it.

---

## 5. Rename Multiple Files

For batch renaming, some Linux systems provide a command named `rename`.

However, its syntax and implementation can vary between Linux distributions.

Always check your system's documentation:

```bash
rename --help
```

or:

```bash
man rename
```

---

## 6. Example of Batch Renaming

Suppose you have:

```text
file1.txt
file2.txt
file3.txt
```

You may want to rename extensions or patterns.

Depending on the installed `rename` implementation, commands may differ.

For this reason, always test batch rename commands on sample files first.

---

## 7. Using a Loop for Batch Renaming

A portable Bash approach can be:

```bash
for file in *.txt; do
    mv "$file" "${file%.txt}.bak"
done
```

This changes:

```text
file1.txt → file1.bak
file2.txt → file2.bak
file3.txt → file3.bak
```

---

## 8. Important Safety Tips

Before batch renaming:

1. Check the files:

```bash
ls
```

2. Test with a small number of files.

3. Use:

```bash
mv -i
```

when overwriting is possible.

4. Make backups before performing large batch operations.

---

## 9. Common Mistakes

### Mistake 1: Forgetting Quotes Around Filenames

For filenames containing spaces, use quotes:

```bash
mv "old file.txt" "new file.txt"
```

---

### Mistake 2: Accidentally Overwriting Files

Use:

```bash
mv -i old.txt new.txt
```

to request confirmation.

---

### Mistake 3: Assuming Every Linux System Has the Same `rename` Command

Different distributions may provide different implementations.

Always check:

```bash
rename --help
```

---

## 10. Related Commands

| Command | Purpose              |
| ------- | -------------------- |
| `mv`    | Rename or move files |
| `cp`    | Copy files           |
| `rm`    | Remove files         |
| `find`  | Find files           |

---

## 11. Practice Exercises

1. Create a file named `old.txt`.
2. Rename it to `new.txt`.
3. Create a directory named `old-project`.
4. Rename it to `new-project`.
5. Create several `.txt` files.
6. Practice batch renaming on test files only.

---

## 12. Quick Reference

```bash
# Rename a file
mv old.txt new.txt

# Rename a directory
mv old-directory new-directory

# Rename safely
mv -i old.txt new.txt

# Check rename command availability
rename --help
```

---

## Summary

The most common way to rename files and directories in Linux is:

```bash
mv OLD_NAME NEW_NAME
```

For simple renaming, `mv` is the standard and most portable approach.

For batch renaming, the available `rename` command may vary depending on your Linux distribution.

