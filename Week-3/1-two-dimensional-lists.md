# Python Lecture: Mutating 2-Dimensional Lists

## Introduction (10 minutes)

Welcome to today's lecture on mutating 2-dimensional lists in Python. This comprehensive 2-hour lecture is designed for new programmers with little to no prior knowledge of Python fundamentals. We will start by reviewing basic concepts such as lists, for loops, and gradually introduce you to the techniques to manipulate 2-dimensional lists.

## Table of Contents

- [Python Lecture: Mutating 2-Dimensional Lists](#python-lecture-mutating-2-dimensional-lists)
  - [Introduction (10 minutes)](#introduction-10-minutes)
  - [Table of Contents](#table-of-contents)
  - [1. Understanding Lists (20 minutes)](#1-understanding-lists-20-minutes)
    - [What are Lists?](#what-are-lists)
    - [Creating and Accessing Lists](#creating-and-accessing-lists)
    - [Lists Within Lists (2-Dimensional Lists)](#lists-within-lists-2-dimensional-lists)
  - [2. Iterating Over Lists (20 minutes)](#2-iterating-over-lists-20-minutes)
    - [Using For Loops to Traverse a List](#using-for-loops-to-traverse-a-list)
    - [Nested For Loops for 2-Dimensional Lists](#nested-for-loops-for-2-dimensional-lists)
  - [3. Modifying 2-Dimensional Lists (35 minutes)](#3-modifying-2-dimensional-lists-35-minutes)
    - [Changing Elements in a 2-Dimensional List](#changing-elements-in-a-2-dimensional-list)
    - [Adding and Removing Elements](#adding-and-removing-elements)
    - [Replacing Rows and Columns](#replacing-rows-and-columns)
  - [4. Code Examples and Practice (45 minutes)](#4-code-examples-and-practice-45-minutes)
    - [Example 1: Modifying a Seating Chart](#example-1-modifying-a-seating-chart)
    - [Example 2: Managing Scores on a Scoreboard](#example-2-managing-scores-on-a-scoreboard)
    - [Example 3: Updating a Grid of Items](#example-3-updating-a-grid-of-items)
    - [Example 4: Adding Rows and Columns](#example-4-adding-rows-and-columns)
  - [5. Advanced Techniques (30 minutes)](#5-advanced-techniques-30-minutes)
    - [Transposing 2-Dimensional Lists](#transposing-2-dimensional-lists)
    - [Creating Copies and Avoiding Mutable Object Issues](#creating-copies-and-avoiding-mutable-object-issues)
    - [Practical Applications of 2-Dimensional Lists](#practical-applications-of-2-dimensional-lists)
  - [6. Conclusion (5 minutes)](#6-conclusion-5-minutes)

## 1. Understanding Lists (20 minutes)

### What are Lists?

- A list is a collection of values that can be of different types (integers, strings, etc.).
- Lists are ordered and indexed, which means each element has a position.

### Creating and Accessing Lists

- Creating lists using square brackets: `my_list = [1, 2, 3, 4, 5]`.
- Accessing elements by index: `my_list[2]` returns `3`.
- Negative indices start from the end: `my_list[-1]` returns `5`.

### Lists Within Lists (2-Dimensional Lists)

- A 2-dimensional list is a list of lists.
- It's like having rows and columns of data.
- Example:

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

## 2. Iterating Over Lists (20 minutes)

### Using For Loops to Traverse a List

- A for loop can be used to go through the elements of a list.
- Example:

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

### Nested For Loops for 2-Dimensional Lists

- When dealing with a 2-dimensional list, you need nested loops to traverse rows and columns.
- Example:

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

for row in matrix:
    for element in row:
        print(element)
```

## 3. Modifying 2-Dimensional Lists (35 minutes)

### Changing Elements in a 2-Dimensional List

- You can change the value of an element in a 2-dimensional list using indexing.
- Example:

```python
matrix[0][1] = 42  # Changes the element in the first row, second column to 42.
```

### Adding and Removing Elements

- You can add elements using `append`, `extend`, or `insert`.
- You can remove elements using `remove`, `pop`, or `del`.

### Replacing Rows and Columns

- To replace a row, simply assign a new list to the row index.
- To replace a column, use a for loop to iterate through rows and change elements.

## 4. Code Examples and Practice (45 minutes)

### Example 1: Modifying a Seating Chart

Let's say you have a seating chart for a theater, and you need to update a reserved seat.

```python
seating_chart = [
    ["A", "B", "C", "D"],
    ["E", "F", "G", "H"],
    ["I", "J", "K", "L"]
]

# Someone reserved seat "F" (row 2, seat 2). Let's update it.
seating_chart[1][1] = "X"
```

### Example 2: Managing Scores on a Scoreboard

You have a scoreboard for a game. A player's score needs to be updated.

```python
scoreboard = [
    ["Alice", 50],
    ["Bob", 45],
    ["Charlie", 60]
]

# Alice's score increased by 10 points.
scoreboard[0][1] += 10
```

### Example 3: Updating a Grid of Items

You have a grid of items, and you need to replace one of them.

```python
grid = [
    ["X", "O", "X"],
    ["O", "X", "O"],
    ["O", "O", "X"]
]

# Let's replace the center element with "O".
grid[1][1] = "O"
```

### Example 4: Adding Rows and Columns

You have a sales dataset, and you want to add a new salesperson's data.

```python
sales_data = [
    ["Name", "Jan", "Feb", "Mar"],
    ["Alice", 100, 120, 90],
    ["Bob", 80, 85, 90]
]

# Adding a new row for "Charlie."
new_salesperson = ["Charlie", 110, 95, 105]
sales_data.append(new_salesperson)

# Adding a new column for "Apr."
for i in range(len(sales_data)):
    sales_data[i].append(0)  # Initial value for April.
```

## 5. Advanced Techniques (30 minutes)

### Transposing 2-Dimensional Lists

- To swap rows and columns, you can use list comprehensions.
- Example:

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6]
]

transposed = [[row[i] for row in matrix] for i in range(len(matrix[0]))]
```

### Creating Copies and Avoiding Mutable Object Issues

- Be cautious when copying 2-dimensional lists. The `copy` module can help avoid issues.
- Example:

```python
import copy

original = [[1, 2], [3, 4]]
shallow_copy = copy.copy(original)
deep_copy = copy.deepcopy(original)
```

### Practical Applications of 2-Dimensional Lists

- 2-dimensional lists are essential for organizing data tables, images, games, and more.
- From creating chess boards to analyzing data sets, 2-D lists have a wide range of applications.

## 6. Conclusion (5 minutes)

In this extensive 2-hour lecture, you've explored the fundamentals of working with 2-dimensional lists in Python. You have learned how to create, access, and modify elements in these lists. Practice is the key to mastering this skill, so continue to work with 2-dimensional lists and explore more complex scenarios.
