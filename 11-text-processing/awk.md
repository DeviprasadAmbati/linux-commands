# `awk` - Process and Analyze Text

## 1. What is `awk`?

`awk` is a powerful text-processing language commonly used in Linux.

It is especially useful for working with structured text containing columns.

`awk` can:

* Extract columns
* Filter data
* Perform calculations
* Format output

---

## 2. Basic Syntax

```bash
awk 'pattern { action }' filename
```

---

## 3. Print a Specific Column

Suppose a file contains:

```text
John 25 Developer
Alice 30 Engineer
```

Run:

```bash
awk '{print $1}' file.txt
```

Output:

```text
John
Alice
```

---

## 4. Print Multiple Columns

```bash
awk '{print $1, $3}' file.txt
```

Output:

```text
John Developer
Alice Engineer
```

---

## 5. Filter Rows

Example:

```bash
awk '$2 > 25' file.txt
```

This displays rows where the second column is greater than 25.

---

## 6. Use a Custom Separator

For CSV-like data:

```bash
awk -F ',' '{print $1}' file.csv
```

The `-F` option specifies the field separator.

---

## 7. Use `awk` with Commands

Example:

```bash
ls -l | awk '{print $9}'
```

This prints the filename column in typical `ls -l` output.

---

## 8. Quick Reference

```bash
awk '{print $1}' file.txt
awk '{print $1, $2}' file.txt
awk '$2 > 25' file.txt
awk -F ',' '{print $1}' file.csv
```

---

## Summary

`awk` is a powerful tool for extracting, filtering, and processing structured text.

