# `id` - Display User and Group Identity

## 1. What is `id`?

The `id` command displays identity information about a user.

It can show:

* User ID (UID).
* Primary Group ID (GID).
* Username.
* Group memberships.

---

## 2. Basic Syntax

```bash
id
```

Example output may look like:

```text
uid=1000(deviprasad) gid=1000(deviprasad) groups=1000(deviprasad),27(sudo)
```

---

## 3. Check Another User

```bash
id username
```

Example:

```bash
id deviprasad
```

---

## 4. Display User ID Only

```bash
id -u
```

---

## 5. Display Group ID

```bash
id -g
```

---

## 6. Display Groups

```bash
id -G
```

---

## 7. Real-World Uses

`id` is useful for:

* Checking Linux user IDs.
* Debugging permission problems.
* Checking group membership.
* System administration.

---

## Quick Reference

```bash
id
id username
id -u
id -g
id -G
```

---

## Summary

`id` provides detailed information about a user's identity and group memberships.

