# `killall` - Terminate Processes by Name

## 1. What is `killall`?

The `killall` command sends signals to processes based on their process name.

Unlike `kill`, which usually targets a PID, `killall` targets matching process names.

---

## 2. Basic Syntax

```bash
killall process_name
```

Example:

```bash
killall firefox
```

This sends the default termination signal to matching processes named `firefox`.

---

## 3. Send a Specific Signal

```bash
killall -9 process_name
```

Example:

```bash
killall -9 firefox
```

⚠️ Use forceful termination carefully.

---

## 4. Ask for Confirmation

```bash
killall -i process_name
```

The `-i` option asks for confirmation before acting on each process.

---

## 5. Why Be Careful?

If multiple processes have the same name, `killall` can affect all matching processes.

Always verify the target process first.

Use:

```bash
ps aux | grep process_name
```

---

## 6. Related Commands

| Command   | Purpose                       |
| --------- | ----------------------------- |
| `kill`    | Send a signal using PID       |
| `killall` | Send a signal by process name |
| `ps`      | View processes                |
| `top`     | Monitor processes             |

---

## 7. Quick Reference

```bash
killall process_name
killall -9 process_name
killall -i process_name
```

---

## Summary

`killall` can manage processes by name and should be used carefully when multiple matching processes may exist.

