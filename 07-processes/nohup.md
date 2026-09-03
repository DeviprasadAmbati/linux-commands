# `nohup` - Run Commands That Continue After Logout

## 1. What is `nohup`?

`nohup` stands for **no hangup**.

It runs a command while ignoring the `SIGHUP` signal, helping the command continue after the terminal session is closed.

---

## 2. Basic Syntax

```bash
nohup command &
```

Example:

```bash
nohup python app.py &
```

---

## 3. Understanding `&`

The `&` symbol runs the command in the background.

Example:

```bash
command &
```

---

## 4. Default Output

If output is not redirected, `nohup` commonly writes output to:

```text
nohup.out
```

---

## 5. Redirect Output

You can redirect output:

```bash
nohup python app.py > output.log 2>&1 &
```

Explanation:

```text
> output.log → Standard output goes to output.log
2>&1         → Standard error goes to the same location
&            → Run in the background
```

---

## 6. Check the Running Process

Use:

```bash
ps aux | grep python
```

or:

```bash
jobs
```

Note that `jobs` only shows jobs belonging to the current shell session.

---

## 7. Real-World Example

Run a long script:

```bash
nohup python backup.py > backup.log 2>&1 &
```

The process can continue even if the terminal disconnects.

---

## 8. Important Note

For long-running production services, tools such as system service managers may be more appropriate than `nohup`.

---

## Quick Reference

```bash
nohup command &
nohup command > output.log 2>&1 &
```

---

## Summary

`nohup` helps commands continue running after terminal logout or disconnection.

