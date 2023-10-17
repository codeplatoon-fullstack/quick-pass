# Lists and Tuples in Python: Capabilities and Limitations

## Introduction (5 minutes)

Welcome to today's lecture on lists and tuples in Python. Lists and tuples are fundamental data structures used for storing collections of items. In this lesson, we'll explore the capabilities and limitations of lists and tuples, understand the concepts of mutable and immutable data structures, and delve into the usage of various built-in methods for each data structure.

## Table of Contents

1. [Lists](#1-lists-45-minutes) (45 minutes)
   - [Creating Lists](#a-creating-lists-5-minutes)
   - [List Mutability](#b-list-mutability-5-minutes)
   - [Common List Operations](#c-common-list-operations-10-minutes)
   - [List Methods](#d-list-methods-15-minutes)
   - [List Slicing](#e-list-slicing-10-minutes)
   - [List Comprehensions](#f-list-comprehensions-5-minutes)
2. [Tuples](#2-tuples-45-minutes) (45 minutes)
   - [Creating Tuples](#a-creating-tuples-5-minutes)
   - [Tuple Immutability](#b-tuple-immutability-5-minutes)
   - [Common Tuple Operations](#c-common-tuple-operations-10-minutes)
   - [Tuple Methods](#d-tuple-methods-15-minutes)
   - [Tuple Unpacking](#e-tuple-unpacking-10-minutes)
3. [Conclusion](#3-conclusion-5-minutes)

### 1. Lists (45 minutes)

#### a. Creating Lists (5 minutes)

- Lists are ordered collections of items.
- Created using square brackets.
- Example:

  ```python
  numbers = [1, 2, 3, 4, 5]
  ```

#### b. List Mutability (5 minutes)

- Lists are mutable, meaning you can change their contents.
- You can add, remove, or modify elements.
- Example:

  ```python
  numbers = [1, 2, 3, 4, 5]
  numbers[0] = 10  # Changes the first element to 10
  ```

#### c. Common List Operations (10 minutes)

- Iteration, length, checking membership, and more.
- Examples:

  ```python
  numbers = [1, 2, 3, 4, 5]
  length = len(numbers)  # Result: 5
  is_two_present = 2 in numbers  # Result: True
  ```

#### d. List Methods (15 minutes)

- Extensive list methods for adding, removing, sorting, etc.
- Examples:

  ```python
  fruits = ["apple", "banana", "cherry"]
  fruits.append("orange")  # Appends "orange" to the list
  fruits.remove("banana")  # Removes "banana" from the list
  fruits.sort()  # Sorts the list alphabetically
  ```
  
List Methods:

- `list.append(x)`: Add an item to the end of the list.
- `list.extend(iterable)`: Extend the list by appending elements from the iterable.
- `list.insert(i, x)`: Insert an item at a given position.
- `list.remove(x)`: Remove the first item from the list with a specific value.
- `list.pop([i])`: Remove the item at the given position in the list.
- `list.clear()`: Remove all items from the list.
- `list.index(x)`: Return the index of the first item with a specific value.
- `list.count(x)`: Return the number of times a specific value appears in the list.
- `list.sort()`: Sort the items of the list in place.
- `list.reverse()`: Reverse the elements of the list in place.
- `list.copy()`: Return a shallow copy of the list.

#### e. List Slicing (10 minutes)

- Allows you to create sublists from a list.
- Syntax: `list[start:stop:step]`.
- Examples:

  ```python
  numbers = [0, 1, 2, 3, 4, 5]
  sub_list = numbers[1:4]  # Results in [1, 2, 3]
  reversed_list = numbers[::-1]  # Reverses the list
  ```

#### f. List Comprehensions (5 minutes)

- Concise way to create lists based on existing lists.
- Examples:

  ```python
  numbers = [1, 2, 3, 4, 5]
  squared_numbers = [x ** 2 for x in numbers]  # Squares each element
  ```

### 2. Tuples (45 minutes)

#### a. Creating Tuples (5 minutes)

- Tuples are ordered collections, similar to lists.
- Created using parentheses.
- Example:

  ```python
  coordinates = (3, 4)
  ```

#### b. Tuple Immutability (5 minutes)

- Tuples are immutable; their contents cannot be changed.
- Once created, elements cannot be added, removed, or modified.
- Example:

  ```python
  coordinates = (3, 4)
  # The following line would raise an error:
  # coordinates[0] = 5
  ```

#### c. Common Tuple Operations (10 minutes)

- Similar operations as lists (iteration, length, checking membership).
- Examples:

  ```python
  coordinates = (3, 4)
  length = len(coordinates)  # Result: 2
  is_five_present = 5 in coordinates  # Result: False
  ```

#### d. Tuple Methods (15 minutes)

- Limited methods due to immutability.
- Examples:

  ```python
  coordinates = (3, 4)
  index = coordinates.index(4)  # Returns the index of 4
  count = coordinates.count(3)  # Counts occurrences of 3
  ```
  
Tuple Methods:

- `tuple.count(value)`: Return the number of times a value appears in the tuple.
- `tuple.index(value, start, stop)`: Return the index of the first occurrence of a value.

#### e. Tuple Unpacking (10 minutes)

- Assigning tuple elements to variables.
- Example:

  ```python
  coordinates = (3, 4)
  x, y = coordinates
  ```

### 3. Conclusion (5 minutes)

In this lecture, you've explored the capabilities and limitations of Python lists and tuples. Lists are mutable and offer extensive methods for manipulation, making them suitable for dynamic collections. Tuples, on the other hand, are immutable and provide security for data that should not change. Understanding when and how to use each structure is crucial in Python programming.

Remember to practice and apply these concepts in your Python projects to become proficient in working with lists and tuples.
