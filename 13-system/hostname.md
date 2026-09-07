# `hostname` - Display or Set the System Hostname

## 1. What is `hostname`?

The `hostname` command displays the name assigned to the current system.

A hostname helps identify a computer on a network.

For example:

```text
server01
```

or:

```text
deviprasad-laptop
```

---

## 2. Display the Current Hostname

Run:

```bash
hostname
```

Example output:

```text
Ambati
```

---

## 3. Display the Fully Qualified Domain Name

Use:

```bash
hostname -f
```

This may display a fully qualified domain name if the system is configured correctly.

---

## 4. Change the Hostname Temporarily

On modern Linux systems, `hostnamectl` is generally preferred for changing the hostname.

Example:

```bash
sudo hostnamectl set-hostname my-server
```

---

## 5. Check Hostname Information

Use:

```bash
hostnamectl
```

This can display information such as:

* Static hostname
* Operating system
* Kernel
* Architecture

---

## Quick Reference

```bash
hostname
hostname -f
hostnamectl
sudo hostnamectl set-hostname my-server
```

---

## Summary

`hostname` displays the name of the current Linux system.

For managing hostnames on modern Linux systems, `hostnamectl` is commonly used.

