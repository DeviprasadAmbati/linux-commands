# File and Directory Exercises

These exercises are designed to practice basic Linux file and directory navigation commands.

Commands covered:

* `pwd`
* `ls`
* `cd`
* `mkdir`
* `touch`

---

## Exercise 1: Check Current Directory

### Objective

Find the absolute path of your current working directory.

### Task

Run:

```bash
pwd
```

### Expected Result

The command should display the absolute path of the directory you are currently inside.

Example:

```text
/home/deviprasad/linux-commands/exercises/01-file-directory
```

---

## Exercise 2: List Files

### Objective

Practice listing files and directories.

### Task

Run:

```bash
ls
```

Then try:

```bash
ls -l
```

And:

```bash
ls -la
```

### Questions

1. What is the difference between `ls` and `ls -l`?
2. What additional files appear when using `ls -a`?
3. What does the `-h` option do when combined with `ls -l`?

Try:

```bash
ls -lah
```

---

## Exercise 3: Create a Directory

### Objective

Create directories using `mkdir`.

### Task

Create the following directory structure:

```text
linux-practice/
├── projects/
├── notes/
└── backups/
```

Commands:

```bash
mkdir linux-practice
mkdir linux-practice/projects
mkdir linux-practice/notes
mkdir linux-practice/backups
```

Verify:

```bash
ls -l linux-practice
```

---

## Exercise 4: Create Nested Directories

### Objective

Learn how to create multiple directory levels using `mkdir -p`.

### Task

Create:

```text
linux-practice/
└── projects/
    └── python/
        └── calculator/
```

Use:

```bash
mkdir -p linux-practice/projects/python/calculator
```

Verify:

```bash
ls -R linux-practice
```

---

## Exercise 5: Move Between Directories

### Objective

Practice navigating the filesystem using `cd`.

### Task

Start from:

```text
linux-practice/
```

Navigate into:

```text
projects/python/calculator
```

Use:

```bash
cd linux-practice/projects/python/calculator
```

Check your location:

```bash
pwd
```

Then move one directory backward:

```bash
cd ..
```

Move backward again:

```bash
cd ..
```

---

## Exercise 6: Go to Home Directory

### Objective

Learn different ways to navigate to the home directory.

### Task

Try:

```bash
cd
```

Then:

```bash
pwd
```

Try:

```bash
cd ~
```

Again verify:

```bash
pwd
```

### Question

What is the difference between:

```bash
cd
```

and:

```bash
cd ~
```

---

## Exercise 7: Create Empty Files

### Objective

Create files using `touch`.

### Task

Inside `linux-practice/notes`, create:

```text
linux.txt
commands.txt
todo.txt
```

Commands:

```bash
cd ~/linux-practice/notes

touch linux.txt commands.txt todo.txt
```

Verify:

```bash
ls -l
```

---

## Exercise 8: Create Multiple Files

### Objective

Practice creating multiple files efficiently.

### Task

Create:

```text
day1.txt
day2.txt
day3.txt
day4.txt
day5.txt
```

Use:

```bash
touch day1.txt day2.txt day3.txt day4.txt day5.txt
```

Verify:

```bash
ls
```

---

## Exercise 9: Explore the Parent Directory

### Objective

Understand `..` and `.`.

### Task

Run:

```bash
pwd
```

Then:

```bash
ls ..
```

Then:

```bash
ls .
```

### Questions

1. What does `.` represent?
2. What does `..` represent?
3. What does `~` represent?

---

## Exercise 10: Combined Challenge

### Objective

Use multiple commands together.

### Task

Create the following structure:

```text
practice/
├── frontend/
│   ├── html/
│   └── css/
├── backend/
│   ├── python/
│   └── node/
└── database/
```

Use as few commands as possible.

### Hint

You can use:

```bash
mkdir -p
```

For example:

```bash
mkdir -p practice/frontend/html
```

---

## Exercise 11: Create Project Files

Inside the structure from Exercise 10, create:

```text
practice/
├── frontend/
│   ├── html/
│   │   └── index.html
│   └── css/
│       └── style.css
├── backend/
│   ├── python/
│   │   └── app.py
│   └── node/
│       └── server.js
└── database/
    └── schema.sql
```

Use `touch` to create the files.

Example:

```bash
touch practice/frontend/html/index.html
```

---

# Mini Challenge

Without looking at the previous examples, create this structure:

```text
my-project/
├── src/
│   ├── main/
│   └── test/
├── docs/
├── config/
└── logs/
```

Then create:

```text
src/main/app.py
src/test/test_app.py
docs/README.md
config/app.conf
logs/app.log
```

Finally verify the complete structure using:

```bash
ls -R my-project
```

---

# Interview Questions

Try answering these without using the terminal.

### 1. What does `pwd` do?

### 2. What is the difference between `ls`, `ls -l`, and `ls -a`?

### 3. What does `cd ..` do?

### 4. What does `cd ~` do?

### 5. What does `mkdir -p` do?

### 6. What does `touch` do?

### 7. What is the difference between `.` and `..`?

### 8. How would you create three directories with one command?

### 9. How would you create five empty files with one command?

### 10. How would you create this structure with one command?

```text
project/
└── src/
    └── python/
        └── app/
```

---

# Practical Goal

After completing these exercises, you should be comfortable with:

```bash
pwd
ls
ls -l
ls -a
ls -la
cd
cd ..
cd ~
mkdir
mkdir -p
touch
```

You should also understand how Linux represents directories using:

```text
.
..
~
/
```

