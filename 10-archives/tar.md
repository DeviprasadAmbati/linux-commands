# `tar` - Create and Extract Archives

## 1. What is `tar`?

`tar` stands for **Tape Archive**.

The `tar` command is used to combine multiple files and directories into a single archive file.

A `.tar` file is an archive that can contain many files.

---

## 2. Basic Syntax

```bash
tar options archive_name files
```

---

## 3. Create an Archive

Use:

```bash
tar -cvf archive.tar directory/
```

Example:

```bash
tar -cvf project.tar project/
```

### Options

```text
c → Create archive
v → Verbose output
f → Archive filename
```

---

## 4. Extract an Archive

Use:

```bash
tar -xvf archive.tar
```

### Options

```text
x → Extract
v → Verbose output
f → Archive filename
```

---

## 5. View Archive Contents

Use:

```bash
tar -tvf archive.tar
```

This lists the files without extracting them.

---

## 6. Create a Compressed Archive

Using gzip compression:

```bash
tar -czvf archive.tar.gz directory/
```

Explanation:

```text
c → Create
z → Use gzip compression
v → Verbose
f → Filename
```

---

## 7. Extract a Compressed Archive

```bash
tar -xzvf archive.tar.gz
```

---

## 8. Create a `.tar.bz2` Archive

```bash
tar -cjvf archive.tar.bz2 directory/
```

---

## 9. Quick Reference

```bash
# Create archive
tar -cvf archive.tar directory/

# Extract archive
tar -xvf archive.tar

# List archive contents
tar -tvf archive.tar

# Create gzip archive
tar -czvf archive.tar.gz directory/

# Extract gzip archive
tar -xzvf archive.tar.gz
```

---

## Summary

`tar` is one of the most important Linux commands for creating and extracting archives.

