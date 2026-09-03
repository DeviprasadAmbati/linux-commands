# `bg` - Run a Job in the Background

## 1. What is `bg`?

The `bg` command resumes a stopped job and continues running it in the background.

---

## 2. How to Create a Stopped Job

Start a command:

```bash
sleep 300
```

Press:

```text
Ctrl + Z
```

This stops the job.

---

## 3. Run the Job in the Background

Use:

```bash
bg
```

---

## 4. Run a Specific Job

First check:

```bash
jobs
```

Then:

```bash
bg %1
```

This resumes job number `1` in the background.

---

## 5. Background vs Foreground

### Foreground

The terminal waits for the command to finish.

### Background

The command runs while you can continue using the terminal.

---

## 6. Related Commands

| Command | Purpose                    |
| ------- | -------------------------- |
| `bg`    | Continue job in background |
| `fg`    | Bring job to foreground    |
| `jobs`  | Display jobs               |

---

## Quick Reference

```bash
Ctrl + Z
bg
jobs
bg %1
```

---

## Summary

`bg` resumes stopped shell jobs and runs them in the background.

