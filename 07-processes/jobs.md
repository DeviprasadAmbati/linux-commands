# `jobs` - Display Shell Jobs

## 1. What is `jobs`?

The `jobs` command displays jobs that are running or stopped in the current shell session.

A shell job is different from the system-wide process list.

---

## 2. Basic Syntax

```bash
jobs
```

---

## 3. Create a Background Job

Run:

```bash
sleep 300 &
```

The `&` sends the command to the background.

Check jobs:

```bash
jobs
```

---

## 4. Example Output

```text
[1]+ Running sleep 300 &
```

Where:

```text
[1] → Job number
Running → Job status
```

---

## 5. Useful Options

### Show Process IDs

```bash
jobs -l
```

This displays process IDs associated with jobs.

---

## 6. Stop a Job

Bring the job to the foreground:

```bash
fg %1
```

You can then stop or manage it.

---

## 7. Related Commands

| Command | Purpose                    |
| ------- | -------------------------- |
| `jobs`  | Display shell jobs         |
| `bg`    | Continue job in background |
| `fg`    | Bring job to foreground    |
| `kill`  | Send signals to processes  |

---

## Quick Reference

```bash
jobs
jobs -l
sleep 300 &
fg %1
```

---

## Summary

`jobs` displays background and stopped jobs belonging to the current shell session.

