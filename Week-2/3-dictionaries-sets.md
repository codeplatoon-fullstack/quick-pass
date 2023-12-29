# Python Dictionaries, Sets, and Their Built-in Methods

## Introduction (5 minutes)

Welcome to today's lecture on Python dictionaries, sets, and their extensive built-in methods. Dictionaries and sets are fundamental data structures in Python, each serving unique purposes. In this lesson, we will explore these data structures and delve into the numerous built-in methods that make them powerful for data manipulation.

## Table of Contents

1. [Dictionaries](#1-dictionaries-45-minutes) (45 minutes)
   - [Creating Dictionaries](#a-creating-dictionaries-5-minutes)
   - [Dictionary Mutability](#b-dictionary-mutability-5-minutes)
   - [Common Dictionary Operations](#c-common-dictionary-operations-10-minutes)
   - [Dictionary Methods](#d-dictionary-methods-15-minutes)
2. [Sets](#2-sets-45-minutes) (45 minutes)
   - [Creating Sets](#a-creating-sets-5-minutes)
   - [Common Set Operations](#b-common-set-operations-10-minutes)
   - [Set Methods](#c-set-methods-15-minutes)
3. [Conclusion](#3-conclusion-5-minutes)

### 1. Dictionaries (45 minutes)

#### a. Creating Dictionaries (5 minutes)

- Dictionaries are unordered collections of key-value pairs.
- Created using curly braces or the `dict()` constructor.
- Example:

  ```python
  person = {"name": "Alice", "age": 30}
  ```

#### b. Dictionary Mutability (5 minutes)

- Dictionaries are mutable, meaning you can change their contents.
- You can add, remove, or modify key-value pairs.
- Example:

  ```python
  person = {"name": "Alice", "age": 30}
  person["age"] = 31  # Changes Alice's age to 31
  ```

#### c. Common Dictionary Operations (10 minutes)

- Accessing, checking membership, iteration, and more.
- Examples:

  ```python
  person = {"name": "Alice", "age": 30}
  age = person["age"]  # Accessing the age
  is_name_present = "name" in person  # Result: True
  ```

#### d. Dictionary Methods (15 minutes)

Dictionary Methods:

- `dict.keys()`: Return a list of all keys.
- `dict.values()`: Return a list of all values.
- `dict.items()`: Return a list of key-value pairs.
- `dict.get(key, default)`: Get the value associated with a key, or a default value if the key is not present.
- `dict.pop(key, default)`: Remove the item with a specific key and return its value, or a default value if the key is not present.
- `dict.popitem()`: Remove and return an arbitrary key-value pair.
- `dict.update(other_dict)`: Update the dictionary with key-value pairs from another dictionary.
- `dict.clear()`: Remove all items from the dictionary.

Code Examples:

```python
person = {"name": "Alice", "age": 30}

# Accessing keys and values
keys = person.keys()
values = person.values()

# Getting a value with a default
city = person.get("city", "Unknown")

# Removing an item
removed_age = person.pop("age")

# Updating the dictionary with another dictionary
additional_info = {"city": "New York", "gender": "Female"}
person.update(additional_info)

# Clearing the dictionary
person.clear()
```

### 2. Sets (45 minutes)

#### a. Creating Sets (5 minutes)

- Sets are unordered collections of unique elements.
- Created using the `set()` constructor.
- Example:

  ```python
  fruits = {"apple", "banana", "cherry"}
  ```

#### b. Common Set Operations (10 minutes)

- Checking membership, adding and removing elements, and more.
- Examples:

  ```python
  fruits = {"apple", "banana", "cherry"}
  is_apple_present = "apple" in fruits  # Result: True
  fruits.add("orange")  # Adds "orange" to the set
  fruits.remove("banana")  # Removes "banana" from the set
  ```

#### c. Set Methods (15 minutes)

Set Methods:

- `set.add(element)`: Add an element to the set.
- `set.remove(element)`: Remove an element from the set; raises an error if the element is not present.
- `set.discard(element)`: Remove an element from the set if it is present.
- `set.pop()`: Remove and return an arbitrary element from the set; raises an error if the set is empty.
- `set.clear()`: Remove all elements from the set.
- `set.union(other_set)`: Return a new set containing all elements from both sets.
- `set.intersection(other_set)`: Return a new set containing elements that are present in both sets.
- `set.difference(other_set)`: Return a new set containing elements that are in the set but not in the other set.
- `set.symmetric_difference(other_set)`: Return a new set containing elements that are in either set but not in both sets.

Code Examples:

```python
fruits = {"apple", "banana", "cherry"}
more_fruits = {"orange", "mango"}

# Combining two sets
all_fruits = fruits.union(more_fruits)

# Finding common elements
common_fruits = fruits.intersection(more_fruits)
```

### 3. Conclusion (5 minutes)

In this lecture, you've explored the power of dictionaries and sets in Python, along with their built-in methods. Dictionaries provide a flexible way to manage data using key-value pairs, while sets offer efficient storage for unique elements. Understanding when and how to use these data structures, as well as their methods, is essential for effective Python programming.

Continue to practice and apply these concepts in your Python projects to become proficient in working with dictionaries and sets.

This lecture comprehensively covers the built-in methods of dictionaries and sets in Python, providing explanations and code examples for each method.

### 4. Assignments

- [Number of Characters](https://replit.com/@cpadmin/Number-of-Characters-Python#main.py)
- [Car Trip](https://replit.com/@cpadmin/Car-Trip-Python#main.py)
- [How much will you spend](https://replit.com/@cpadmin/How-much-will-you-spend#main.py)
- [Employee Data](https://replit.com/@cpadmin/Employee-Data-Python#main.py)
