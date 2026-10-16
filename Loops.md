# 🔄 Loops in Python

A **loop** is used when we want to repeat a block of code multiple times.

There are mainly two basic loops:

- `for` loop → used when we generally know how many times we want to repeat.
- `while` loop → used when repetition depends on a condition.
- **Nested loop** → a loop inside another loop.

---

# 1️⃣ 10 Simple `for` Loop Examples

## Example 1: Print numbers 1 to 5

```python
for i in range(1, 6):
    print(i)
```

**Output:**
```text
1
2
3
4
5
```

---

## Example 2: Print "Hello" 5 times

```python
for i in range(5):
    print("Hello")
```

**Output:**
```text
Hello
Hello
Hello
Hello
Hello
```

---

## Example 3: Print even numbers

```python
for i in range(2, 11, 2):
    print(i)
```

**Output:**
```text
2
4
6
8
10
```

---

## Example 4: Print odd numbers

```python
for i in range(1, 10, 2):
    print(i)
```

**Output:**
```text
1
3
5
7
9
```

---

## Example 5: Print numbers from 10 to 1

```python
for i in range(10, 0, -1):
    print(i)
```

**Output:**
```text
10
9
8
7
6
5
4
3
2
1
```

---

## Example 6: Print multiplication table

```python
num = 5

for i in range(1, 11):
    print(num * i)
```

**Output:**
```text
5
10
15
20
25
30
35
40
45
50
```

A better version:

```python
num = 5

for i in range(1, 11):
    print(num, "x", i, "=", num * i)
```

---

## Example 7: Calculate sum of numbers

```python
total = 0

for i in range(1, 6):
    total = total + i

print("Sum =", total)
```

**Output:**
```text
Sum = 15
```

Because:

```text
1 + 2 + 3 + 4 + 5 = 15
```

---

## Example 8: Print items from a list

```python
fruits = ["Apple", "Banana", "Mango", "Orange"]

for fruit in fruits:
    print(fruit)
```

**Output:**
```text
Apple
Banana
Mango
Orange
```

---

## Example 9: Find numbers greater than 5

```python
numbers = [2, 7, 4, 9, 3, 8]

for num in numbers:
    if num > 5:
        print(num)
```

**Output:**
```text
7
9
8
```

---

## Example 10: Count vowels

```python
word = "education"

count = 0

for letter in word:
    if letter in "aeiou":
        count = count + 1

print("Vowels =", count)
```

**Output:**
```text
Vowels = 5
```

---

# 2️⃣ 10 Simple `while` Loop Examples

Remember:

```python
while condition:
    # code
```

The loop continues **while the condition is True**.

---

## Example 1: Print numbers 1 to 5

```python
i = 1

while i <= 5:
    print(i)
    i = i + 1
```

**Output:**
```text
1
2
3
4
5
```

⚠️ Important:

```python
i = i + 1
```

is necessary. Otherwise, the loop can become an **infinite loop**.

---

## Example 2: Print Hello 5 times

```python
i = 1

while i <= 5:
    print("Hello")
    i = i + 1
```

---

## Example 3: Print even numbers

```python
i = 2

while i <= 10:
    print(i)
    i = i + 2
```

**Output:**
```text
2
4
6
8
10
```

---

## Example 4: Print odd numbers

```python
i = 1

while i <= 9:
    print(i)
    i = i + 2
```

**Output:**
```text
1
3
5
7
9
```

---

## Example 5: Countdown

```python
i = 10

while i >= 1:
    print(i)
    i = i - 1
```

**Output:**
```text
10
9
8
7
6
5
4
3
2
1
```

---

## Example 6: Multiplication table

```python
num = 5
i = 1

while i <= 10:
    print(num, "x", i, "=", num * i)
    i = i + 1
```

---

## Example 7: Sum of numbers

```python
i = 1
total = 0

while i <= 5:
    total = total + i
    i = i + 1

print("Sum =", total)
```

**Output:**
```text
Sum = 15
```

---

## Example 8: Print characters of a word

