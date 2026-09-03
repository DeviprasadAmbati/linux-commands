# `scp` - Securely Copy Files Between Systems

## 1. What is `scp`?

`scp` stands for **Secure Copy**.

It is used to copy files securely between computers using SSH.

---

## 2. Basic Syntax

```bash
scp source destination
```

---

## 3. Copy a File to a Remote Server

```bash
scp file.txt username@server:/home/username/
```

Example:

```bash
scp project.zip devuser@192.168.1.10:/home/devuser/
```

---

## 4. Copy a File from a Remote Server

```bash
scp username@server:/home/username/file.txt .
```

The `.` means the current directory.

---

## 5. Copy a Directory

Use the `-r` option:

```bash
scp -r project/ username@server:/home/username/
```

---

## 6. Specify a Different SSH Port

Use uppercase `P`:

```bash
scp -P 2222 file.txt username@server:/home/username/
```

---

## 7. Common Uses

```bash
# Upload file
scp file.txt user@server:/path/

# Download file
scp user@server:/path/file.txt .

# Copy directory
scp -r directory/ user@server:/path/
```

---

## Summary

`scp` securely copies files between systems using SSH.

