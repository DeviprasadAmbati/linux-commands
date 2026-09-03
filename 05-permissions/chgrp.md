# `chgrp` - Change File Group

## 1. What is `chgrp`?

`chgrp` stands for **change group**.

The `chgrp` command is used to change the group ownership of files and directories.

Every Linux file has:

* A user owner.
* A group owner.

---

## 2. Basic Syntax

```bash
chgrp GROUP FILE
```

Example:

```bash
chgrp developers file.txt
```

This changes the group ownership of `file.txt`.

---

## 3. View Group Ownership

Use:

```bash
ls -l
```

Example:

```text
-rw-r--r-- 1 deviprasad developers 1024 file.txt
```

The group is:

```text
developers
```

---

## 4. Change Group of a File

```bash
chgrp developers file.txt
```

Depending on the file and your permissions, administrator privileges may be required.

---

## 5. Change Group of a Directory

```bash
chgrp developers project/
```

---

## 6. Change Group Recursively

```bash
sudo chgrp -R developers project/
```

This changes the group ownership of the directory and everything inside it.

---

## 7. Important Options

### `-R` - Recursive

```bash
chgrp -R group directory/
```

Changes the group for all contents.

---

### `-v` - Verbose

```bash
chgrp -v group file.txt
```

Shows information about the changes.

---

## 8. `chgrp` vs `chown`

| Command | Purpose            |
| ------- | ------------------ |
| `chown` | Change owner       |
| `chgrp` | Change group       |
| `chmod` | Change permissions |

You can also change the owner and group together:

```bash
sudo chown user:group file
```

---

## 9. Real-World Example

Suppose multiple developers belong to the group:

```text
developers
```

You can assign a project directory to that group:

```bash
sudo chgrp -R developers project/
```

Then permissions can be configured using:

```bash
chmod
```

to control what group members can access.

---

## 10. Common Mistakes

### Mistake: Changing the Wrong Group

Check existing ownership first:

```bash
ls -l
```

Check available groups:

```bash
groups
```

Then make the change.

---

## 11. Practice Exercises

1. Create a test file.
2. Check its owner and group.
3. Run `groups`.
4. Change the group only if you have permission.
5. Practice recursive changes in a safe test directory.

---

## 12. Quick Reference

```bash
# Change group
chgrp group file

# Change directory group
chgrp group directory/

# Recursive change
sudo chgrp -R group directory/

# Verbose mode
chgrp -v group file
```

---

## Summary

`chgrp` changes the group ownership of files and directories.

Use it when you want to manage access for multiple users through Linux groups.

