# `uptime` - Display System Running Time

## 1. What is `uptime`?

The `uptime` command displays how long the system has been running since the last boot.

It also displays:

* Current time
* Number of logged-in users
* System load average

---

## 2. Basic Syntax

```bash
uptime
```

Example output:

```text
18:00:00 up 2 days, 4:30, 2 users, load average: 0.20, 0.15, 0.10
```

---

## 3. Understanding the Output

```text
up 2 days, 4:30
```

This means the system has been running for:

```text
2 days and 4 hours 30 minutes
```

---

## 4. Load Average

Example:

```text
load average: 0.20, 0.15, 0.10
```

These values generally represent average system load over:

* 1 minute
* 5 minutes
* 15 minutes

---

## 5. Human-Friendly Output

Use:

```bash
uptime -p
```

Example:

```text
up 2 days, 4 hours, 30 minutes
```

---

## 6. Check System Boot Time

Use:

```bash
uptime -s
```

This displays the system startup time.

---

## Quick Reference

```bash
uptime
uptime -p
uptime -s
```

---

## Summary

`uptime` shows how long the Linux system has been running and provides load average information.

