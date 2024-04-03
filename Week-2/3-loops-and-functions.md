# Python Loops and Functions

## Introduction

Welcome to Day 3 of the Python Quick Pass! Today, we'll explore loops, a fundamental concept in programming, and dive into the world of functions. Loops allow us to perform repetitive tasks, and functions help us structure our code and make it more organized and reusable. Let's get started!

## Table of Contents

- [Python Loops and Functions](#python-loops-and-functions)
  - [Introduction](#introduction)
  - [Table of Contents](#table-of-contents)
    - [1. Loops](#1-loops)
      - [a. for i in x (for element in iterable)](#a-for-i-in-x-for-element-in-iterable)
      - [b. for i in range (for i in range(start, stop, step))](#b-for-i-in-range-for-i-in-rangestart-stop-step)
      - [c. for idx, item in enumerate(iterable)](#c-for-idx-item-in-enumerateiterable)
      - [d. for key, value in dict.items()](#d-for-key-value-in-dictitems)
      - [e. When to Choose](#e-when-to-choose)
      - [f. while Loop](#f-while-loop)
    - [2. Loops with Data Structures](#2-loops-with-data-structures)
      - [a. Strings](#a-strings)
      - [b. Lists](#b-lists)
      - [c. Tuples](#c-tuples)
      - [d. Dictionaries](#d-dictionaries)
    - [3. Functions](#3-functions)
      - [Basic Function](#basic-function)
      - [Functions with Multiple Parameters](#functions-with-multiple-parameters)
      - [Nested Functions](#nested-functions)
      - [Variable Scope within Functions](#variable-scope-within-functions)
      - [The `return` Statement](#the-return-statement)
      - [When to Use `print` Statements](#when-to-use-print-statements)
    - [4. Conclusion](#4-conclusion)

### 1. Loops

Loops are used to execute a block of code repeatedly. Python provides several types of loops. Let's explore them.

Here are examples of different types of `for` loops in Python along with explanations for their use cases:

#### a. for i in x (for element in iterable)

```python
urls = ["www.reddit.com", "www.nike.com", "www.codeplatoon.org", "www.amazon.com"]
for url in urls:
    print(url)
```

**Use Case:** This loop iterates through the elements of a list or any iterable. It's suitable when you want to perform the same operation for each item in the iterable. In this case, it's used to print each website URL.

#### b. for i in range (for i in range(start, stop, step))

```python
for i in range(1, 6, 2):
    print(i)
```

**Use Case:** The `for i in range` loop is used when you need to iterate a specific number of times, often with a loop counter (`i`) that increments by a constant value (`step`). It's useful for tasks where you need to control the number of iterations and when you don't necessarily need to access elements in a collection.

#### c. for idx, item in enumerate(iterable)

```python
fruits = ["Bananas", "Apples", "Cherries"]
for index, fruit in enumerate(fruits):
    print(f"Index {index}: {fruit}")
```

**Use Case:** The `for idx, item in enumerate` loop allows you to access both the elements and their indices within an iterable. This is helpful when you need to keep track of the position of each element in the collection.

#### d. for key, value in dict.items()

```python
phones = {"Francisco": "555-555-5555", "Alex": "222-222-2222", "Allison": "111-111-1111"}
for name, number in phones.items():
    print(f"{name}'s phone number is {number}")
```

**Use Case:** The `for key, value in dict.items()` loop is used to iterate through the key-value pairs in a dictionary. It's beneficial when you need to work with both keys and values from a dictionary simultaneously.

#### e. When to Choose

- Use `for i in x` when you want to iterate through the elements of a collection.
- Use `for i in range` when you need a loop with a specific number of iterations.
- Use `for idx, item in enumerate` when you need to access both elements and their indices within an iterable.
- Use `for key, value in dict.items()` when working with key-value pairs in a dictionary.

Choose the appropriate `for` loop based on your specific task and what you need to achieve in your code. Each type of loop serves a different purpose and offers advantages depending on the situation.

#### f. while Loop

The `while` loop repeatedly executes a block of code as long as a condition is `True`.

_Be careful with while loops. You can easily start an infinite loop with a typo_

Syntax:

```python
while condition:
    # Code to execute while the condition is True
```

Example:

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

### 2. Loops with Data Structures

Let's explore how loops can be used with various data structures.

#### a. Strings

Strings are an interable data structure. You can loop through characters in a string using a `for-in` loop.

Example:

```python
text = "Hello, World!"
for char in text:
    print(char)
```

#### b. Lists

Loops are often used to iterate through the elements of a list.

Example:

```python
auto_brands = ["Chevrolet", "Tesla", "Jeep"]
for brand in auto_brands
    print(brand)
```

#### c. Tuples

Similar to lists, you can use loops to iterate through elements in a tuple.

Example:

```python
coordinates = (3, 4)
for coordinate in coordinates:
    print(coordinate)
```

#### d. Dictionaries

Dictionaries are iterable, and you can loop through keys, values, or key-value pairs.

Example:

```python
person = {"name": "Alice", "age": 25}
for key in person:
    print(key, person[key])
```

### 3. Functions

Functions are a fundamental concept in Python, allowing you to define reusable blocks of code. Let's delve deeper into functions, including ones with multiple parameters, nested functions, variable scope, the purpose of the `return` statement, and when to use a `print` statement.

#### Basic Function

The syntax for defining a basic function in Python is as follows:

```python
def function_name(parameter1, parameter2, ...):
    # Code to execute inside the function
    return result  # (optional)
```

Example of a basic function:

```python
def greet(name):
    return f"Hello, {name}!"

message = greet("Alice")
print(message)
```

In the example, we defined a function `greet` that takes one parameter, `name`. It returns a greeting message with the provided name and assigns it to the variable `message`, which is then printed.

#### Functions with Multiple Parameters

You can create functions with multiple parameters to handle more complex tasks. For instance:

```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)  # Output: 8
```

Here, the function `add` accepts two parameters, `a` and `b`, and returns their sum.

#### Nested Functions

Python allows you to define functions within functions, known as nested functions. This is useful for encapsulating logic and reusing code fragments.

```python
def outer_function(x):
    def inner_function(y):
        return x + y
    return inner_function

add_five = outer_function(5)
result = add_five(3)
print(result)  # Output: 8
```

In this example, `inner_function` is nested within `outer_function`. The `outer_function` returns the `inner_function`, which can then be used to add `5` to a value.

#### Variable Scope within Functions

Variables inside a function have local scope, meaning they are only accessible within that function. Here's an illustration:

```python
def my_function():
    x = 10
    print(x)

my_function()
print(x)  # This will raise an error
```

In this case, `x` is a local variable, and attempting to print it outside the function scope will result in an error.

#### The `return` Statement

The `return` statement is used to specify the value that a function should return. It's optional, and a function can return nothing (i.e., `None`) if `return` is omitted.

```python
def multiply(a, b):
    return a * b

result = multiply(4, 3)
print(result)  # Output: 12
```

In this example, the `multiply` function returns the product of `a` and `b`.

#### When to Use `print` Statements

While functions are designed to encapsulate logic and produce results, you might need to use `print` statements within functions for debugging purposes or to provide visual feedback. It's common to print intermediate results or diagnostic information while developing and testing code.

```python
def complex_calculation(x, y):
    result = x * y
    print(f"Intermediate result: {result}")
    return result
```

In this example, the `print` statement helps monitor the progress of the `complex_calculation` function.

Functions in Python are powerful tools for organizing and reusing code. Whether you need to define functions with multiple parameters, nest functions, manage variable scope, or control the output using `return` and `print`, understanding how to use functions effectively is crucial for building complex and maintainable programs.

### 4. Conclusion

Today, we've delved into loops, an essential tool for performing repetitive tasks, and functions, which help us organize and reuse code. You've learned about different types of loops and how to use them with various data structures. Additionally, you've seen how to create and call functions in Python.

Keep practicing loops and functions as they are fundamental building blocks for creating more complex Python programs. We look forward to seeing you for Day 4, where we'll explore more advanced Python concepts.
