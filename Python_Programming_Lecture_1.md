# Python Programming – Lecture 1
## Complete Beginner Introduction

### 1. Learning Objectives
By the end of this lecture, students should be able to:
- Explain what Python is.
- Understand why Python is popular.
- Identify common uses of Python.
- Install/check Python on a computer.
- Run Python code using the terminal and an editor.
- Understand Python syntax, indentation, comments, variables, and basic data types.
- Write simple `print()` programs.
- Take input from a user.
- Perform basic arithmetic.

---

## 2. What is Programming?

Programming means giving instructions to a computer so that it can perform a task.

Example:

```text
Human thinking:
Ask the user for their name
→ take the name
→ display a greeting
```

Python version:

```python
name = input("Enter your name: ")
print("Hello", name)
```

### Simple definition
> Programming = Problem + Logic + Instructions + Output

---

## 3. What is Python?

Python is a high-level, general-purpose programming language known for readable syntax and a large ecosystem of libraries.

Python was created by **Guido van Rossum** and first released in 1991.

Python is commonly used for:
- Web development
- Automation
- Data analysis
- Artificial Intelligence and Machine Learning
- Scripting
- Testing
- DevOps and cloud automation
- Education

---

## 4. Why Learn Python?

Python is beginner-friendly because its syntax is relatively simple and readable.

Compare:

```python
print("Hello World")
```

The same basic idea in a lower-level language can require more syntax.

### Key advantages
- Easy to read
- Large community
- Huge library ecosystem
- Cross-platform
- Useful for automation
- Widely used in modern technology

---

## 5. Where is Python Used?

| Area | Examples |
|---|---|
| Web | Django, Flask, FastAPI |
| Data | NumPy, pandas |
| AI/ML | scikit-learn, PyTorch |
| Automation | Scripts, file operations |
| DevOps | Cloud automation, CI/CD utilities |
| Testing | pytest |
| Education | Beginner programming |
| Cybersecurity | Security automation and tooling |

---

## 6. Python Installation

### Check whether Python is installed

Windows:

```powershell
python --version
```

or:

```powershell
py --version
```

Linux/macOS:

```bash
python3 --version
```

### Start the Python interpreter

Windows:

```powershell
python
```

Linux/macOS:

```bash
python3
```

Then:

```python
print("Hello Python")
```

Exit:

```python
exit()
```

---

## 7. Your First Python Program

```python
print("Hello World")
```

### What happens?

- `print()` is a built-in Python function.
- `"Hello World"` is a string.
- Python sends the string to the output.

Another example:

```python
print("Welcome to Python Programming")
print("Lecture 1")
```

---

## 8. Python File

Python source files normally use the `.py` extension.

Example:

```text
hello.py
```

Content:

```python
print("Hello World")
```

Run it from the terminal:

```powershell
python hello.py
```

---

## 9. Comments

Comments are notes for humans. Python ignores them during normal execution.

Single-line comment:

```python
# This is a comment
print("Hello")
```

Comments are useful for explaining code.

```python
# Ask the user for their name
name = input("Enter your name: ")
print(name)
```

Avoid unnecessary comments that simply repeat obvious code.

---

## 10. Python Indentation

Python uses indentation to define code blocks.

Correct:

```python
if 10 > 5:
    print("10 is greater than 5")
```

Incorrect:

```python
if 10 > 5:
print("10 is greater than 5")
```

A common convention is **4 spaces** for indentation.

Indentation is not decoration in Python—it is part of the syntax.

---

## 11. Variables

A variable is a name that refers to a value.

```python
name = "Sahil"
age = 25
```

Here:
- `name` stores a string.
- `age` stores an integer.

Python does not require you to declare the variable type separately.

```python
city = "Pune"
marks = 85
price = 99.50
```

### Naming examples

Good:

```python
student_name = "Amit"
total_marks = 450
```

Avoid:

```python
student-name = "Amit"
```

Use meaningful names.

---

## 12. Basic Data Types

### String

```python
name = "Rahul"
```

### Integer

```python
age = 20
```

### Float

```python
price = 99.50
```

### Boolean

```python
is_student = True
```

Check a type:

```python
print(type(name))
print(type(age))
print(type(price))
print(type(is_student))
```

---

## 13. The `print()` Function

```python
name = "Amit"
age = 21

print(name)
print(age)
print("Name:", name)
print("Age:", age)
```

### f-string

A clean way to format output:

```python
name = "Amit"
age = 21

print(f"My name is {name} and I am {age} years old.")
```

---

## 14. Taking User Input

```python
name = input("Enter your name: ")
print("Hello", name)
```

Important:

> `input()` returns text (a string).

So this:

```python
age = input("Enter your age: ")
```

stores text, even if the user enters `20`.

Convert it when you need a number:

```python
age = int(input("Enter your age: "))
```

---

## 15. Type Conversion

Common conversions:

```python
int("25")
float("10.5")
str(100)
```

Example:

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print(a + b)
```

---

## 16. Arithmetic Operators

| Operator | Meaning | Example |
|---|---|---|
| `+` | Addition | `10 + 5` |
| `-` | Subtraction | `10 - 5` |
| `*` | Multiplication | `10 * 5` |
| `/` | Division | `10 / 5` |
| `//` | Floor division | `10 // 3` |
| `%` | Remainder | `10 % 3` |
| `**` | Power | `2 ** 3` |

Example:

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(a ** b)
```

---

## 17. Mini Program – Student Introduction

```python
name = input("Enter your name: ")
age = int(input("Enter your age: "))
city = input("Enter your city: ")

print("\n--- Student Information ---")
print(f"Name: {name}")
print(f"Age: {age}")
print(f"City: {city}")
```

---

## 18. Mini Program – Calculator

```python
a = float(input("Enter first number: "))
b = float(input("Enter second number: "))

print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)
```

---

## 19. Common Beginner Errors

### NameError

```python
print(name)
```

when `name` has not been defined.

### SyntaxError

```python
print("Hello"
```

A bracket is missing.

### ValueError

```python
age = int(input("Enter age: "))
```

If the user enters:

```text
twenty
```

Python cannot convert it directly to an integer.

### IndentationError

Incorrect indentation inside a code block.

---

## 20. Good Beginner Habits

- Practice by typing code, not only reading it.
- Use meaningful variable names.
- Read error messages carefully.
- Make small programs first.
- Test one change at a time.
- Use comments when they add useful context.
- Do not blindly copy code—understand each line.
- Practice every day.

---

## 21. Classroom Practice

### Task 1
Print:
```text
Hello Python
I am learning programming
```

### Task 2
Create variables for:
- Name
- Age
- City
- Course

Print them.

### Task 3
Take two numbers from the user and print:
- Sum
- Difference
- Product
- Division

### Task 4
Create a program that calculates the area of a rectangle.

Formula:

```text
Area = length × width
```

### Task 5
Create a simple marks calculator:

Input:
- Student name
- Marks in 3 subjects

Output:
- Total
- Average

---

## 22. Lecture Summary

Today we learned:
1. What programming means
2. What Python is
3. Why Python is popular
4. Where Python is used
5. How to check/install Python
6. Python files and `.py`
7. `print()`
8. Comments
9. Indentation
10. Variables
11. Basic data types
12. `input()`
13. Type conversion
14. Arithmetic operators
15. Basic programs
16. Common beginner errors

### Next Lecture
Suggested next topics:
- Comparison operators
- Logical operators
- `if`, `elif`, `else`
- Nested conditions
- More practice problems
