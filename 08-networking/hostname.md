# `hostname` - Display or Manage the System Hostname

## 1. What is a Hostname?

A hostname is the name used to identify a computer on a network.

For example:

```text
Ambati
```

or:

```text
server01
```

---

## 2. Display the Current Hostname

Run:

```bash
hostname
```

---

## 3. Display Additional Information

You can use:

```bash
hostnamectl
```

This command can display additional system and hostname information on systems using `systemd`.

---

## 4. Display the Fully Qualified Domain Name

On systems where it is configured:

```bash
hostname -f
```

This may display something like:

```text
server.example.com
```

---

## 5. Temporary Hostname Changes

A hostname can sometimes be changed temporarily using:

```bash
sudo hostname new-hostname
```

The exact behavior and persistence can depend on the Linux distribution.

For modern `systemd` systems, `hostnamectl` is commonly preferred for persistent configuration.

---

## 6. Change the Hostname Using `hostnamectl`

```bash
sudo hostnamectl set-hostname new-hostname
```

Example:

```bash
sudo hostnamectl set-hostname dev-server
```

---

## 7. Why Is the Hostname Important?

Hostnames are useful for:

* Identifying servers.
* Managing networks.
* Connecting using SSH.
* System administration.

---

## Quick Reference

```bash
# Display hostname
hostname

# Display system hostname information
hostnamectl

# Set hostname
sudo hostnamectl set-hostname new-hostname
```

---

## Summary

The `hostname` command displays the name of your Linux system.

For modern systems, `hostnamectl` provides additional hostname management features.

