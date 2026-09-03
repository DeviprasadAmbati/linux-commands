# `chown` - Change File Owner

## 1. What is `chown`?

`chown` stands for **change owner**.

The `chown` command is used to change the ownership of files and directories.

In Linux, every file has:

* An owner.
* A group.

---

## 2. Basic Syntax

```bash
chown OWNER FILE
```

Example:

```bash
chown deviprasad file.txt
```

This changes the owner of `file.txt` to `deviprasad`.

Changing ownership usually requires appropriate permissions, often administrator privileges.

---

## 3. View File Ownership

Use:

```bash
ls -l
```

Example:

```text
-rw-r--r-- 1 deviprasad developers 1024 file.txt
```

This shows:

```text
Owner → deviprasad
Group → developers
```

---

## 4. Change File Owner

```bash
sudo chown username file.txt
```

Example:

```bash
sudo chown deviprasad file.txt
```

---

## 5. Change Owner and Group

You can change both at the same time:

```bash
sudo chown user:group file.txt
```

Example:

```bash
sudo chown deviprasad:developers file.txt
```

---

## 6. Change Ownership of a Directory

```bash
sudo chown username directory/
```

---

## 7. Change Ownership Recursively

```bash
sudo chown -R username directory/
```

This changes the ownership of the directory and its contents.

Example:

```bash
sudo chown -R deviprasad:developers project/
```

---

## 8. Important Options

### `-R` - Recursive

```bash
sudo chown -R user directory/
```

Changes ownership for everything inside the directory.

---

### `-v` - Verbose

```bash
sudo chown -v user file.txt
```

Displays information about changes being made.

---

## 9. Real-World Examples

### Change ownership of a project

```bash
sudo chown -R developer project/
```

### Change web application ownership

```bash
sudo chown -R www-data:www-data /var/www/application
```

The appropriate service user can vary by Linux distribution and web server configuration.

---

## 10. Common Mistakes

### Mistake 1: Changing Ownership of System Files

Changing ownership incorrectly can break applications or the operating system.

Always verify the target before running:

```bash
sudo chown -R
```

---

### Mistake 2: Using `-R` Without Checking

Recursive ownership changes affect every file and directory inside the target.

Use:

```bash
ls -la
```

before making changes.

---

## 11. Related Commands

| Command | Purpose                        |
| ------- | ------------------------------ |
| `chown` | Change owner                   |
| `chgrp` | Change group                   |
| `chmod` | Change permissions             |
| `ls -l` | View ownership and permissions |

---

## 12. Practice Exercises

Create a practice directory:

```bash
mkdir ownership-practice
```

Create a file:

```bash
touch ownership-practice/test.txt
```

Check ownership:

```bash
ls -l ownership-practice/test.txt
```

Practice only on files you understand and have permission to manage.

---

## 13. Quick Reference

```bash
# Change owner
sudo chown user file

# Change owner and group
sudo chown user:group file

# Change directory ownership
sudo chown user directory/

# Recursive ownership
sudo chown -R user directory/

# Verbose mode
sudo chown -v user file
```

---

## Summary

`chown` changes file and directory ownership.

The most useful forms are:

```bash
sudo chown user file
sudo chown user:group file
sudo chown -R user:group directory/
```

