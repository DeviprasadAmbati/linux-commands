# `wget` - Download Files from the Internet

## 1. What is `wget`?

`wget` stands for **Web Get**.

It is a command-line tool used to download files from web servers.

---

## 2. Basic Syntax

```bash
wget URL
```

Example:

```bash
wget https://example.com/file.zip
```

---

## 3. Download and Save with a Custom Name

```bash
wget -O filename URL
```

Example:

```bash
wget -O application.zip https://example.com/file.zip
```

---

## 4. Continue a Download

Use:

```bash
wget -c URL
```

The `-c` option attempts to continue a partially downloaded file.

---

## 5. Download in the Background

```bash
wget -b URL
```

This runs the download in the background.

---

## 6. Download Multiple Files

Create a file containing URLs:

```text
https://example.com/file1.zip
https://example.com/file2.zip
```

Then run:

```bash
wget -i urls.txt
```

---

## 7. `wget` vs `curl`

| Tool   | Common Use                  |
| ------ | --------------------------- |
| `wget` | Download files              |
| `curl` | Transfer data and test APIs |

Both tools are powerful and have overlapping capabilities.

---

## Quick Reference

```bash
wget URL
wget -O filename URL
wget -c URL
wget -b URL
wget -i urls.txt
```

---

## Summary

`wget` is commonly used for downloading files from the command line.

