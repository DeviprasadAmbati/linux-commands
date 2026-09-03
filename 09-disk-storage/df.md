# `df` - Display Disk Space Usage

## 1. What is `df`?

`df` stands for **Disk Filesystem**.

The `df` command displays information about disk space usage for mounted filesystems.

It helps you answer questions such as:

* How much disk space is available?
* How much disk space is used?
* Which filesystem is full?

---

## 2. Basic Syntax

```bash
df
```

This displays disk usage information for mounted filesystems.

---

## 3. Human-Readable Output

The most commonly used option is:

```bash
df -h
```

The `-h` option displays sizes in a human-readable format such as:

```text
MB
GB
TB
```

---

## 4. Example Output

```text
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        50G   20G   28G  42% /
```

### Understanding the Columns

| Column       | Meaning            |
| ------------ | ------------------ |
| `Filesystem` | Disk or filesystem |
| `Size`       | Total size         |
| `Used`       | Used space         |
| `Avail`      | Available space    |
| `Use%`       | Percentage used    |
| `Mounted on` | Mount location     |

---

## 5. Check a Specific Directory

You can check the filesystem containing a directory:

```bash
df -h /home
```

---

## 6. Display Filesystem Type

Use:

```bash
df -Th
```

This can display filesystem types along with human-readable sizes.

---

## 7. Real-World Example

When a server reports:

```text
No space left on device
```

Run:

```bash
df -h
```

This helps identify which mounted filesystem is full.

---

## 8. Quick Reference

```bash
df
df -h
df -Th
df -h /home
```

---

## Summary

`df` is used to check available and used disk space on mounted filesystems.

The most commonly used command is:

```bash
df -h
```

