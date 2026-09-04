# `cut` - Extract Sections from Text

## 1. What is `cut`?

The `cut` command extracts specific sections from each line of text.

It is commonly used to extract:

* Columns
* Fields
* Characters

---

## 2. Extract Characters

Example:

```bash
cut -c 1-5 file.txt
```

This extracts characters 1 through 5 from every line.

---

## 3. Extract Fields

Suppose the file contains:

```text
John:Developer:India
Alice:Engineer:USA
```

Use:

```bash
cut -d ':' -f 1 file.txt
```

Output:

```text
John
Alice
```

---

## 4. Understanding Options

```text
-d → Delimiter
-f → Field
-c → Characters
```

---

## 5. Extract Multiple Fields

```bash
cut -d ':' -f 1,2 file.txt
```

---

## 6. Extract a Column from `/etc/passwd`

Example:

```bash
cut -d ':' -f 1 /etc/passwd
```

This displays usernames.

---

## Quick Reference

```bash
cut -c 1-5 file.txt
cut -d ':' -f 1 file.txt
cut -d ':' -f 1,2 file.txt
cut -d ':' -f 1 /etc/passwd
```

---

## Summary

`cut` extracts specific characters or fields from text.

