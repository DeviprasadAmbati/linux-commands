# `gzip` - Compress Files

## 1. What is `gzip`?

`gzip` is a Linux command used to compress files.

It reduces the size of files and creates compressed files with the `.gz` extension.

---

## 2. Basic Syntax

```bash
gzip filename
```

Example:

```bash
gzip file.txt
```

This creates:

```text
file.txt.gz
```

The original file is normally replaced by the compressed version.

---

## 3. Keep the Original File

Use:

```bash
gzip -k file.txt
```

The `-k` option keeps the original file.

---

## 4. View Compression Information

Use:

```bash
gzip -v file.txt
```

The `-v` option displays detailed compression information.

---

## 5. Compress Multiple Files

```bash
gzip file1.txt file2.txt file3.txt
```

Each file is compressed separately.

---

## 6. Important Note

`gzip` compresses individual files.

To archive multiple files and directories together, `tar` is commonly used first.

Example:

```bash
tar -czvf project.tar.gz project/
```

---

## Quick Reference

```bash
gzip file.txt
gzip -k file.txt
gzip -v file.txt
```

---

## Summary

`gzip` compresses files and typically creates files ending with:

```text
.gz
```

