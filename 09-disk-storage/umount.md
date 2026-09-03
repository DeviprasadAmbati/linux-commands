# `umount` - Unmount a Filesystem

## 1. What is `umount`?

The `umount` command disconnects a mounted filesystem from the Linux directory structure.

Notice that the command is spelled:

```text
umount
```

There is no `n` after the `u`.

---

## 2. Basic Syntax

```bash
umount mount_point
```

Example:

```bash
sudo umount /mnt
```

---

## 3. Unmount Using the Device Name

You can also specify the device:

```bash
sudo umount /dev/sdb1
```

---

## 4. Why Unmount a Device?

Unmounting ensures that data is properly written before disconnecting a storage device.

This is especially important before removing:

* USB drives
* External hard drives
* Other removable storage

---

## 5. Device Is Busy

You may see:

```text
target is busy
```

This means a process is currently using the filesystem.

You can check your current directory:

```bash
pwd
```

Make sure your terminal is not currently inside the mounted directory.

---

## 6. Quick Reference

```bash
sudo umount /mnt
sudo umount /dev/sdb1
```

---

## Summary

`umount` safely disconnects a mounted filesystem from the Linux directory structure.

