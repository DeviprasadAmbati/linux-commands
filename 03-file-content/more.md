# `more` - View File Contents Page by Page

## 1. What is `more`?

The `more` command displays file contents one screen at a time.

It is useful when a file is too large to comfortably display using `cat`.

---

## 2. Basic Syntax

```bash
more FILE_NAME
```

Example:

```bash
more notes.txt
```

---

## 3. Basic Navigation

| Key     | Action    |
| ------- | --------- |
| `Space` | Next page |
| `Enter` | Next line |
| `q`     | Quit      |

---

## 4. `more` vs `less`

| Feature             | `more`  | `less`   |
| ------------------- | ------- | -------- |
| Forward navigation  | Yes     | Yes      |
| Backward navigation | Limited | Yes      |
| Search              | Basic   | Advanced |
| Large files         | Good    | Better   |

In most modern Linux environments, `less` is generally preferred.

---

## 5. Real-World Example

```bash
more /etc/passwd
```

You can also use it with command output:

```bash
ls -la | more
```

---

## 6. Related Commands

| Command | Purpose              |
| ------- | -------------------- |
| `cat`   | Display all content  |
| `more`  | Display page by page |
| `less`  | Advanced file viewer |

---

## Practice Exercises

1. Open a text file using `more`.
2. Move to the next page.
3. Exit using `q`.
4. Compare `more` with `less`.

---

## Summary

`more` is a simple command for viewing long text page by page.

For more powerful navigation, consider using:

```bash
less file.txt
```

