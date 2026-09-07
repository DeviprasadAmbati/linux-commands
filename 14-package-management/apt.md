# `apt` - Advanced Package Management Tool

## 1. What is `apt`?

`apt` is a package management command used on Debian and Ubuntu-based Linux distributions.

It is used to:

* Install software
* Remove software
* Update package information
* Upgrade installed packages
* Search for packages

---

## 2. Update Package Information

Run:

```bash
sudo apt update
```

This downloads the latest package information from configured repositories.

It does not normally upgrade installed packages by itself.

---

## 3. Upgrade Installed Packages

Use:

```bash
sudo apt upgrade
```

This upgrades installed packages to newer available versions.

---

## 4. Install a Package

Example:

```bash
sudo apt install nginx
```

This installs the `nginx` package.

---

## 5. Remove a Package

Use:

```bash
sudo apt remove nginx
```

This removes the package but may keep some configuration files.

---

## 6. Completely Remove a Package

Use:

```bash
sudo apt purge nginx
```

This removes the package and its system-wide configuration files.

---

## 7. Search for a Package

```bash
apt search nginx
```

---

## 8. Display Package Information

```bash
apt show nginx
```

---

## 9. Recommended Update Workflow

A common workflow is:

```bash
sudo apt update
sudo apt upgrade
```

---

## Quick Reference

```bash
sudo apt update
sudo apt upgrade
sudo apt install package-name
sudo apt remove package-name
sudo apt purge package-name
apt search package-name
apt show package-name
```

---

## Summary

`apt` is the primary package management command on modern Debian and Ubuntu-based Linux systems.

