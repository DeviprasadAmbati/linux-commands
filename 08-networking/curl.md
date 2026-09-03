# `curl` - Transfer Data Using URLs

## 1. What is `curl`?

`curl` stands for **Client URL**.

It is a command-line tool used to transfer data between your computer and a server.

`curl` supports many protocols, including:

* HTTP
* HTTPS
* FTP
* SFTP

It is commonly used by developers to test APIs and download data.

---

## 2. Basic Syntax

```bash
curl URL
```

Example:

```bash
curl https://example.com
```

---

## 3. Follow Redirects

Use:

```bash
curl -L URL
```

Example:

```bash
curl -L https://example.com
```

The `-L` option follows HTTP redirects.

---

## 4. Download a File

```bash
curl -O URL
```

Example:

```bash
curl -O https://example.com/file.zip
```

`-O` saves the file using its original filename.

---

## 5. Save Output with a Custom Name

```bash
curl -o filename URL
```

Example:

```bash
curl -o page.html https://example.com
```

---

## 6. Display HTTP Headers

```bash
curl -I https://example.com
```

This sends a request to retrieve response headers.

---

## 7. Send an API Request

Example:

```bash
curl https://api.example.com/users
```

---

## 8. Send a POST Request

Example:

```bash
curl -X POST https://api.example.com/users
```

Real APIs often require additional headers, authentication, and request data.

---

## 9. Why Developers Use `curl`

`curl` is useful for:

* Testing APIs.
* Checking websites.
* Downloading files.
* Sending HTTP requests.
* Debugging network problems.

---

## Quick Reference

```bash
curl URL
curl -L URL
curl -O URL
curl -o filename URL
curl -I URL
curl -X POST URL
```

---

## Summary

`curl` is a powerful command-line tool for transferring data and testing web services.

