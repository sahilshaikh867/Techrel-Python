# 🐍 Python Variables

## What is a Variable?

A **variable is a name used to store data/value in a program.**

Think of it like a **box with a name**:

```python
name = "Sahil"
age = 22
```

Here:

- `name` → variable
- `"Sahil"` → value
- `age` → variable
- `22` → value

---

## Example 1: Store a Name

```python
name = "Sahil"

print(name)
```

**Output:**
```text
Sahil
```

---

## Example 2: Store Age

```python
age = 22

print(age)
```

**Output:**
```text
22
```

---

## Example 3: Store Multiple Variables

```python
name = "Sahil"
age = 22
city = "Pune"

print(name)
print(age)
print(city)
```

**Output:**
```text
Sahil
22
Pune
```

---

## Example 4: Different Types of Variables

Python can store different types of values.

```python
name = "Sahil"       # String
age = 22             # Integer
height = 5.8         # Float
is_student = True    # Boolean

print(name)
print(age)
print(height)
print(is_student)
```

### Types:

```text
name       → str
age        → int
height     → float
is_student → bool
```

---

## Example 5: Change the Value of a Variable

Variables can be changed.

```python
age = 20

print(age)

age = 21

print(age)
```

**Output:**
```text
20
21
```

The variable `age` first contains `20`, then we replace it with `21`.

---

## Example 6: Add Two Variables

```python
num1 = 10
num2 = 20

result = num1 + num2

print(result)
```

**Output:**
```text
30
```

Here:

```text
num1 = 10
num2 = 20

10 + 20 = 30
```

---

## Example 7: Calculate Student Marks

```python
maths = 80
science = 75
english = 85

total = maths + science + english

print("Total Marks =", total)
```

**Output:**
```text
Total Marks = 240
```

This is a good **real-world example** for students.

---

## Example 8: Calculate Average

```python
maths = 80
science = 75
english = 85

total = maths + science + english
average = total / 3

print("Total =", total)
print("Average =", average)
```

**Output:**
```text
Total = 240
Average = 80.0
```

---

## Example 9: User Input into Variables

Variables become much more useful when combined with `input()`.

```python
name = input("Enter your name: ")
age = input("Enter your age: ")

print("Name:", name)
print("Age:", age)
```

If the user enters:

```text
Enter your name: Sahil
Enter your age: 22
```

Output:

```text
Name: Sahil
Age: 22
```

### Important

`input()` normally returns a **string**.

For numbers, use:

```python
age = int(input("Enter your age: "))
```

---

## Example 10: Simple Shopping Bill

This is a nice practical example.

```python
product = "Laptop"
price = 50000
quantity = 2

total = price * quantity

print("Product:", product)
print("Price:", price)
print("Quantity:", quantity)
print("Total:", total)
```

**Output:**

```text
Product: Laptop
Price: 50000
Quantity: 2
Total: 100000
```

---

# 🧠 Bonus: Variable Naming Rules

Students should learn these early.

### ✅ Correct

```python
name = "Sahil"
student_age = 22
total_marks = 450
student1 = "Rahul"
```

### ❌ Incorrect

```python
student age = 22     # Space not allowed
1student = "Rahul"   # Cannot start with number
student-name = "A"   # Hyphen not allowed
```

### Python is case-sensitive

These are **different variables**:

```python
name = "Sahil"
Name = "Rahul"
NAME = "Amit"
```

Python treats them as three different names.
