# `fg` - Bring a Job to the Foreground

## 1. What is `fg`?

The `fg` command brings a background or stopped job into the foreground.

---

## 2. Basic Usage

First check:

```bash
jobs
```

Then run:

```bash
fg
```

This brings the most recent job to the foreground.

---

## 3. Bring a Specific Job

```bash
fg %1
```

This brings job number `1` to the foreground.

---

## 4. Example Workflow

Start:

```bash
sleep 300
```

Press:

```text
Ctrl + Z
```

Check:

```bash
jobs
```

Resume in the background:

```bash
bg
```

Bring it back:

```bash
fg
```

---

## 5. Related Commands

| Command | Purpose        |
| ------- | -------------- |
| `fg`    | Foreground job |
| `bg`    | Background job |
| `jobs`  | Display jobs   |

---

## Quick Reference

```bash
jobs
fg
fg %1
```

---

## Summary

`fg` brings shell jobs into the foreground so they interact directly with the terminal.

