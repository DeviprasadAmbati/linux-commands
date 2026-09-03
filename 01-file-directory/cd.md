# `cd` - Change Directory

## 1. What is `cd`?

`cd` stands for **Change Directory**.

It is used to move from one directory to another in the Linux file system.

---

## 2. Basic Syntax

```bash
cd [DIRECTORY]
```

Example:

```bash
cd Documents
```

This moves you into the `Documents` directory.

---

## 3. Check Your Location

After changing directories, use:

```bash
pwd
```

to check your current location.

---

## 4. Important Examples

### Move into a Directory

```bash
cd Documents
```

---

### Move to the Parent Directory

```bash
cd ..
```

`..` means the parent directory.

For example:

```text
/home/deviprasad/linux-commands
```

Running:

```bash
cd ..
```

moves you to:

```text
/home/deviprasad
```

---

### Move to the Home Directory

```bash
cd
```

or:

```bash
cd ~
```

Both usually move you to your home directory.

---

### Move Using an Absolute Path

```bash
cd /home/deviprasad/linux-commands
```

An absolute path starts from the root directory `/`.

---

### Move Using a Relative Path

```bash
cd 01-file-directory
```

A relative path starts from your current directory.

---

### Move Back to the Previous Directory

```bash
cd -
```

This switches you back to the previously visited directory.

---

## 5. Directory Navigation Symbols

| Symbol | Meaning           |
| ------ | ----------------- |
| `.`    | Current directory |
| `..`   | Parent directory  |
| `~`    | Home directory    |
| `/`    | Root directory    |

---

## 6. Common Mistakes

### Mistake 1: Directory Does Not Exist

If you run:

```bash
cd wrong-folder
```

Linux may show:

```text
No such file or directory
```

Use:

```bash
ls
```

to check the correct directory name.

---

### Mistake 2: Forgetting Spaces in Directory Names

If a directory contains spaces:

```text
My Projects
```

Use:

```bash
cd "My Projects"
```

or:

```bash
cd My\ Projects
```

---

## 7. Related Commands

| Command | Purpose                  |
| ------- | ------------------------ |
| `pwd`   | Show current directory   |
| `ls`    | List directory contents  |
| `mkdir` | Create directories       |
| `rmdir` | Remove empty directories |

---

## 8. Practice Exercises

1. Go to your home directory.
2. Enter your `linux-commands` repository.
3. Enter `01-file-directory`.
4. Move back to the parent directory.
5. Use `cd -` to return to the previous directory.
6. Use `pwd` after every movement.

---

## 9. Quick Reference

```bash
cd folder
cd ..
cd ~
cd /
cd -
```

---

## Summary

`cd` is used to navigate through the Linux file system.

The most important commands are:

```bash
cd folder
cd ..
cd ~
cd -
```

