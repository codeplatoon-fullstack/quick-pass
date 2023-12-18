# Python Variables and Data Types

## Introduction (5 minutes)

Welcome to today's lecture on Python variables and data types. We'll learn about creating variables, naming conventions, and various data types in Python, such as dictionaries, tuples, lists, integers, strings, floats, and more. Additionally, we'll explore built-in methods for each data type and understand the concept of mutability and immutability.

## Table of Contents

1. [Variables](#1-variables-10-minutes) (10 minutes)
2. [Naming Conventions](#2-naming-conventions-10-minutes) (10 minutes)
3. [Data Types](#3-data-types-85-minutes) (85 minutes)
   - [Integers (int)](#a-integers-int)
   - [Floating-Point Numbers (float)](#b-floating-point-numbers-float)
   - [Strings (str)](#c-strings-str)
   - [Lists](#d-lists)
   - [Tuples](#e-tuples)
   - [Dictionaries (dict)](#f-dictionaries-dict)
   - [Sets](#g-sets-set)
   - [Booleans](#h-booleans-bool)
4. [Mutability and Immutability](#4-mutability-and-immutability-10-minutes) (10 minutes)
5. [Conclusion](#5-conclusion-5-minutes) (5 minutes)

### 1. Variables (10 minutes)

- Variables are used to store data in memory.
- In Python, you don't need to declare the data type explicitly.
- Example:

  ```python
  age = 25
  name = "Alice"
  ```

- The "`=`" sign is called the assignment operator and is used to assign variables. In Python, we use "`==`" to check for equality.
- You can check the type of a variable using the `type()` method.
- Example:

  ```python
  my_variable = 12.3
  type(my_variable)
  <class 'float'>
  ```

### 2. Naming Conventions (10 minutes)

- Variable names can consist of letters, numbers, and underscores.
- They must start with a letter or underscore but cannot start with a number.
- Variables are case-sensitive and should be written utilizing snake casing (yes = `a_variable` | not = `aVariable`).
- Use descriptive names for better code readability.

### 3. Data Types (85 minutes)

#### a. Integers (int)

- Whole numbers.
- Example:

  ```python
  age = 25
  # INTEGERS
  integer = 3
  integer = -3
  integer = 0
  not_an_integer ="3"
  not_an_integer = '3'
  ```

##### Integer Built in Methods

- Basic operations: `+, -, *, **, /, //, %`
- Other methods: `abs()`, `divmod()`, `pow()`

#### b. Floating-Point Numbers (float)

- Numbers with a decimal point.
- Example:

  ```python
  price = 19.99
  # FLOAT
  float_num = 1.12482
  float_num = 3749.0
  float_num = 0.0
  not_a_float = 1
  not_a_float = 2
  not_a_float = "0.0"
  ```

##### Float Built in Methods

- Basic operations: `+, -, *, **, /, //, %`
- Conversion methods: `int()`, `str()`, `round()`

#### c. Strings (str)

- Sequences of characters enclosed in single or double quotes.
- Example:

  ```python
  name = "Alice"
  # STRING
  string = "Hello I am a string"
  string = 'Hello I am also a string, notice that I can use either double or single quotes but still count as a string'
  string = """I am a rare kind of string that is wrapped by three sets of double quotes. I will explain my purpose later on"""
  f_string = f"I am a string that is prepended by an 'f', for now just remember I exist. I will explain my purpose later on"
  not_a_string = I am not a string because I am not wrapped by neither single nor double quotes
  ```

##### Strings Built In Methods

- String manipulation: `upper()`, `lower()`, `strip()`
- Searching and slicing: `find()`, `split()`, `replace()`

#### d. Lists

- Ordered collections of items, mutable.
- Example:

  ```python
  fruits = ["apple", "banana", "cherry"]
  # LISTS
  my_list = [1, 2, 3, 4, 5]
  colors = ["red", "green", "blue"]
  mixed_data = [42, "apple", True, 3.14]
  nested_list = [[1,2], ['grape', 'orange']]
  ```

##### Lists Built in Methods

- List manipulation: `append()`, `extend()`, `insert()`
- Removing elements: `remove()`, `pop()`, `clear()`

#### e. Tuples

- Ordered collections of items, immutable.
- Example:

  ```python
  coordinates = (3, 4)
  # TUPLES
  my_tuple = (1, 2, 3, 4, 5)
  coordinates = (3.14, 2.71)
  single_value_tuple = (42,)  # Note the trailing comma to indicate it's a tuple
  nested_tuple = ((1, 2), ("a", "b"))
  ```

##### Tuples Built In Methods

- Tuples are immutable, so they have fewer methods compared to lists.

#### f. Dictionaries (dict)

- Key-value pairs, mutable.
- Example:

  ```python
  # Dictionaries
  person = {"name": "Alice", "age": 25}
  person = {"name": "Alice", "age": 30, "city": "New York"}
  book = {"title": "Python Programming", "author": "John Smith", "pages": 400}
  nested_dict = {"person": {"name": "Bob", "age": 25}, "location": {"city": "Los Angeles"}}
  ```

##### Dictionary Built In Methods

- Dictionary methods: `keys()`, `values()`, `items()`
- Dictionary operations: `get()`, `pop()`, `update()`

#### g. Sets (set)

- Unordered collections of unique elements, mutable.
- Example:

  ```python
  # Sets
  my_set = {1, 2, 3, 4, 5}
  colors = {"red", "green", "blue"}
  mixed_set = {1, "apple", True, 3.14}
  ```

##### Set Built-In Methods

- Set methods: `add()`, `remove()`, `union()`
- Set operations: `intersection()`, `difference()`, `issubset()`

#### h. Booleans (bool)

- Represents binary values `True` and `False`.
- Example:

  ```python
  # Booleans
  is_student = True
  is_registered = False
  not_a_boolean = 'True'
  not_a_boolean = 'False'
  not_a_boolean = true
  not_a_boolean = false
  ```

##### Boolean Operations

- Logical operations: `and`, `or`, `not`
- Comparison operators: `==`, `!=`, `>`, `<`, `>=`, `<=`

### 4. Mutability and Immutability (10 minutes)

- Mutable data types (e.g., lists and dictionaries) can be modified in-place.
- Immutable data types (e.g., strings and tuples) cannot be modified once created.

### 5. Conclusion (5 minutes)

Today, we've covered the essentials of Python variables and data types. You've learned how to create variables, follow naming conventions, and work with various data types. Additionally, you've explored built-in methods for each data type and understand the concept of mutability and immutability. Keep practicing to master these concepts and become a proficient Python programmer!

### 6. Assignments

- [Data Type Practice](https://replit.com/@cpadmin/creatingdatatypes#main.py)
- [Fist and Last Name](https://replit.com/@cpadmin/First-Last-Name-Python)
