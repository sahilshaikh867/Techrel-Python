
> **Note:** Python keywords are reserved words such as `if`, `else`, `for`, `while`, `def`, `class`, `try`, `import`, `lambda`, `yield`, etc. You cannot normally use them as variable names.

# 🐍 Python Keywords 

## 🟢 Level 1 — Beginner

### 1. `if`

```python
age = 20

if age >= 18:
    print("Adult")
```

---

### 2. `else`

```python
age = 15

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

---

### 3. `elif`

```python
marks = 75

if marks >= 90:
    print("A")
elif marks >= 60:
    print("B")
else:
    print("C")
```

---

### 4. `for`

```python
for i in range(5):
    print(i)
```

---

### 5. `while`

```python
i = 1

while i <= 5:
    print(i)
    i += 1
```

---

### 6. `in`

```python
fruits = ["Apple", "Mango", "Banana"]

if "Mango" in fruits:
    print("Mango found")
```

---

### 7. `not`

```python
is_raining = False

if not is_raining:
    print("Go outside")
```

---

### 8. `and`

```python
age = 25
has_id = True

if age >= 18 and has_id:
    print("Allowed")
```

---

### 9. `or`

```python
day = "Sunday"

if day == "Saturday" or day == "Sunday":
    print("Weekend")
```

---

### 10. `True`

```python
is_logged_in = True

if is_logged_in:
    print("Welcome")
```

---

### 11. `False`

```python
is_logged_in = False

if not is_logged_in:
    print("Please login")
```

---

### 12. `None`

```python
name = None

print(name)
```

`None` means **no value / empty value**.

---

### 13. `break`

```python
for i in range(1, 10):
    if i == 5:
        break

    print(i)
```

Output:

```text
1
2
3
4
```

---

### 14. `continue`

```python
for i in range(1, 6):
    if i == 3:
        continue

    print(i)
```

Output:

```text
1
2
4
5
```

---

### 15. `pass`

```python
age = 20

if age >= 18:
    pass
```

`pass` means **do nothing for now**.

---

# 🟡 Level 2 — Beginner to Intermediate

## 16. `def`

Used to create a function.

```python
def hello():
    print("Hello")

hello()
```

---

## 17. `return`

```python
def add(a, b):
    return a + b

result = add(10, 20)

print(result)
```

---

## 18. `import`

```python
import math

print(math.sqrt(25))
```

---

## 19. `from`

```python
from math import sqrt

print(sqrt(25))
```

---

## 20. `as`

Used to create an alias.

```python
import math as m

print(m.sqrt(25))
```

---

## 21. `is`

Checks whether two variables refer to the same object.

```python
x = None

if x is None:
    print("No value")
```

---

## 22. `is not`

```python
x = 10

if x is not None:
    print("Value exists")
```

---

## 23. `assert`

Used to test an assumption.

```python
age = 20

assert age >= 18

print("Valid age")
```

If the condition is false, Python raises an `AssertionError`.

---

## 24. `global`

Used when modifying a global variable inside a function.

```python
count = 0

def increase():
    global count
    count += 1

increase()

print(count)
```

Output:

```text
1
```

---

## 25. `nonlocal`

Used with nested functions.

```python
def outer():
    x = 10

    def inner():
        nonlocal x
        x += 5

    inner()

    print(x)

outer()
```

Output:

```text
15
```

---

# 🟠 Level 3 — Intermediate

## 26. `class`

Used to create a class.

```python
class Student:
    name = "Sahil"

student = Student()

print(student.name)
```

---

## 27. `del`

Deletes a variable or object reference.

```python
name = "Sahil"

del name
```

After this, `name` no longer exists.

---

## 28. `try`

Used for error handling.

```python
try:
    print(10 / 0)
```

---

## 29. `except`

Handles an error.

```python
try:
    print(10 / 0)
except:
    print("Something went wrong")
```

---

## 30. `finally`

Runs whether an error occurs or not.

```python
try:
    print("Hello")
except:
    print("Error")
finally:
    print("Finished")
```

Output:

```text
Hello
Finished
```

---

## 31. `raise`

Used to manually generate an exception.

```python
age = 15

if age < 18:
    raise Exception("You are not eligible")
```

---

## 32. `with`

Commonly used when working with files.

```python
with open("data.txt", "r") as file:
    data = file.read()

print(data)
```

---

## 33. `yield`

Used in generators.

```python
def numbers():
    yield 1
    yield 2
    yield 3

for number in numbers():
    print(number)
```

Output:

```text
1
2
3
```

---

## 34. `lambda`

Creates a small anonymous function.

```python
square = lambda x: x * x

print(square(5))
```

Output:

```text
25
```

---

## 35. `match`

Python's pattern matching.

```python
day = "Monday"

