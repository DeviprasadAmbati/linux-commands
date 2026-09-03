# `wc` - Count Lines, Words, and Characters

## 1. What is `wc`?

`wc` stands for **word count**.

It is used to count:

* Lines.
* Words.
* Bytes.
* Characters.

---

## 2. Basic Syntax

```bash
wc FILE_NAME
```

Example:

```bash
wc notes.txt
```

The output normally contains:

```text
lines words bytes filename
```

---

## 3. Count Lines

```bash
wc -l notes.txt
```

---

## 4. Count Words

```bash
wc -w notes.txt
```

---

## 5. Count Characters

```bash
wc -m notes.txt
```

---

## 6. Count Bytes

```bash
wc -c notes.txt
```

---

## 7. Real-World Examples

### Count lines in a log

```bash
wc -l application.log
```

### Count Python source code lines

```bash
wc -l app.py
```

### Count words in a document

```bash
wc -w document.txt
```

---

## 8. Use `wc` with Pipes

Count files:

```bash
ls | wc -l
```

Count matching results:

```bash
grep "error" application.log | wc -l
```

---

## 9. Related Commands

| Command | Purpose         |
| ------- | --------------- |
| `wc`    | Count content   |
| `grep`  | Search text     |
| `cat`   | Display content |
| `sort`  | Sort lines      |

---

## Practice Exercises

1. Create a text file.
2. Count its lines.
3. Count its words.
4. Count its characters.
5. Use `ls | wc -l`.

---

## Quick Reference

```bash
wc file.txt
wc -l file.txt
wc -w file.txt
wc -m file.txt
wc -c file.txt
```

---

## Summary

`wc` is used to count lines, words, bytes, and characters.

The most commonly used option is:

```bash
wc -l file.txt
```

