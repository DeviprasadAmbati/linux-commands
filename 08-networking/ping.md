# `ping` - Test Network Connectivity

## 1. What is `ping`?

The `ping` command is used to test network connectivity between your computer and another device or server.

It sends network packets to a destination and waits for a response.

`ping` is commonly used to check:

* Whether a host is reachable.
* Whether an internet connection is working.
* Network response time.
* Packet loss.

---

## 2. Basic Syntax

```bash
ping destination
```

Example:

```bash
ping google.com
```

---

## 3. Understanding How `ping` Works

`ping` uses the **ICMP (Internet Control Message Protocol)**.

The basic process is:

```text
Your Computer
      |
      | ICMP Request
      ▼
Destination Server
      |
      | ICMP Reply
      ▼
Your Computer
```

If the destination responds, the connection is working.

---

## 4. Example Output

```text
64 bytes from server: icmp_seq=1 ttl=117 time=20 ms
```

Important information:

* `icmp_seq` → Packet sequence number.
* `ttl` → Time To Live value.
* `time` → Response time.

---

## 5. Stop `ping`

On many Linux systems, `ping` continues running until stopped.

Press:

```text
Ctrl + C
```

---

## 6. Send a Specific Number of Packets

Use the `-c` option:

```bash
ping -c 4 google.com
```

This sends 4 packets and then stops.

---

## 7. Check Your Local Network

You can ping your router or another device:

```bash
ping 192.168.1.1
```

The address will depend on your network configuration.

---

## 8. Common Problems

### Unknown Host

Example:

```text
ping: unknown host example.com
```

This may indicate a DNS problem.

### No Response

A destination may not respond because:

* The host is offline.
* A firewall blocks ICMP.
* The server is configured not to respond to ping.

A failed ping does not always mean the server or service is unavailable.

---

## 9. Practice Commands

```bash
ping -c 4 google.com
ping -c 4 localhost
ping -c 4 8.8.8.8
```

---

## 10. Quick Reference

```bash
# Ping a domain
ping google.com

# Send 4 packets
ping -c 4 google.com

# Ping an IP address
ping 8.8.8.8
```

---

## Summary

`ping` is one of the most useful commands for testing basic network connectivity.

The most commonly used command is:

```bash
ping -c 4 google.com
```