match day:
    case "Monday":
        print("Start of week")
    case "Sunday":
        print("Weekend")
```

---

## 36. `case`

Used inside `match`.

```python
number = 2

match number:
    case 1:
        print("One")
    case 2:
        print("Two")
```

---

# 🔴 Level 4 — Advanced

## 37. `async`

Used to define an asynchronous function.

```python
async def hello():
    print("Hello")
```

---

## 38. `await`

Waits for an asynchronous operation.

```python
import asyncio

async def hello():
    await asyncio.sleep(1)
    print("Hello")

asyncio.run(hello())
```

---

## 39. `async` + `await`

A practical combination:

```python
import asyncio

async def task():
    print("Task started")

    await asyncio.sleep(2)

    print("Task completed")

asyncio.run(task())
```

---

## 40. `yield` with generator

```python
def count():
    for i in range(1, 4):
        yield i

numbers = count()

print(next(numbers))
print(next(numbers))
print(next(numbers))
```

Output:

```text
1
2
3
```

---

## 41. `yield` for large data

```python
def generate_numbers():
    for i in range(1000000):
        yield i

for number in generate_numbers():
    if number == 5:
        break

    print(number)
```

Generators are useful because they don't need to create all values in memory at once.

---

## 42. `class` + `__init__`

```python
class Student:

    def __init__(self, name):
        self.name = name

student = Student("Sahil")

print(student.name)
```

---

## 43. `class` + `return`

```python
class Calculator:

    def add(self, a, b):
        return a + b

c = Calculator()

print(c.add(10, 20))
```

---

## 44. `try` + `except` + `finally`

```python
try:
    number = int(input("Enter number: "))
    result = 10 / number

except ValueError:
    print("Please enter a number")

except ZeroDivisionError:
    print("Cannot divide by zero")

finally:
    print("Program finished")
```

This is much closer to real-world Python programming.

---

## 45. `raise` with custom condition

```python
def check_age(age):

    if age < 18:
        raise ValueError("Age must be 18 or above")

    return "Allowed"

print(check_age(20))
```

---

## 46. `nonlocal` with nested function

```python
def counter():

    count = 0

    def increase():
        nonlocal count
        count += 1
        return count

    return increase


c = counter()

print(c())
print(c())
print(c())
```

Output:

```text
1
2
3
```

---

## 47. `global` example

```python
message = "Hello"

def change_message():

    global message

    message = "Welcome"

change_message()

print(message)
```

Output:

```text
Welcome
```

---

## 48. `with` + file handling

```python
with open("student.txt", "w") as file:
    file.write("Sahil")
```

The `with` statement automatically handles closing the file.

---

## 49. `match` with multiple cases

```python
command = "start"

match command:

    case "start":
        print("Starting server")

    case "stop":
        print("Stopping server")

    case "restart":
        print("Restarting server")

    case _:
        print("Unknown command")
```

This kind of pattern matching can be useful in CLI applications.

---

## 50. Advanced: `async` + `await` + function

```python
import asyncio

async def download_file(name):

    print("Downloading", name)

    await asyncio.sleep(2)

    print("Download complete:", name)


async def main():

    await asyncio.gather(
        download_file("file1"),
        download_file("file2"),
        download_file("file3")
    )


asyncio.run(main())
```

This introduces students to **asynchronous programming**, which becomes useful in APIs, web servers, networking, and other I/O-heavy applications.

---

# 📚 Python Keywords — Quick Learning Order

I'd teach them like this:

### 🟢 Beginner

```text
1. True
2. False
3. None
4. if
5. else
6. elif
7. and
8. or
9. not
10. in
11. for
12. while
13. break
14. continue
15. pass
```

### 🟡 Functions & Modules

```text
16. def
17. return
18. import
19. from
20. as
21. is
22. is not
```

### 🟠 Error Handling & OOP

```text
23. assert
24. global
25. nonlocal
26. class
27. del
28. try
29. except
30. finally
31. raise
32. with
```

### 🔴 Advanced

```text
33. yield
34. lambda
35. match
36. case
37. async
38. await
```

And then teach the combinations through projects:

```text
Variables
   ↓
Operators
   ↓
if / elif / else
   ↓
for / while
   ↓
break / continue
   ↓
Functions
   ↓
Lists / Dictionaries
   ↓
Exception Handling
   ↓
File Handling
   ↓
OOP
   ↓
Modules
   ↓
Generators
   ↓
Lambda
   ↓
Async / Await
```

**One important correction for students:** Python has **35 reserved keywords in current Python 3.x**, not 50. So the 50 examples above are **50 keyword-based examples/concepts**, with several examples reusing the same keyword in progressively harder situations.
