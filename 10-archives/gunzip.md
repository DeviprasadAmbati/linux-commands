# `gunzip` - Decompress Gzip Files

## 1. What is `gunzip`?

`gunzip` is used to decompress files created with `gzip`.

It is commonly used with files ending in:

```text
.gz
```

---

## 2. Basic Syntax

```bash
gunzip filename.gz
```

Example:

```bash
gunzip file.txt.gz
```

This decompresses the file.

---

## 3. Keep the Compressed File

Use:

```bash
gunzip -k file.txt.gz
```

This keeps the original compressed `.gz` file.

---

## 4. Alternative Command

You can also use:

```bash
gzip -d file.txt.gz
```

Both commands can be used for decompression.

---

## 5. Decompress Multiple Files

```bash
gunzip file1.gz file2.gz
```

---

## Quick Reference

```bash
gunzip file.txt.gz
gunzip -k file.txt.gz
gzip -d file.txt.gz
```

---

## Summary

`gunzip` decompresses files that were compressed using `gzip`.

