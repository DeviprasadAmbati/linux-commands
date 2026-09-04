# `env` - Display Environment Variables

## 1. What is `env`?

The `env` command displays the environment variables available to a command or shell.

---

## 2. Display Environment Variables

```bash
env
```

---

## 3. Example Variables

Common environment variables include:

```text
HOME
USER
PATH
SHELL
```

---

## 4. Display a Specific Variable

You can use:

```bash
echo $HOME
```

Example:

```bash
echo $PATH
```

---

## 5. Run a Command with a Temporary Variable

Example:

```bash
env NAME="Linux" bash -c 'echo $NAME'
```

The variable is available to that command.

---

## Summary

`env` displays and manages environment variables for commands.

