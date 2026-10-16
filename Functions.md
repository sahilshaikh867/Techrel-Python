# 🐍 Python Functions 
### Beginner → Professional

---

# 🟢 LEVEL 1 — Function Basics

## 1. Simple Function

```python
# Define a simple function
def greet():
    print("Hello, Welcome to Python!")

# Call the function
greet()
```

---

## 2. Function with One Parameter

```python
# name is a parameter of the function
def greet(name):
    print("Hello", name)

# Passing "Sahil" as an argument
greet("Sahil")
```

**Output:**
```text
Hello Sahil
```

---

## 3. Function with Two Parameters

```python
# Function accepts two values
def add(a, b):
    print(a + b)

# Call the function
add(10, 20)
```

---

## 4. Function Returning a Value

```python
# return sends the result back to the caller
def add(a, b):
    return a + b

# Store returned value in a variable
result = add(10, 20)

print(result)
```

---

## 5. Function for Subtraction

```python
def subtract(a, b):
    # Subtract b from a
    return a - b

result = subtract(20, 5)

print(result)
```

---

## 6. Function for Multiplication

```python
def multiply(a, b):
    # Multiply two numbers
    return a * b

print(multiply(5, 4))
```

---

## 7. Function for Division

```python
def divide(a, b):
    # Divide a by b
    return a / b

print(divide(20, 5))
```

---

## 8. Function with Default Parameter

```python
# If no name is provided, "Guest" will be used
def greet(name="Guest"):
    print("Hello", name)

greet()
greet("Sahil")
```

---

## 9. Function with Multiple Parameters

```python
def student_info(name, age, city):
    # Display student information
    print("Name:", name)
    print("Age:", age)
    print("City:", city)

student_info("Sahil", 22, "Pune")
```

---

## 10. Function to Check Even Number

```python
def check_even(number):
    # % gives the remainder
    if number % 2 == 0:
        return True
    else:
        return False

print(check_even(10))
```

---

# 🟢 LEVEL 2 — Beginner Practical Functions

## 11. Calculate Square

```python
def square(number):
    # Multiply number by itself
    return number * number

print(square(5))
```

---

## 12. Calculate Cube

```python
def cube(number):
    # Calculate cube of a number
    return number ** 3

print(cube(3))
```

---

## 13. Find Maximum of Two Numbers

```python
def maximum(a, b):
    # Compare two numbers
    if a > b:
        return a
    else:
        return b

print(maximum(10, 20))
```

---

## 14. Find Minimum of Two Numbers

```python
def minimum(a, b):
    if a < b:
        return a
    else:
        return b

print(minimum(10, 20))
```

---

## 15. Check Positive, Negative or Zero

```python
def check_number(number):

    if number > 0:
        return "Positive"

    elif number < 0:
        return "Negative"

    else:
        return "Zero"


print(check_number(-10))
```

---

## 16. Calculate Area of Circle

```python
def circle_area(radius):

    # Approximate value of PI
    pi = 3.14159

    # Formula: π × r²
    return pi * radius ** 2


print(circle_area(5))
```

---

## 17. Calculate Rectangle Area

```python
def rectangle_area(length, width):

    # Formula: length × width
    return length * width


print(rectangle_area(10, 5))
```

---

## 18. Convert Celsius to Fahrenheit

```python
def celsius_to_fahrenheit(celsius):

    # Formula:
    # Fahrenheit = (Celsius × 9/5) + 32
    return (celsius * 9 / 5) + 32


print(celsius_to_fahrenheit(30))
```

---

## 19. Check Voting Eligibility

```python
def check_voting_age(age):

    # A person must be 18 or older
    if age >= 18:
        return "Eligible to vote"
    else:
        return "Not eligible to vote"


print(check_voting_age(20))
```

---

## 20. Calculate Student Grade

```python
def calculate_grade(marks):

    if marks >= 90:
        return "A"

    elif marks >= 75:
        return "B"

    elif marks >= 60:
        return "C"

    elif marks >= 40:
        return "D"

    else:
        return "Fail"


print(calculate_grade(82))
```

---

# 🟡 LEVEL 3 — Functions + Loops

## 21. Print Numbers

```python
def print_numbers(n):

    # Loop from 1 to n
    for i in range(1, n + 1):
        print(i)


print_numbers(5)
```

---

## 22. Calculate Sum

```python
def calculate_sum(n):

    total = 0

    # Add every number to total
    for i in range(1, n + 1):
        total += i

    return total


print(calculate_sum(10))
```

---

## 23. Multiplication Table

```python
def multiplication_table(number):

    for i in range(1, 11):

        # Print multiplication result
        print(number, "x", i, "=", number * i)


multiplication_table(5)
```

