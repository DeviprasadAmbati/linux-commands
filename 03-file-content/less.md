# `less` - View File Contents Page by Page

## 1. What is `less`?

The `less` command is used to view text files one page at a time.

It is especially useful for:

* Large files.
* Log files.
* Configuration files.
* Long command output.

Unlike `cat`, `less` does not print the entire file at once.

---

## 2. Basic Syntax

```bash
less FILE_NAME
```

Example:

```bash
less large-file.txt
```

---

## 3. Navigation Inside `less`

| Key     | Action            |
| ------- | ----------------- |
| `Space` | Next page         |
| `b`     | Previous page     |
| `Enter` | Next line         |
| `g`     | Beginning of file |
| `G`     | End of file       |
| `q`     | Quit              |

---

## 4. Search Inside a File

Press:

```text
/word
```

Then press Enter.

Example:

```text
/error
```

Press:

```text
n
```

to move to the next matching result.

Press:

```text
N
```

to move to the previous matching result.

---

## 5. Real-World Examples

### View a large log file

```bash
less application.log
```

### View a configuration file

```bash
less /etc/passwd
```

### View command output

```bash
ls -la | less
```

This allows you to read long output page by page.

---

## 6. Common Mistakes

### Mistake: Forgetting How to Exit

Press:

```text
q
```

to quit `less`.

---

## 7. Related Commands

| Command | Purpose                |
| ------- | ---------------------- |
| `cat`   | Display entire file    |
| `less`  | View file page by page |
| `more`  | Basic paginated viewer |
| `head`  | View beginning         |
| `tail`  | View end               |

---

## Practice Exercises

1. Open a large text file using `less`.
2. Navigate using Space and `b`.
3. Search for a word.
4. Move to the beginning using `g`.
5. Move to the end using `G`.
6. Exit using `q`.

---

## Quick Reference

```bash
less file.txt
ls -la | less
```

Inside `less`:

```text
Space → Next page
b     → Previous page
g     → Beginning
G     → End
/word → Search
n     → Next result
q     → Quit
```

---

## Summary

Use `less` when working with large files or long output.

```bash
less file.txt
```

