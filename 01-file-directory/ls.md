# `ls` - List Directory Contents

## 1. What is `ls`?

`ls` stands for **list**.

It is used to display files and directories inside a directory.

It is one of the most commonly used Linux commands.

---

## 2. Basic Syntax

```bash
ls [OPTIONS] [DIRECTORY]
```

The simplest usage is:

```bash
ls
```

This displays the contents of your current directory.

For example:

```text
01-file-directory
02-file-operations
README.md
```

---

## 3. List a Specific Directory

You can list the contents of another directory without moving into it.

```bash
ls /home/deviprasad/linux-commands
```

You can also use a relative path:

```bash
ls ..
```

`..` represents the parent directory.

---

## 4. Important Options

### `ls -l` — Long Listing Format

```bash
ls -l
```

Displays detailed information including:

* File permissions
* Number of links
* Owner
* Group
* File size
* Modification date
* File name

Example:

```text
-rw-r--r-- 1 deviprasad deviprasad 1200 Sep 03 20:00 README.md
```

---

### `ls -a` — Show Hidden Files

```bash
ls -a
```

Files beginning with a `.` are hidden by default.

Examples:

```text
.git
.gitignore
.bashrc
```

---

### `ls -h` — Human Readable File Sizes

Usually used with `-l`:

```bash
ls -lh
```

Instead of showing:

```text
1048576
```

Linux can display:

```text
1.0M
```

---

### `ls -la` — Long Format and Hidden Files

```bash
ls -la
```

This is one of the most commonly used combinations.

---

### `ls -lah` — Complete Detailed Listing

```bash
ls -lah
```

Shows:

* Hidden files
* Permissions
* Owners
* File sizes
* Human-readable sizes

---

### `ls -t` — Sort by Modification Time

```bash
ls -lt
```

Displays recently modified files first.

---

### `ls -R` — Recursive Listing

```bash
ls -R
```

Displays files inside subdirectories recursively.

Be careful when using this command in very large directories because the output can be very large.

---

## 5. Real-World Examples

### Check files in the current directory

```bash
ls
```

### Check all files, including hidden files

```bash
ls -a
```

### Check file permissions

```bash
ls -l
```

### Check file sizes

```bash
ls -lh
```

### Check recently modified files

```bash
ls -lt
```

---

## 6. Common Mistakes

### Mistake 1: Thinking `ls` changes directories

```bash
ls Documents
```

only displays the contents of `Documents`.

It does not enter the directory.

To enter it:

```bash
cd Documents
```

---

### Mistake 2: Hidden files are not displayed

Use:

```bash
ls -a
```

to display hidden files.

---

## 7. Related Commands

| Command | Purpose                     |
| ------- | --------------------------- |
| `pwd`   | Show current directory      |
| `cd`    | Change directory            |
| `find`  | Search for files            |
| `tree`  | Display directory structure |

---

## 8. Practice Exercises

1. List the current directory.
2. List hidden files.
3. Display detailed information.
4. Display human-readable file sizes.
5. Sort files by modification time.
6. Run `ls -la` and understand the output.

---

## 9. Quick Reference

```bash
ls
ls -l
ls -a
ls -la
ls -lh
ls -lah
ls -lt
ls -R
```

---

## Summary

`ls` is used to list files and directories.

The most important versions to remember are:

```bash
ls
ls -l
ls -a
ls -la
ls -lh
```

