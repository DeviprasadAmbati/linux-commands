# `uname` - Display System Information

## 1. What is `uname`?

`uname` stands for **Unix Name**.

The `uname` command displays information about the Linux system and kernel.

It can show information such as:

* Operating system name
* Kernel name
* Kernel version
* Machine architecture

---

## 2. Basic Syntax

```bash
uname
```

Example output:

```text
Linux
```

---

## 3. Display All System Information

The most commonly used option is:

```bash
uname -a
```

This displays detailed system information.

Example output may include:

```text
Linux hostname 6.x.x-generic x86_64 GNU/Linux
```

---

## 4. Display the Kernel Version

Use:

```bash
uname -r
```

Example:

```text
6.8.0-xx-generic
```

---

## 5. Display Machine Architecture

Use:

```bash
uname -m
```

Example:

```text
x86_64
```

This usually indicates a 64-bit system architecture.

---

## 6. Display the Operating System Name

Use:

```bash
uname -s
```

Example:

```text
Linux
```

---

## 7. Quick Reference

```bash
uname
uname -a
uname -r
uname -m
uname -s
```

---

## Summary

`uname` displays information about the operating system and Linux kernel.

The most commonly used command is:

```bash
uname -a
```

