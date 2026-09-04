# `man` - Display Command Documentation

## 1. What is `man`?

`man` stands for **manual**.

The `man` command displays documentation for Linux commands, programs, and system components.

---

## 2. Basic Syntax

```bash
man command
```

Example:

```bash
man ls
```

This opens the manual page for the `ls` command.

---

## 3. Navigation

Inside a manual page:

| Key     | Action             |
| ------- | ------------------ |
| `Space` | Next page          |
| `b`     | Previous page      |
| `/text` | Search for text    |
| `n`     | Next search result |
| `q`     | Quit               |

---

## 4. Search Manual Pages

You can search available manual page descriptions using:

```bash
man -k keyword
```

Example:

```bash
man -k copy
```

---

## 5. View a Specific Manual Section

Some commands have documentation in different sections.

Example:

```bash
man 5 passwd
```

This opens the relevant manual page from section 5.

---

## 6. Why Use `man`?

Whenever you forget how a Linux command works, try:

```bash
man command_name
```

For example:

```bash
man grep
```

---

## Quick Reference

```bash
man ls
man grep
man -k keyword
man 5 passwd
```

---

## Summary

`man` is the built-in documentation system for Linux and Unix commands.

