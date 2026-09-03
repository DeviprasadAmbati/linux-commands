# `umask` - Set Default File Permissions

## 1. What is `umask`?

`umask` stands for **user file creation mode mask**.

The `umask` command controls the default permissions assigned to newly created files and directories.

It does not normally change permissions of existing files.

---

## 2. Check Your Current `umask`

Run:

```bash
umask
```

Example output:

```text
0022
```

---

## 3. How `umask` Works

The `umask` value removes permissions from the default permissions used when new files and directories are created.

Typical maximum starting permissions are:

```text
Files       → 666
Directories → 777
```

The execute bit is normally not automatically granted to newly created regular files.

---

## 4. Example: `umask 022`

```bash
umask 022
```

Typical result:

```text
Files       → 644
Directories → 755
```

This means:

```text
Owner   → Read and Write
Group   → Read
Others  → Read
```

for typical new files.

---

## 5. Example: `umask 077`

```bash
umask 077
```

Typical result:

```text
Files       → 600
Directories → 700
```

This is useful when newly created files should be private.

---

## 6. Common `umask` Values

| Umask | Typical File Permission | Typical Directory Permission |
| ----- | ----------------------- | ---------------------------- |
| `022` | 644                     | 755                          |
| `002` | 664                     | 775                          |
| `077` | 600                     | 700                          |

Actual results can depend on the program creating the file.

---

## 7. Temporarily Change `umask`

```bash
umask 077
```

This affects the current shell session and programs started from it.

---

## 8. Check Symbolic Format

You can use:

```bash
umask -S
```

Example output may look like:

```text
u=rwx,g=rx,o=rx
```

---

## 9. Common Mistakes

### Mistake 1: Thinking `umask` Changes Existing Files

`umask` affects newly created files and directories.

To change existing permissions, use:

```bash
chmod
```

---

### Mistake 2: Using an Incorrect Mask

Always understand the permissions you are setting before changing the mask.

Check your current value:

```bash
umask
```

---

## 10. Practice Exercises

1. Check your current `umask`.
2. Create a test file.
3. Check its permissions.
4. Set:

```bash
umask 077
```

5. Create another test file.
6. Compare permissions.

Remember that this change affects the current shell session.

---

## 11. Related Commands

| Command | Purpose                     |
| ------- | --------------------------- |
| `umask` | Set default permission mask |
| `chmod` | Change existing permissions |
| `chown` | Change ownership            |
| `chgrp` | Change group ownership      |

---

## 12. Quick Reference

```bash
# Check umask
umask

# Show symbolic format
umask -S

# Set umask
umask 022

# Private default permissions
umask 077
```

---

## Summary

`umask` controls the default permissions of newly created files and directories.

Common values:

```text
022 → Typical files: 644, directories: 755

077 → Typical files: 600, directories: 700
```

