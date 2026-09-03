# `top` - Monitor Running Processes

## 1. What is `top`?

`top` is an interactive Linux command used to monitor running processes in real time.

It displays information about:

* CPU usage
* Memory usage
* Running processes
* Process IDs
* System load

---

## 2. Basic Syntax

```bash
top
```

The display updates automatically.

---

## 3. Understanding the Information

The top section typically displays:

* System uptime
* Number of users
* Load average
* CPU usage
* Memory usage

The lower section displays running processes.

---

## 4. Important Columns

| Column    | Meaning         |
| --------- | --------------- |
| `PID`     | Process ID      |
| `USER`    | Process owner   |
| `%CPU`    | CPU usage       |
| `%MEM`    | Memory usage    |
| `COMMAND` | Running command |

---

## 5. Useful Keyboard Commands

While `top` is running:

| Key | Action               |
| --- | -------------------- |
| `q` | Quit                 |
| `k` | Kill a process       |
| `P` | Sort by CPU usage    |
| `M` | Sort by memory usage |

---

## 6. Monitor a Specific User

```bash
top -u username
```

Example:

```bash
top -u deviprasad
```

---

## 7. Real-World Uses

Use `top` when:

* Your system is slow.
* CPU usage is high.
* Memory usage is high.
* You want to identify resource-heavy processes.

---

## 8. Related Commands

| Command | Purpose                      |
| ------- | ---------------------------- |
| `top`   | Real-time process monitoring |
| `ps`    | Process information          |
| `htop`  | Interactive process viewer   |
| `kill`  | Stop a process               |

---

## 9. Quick Reference

```bash
top
top -u username
```

Inside `top`:

```text
q → Quit
P → Sort by CPU
M → Sort by Memory
k → Kill process
```

---

## Summary

`top` provides real-time information about Linux processes and system resource usage.

