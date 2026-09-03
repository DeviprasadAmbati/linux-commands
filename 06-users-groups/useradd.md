# `useradd` - Create a New Linux User

## 1. What is `useradd`?

The `useradd` command is used to create a new user account on a Linux system.

This operation usually requires administrator privileges.

---

## 2. Basic Syntax

```bash
sudo useradd username
```

Example:

```bash
sudo useradd john
```

---

## 3. Create a User with a Home Directory

On many systems, use:

```bash
sudo useradd -m john
```

The `-m` option creates the user's home directory if needed.

---

## 4. Specify a Home Directory

```bash
sudo useradd -m -d /home/john john
```

---

## 5. Specify a Login Shell

```bash
sudo useradd -m -s /bin/bash john
```

---

## 6. Add a User to a Group

```bash
sudo useradd -G developers john
```

This creates the user with supplementary group membership as specified.

---

## 7. Set a Password

After creating a user:

```bash
sudo passwd john
```

---

## 8. Verify the User

```bash
id john
```

You can also check account information using system tools appropriate to your distribution.

---

## 9. Common Mistakes

### Mistake: Forgetting `-m`

Without `-m`, behavior regarding home directory creation can depend on system configuration.

When you want a normal user home directory, explicitly using `-m` is a clear approach.

---

## Practice Exercises

Create a test user only on a system where you have administrator permission:

```bash
sudo useradd -m testuser
```

Set a password:

```bash
sudo passwd testuser
```

Verify:

```bash
id testuser
```

Remove the test account when finished using the appropriate user management command.

---

## Quick Reference

```bash
sudo useradd username
sudo useradd -m username
sudo useradd -m -s /bin/bash username
sudo useradd -G group username
sudo passwd username
```

---

## Summary

`useradd` creates Linux user accounts.

A common command is:

```bash
sudo useradd -m username
```

