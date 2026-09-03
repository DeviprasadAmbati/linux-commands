# `passwd` - Manage User Passwords

## 1. What is `passwd`?

The `passwd` command is primarily used to change a user's password.

It can also be used by administrators for certain password and account management tasks.

---

## 2. Change Your Own Password

Run:

```bash
passwd
```

You will typically be asked to enter:

1. Your current password.
2. Your new password.
3. Your new password again.

---

## 3. Change Another User's Password

An administrator can typically run:

```bash
sudo passwd username
```

Example:

```bash
sudo passwd john
```

---

## 4. Lock a User Password

Administrators can lock password authentication for an account:

```bash
sudo passwd -l username
```

This does not necessarily disable every possible login method, such as SSH keys or other authentication mechanisms.

---

## 5. Unlock a User Password

```bash
sudo passwd -u username
```

---

## 6. Check Password Status

```bash
sudo passwd -S username
```

This displays password status information.

---

## 7. Important Security Practices

* Use strong passwords.
* Do not share passwords.
* Avoid using passwords in scripts.
* Use appropriate access controls.
* Lock or disable unused accounts according to your organization's policies.

---

## Practice Exercises

Change your own password only if you intend to:

```bash
passwd
```

For learning, use a test user on a safe system where you have administrator privileges.

---

## Quick Reference

```bash
# Change your password
passwd

# Change another user's password
sudo passwd username

# Lock password authentication
sudo passwd -l username

# Unlock password authentication
sudo passwd -u username

# Check password status
sudo passwd -S username
```

---

## Summary

`passwd` is used to manage passwords for Linux user accounts.

The most common command is:

```bash
passwd
```

Administrators can manage other users with:

```bash
sudo passwd username
```

