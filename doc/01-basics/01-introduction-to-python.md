# Introduction to Python

Python is a **general-purpose programming language**. It is designed to be easy to read, easy to write, and powerful enough to build almost anything.

## What can you do with Python?

Python is used for:

- Web Development
- Automation
- Data Science
- Machine Learning & AI
- Cybersecurity
- Desktop Applications
- Web Scraping
- Game Development
- APIs and Backend Development

## Why is Python popular?

- Simple and readable syntax
- Beginner-friendly
- Works on Windows, Linux, and macOS
- Huge collection of libraries
- Large community support

## Python Syntax Example

```python
print("Hello, World!")
```

**Output**

```text
Hello, World!
```

Python uses simple English-like syntax, so you can focus on solving problems instead of remembering complicated rules.

## Why choose Python?

Suppose you want to display text on the screen.

In C:

```c
#include <stdio.h>

int main() {
    printf("Hello, World!");
    return 0;
}
```

In Python:

```python
print("Hello, World!")
```

Python requires less code, making programs easier to write and understand.

## Where to use Python?

| Field | Example |
|--------|---------|
| Web Development | Django, Flask, FastAPI |
| AI & Machine Learning | TensorFlow, PyTorch |
| Data Analysis | Pandas, NumPy |
| Automation | File handling, Scripts |
| Cybersecurity | Network tools, Automation |
| Desktop Apps | Tkinter, PyQt |
| Web Scraping | BeautifulSoup, Selenium |

## Summary

Python is a simple, powerful, and versatile programming language. It is an excellent choice for beginners and professionals because the same language can be used for small scripts as well as large-scale applications.

---


# Installing Python

Before writing Python code, you need to install Python on your computer.

## Step 1: Download Python

Go to the official Python website:

👉 https://www.python.org/downloads/

The website automatically recommends the latest stable version for your operating system.

## Step 2: Run the Installer

Open the downloaded installer.

### **Windows**

✔️ Check **"Add Python to PATH"**

Then click:

```
Install Now
```

> **Why check "Add Python to PATH"?**
>
> It allows you to run Python from the Command Prompt without typing its installation folder every time.

---

### **Linux (Ubuntu/Debian)**

Most Linux distributions already include Python.

Check whether Python is installed:

```bash
python3 --version
```

If Python is not installed:

```bash
sudo apt update
sudo apt install python3
```

---

### **macOS**

Check if Python is installed:

```bash
python3 --version
```

If it isn't, download it from:

https://www.python.org/downloads/

or install it using Homebrew:

```bash
brew install python
```

---

# Verify the Installation

Open your terminal or command prompt.

### Windows

```cmd
python --version
```

or

```cmd
py --version
```

### Linux / macOS

```bash
python3 --version
```

Example output:

```text
Python 3.13.7
```

If you see a version number, Python has been installed successfully.

---

# Running Python

Open a terminal.

Start Python:

### Windows

```cmd
python
```

or

```cmd
py
```

### Linux / macOS

```bash
python3
```

You'll see something like:

```text
Python 3.13.7
>>>
```

The `>>>` symbol is called the **Python Interpreter**.

It means Python is ready to execute your code.

---

# Your First Command

Type:

```python
print("Hello, World!")
```

Output:

```text
Hello, World!
```

Exit the interpreter:

```python
exit()
```

or press:

**Ctrl + Z**, then **Enter** (Windows)

**Ctrl + D** (Linux/macOS)

---

# Install VS Code (Recommended)

Although you can write Python in any text editor, **Visual Studio Code** provides features like:

- Syntax highlighting
- Auto-completion
- Error detection
- Built-in terminal
- Extensions

Download:

https://code.visualstudio.com/

Install the **Python** extension from Microsoft.

> **Why use VS Code?**
>
> It makes writing and debugging Python programs much easier.

---

# Common Installation Problems

## `'python' is not recognized`

Python is not added to your system PATH.

Solution:

- Reinstall Python
- Check **"Add Python to PATH"**
- Restart your terminal

---

## Wrong Python Version

Check installed versions:

```cmd
py -0
```

Choose a specific version:

```cmd
py -3.13
```

---

# Summary

- Download Python from the official website.
- Install it and add Python to PATH.
- Verify the installation using `python --version`.
- Run Python from the terminal.
- Install VS Code for a better coding experience.

---

## Next Chapter

➡️ **Writing and Running Your First Python Program**