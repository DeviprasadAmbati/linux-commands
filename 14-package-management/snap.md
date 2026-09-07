# `snap` - Manage Snap Packages

## 1. What is `snap`?

`snap` is a package management system used on many Linux distributions.

Snap packages are designed to bundle applications and their dependencies.

---

## 2. List Installed Snap Packages

```bash
snap list
```

---

## 3. Search for a Package

Example:

```bash
snap find code
```

---

## 4. Install a Package

Example:

```bash
sudo snap install code --classic
```

The `--classic` option is required for some applications that need broader system access.

---

## 5. Remove a Package

```bash
sudo snap remove code
```

---

## 6. Update Snap Packages

```bash
sudo snap refresh
```

---

## 7. Display Package Information

```bash
snap info code
```

---

## Quick Reference

```bash
snap list
snap find package-name
sudo snap install package-name
sudo snap remove package-name
sudo snap refresh
snap info package-name
```

---

## Summary

`snap` is used to install and manage Snap packages on supported Linux systems.

