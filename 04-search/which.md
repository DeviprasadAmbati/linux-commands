# `which` - Find the Location of a Command

## 1. What is `which`?

The `which` command displays the path of an executable command.

It searches the directories listed in your `PATH` environment variable.

---

## 2. Basic Syntax

```bash
which COMMAND
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

## 3. Find Multiple Commands

```bash
which python git ls
```

---

## 4. Understand the `PATH`

Display your `PATH`:

```bash
echo $PATH
```

Linux searches these directories when you run a command.

---

## 5. Real-World Examples

### Find Git

```bash
which git
```

### Find Python

```bash
which python3
```

### Find PostgreSQL client

```bash
which psql
```

---

## 6. Common Mistakes

### Mistake: Using `which` for All Shell Commands

`which` is mainly useful for locating executables found through `PATH`.

For shell built-ins, aliases, or functions, use:

```bash
type COMMAND
```

Example:

```bash
type cd
```

---

## 7. Related Commands

| Command   | Purpose                    |
| --------- | -------------------------- |
| `which`   | Find executable path       |
| `whereis` | Find command-related files |
| `type`    | Identify command type      |
| `find`    | Search file system         |

---

## Practice Exercises

1. Find the location of `git`.
2. Find the location of `python3`.
3. Find the location of `ls`.
4. Run `echo $PATH`.
5. Compare `which cd` and `type cd`.

---

## Quick Reference

```bash
which git
which python3
which ls
echo $PATH
type cd
```

---

## Summary

`which` helps you find the executable location of commands available through your `PATH`.

```bash
which COMMAND
```

