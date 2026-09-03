# `groups` - Display User Group Membership

## 1. What is `groups`?

The `groups` command displays the groups to which a user belongs.

---

## 2. Check Current User Groups

```bash
groups
```

---

## 3. Check Another User

```bash
groups username
```

Example:

```bash
groups deviprasad
```

---

## 4. Why Are Groups Important?

Groups allow administrators to manage permissions for multiple users.

Instead of assigning permissions individually, users can be placed into a group.

Example:

```text
developers
```

All members of the group can receive appropriate access permissions.

---

## 5. Related Commands

| Command    | Purpose                   |
| ---------- | ------------------------- |
| `groups`   | Display groups            |
| `id`       | User identity information |
| `groupadd` | Create a group            |
| `chgrp`    | Change file group         |

---

## Practice Exercises

```bash
groups
id
id -G
```

Compare the group information.

---

## Summary

Use:

```bash
groups
```

to quickly check group memberships.

