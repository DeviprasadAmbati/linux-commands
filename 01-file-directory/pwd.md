# `pwd` - Print Working Directory

## 1. What is `pwd`?

`pwd` stands for **Print Working Directory**.

It is a Linux command used to display the complete path of the directory you are currently working in.

---

## 2. Why do we use `pwd`?

When working in the Linux terminal, you may move between many directories using the `cd` command.

The `pwd` command helps you answer:

> **Where am I currently located in the Linux file system?**

It displays your current directory's absolute path.

---

## 3. Basic Syntax

```bash
pwd
```

---

## 4. Example

Suppose you are currently inside:

```text
/home/deviprasad/linux-commands
```

Run:

```bash
pwd
```

Output:

```text
/home/deviprasad/linux-commands
```

This tells you exactly where you are in the Linux file system.

---

## 5. Understanding the Output

Example:

```text
/home/deviprasad/linux-commands
```

Let's break it down:

```text
/
│
└── home
    │
    └── deviprasad
        │
        └── linux-commands
```

* `/` → Root directory
* `home` → Contains user home directories
* `deviprasad` → Your user home directory
* `linux-commands` → Your current project directory

---

## 6. Why is `pwd` Important?

The terminal does not always make it obvious where you are.

For example, before running commands like:

```bash
rm
```

```bash
mv
```

```bash
cp
```

you should know your current directory.

You can check it using:

```bash
pwd
```

This helps prevent accidentally modifying or deleting files in the wrong location.

---

## 7. Real-World Examples

### Example 1: Check your current location

```bash
pwd
```

Output:

```text
/home/deviprasad
```

---

### Example 2: After changing directories

```bash
cd Documents
```

Now run:

```bash
pwd
```

Output:

```text
/home/deviprasad/Documents
```

---

### Example 3: Inside a project

```bash
cd ~/linux-commands
```

Then:

```bash
pwd
```

Output:

```text
/home/deviprasad/linux-commands
```

---

## 8. `pwd` Options

### `pwd -L`

Displays the logical current directory path.

```bash
pwd -L
```

This is the default behavior in many shells.

---

### `pwd -P`

Displays the physical path by resolving symbolic links.

```bash
pwd -P
```

This is useful when your current directory contains symbolic links.

---

## 9. Logical vs Physical Path

Suppose:

```text
/home/deviprasad/project-link
```

is a symbolic link pointing to:

```text
/var/projects/linux-project
```

Using:

```bash
pwd -L
```

might display:

```text
/home/deviprasad/project-link
```

Using:

```bash
pwd -P
```

might display:

```text
/var/projects/linux-project
```

---

## 10. Common Mistakes

### Mistake 1: Confusing `pwd` with `cd`

`pwd`:

```bash
pwd
```

Only displays your current location.

It does not change your directory.

To change directories, use:

```bash
cd
```

---

### Mistake 2: Thinking `pwd` lists files

`pwd` does not show files.

To list files and directories, use:

```bash
ls
```

---

## 11. Related Commands

| Command | Purpose                     |
| ------- | --------------------------- |
| `pwd`   | Show current directory      |
| `ls`    | List files and directories  |
| `cd`    | Change directory            |
| `mkdir` | Create a directory          |
| `tree`  | Display directory structure |

---

## 12. Practice Exercises

### Beginner

1. Open your terminal.
2. Run:

```bash
pwd
```

3. Change to your home directory:

```bash
cd ~
```

4. Run:

```bash
pwd
```

5. Change to your `linux-commands` project.

6. Run:

```bash
pwd
```

---

### Intermediate

1. Create a symbolic link to a directory.
2. Enter the symbolic link directory.
3. Run:

```bash
pwd -L
```

4. Run:

```bash
pwd -P
```

5. Compare the outputs.

---

## 13. Quick Reference

```bash
# Show current directory
pwd

# Show logical path
pwd -L

# Show physical path
pwd -P
```

---

## Summary

The `pwd` command stands for **Print Working Directory**.

It is used to display your current location in the Linux file system.

The most important command to remember is:

```bash
pwd
```

Use `pwd` whenever you want to know:

> **Where am I currently working?**

