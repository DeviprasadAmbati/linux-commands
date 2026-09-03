# `ps` - Display Running Processes

## 1. What is `ps`?

`ps` stands for **process status**.

The `ps` command displays information about currently running processes.

A **process** is a program that is currently running on the Linux system.

For example, when you run:

```bash
python app.py
```

Linux creates a process for the Python program.

---

## 2. Basic Syntax

```bash
ps
```

This displays processes associated with the current terminal session.

---

## 3. Display All Processes

A commonly used command is:

```bash
ps aux
```

This displays processes for all users.

The output can include:

* User
* Process ID (PID)
* CPU usage
* Memory usage
* Process status
* Command

---

## 4. Understanding Process ID

Every running process has a unique number called a **PID**.

Example:

```text
PID
1234
```

The PID is useful when managing or stopping a process.

For example:

```bash
kill 1234
```

---

## 5. Common Options

### `ps aux`

```bash
ps aux
```

Displays detailed information about processes from all users.

### `ps -ef`

```bash
ps -ef
```

Another commonly used format for displaying system processes.

---

## 6. Find a Specific Process

You can combine `ps` with `grep`:

```bash
ps aux | grep nginx
```

This searches the process list for `nginx`.

---

## 7. Real-World Examples

Check whether PostgreSQL is running:

```bash
ps aux | grep postgres
```

Check Python processes:

```bash
ps aux | grep python
```

---

## 8. Useful Related Commands

| Command | Purpose            |
| ------- | ------------------ |
| `ps`    | Display processes  |
| `top`   | Monitor processes  |
| `kill`  | Stop a process     |
| `jobs`  | Display shell jobs |

---

## 9. Practice Exercises

Try:

```bash
ps
```

Then:

```bash
ps aux
```

Try finding your shell:

```bash
ps aux | grep bash
```

---

## 10. Quick Reference

```bash
ps
ps aux
ps -ef
ps aux | grep process_name
```

---

## Summary

`ps` is used to view information about running processes.

The most commonly used commands are:

```bash
ps aux
ps -ef
```

