# `groupadd` - Create a Linux Group

## 1. What is `groupadd`?

The `groupadd` command is used to create a new group on a Linux system.

Groups are used to manage permissions and access for multiple users.

---

## 2. Basic Syntax

```bash
sudo groupadd groupname
```

Example:

```bash
sudo groupadd developers
```

---

## 3. Verify a Group

You can check group information using:

```bash
getent group developers
```

---

## 4. Add Users to a Group

A user can be added to a supplementary group using:

```bash
sudo usermod -aG developers username
```

The `-aG` options append the user to the specified supplementary group.

---

## 5. Why Use Groups?

Suppose you have:

```text
developer1
developer2
developer3
```

Instead of managing permissions individually, create:

```text
developers
```

and manage access through the group.

---

## Practice Exercises

Create a test group:

```bash
sudo groupadd testgroup
```

Verify:

```bash
getent group testgroup
```

---

## Quick Reference

```bash
sudo groupadd groupname
getent group groupname
sudo usermod -aG groupname username
```

---

## Summary

`groupadd` creates Linux groups that can be used to manage access and permissions for multiple users.

