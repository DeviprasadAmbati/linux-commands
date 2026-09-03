# `lsblk` - List Block Devices

## 1. What is `lsblk`?

`lsblk` stands for **List Block Devices**.

It displays information about storage devices connected to the Linux system.

This can include:

* Hard disks
* SSDs
* USB drives
* Partitions

---

## 2. Basic Syntax

```bash
lsblk
```

---

## 3. Example Output

```text
NAME   SIZE TYPE MOUNTPOINT
sda    100G disk
├─sda1  50G part /
└─sda2  50G part /home
```

---

## 4. Understanding the Output

| Column       | Meaning                     |
| ------------ | --------------------------- |
| `NAME`       | Device name                 |
| `SIZE`       | Device size                 |
| `TYPE`       | Device type                 |
| `MOUNTPOINT` | Where the device is mounted |

---

## 5. Display Filesystem Information

Use:

```bash
lsblk -f
```

This can display:

* Filesystem type
* UUID
* Mount points

---

## 6. Display Additional Information

Use:

```bash
lsblk -o NAME,SIZE,TYPE,FSTYPE,MOUNTPOINTS
```

This allows you to choose the columns displayed.

---

## 7. Real-World Use

Before mounting a new disk, you can check available devices:

```bash
lsblk
```

Always identify the correct device carefully before performing destructive operations.

---

## 8. Quick Reference

```bash
lsblk
lsblk -f
lsblk -o NAME,SIZE,TYPE,FSTYPE,MOUNTPOINTS
```

---

## Summary

`lsblk` displays information about disks, partitions, and other block devices.

The most commonly used command is:

```bash
lsblk
```

