# `nslookup` - Query DNS Information

## 1. What is `nslookup`?

`nslookup` stands for **name server lookup**.

It is used to query DNS servers and retrieve information about domain names.

---

## 2. Basic Syntax

```bash
nslookup domain_name
```

Example:

```bash
nslookup google.com
```

---

## 3. What Does DNS Do?

DNS converts domain names into IP addresses.

Example:

```text
google.com
     ↓
DNS Lookup
     ↓
IP Address
```

Without DNS, users would need to remember IP addresses instead of domain names.

---

## 4. Query a Specific DNS Server

```bash
nslookup google.com 8.8.8.8
```

This queries the specified DNS server.

---

## 5. Reverse DNS Lookup

You can query an IP address:

```bash
nslookup 8.8.8.8
```

Depending on DNS configuration, this may return hostname information.

---

## 6. Why Use `nslookup`?

It is useful for:

* Debugging DNS problems.
* Finding IP addresses.
* Checking DNS configuration.
* Performing reverse lookups.

---

## 7. Modern Alternatives

Many administrators also use:

```bash
dig
```

Example:

```bash
dig google.com
```

---

## Quick Reference

```bash
nslookup google.com
nslookup google.com 8.8.8.8
nslookup 8.8.8.8
dig google.com
```

---

## Summary

`nslookup` is used to query DNS servers and troubleshoot domain name resolution.

