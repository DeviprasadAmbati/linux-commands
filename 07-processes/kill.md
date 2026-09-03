# `kill` - Send Signals to Processes

## 1. What is `kill`?

The `kill` command sends a signal to a process.

Despite its name, `kill` is not limited to terminating processes.

The default signal requests that the process terminate gracefully.

---

## 2. Basic Syntax

```bash
kill PID
```

Example:

```bash
kill 1234
```

---

## 3. Find the Process ID

Use:

```bash
ps aux
```

or:

```bash
ps aux | grep process_name
```

Then identify the PID.

---

## 4. Common Signals

| Signal    | Number | Purpose                      |
| --------- | -----: | ---------------------------- |
| `SIGTERM` |   `15` | Request graceful termination |
| `SIGKILL` |    `9` | Force termination            |
| `SIGHUP`  |    `1` | Hangup/reload-related signal |

---

## 5. Gracefully Stop a Process

```bash
kill PID
```

or:

```bash
kill -15 PID
```

---

## 6. Force Stop a Process

```bash
kill -9 PID
```

⚠️ `SIGKILL` cannot be handled or ignored by the target process and may prevent normal cleanup.

Use it only when a normal termination request does not work.

---

## 7. List Available Signals

```bash
kill -l
```

---

## 8. Real-World Example

Suppose a process has PID:

```text
4321
```

First try:

```bash
kill 4321
```

If necessary:

```bash
kill -9 4321
```

---

## 9. Practice Exercise

Start a command:

```bash
sleep 300
```

Open another terminal and find it:

```bash
ps aux | grep sleep
```

Then stop it using its PID.

---

## Quick Reference

```bash
kill PID
kill -15 PID
kill -9 PID
kill -l
```

---

## Summary

`kill` sends signals to processes.

Always try graceful termination first before using:

```bash
kill -9 PID
```

