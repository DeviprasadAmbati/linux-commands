# `ip` - Display and Manage Network Configuration

## 1. What is the `ip` Command?

The `ip` command is a modern Linux command used to display and manage network configuration.

It can be used to view:

* Network interfaces.
* IP addresses.
* Routing tables.
* Network links.

The `ip` command is part of the `iproute2` package and is commonly used instead of older networking tools.

---

## 2. Basic Syntax

```bash
ip OBJECT COMMAND
```

Examples:

```bash
ip address
ip link
ip route
```

---

## 3. Display IP Addresses

Use:

```bash
ip addr
```

or:

```bash
ip address
```

This displays network interfaces and their assigned IP addresses.

---

## 4. Display Network Interfaces

Use:

```bash
ip link
```

This displays available network interfaces.

Example interfaces may include:

```text
lo
eth0
wlan0
```

Depending on your Linux system, interface names may be different.

---

## 5. Display Routing Information

Use:

```bash
ip route
```

This displays the routing table.

Example:

```text
default via 192.168.1.1 dev eth0
```

This usually indicates the default gateway used to reach other networks.

---

## 6. Display Only IPv4 Addresses

```bash
ip -4 addr
```

---

## 7. Display Only IPv6 Addresses

```bash
ip -6 addr
```

---

## 8. Check a Specific Interface

Example:

```bash
ip addr show eth0
```

---

## 9. Common Commands

```bash
# Show IP addresses
ip addr

# Show interfaces
ip link

# Show routing table
ip route

# Show IPv4 addresses
ip -4 addr

# Show IPv6 addresses
ip -6 addr
```

---

## 10. Why Use `ip`?

The `ip` command provides a powerful and modern way to inspect and manage Linux networking.

It is commonly preferred over older commands such as `ifconfig`.

---

## Summary

The `ip` command is used to inspect and manage Linux networking.

The most commonly used commands are:

```bash
ip addr
ip link
ip route
```

