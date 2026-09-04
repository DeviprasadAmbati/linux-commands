# `sed` - Stream Editor for Text Processing

## 1. What is `sed`?

`sed` stands for **Stream Editor**.

It is used to perform text transformations on input.

Common uses include:

* Replacing text
* Deleting lines
* Printing specific lines
* Modifying file content

---

## 2. Basic Syntax

```bash
sed 'command' filename
```

---

## 3. Replace Text

Example:

```bash
sed 's/old/new/' file.txt
```

This replaces the first occurrence of `old` with `new` on each line.

---

## 4. Replace All Occurrences

Use the `g` flag:

```bash
sed 's/old/new/g' file.txt
```

---

## 5. Replace Text and Save Changes

Use:

```bash
sed -i 's/old/new/g' file.txt
```

⚠️ The `-i` option modifies the file directly.

Be careful when using it.

---

## 6. Delete a Specific Line

Example:

```bash
sed '5d' file.txt
```

This removes line 5 from the output.

---

## 7. Print Specific Lines

Print lines 1 through 5:

```bash
sed -n '1,5p' file.txt
```

---

## 8. Use `sed` with Pipes

Example:

```bash
echo "hello world" | sed 's/world/Linux/'
```

Output:

```text
hello Linux
```

---

## 9. Quick Reference

```bash
sed 's/old/new/' file.txt
sed 's/old/new/g' file.txt
sed -i 's/old/new/g' file.txt
sed '5d' file.txt
sed -n '1,5p' file.txt
```

---

## Summary

`sed` is a powerful command for editing and transforming text from the command line.

