# `echo` - Display Text and Variables

## 1. What is `echo`?

The `echo` command displays text or the value of variables in the terminal.

It is commonly used in:

* Shell commands
* Shell scripts
* Debugging
* Automation

---

## 2. Display Text

```bash
echo "Hello Linux"
```

Output:

```text
Hello Linux
```

---

## 3. Display a Variable

Example:

```bash
echo $HOME
```

This displays the value of the `HOME` environment variable.

---

## 4. Create a New Line

By default, `echo` adds a new line after the output.

---

## 5. Use Escape Sequences

On many shells:

```bash
echo -e "Hello\nLinux"
```

Output:

```text
Hello
Linux
```

---

## 6. Common Uses

```bash
echo "Hello"
echo $USER
echo $HOME
echo $PATH
```

---

## Summary

`echo` displays text and variable values in the terminal.