---

## 24. Count Even Numbers

```python
def count_even(numbers):

    count = 0

    for number in numbers:

        # Check whether number is even
        if number % 2 == 0:
            count += 1

    return count


numbers = [1, 2, 4, 7, 8, 10]

print(count_even(numbers))
```

---

## 25. Find Largest Number in List

```python
def find_largest(numbers):

    largest = numbers[0]

    for number in numbers:

        if number > largest:
            largest = number

    return largest


numbers = [10, 25, 7, 40, 15]

print(find_largest(numbers))
```

---

## 26. Calculate List Average

```python
def calculate_average(numbers):

    total = 0

    for number in numbers:
        total += number

    # len() gives number of elements
    return total / len(numbers)


marks = [80, 75, 90, 85]

print(calculate_average(marks))
```

---

## 27. Count Vowels

```python
def count_vowels(text):

    count = 0

    # Check every character
    for character in text.lower():

        if character in "aeiou":
            count += 1

    return count


print(count_vowels("Python Programming"))
```

---

## 28. Reverse a String

```python
def reverse_string(text):

    # [::-1] reverses the string
    return text[::-1]


print(reverse_string("Python"))
```

---

## 29. Check Palindrome

```python
def is_palindrome(text):

    # Convert to lowercase
    text = text.lower()

    # Compare original with reversed text
    return text == text[::-1]


print(is_palindrome("madam"))
```

---

## 30. Find Factorial

```python
def factorial(number):

    result = 1

    for i in range(1, number + 1):
        result *= i

    return result


print(factorial(5))
```

---

# 🟡 LEVEL 4 — Arguments and Advanced Function Basics

## 31. Keyword Arguments

```python
def student(name, age, city):

    print("Name:", name)
    print("Age:", age)
    print("City:", city)


# Arguments are passed using parameter names
student(
    name="Sahil",
    age=22,
    city="Pune"
)
```

---

## 32. Positional Arguments

```python
def add(a, b):

    return a + b


# Values are assigned according to position
print(add(10, 20))
```

---

## 33. `*args`

`*args` allows a function to accept **multiple positional arguments**.

```python
def add_numbers(*numbers):

    total = 0

    # Loop through all received numbers
    for number in numbers:
        total += number

    return total


print(add_numbers(10, 20))
print(add_numbers(10, 20, 30, 40))
```

---

## 34. `**kwargs`

`**kwargs` allows multiple **keyword arguments**.

```python
def student_info(**details):

    # details is stored as a dictionary
    for key, value in details.items():
        print(key, ":", value)


student_info(
    name="Sahil",
    age=22,
    city="Pune"
)
```

---

## 35. Combining Normal Parameter and `*args`

```python
def calculate_average(name, *marks):

    total = sum(marks)

    average = total / len(marks)

    print("Student:", name)
    print("Average:", average)


calculate_average("Sahil", 80, 75, 90)
```

---

## 36. Function Returning Multiple Values

```python
def calculate(a, b):

    addition = a + b
    subtraction = a - b
    multiplication = a * b

    # Return three values
    return addition, subtraction, multiplication


result = calculate(10, 5)

print(result)
```

---

## 37. Unpacking Returned Values

```python
def calculate(a, b):

    return a + b, a - b


# Store returned values separately
addition, subtraction = calculate(10, 5)

print("Addition:", addition)
print("Subtraction:", subtraction)
```

---

## 38. Function Inside Another Function

```python
def outer():

    print("Outer function")

    def inner():

        print("Inner function")

    # Call inner function
    inner()


outer()
```

---

## 39. Recursive Function

A recursive function **calls itself**.

```python
def countdown(number):

    if number == 0:
        print("Done!")
        return

    print(number)

    # Function calls itself
    countdown(number - 1)


countdown(5)
```

---

## 40. Recursive Factorial

```python
def factorial(number):

    # Base condition
    if number == 0:
        return 1

    # Function calls itself
    return number * factorial(number - 1)


print(factorial(5))
```

---

# 🟠 LEVEL 5 — Advanced Functions

## 41. Lambda Function

A lambda is a **small anonymous function**.

```python
# Normal function:
def square(x):
    return x * x


# Lambda version:
square_lambda = lambda x: x * x

print(square_lambda(5))
```

---

## 42. Lambda with Two Arguments

```python
# Lambda accepts two parameters
add = lambda a, b: a + b

print(add(10, 20))
```

---

## 43. Function as an Argument

Functions can be passed to other functions.

```python
def square(number):
    return number * number


def calculate(function, number):

    # Call the function received as an argument
    return function(number)


result = calculate(square, 5)

print(result)
```

This concept is called a **higher-order function**.

---

