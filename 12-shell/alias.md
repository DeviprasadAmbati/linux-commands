# `alias` - Create Command Shortcuts

## 1. What is an Alias?

An alias is a shortcut for a command.

It allows you to create shorter or customized commands.

---

## 2. Create an Alias

Example:

```bash
alias ll='ls -la'
```

Now you can run:

```bash
ll
```

instead of:

```bash
ls -la
```

---

## 3. Display All Aliases

```bash
alias
```

---

## 4. Remove an Alias

```bash
unalias ll
```

---

## 5. Make an Alias Permanent

Aliases created in the terminal are usually temporary.

For Bash, you can add aliases to:

```text
~/.bashrc
```

Example:

```bash
vim ~/.bashrc
```

Add:

```bash
alias ll='ls -la'
```

Then reload:

```bash
source ~/.bashrc
```

---

## Summary

`alias` allows you to create shortcuts for frequently used commands.

