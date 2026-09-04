# `source` - Execute a Script in the Current Shell

## 1. What is `source`?

The `source` command executes commands from a file in the current shell session.

A common alternative syntax is:

```bash
. filename
```

---

## 2. Basic Syntax

```bash
source filename
```

---

## 3. Reload `.bashrc`

Example:

```bash
source ~/.bashrc
```

This reloads Bash configuration without opening a new terminal.

---

## 4. Why Use `source`?

Suppose you add an alias:

```bash
alias ll='ls -la'
```

to:

```text
~/.bashrc
```

Run:

```bash
source ~/.bashrc
```

The alias becomes available in the current shell session.

---

## Summary

`source` runs commands from a file in the current shell environment.

