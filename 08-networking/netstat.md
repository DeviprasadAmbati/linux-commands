# `netstat` - Display Network Connections

## 1. What is `netstat`?

`netstat` stands for **network statistics**.

It is an older command used to display network connections, routing information, and network statistics.

---

## 2. Basic Usage

```bash
netstat
```

---

## 3. Display Listening Ports

```bash
netstat -tuln
```

Explanation:

```text
t → TCP
u → UDP
l → Listening ports
n → Show numerical addresses
```

---

## 4. Display All Connections

```bash
netstat -a
```

---

## 5. Display Routing Table

```bash
netstat -r
```

---

## 6. Modern Alternatives

On modern Linux systems, the `ss` command is often preferred.

Example:

```bash
ss -tuln
```

---

## 7. Why Might `netstat` Be Missing?

On many modern Linux systems, `netstat` is not installed by default.

On Ubuntu or Debian:

```bash
sudo apt install net-tools
```

---

## Quick Reference

```bash
netstat
netstat -tuln
netstat -a
netstat -r
ss -tuln
```

---

## Summary

`netstat` displays network connections and statistics.

For modern Linux systems, `ss` is commonly used as an alternative.