```python
word = "Python"

i = 0

while i < len(word):
    print(word[i])
    i = i + 1
```

**Output:**
```text
P
y
t
h
o
n
```

---

## Example 9: Keep asking for password

```python
password = ""

while password != "1234":
    password = input("Enter password: ")

print("Login successful!")
```

The loop continues until the user enters:

```text
1234
```

---

## Example 10: Simple number guessing

```python
number = 7
guess = 0

while guess != number:
    guess = int(input("Guess the number: "))

print("Correct!")
```

The user keeps guessing until they enter `7`.

---

# 3️⃣ 10 Nested Loop Examples

### What is a nested loop?

A **nested loop means a loop inside another loop.**

Basic structure:

```python
for i in range(...):
    for j in range(...):
        print(...)
```

Think of it like:

> **Outer loop → controls rows**  
> **Inner loop → controls columns**

---

## Example 1: Print 3 × 3 numbers

```python
for i in range(3):
    for j in range(3):
        print(i, j)
```

**Output:**

```text
0 0
0 1
0 2
1 0
1 1
1 2
2 0
2 1
2 2
```

---

## Example 2: Print stars in a square

```python
for i in range(3):
    for j in range(3):
        print("*", end=" ")
    print()
```

**Output:**

```text
* * *
* * *
* * *
```

Here:

```python
print()
```

moves to the next line.

---

## Example 3: Print 5 × 5 stars

```python
for i in range(5):
    for j in range(5):
        print("*", end=" ")
    print()
```

**Output:**

```text
* * * * *
* * * * *
* * * * *
* * * * *
* * * * *
```

---

## Example 4: Print a number pattern

```python
for i in range(1, 4):
    for j in range(1, 4):
        print(j, end=" ")
    print()
```

**Output:**

```text
1 2 3
1 2 3
1 2 3
```

---

## Example 5: Print increasing stars

```python
for i in range(1, 6):
    for j in range(i):
        print("*", end=" ")
    print()
```

**Output:**

```text
*
* *
* * *
* * * *
* * * * *
```

This is a very important beginner pattern.

---

## Example 6: Print increasing numbers

```python
for i in range(1, 6):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
```

**Output:**

```text
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

---

## Example 7: Multiplication tables from 1 to 3

```python
for i in range(1, 4):
    print("Table of", i)

    for j in range(1, 11):
        print(i, "x", j, "=", i * j)

    print()
```

This produces:

```text
Table of 1
1 x 1 = 1
1 x 2 = 2
...
1 x 10 = 10

Table of 2
2 x 1 = 2
...
```

---

## Example 8: Print a 4 × 4 number grid

```python
for i in range(1, 5):
    for j in range(1, 5):
        print(j, end=" ")
    print()
```

**Output:**

```text
1 2 3 4
1 2 3 4
1 2 3 4
1 2 3 4
```

---

## Example 9: Nested loop with lists

```python
students = [
    ["Sahil", "Python"],
    ["Rahul", "Java"],
    ["Amit", "JavaScript"]
]

for student in students:
    for item in student:
        print(item)
```

**Output:**

```text
Sahil
Python
Rahul
Java
Amit
JavaScript
```

This is useful for understanding **lists inside lists**.

---

## Example 10: Simple multiplication grid

```python
for i in range(1, 6):
    for j in range(1, 6):
        print(i * j, end="\t")
    print()
```

**Output:**

```text
1    2    3    4    5
2    4    6    8    10
3    6    9    12   15
4    8    12   16   20
5    10   15   20   25
```

This is a great example to show students why nested loops are useful.

---

# 🧠 Quick Comparison

| Loop | Main Idea | Example Use |
|---|---|---|
| `for` | Repeat over a sequence/range | Print 1–10 |
| `while` | Repeat while condition is true | Password checking |
| Nested `for` | Loop inside another loop | Patterns, tables, grids |
| Nested `while` | `while` inside `while` | More complex repetition |

**1. `for` → 2. `while` → 3. `break/continue` → 4. nested loops → 5. pattern programs.**

That progression keeps the brain from filing a formal complaint. 😄
