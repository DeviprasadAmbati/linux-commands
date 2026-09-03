# `mkdir` - Make Directory

## 1. What is `mkdir`?

`mkdir` stands for **Make Directory**.

It is used to create new directories in Linux.

---

## 2. Basic Syntax

```bash
mkdir DIRECTORY_NAME
```

Example:

```bash
mkdir projects
```

This creates a directory named:

```text
projects
```

---

## 3. Create Multiple Directories

You can create multiple directories in one command:

```bash
mkdir project1 project2 project3
```

---

## 4. Create Nested Directories

Suppose you want to create:

```text
project/
└── src/
    └── python/
```

Use:

```bash
mkdir -p project/src/python
```

The `-p` option creates parent directories automatically.

---

## 5. Create Multiple Nested Directories

```bash
mkdir -p project/{src,docs,tests}
```

This creates:

```text
project/
├── docs/
├── src/
└── tests/
```

---

## 6. Important Options

### `-p` — Create Parent Directories

```bash
mkdir -p project/src/python
```

Without `-p`, the command may fail if the parent directories do not exist.

---

### `-v` — Verbose Output

```bash
mkdir -v test-folder
```

Linux displays information about what was created.

---

## 7. Real-World Examples

### Create a project

```bash
mkdir my-project
```

### Create a project structure

```bash
mkdir -p my-project/src
mkdir -p my-project/tests
mkdir -p my-project/docs
```

### Create multiple folders

```bash
mkdir images videos documents
```

---

## 8. Common Mistakes

### Mistake 1: Directory Already Exists

If the directory already exists:

```bash
mkdir project
```

may display an error.

Using:

```bash
mkdir -p project
```

will not fail if the directory already exists.

---

### Mistake 2: Forgetting Parent Directories

This may fail:

```bash
mkdir project/src/python
```

if `project` does not exist.

Use:

```bash
mkdir -p project/src/python
```

---

## 9. Related Commands

| Command | Purpose                  |
| ------- | ------------------------ |
| `mkdir` | Create directories       |
| `rmdir` | Remove empty directories |
| `cd`    | Change directory         |
| `ls`    | List directories         |

---

## 10. Practice Exercises

1. Create a directory named `practice`.
2. Create three directories in one command.
3. Create a nested directory structure.
4. Use `mkdir -p`.
5. Create a project structure containing `src`, `docs`, and `tests`.

---

## 11. Quick Reference

```bash
mkdir folder
mkdir folder1 folder2 folder3
mkdir -p project/src/python
mkdir -v folder
```

---

## Summary

`mkdir` is used to create directories.

The most important option is:

```bash
mkdir -p
```

It allows you to create nested directory structures safely.

