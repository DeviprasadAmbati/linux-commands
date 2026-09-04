# `history` - Display Command History

## 1. What is `history`?

The `history` command displays commands previously executed in the current shell history.

---

## 2. Display Command History

```bash
history
```

---

## 3. Display Recent Commands

```bash
history 10
```

This displays the last 10 commands.

---

## 4. Search Command History

You can combine it with `grep`:

```bash
history | grep git
```

---

## 5. Run a Previous Command

If history shows:

```text
100  git status
```

You can run it again using:

```bash
!100
```

---

## 6. Run the Previous Command

Use:

```bash
!!
```

This repeats the previous command.

Use this carefully because it immediately executes the previous command.

---

## Summary

`history` helps you view and reuse previously executed shell commands.

