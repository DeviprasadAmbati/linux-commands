# `fdisk` - Manage Disk Partitions

## 1. What is `fdisk`?

`fdisk` is a command-line utility used to view and manage disk partition tables.

It can be used to:

* View disks.
* View partitions.
* Create partitions.
* Delete partitions.

---

## 2. List Disk Partitions

Use:

```bash
sudo fdisk -l
```

This displays information about available disks and partitions.

---

## 3. Manage a Specific Disk

Example:

```bash
sudo fdisk /dev/sdb
```

This opens an interactive partition management session.

---

## 4. Important Warning

⚠️ `fdisk` can modify partition tables.

Incorrect usage can make data inaccessible.

Always verify the target disk:

```bash
lsblk
```

Before making changes.

---

## 5. Common Interactive Commands

Inside `fdisk`:

| Command | Purpose               |
| ------- | --------------------- |
| `m`     | Display help          |
| `p`     | Print partition table |
| `n`     | Create partition      |
| `d`     | Delete partition      |
| `w`     | Write changes         |
| `q`     | Quit without saving   |

---

## 6. Safe Learning Practice

You can safely start by listing disks:

```bash
sudo fdisk -l
```

Avoid modifying disks unless you understand the partition layout and have backups.

---

## Quick Reference

```bash
sudo fdisk -l
sudo fdisk /dev/sdb
```

---

## Summary

`fdisk` is used to inspect and manage disk partitions.

⚠️ Use it carefully because partition changes can affect access to data.

