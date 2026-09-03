# `ifconfig` - Display Network Interface Configuration

## 1. What is `ifconfig`?

`ifconfig` stands for **interface configuration**.

It is an older Linux command used to display and configure network interfaces.

---

## 2. Basic Usage

```bash
ifconfig
```

This displays information about available network interfaces.

---

## 3. Example Information

The output can include:

* IP address.
* Network interface name.
* MAC address.
* Network statistics.
* Received packets.
* Transmitted packets.

---

## 4. Check a Specific Interface

```bash
ifconfig eth0
```

---

## 5. Why Might `ifconfig` Not Work?

On many modern Linux distributions, `ifconfig` is not installed by default.

You may see:

```text
command not found
```

The modern replacement is usually:

```bash
ip addr
```

---

## 6. Install `ifconfig`

On Ubuntu or Debian systems:

```bash
sudo apt install net-tools
```

---

## 7. `ifconfig` vs `ip`

| Command    | Status                |
| ---------- | --------------------- |
| `ifconfig` | Older networking tool |
| `ip addr`  | Modern alternative    |

For modern Linux systems, learning the `ip` command is generally recommended.

---

## Quick Reference

```bash
ifconfig
ifconfig eth0
ip addr
```

---

## Summary

`ifconfig` is an older command for viewing and configuring network interfaces.

The modern alternative is:

```bash
ip addr
```

