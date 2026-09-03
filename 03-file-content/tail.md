# `tail` - Display the End of a File

## 1. What is `tail`?

The `tail` command displays the last lines of a file.

By default, it displays the last **10 lines**.

---

## 2. Basic Syntax

```bash
tail FILE_NAME
```

Example:

```bash
tail application.log
```

---

## 3. Display Specific Number of Lines

```bash
tail -n 20 application.log
```

Displays the last 20 lines.

---

## 4. Follow a File in Real Time

One of the most useful options is:

```bash
tail -f application.log
```

This continuously displays new lines added to the file.

Press:

```text
CTRL + C
```

to stop.

---

## 5. Real-World Examples

### Monitor an application log

```bash
tail -f application.log
```

### View the last 50 lines

```bash
tail -n 50 application.log
```

### Monitor a system log

```bash
tail -f /var/log/syslog
```

The exact log file may differ depending on your Linux distribution.

---

## 6. Common Mistakes

### Mistake: Forgetting to Stop `tail -f`

Use:

```text
CTRL + C
```

to stop following the file.

---

## 7. Related Commands

| Command | Purpose           |
| ------- | ----------------- |
| `head`  | Beginning of file |
| `tail`  | End of file       |
| `less`  | View files        |
| `cat`   | Display files     |

---

## Practice Exercises

1. Create a text file with multiple lines.
2. Run `tail file.txt`.
3. Run `tail -n 5 file.txt`.
4. Open another terminal.
5. Run `tail -f file.txt`.
6. Add new lines and observe them.

---

## Quick Reference

```bash
tail file.txt
tail -n 5 file.txt
tail -n 50 file.txt
tail -f application.log
```

---

## Summary

`tail` displays the end of files.

The most useful commands are:

```bash
tail -n 20 file.txt
tail -f application.log
```

