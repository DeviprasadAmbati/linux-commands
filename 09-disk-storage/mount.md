# `mount` - Attach a Filesystem

## 1. What is `mount`?

The `mount` command attaches a filesystem to a directory in the Linux filesystem.

That directory is called a **mount point**.

Linux makes storage devices available through the directory structure.

---

## 2. Basic Syntax

```bash
mount device mount_point
```

Example:

```bash
sudo mount /dev/sdb1 /mnt
```

---

## 3. Understanding Mounting

Example:

```text
/dev/sdb1
    │
    │ mount
    ▼
/mnt
```

After mounting, the files on the device can be accessed through:

```text
/mnt
```

---

## 4. Create a Mount Point

Before mounting, create a directory:

```bash
sudo mkdir /mnt/mydisk
```

Then mount:

```bash
sudo mount /dev/sdb1 /mnt/mydisk
```

---

## 5. View Mounted Filesystems

Run:

```bash
mount
```

You can also use:

```bash
findmnt
```

---

## 6. Mount an ISO File

Example:

```bash
sudo mount -o loop file.iso /mnt
```

The `loop` option allows the ISO file to be treated like a storage device.

---

## 7. Important Warning

⚠️ Always verify the correct device using:

```bash
lsblk
```

before mounting or performing disk operations.

---

## Quick Reference

```bash
mount
sudo mount /dev/sdb1 /mnt
sudo mkdir /mnt/mydisk
sudo mount /dev/sdb1 /mnt/mydisk
```

---

## Summary

`mount` makes a filesystem accessible through a directory called a mount point.

