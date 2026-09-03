# `userdel` - Delete a Linux User

## 1. What is `userdel`?

The `userdel` command is used to remove a user account from a Linux system.

This usually requires administrator privileges.

---

## 2. Basic Syntax

```bash
sudo userdel username
```

Example:

```bash
sudo userdel testuser
```

---

## 3. Remove User and Home Directory

```bash
sudo userdel -r username
```

The `-r` option removes the user's home directory and mail spool when applicable.

⚠️ Be careful because user data can be permanently removed.

---

## 4. Verify Before Deleting

Check the user:

```bash
id username
```

Make sure you are deleting the correct account.

---

## 5. Common Mistakes

### Mistake: Removing the Wrong User

Always verify:

```bash
id username
```

before deletion.

---

### Mistake: Using `-r` Without Understanding

```bash
sudo userdel -r username
```

can remove user-related files.

Use it carefully.

---

## Practice Exercises

Create a test user:

```bash
sudo useradd -m testuser
```

Verify:

```bash
id testuser
```

Remove:

```bash
sudo userdel -r testuser
```

Only practice with a test account.

---

## Quick Reference

```bash
sudo userdel username
sudo userdel -r username
id username
```

---

## Summary

`userdel` removes Linux user accounts.

Use `-r` carefully when you also want to remove the user's home directory.

