# `dpkg` - Debian Package Manager

## 1. What is `dpkg`?

`dpkg` is the low-level package management system used by Debian-based Linux distributions.

It works directly with `.deb` package files.

---

## 2. Install a `.deb` Package

Example:

```bash
sudo dpkg -i package.deb
```

---

## 3. List Installed Packages

```bash
dpkg -l
```

---

## 4. Search for an Installed Package

Example:

```bash
dpkg -l | grep nginx
```

---

## 5. Display Package Information

```bash
dpkg -s package-name
```

---

## 6. Find Which Package Owns a File

Example:

```bash
dpkg -S /usr/bin/python3
```

This can identify the installed package that owns a particular file.

---

## 7. Remove a Package

```bash
sudo dpkg -r package-name
```

---

## 8. Important Note

When manually installing a `.deb` file, dependency problems may occur.

If required dependencies are missing, you can often resolve them using:

```bash
sudo apt --fix-broken install
```

---

## Quick Reference

```bash
sudo dpkg -i package.deb
dpkg -l
dpkg -s package-name
dpkg -S /path/to/file
sudo dpkg -r package-name
```

---

## Summary

`dpkg` is the low-level package manager used to install and manage Debian `.deb` packages.

