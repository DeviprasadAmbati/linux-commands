# `free` - Display Memory Usage

## 1. What is `free`?

The `free` command displays information about system memory usage.

It shows information about:

* RAM
* Used memory
* Available memory
* Swap memory

---

## 2. Basic Syntax

```bash
free
```

---

## 3. Human-Readable Format

The most commonly used command is:

```bash
free -h
```

This displays memory sizes in an easier-to-read format such as:

```text
MB
GB
```

---

## 4. Example Output

```text
               total        used        free      shared  buff/cache   available
Mem:            16Gi        6Gi         2Gi         1Gi         8Gi         9Gi
Swap:            2Gi         0Gi         2Gi
```

---

## 5. Understanding Important Columns

| Column      | Meaning                               |
| ----------- | ------------------------------------- |
| `total`     | Total memory                          |
| `used`      | Memory currently in use               |
| `free`      | Completely unused memory              |
| `available` | Memory available for new applications |

---

## 6. Display Memory Repeatedly

Use:

```bash
free -h -s 2
```

This refreshes the memory information every 2 seconds.

Stop with:

```text
Ctrl + C
```

---

## 7. Real-World Use

If a system is slow, check memory usage:

```bash
free -h
```

You can combine this with:

```bash
top
```

or:

```bash
htop
```

to identify processes using memory.

---

## Quick Reference

```bash
free
free -h
free -h -s 2
```

---

## Summary

`free` displays RAM and swap memory usage.

The most commonly used command is:

```bash
free -h
```

