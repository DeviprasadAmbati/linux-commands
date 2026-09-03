# `ssh` - Securely Connect to Remote Systems

## 1. What is SSH?

`SSH` stands for **Secure Shell**.

The `ssh` command is used to securely connect to a remote computer or server.

It is commonly used for:

* Managing Linux servers.
* Running remote commands.
* Secure administration.
* Remote development.

---

## 2. Basic Syntax

```bash
ssh username@hostname
```

Example:

```bash
ssh devuser@192.168.1.10
```

---

## 3. Connect Using a Hostname

```bash
ssh username@server.example.com
```

---

## 4. Specify a Port

SSH normally uses port `22`.

To use a different port:

```bash
ssh -p 2222 username@server.example.com
```

---

## 5. Run a Remote Command

You can execute a command remotely:

```bash
ssh username@server.example.com "uptime"
```

---

## 6. Exit an SSH Session

Use:

```bash
exit
```

or press:

```text
Ctrl + D
```

---

## 7. SSH Keys

SSH can use public/private key authentication.

A common command for generating a key is:

```bash
ssh-keygen
```

SSH keys can provide a more secure and convenient alternative to password-based authentication when configured correctly.

---

## 8. Common Uses

```bash
# Connect to server
ssh user@server

# Connect using port
ssh -p 2222 user@server

# Run remote command
ssh user@server "uptime"
```

---

## Summary

`ssh` allows secure remote access to Linux systems and servers.

