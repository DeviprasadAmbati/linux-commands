# `tr` - Translate or Delete Characters

## 1. What is `tr`?

`tr` stands for **translate**.

It is used to replace, delete, or transform characters from standard input.

---

## 2. Convert Lowercase to Uppercase

```bash
echo "hello" | tr 'a-z' 'A-Z'
```

Output:

```text
HELLO
```

---

## 3. Convert Uppercase to Lowercase

```bash
echo "HELLO" | tr 'A-Z' 'a-z'
```

Output:

```text
hello
```

---

## 4. Replace Characters

Example:

```bash
echo "hello world" | tr ' ' '_'
```

Output:

```text
hello_world
```

---

## 5. Delete Characters

Use:

```bash
echo "hello123" | tr -d '0-9'
```

Output:

```text
hello
```

---

## 6. Remove Repeated Characters

Use:

```bash
echo "helloooo" | tr -s 'o'
```

Output:

```text
hello
```

The `-s` option squeezes repeated characters.

---

## Quick Reference

```bash
tr 'a-z' 'A-Z'
tr 'A-Z' 'a-z'
tr ' ' '_'
tr -d '0-9'
tr -s 'o'
```

---

## Summary

`tr` is used to translate, delete, and transform characters in text streams.

