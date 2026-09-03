# `zip` - Create ZIP Archives

## 1. What is `zip`?

The `zip` command creates compressed ZIP archives.

ZIP files are commonly used because they are supported by Linux, Windows, and macOS.

---

## 2. Create a ZIP File

```bash
zip archive.zip file.txt
```

Example:

```bash
zip project.zip project.txt
```

---

## 3. Add Multiple Files

```bash
zip archive.zip file1.txt file2.txt file3.txt
```

---

## 4. Compress a Directory

Use the `-r` option:

```bash
zip -r archive.zip directory/
```

Example:

```bash
zip -r project.zip project/
```

The `-r` option recursively includes files and subdirectories.

---

## 5. View ZIP Contents

You can use:

```bash
unzip -l archive.zip
```

---

## Quick Reference

```bash
zip archive.zip file.txt
zip archive.zip file1.txt file2.txt
zip -r archive.zip directory/
```

---

## Summary

`zip` creates compressed ZIP archives and is commonly used for cross-platform file sharing.

