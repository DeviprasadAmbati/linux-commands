# `chmod` - Change File Permissions

## 1. What is `chmod`?

`chmod` stands for **change mode**.

The `chmod` command is used to change the permissions of files and directories in Linux.

Linux permissions control who can:

* Read a file.
* Write or modify a file.
* Execute a file or access a directory.

---

## 2. Understanding Linux Permissions

Linux has three basic permissions:

| Symbol | Permission | Meaning                          |
| ------ | ---------- | -------------------------------- |
| `r`    | Read       | View file contents               |
| `w`    | Write      | Modify a file                    |
| `x`    | Execute    | Run a file or access a directory |

Example:

```text
rwxr-xr--
```

This represents permissions for:

```text
Owner | Group | Others
rwx   | r-x   | r--
```

---

## 3. View File Permissions

Use:

```bash
ls -l
```

Example output:

```text
-rwxr-xr-- 1 user group 1024 file.sh
```

The permission section is:

```text
rwxr-xr--
```

---

## 4. Permission Groups

Linux permissions are divided into three groups:

### Owner (`u`)

The user who owns the file.

### Group (`g`)

Users belonging to the file's group.

### Others (`o`)

Everyone else.

You can also use:

```text
a
```

which means:

```text
all
```

---

## 5. Symbolic Mode

The basic syntax is:

```bash
chmod WHO OPERATION PERMISSION FILE
```

Example:

```bash
chmod u+x script.sh
```

This means:

```text
u → User/Owner
+ → Add permission
x → Execute permission
```

---

## 6. Add Permissions

### Add execute permission

```bash
chmod +x script.sh
```

### Add write permission for the owner

```bash
chmod u+w file.txt
```

### Add read permission for the group

```bash
chmod g+r file.txt
```

---

## 7. Remove Permissions

### Remove write permission

```bash
chmod u-w file.txt
```

### Remove execute permission

```bash
chmod o-x script.sh
```

---

## 8. Set Exact Permissions

Use:

```bash
chmod u=rwx,g=rx,o=r file.txt
```

This sets:

```text
Owner  → rwx
Group  → r-x
Others → r--
```

---

# 9. Numeric Permissions

Linux permissions can also be represented using numbers.

| Permission    | Value |
| ------------- | ----: |
| Read (`r`)    |     4 |
| Write (`w`)   |     2 |
| Execute (`x`) |     1 |

Add the values together.

For example:

```text
rwx = 4 + 2 + 1 = 7
r-x = 4 + 1 = 5
r-- = 4
```

Therefore:

```text
rwxr-xr--
```

becomes:

```text
754
```

---

## 10. Common Numeric Permissions

| Number | Permission |
| ------ | ---------- |
| `777`  | rwxrwxrwx  |
| `755`  | rwxr-xr-x  |
| `700`  | rwx------  |
| `644`  | rw-r--r--  |
| `600`  | rw-------  |

---

## 11. Examples

### Make a script executable

```bash
chmod +x script.sh
```

### Set permissions to 755

```bash
chmod 755 script.sh
```

### Set permissions to 644

```bash
chmod 644 file.txt
```

### Make a private file

```bash
chmod 600 secret.txt
```

---

## 12. Change Directory Permissions Recursively

Use:

```bash
chmod -R 755 directory/
```

The `-R` option means **recursive**.

It changes permissions for the directory and everything inside it.

⚠️ Be careful when using recursive permission changes because files and directories may need different permissions.

---

## 13. Common Mistakes

### Mistake 1: Using `777` Everywhere

```bash
chmod 777 file.txt
```

gives everyone full permissions.

This can create security problems.

Use the minimum permissions required.

---

### Mistake 2: Forgetting Execute Permission

A script may not run if execute permission is missing.

Use:

```bash
chmod +x script.sh
```

---

## 14. Practice Exercises

1. Create a file:

```bash
touch test.txt
```

2. Check permissions:

```bash
ls -l test.txt
```

3. Set permissions:

```bash
chmod 644 test.txt
```

4. Create a script and make it executable:

```bash
chmod +x script.sh
```

5. Experiment with `u`, `g`, and `o`.

---

## 15. Quick Reference

```bash
# Add execute permission
chmod +x file

# Set permission using numbers
chmod 755 directory
chmod 644 file

# Add permission
chmod u+x file

# Remove permission
chmod o-w file

# Change recursively
chmod -R 755 directory
```

---

## Summary

`chmod` controls Linux file and directory permissions.

The most commonly used commands are:

```bash
chmod +x script.sh
chmod 644 file.txt
chmod 755 directory/
chmod 600 secret.txt
```

Always follow the principle of giving only the permissions that are necessary.

