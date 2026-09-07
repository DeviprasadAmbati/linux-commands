# `apt-get` - Package Management Command

## 1. What is `apt-get`?

`apt-get` is a command-line package management tool for Debian and Ubuntu-based systems.

It is an older and more script-oriented interface compared with `apt`.

It is commonly used in:

* Automation scripts
* Server management
* System administration

---

## 2. Update Package Lists

```bash
sudo apt-get update
```

---

## 3. Upgrade Packages

```bash
sudo apt-get upgrade
```

---

## 4. Install a Package

Example:

```bash
sudo apt-get install nginx
```

---

## 5. Remove a Package

```bash
sudo apt-get remove nginx
```

---

## 6. Remove Configuration Files

```bash
sudo apt-get purge nginx
```

---

## 7. Remove Unused Dependencies

Use:

```bash
sudo apt-get autoremove
```

This removes packages that were automatically installed as dependencies but are no longer required.

---

## 8. `apt` vs `apt-get`

| Command   | Common Usage               |
| --------- | -------------------------- |
| `apt`     | Interactive terminal usage |
| `apt-get` | Scripts and automation     |

---

## Quick Reference

```bash
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install package-name
sudo apt-get remove package-name
sudo apt-get purge package-name
sudo apt-get autoremove
```

---

## Summary

`apt-get` is a powerful package management tool commonly used for automation and system administration.

