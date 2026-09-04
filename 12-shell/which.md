# `which` - Locate a Command

## 1. What is `which`?

The `which` command shows the path of the executable that would be run when you type a command.

---

## 2. Basic Syntax

```bash
which command
```

Example:

```bash
which python
```

Possible output:

```text
/usr/bin/python
```

---

## 3. Check Multiple Commands

```bash
which python git bash
```

---

## 4. Why Is This Useful?

`which` helps you determine:

* Which executable is being used.
* Whether a command is available in your `PATH`.
* Whether multiple installations may exist.

---

## 5. Related Command

For shell commands, aliases, functions, and built-ins, use:

```bash
type command
```

Example:

```bash
type cd
```

---

## Summary

`which` helps locate executable commands available through the shell's `PATH`.

