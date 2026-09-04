# `wc` - Count Lines, Words, and Characters

## 1. What is `wc`?

`wc` stands for **Word Count**.

It counts information in files such as:

* Lines
* Words
* Characters
* Bytes

---

## 2. Basic Syntax

```bash
wc file.txt
```

---

## 3. Count Lines

```bash
wc -l file.txt
```

---

## 4. Count Words

```bash
wc -w file.txt
```

---

## 5. Count Characters

```bash
wc -m file.txt
```

---

## 6. Count Bytes

```bash
wc -c file.txt
```

---

## 7. Use with Pipes

Example:

```bash
ls | wc -l
```

This counts the number of lines produced by `ls`.

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

`wc` counts lines, words, characters, and bytes.

