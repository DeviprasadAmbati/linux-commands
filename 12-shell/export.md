# `export` - Set Environment Variables

## 1. What is `export`?

The `export` command marks a shell variable so that it is available to child processes.

It is commonly used to create environment variables.

---

## 2. Create an Environment Variable

```bash
export NAME="Deviprasad"
```

Check it:

```bash
echo $NAME
```

---

## 3. Set the `PATH`

Example:

```bash
export PATH=$PATH:/new/path
```

This adds a directory to the existing `PATH`.

---

## 4. Temporary Environment Variables

Variables created using `export` normally exist only for the current shell session unless they are configured in shell startup files.

---

## 5. Make Variables Persistent

For Bash, add the export command to:

```text
~/.bashrc
```

Example:

```bash
export NAME="Deviprasad"
```

Reload:

```bash
source ~/.bashrc
```

---

## Summary

`export` creates environment variables that can be inherited by child processes.