## 44. `map()` with Function

```python
numbers = [1, 2, 3, 4, 5]


def square(number):
    return number * number


# Apply square() to every number
result = map(square, numbers)

# Convert map object to list
print(list(result))
```

Output:

```text
[1, 4, 9, 16, 25]
```

---

## 45. `filter()` with Function

```python
numbers = [1, 2, 3, 4, 5, 6]


def is_even(number):

    return number % 2 == 0


# Keep only numbers where function returns True
result = filter(is_even, numbers)

print(list(result))
```

Output:

```text
[2, 4, 6]
```

---

## 46. Closure

A closure is a function that **remembers values from its outer function**.

```python
def multiplier(x):

    def multiply(number):

        # Inner function remembers x
        return number * x

    return multiply


double = multiplier(2)

triple = multiplier(3)

print(double(5))
print(triple(5))
```

Output:

```text
10
15
```

---

## 47. Decorator

A decorator allows us to **add functionality to an existing function**.

```python
def decorator(function):

    def wrapper():

        print("Before function")

        # Call original function
        function()

        print("After function")

    return wrapper


@decorator
def hello():

    print("Hello!")


hello()
```

Output:

```text
Before function
Hello!
After function
```

---

## 48. Decorator with Arguments

```python
def login_required(function):

    def wrapper(username):

        # Check whether user is logged in
        if username == "Sahil":

            function(username)

        else:

            print("Access denied")

    return wrapper


@login_required
def dashboard(username):

    print("Welcome to dashboard,", username)


dashboard("Sahil")
dashboard("Rahul")
```

This pattern is commonly seen in **web applications and APIs**.

---

# 🔴 LEVEL 6 — Professional Python

## 49. Type Hints + Docstring

This is closer to professional Python code.

```python
def calculate_total(price: float, quantity: int) -> float:
    """
    Calculate the total price.

    Parameters:
        price: Price of one item.
        quantity: Number of items.

    Returns:
        Total price.
    """

    return price * quantity


total = calculate_total(500.0, 3)

print("Total:", total)
```

### Why this is professional?

It provides:

- Type hints
- Documentation
- Clear parameter names
- Clear return type
- Readable structure

---

# 🔴 50. Professional Function with Validation and Exception Handling

```python
def withdraw_money(balance: float, amount: float) -> float:
    """
    Withdraw money from an account.

    Parameters:
        balance: Current account balance.
        amount: Amount to withdraw.

    Returns:
        Updated account balance.

    Raises:
        ValueError: If the withdrawal amount is invalid.
    """

    # Check whether amount is positive
    if amount <= 0:
        raise ValueError("Withdrawal amount must be greater than zero")

    # Check whether sufficient balance exists
    if amount > balance:
        raise ValueError("Insufficient balance")

    # Calculate new balance
    new_balance = balance - amount

    return new_balance


try:

    balance = 10000

    amount = 2500

    # Call the function
    balance = withdraw_money(balance, amount)

    print("Withdrawal successful")
    print("Remaining balance:", balance)

except ValueError as error:

    # Handle validation errors
    print("Error:", error)
```

This combines several concepts:

```text
Function
   ↓
Type Hints
   ↓
Docstring
   ↓
Validation
   ↓
Exception Handling
   ↓
Return Value
```

---

# 📊 50 Functions — Learning Roadmap

| Level | Examples | Concepts |
|---|---:|---|
| 🟢 Beginner | 1–10 | Basic functions, parameters, return |
| 🟢 Beginner | 11–20 | Practical functions |
| 🟡 Intermediate | 21–30 | Loops + functions |
| 🟡 Intermediate | 31–40 | Arguments, `*args`, `**kwargs`, recursion |
| 🟠 Advanced | 41–48 | Lambda, map, filter, closures, decorators |
| 🔴 Professional | 49–50 | Type hints, docstrings, validation, exceptions |

## ⭐ Most Important Concepts Students Should Remember

```text
def
 ↓
Function
 ↓
Parameter
 ↓
Argument
 ↓
return
 ↓
Default Argument
 ↓
Positional Argument
 ↓
Keyword Argument
 ↓
*args
 ↓
**kwargs
 ↓
Nested Function
 ↓
Recursion
 ↓
Lambda
 ↓
Higher-Order Function
 ↓
map / filter
 ↓
Closure
 ↓
Decorator
 ↓
Type Hints
 ↓
Docstrings
 ↓
Exception Handling
```

**Teaching tip:** Don't jump from `def hello()` straight to decorators. 😄 Let students first become comfortable with **parameters → return → loops → lists → `*args/**kwargs` → recursion**, then introduce the advanced concepts. That progression mirrors how functions actually become useful in real Python applications.
