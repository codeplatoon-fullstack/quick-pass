# Python Strings and Their Built-in Methods

## Introduction (5 minutes)

Welcome to today's lecture on Python strings and their built-in methods. Strings are one of the most fundamental data types in Python, and they come with a wide range of methods that allow you to manipulate and transform them in various ways. In this lesson, we will explore the essential built-in string methods, how they work, and when and how to use them effectively.

## Table of Contents

1. [Built-in String Methods](#1-built-in-string-methods-90-minutes) (90 minutes)
   - [str.upper()](#a-strupper-5-minutes)
   - [str.lower()](#b-strlower-5-minutes)
   - [str.capitalize()](#c-strcapitalize-5-minutes)
   - [str.title()](#d-strtitle-5-minutes)
   - [str.strip()](#e-strstrip-5-minutes)
   - [str.startswith()](#f-strstartswith-5-minutes)
   - [str.endswith()](#g-strendswith-5-minutes)
   - [str.find()](#h-strfind-5-minutes)
   - [str.count()](#i-strcount-5-minutes)
   - [str.replace()](#j-strreplace-5-minutes)
   - [str.split()](#k-strsplit-5-minutes)
   - [str.join()](#l-strjoin-5-minutes)
   - [str.isalpha()](#m-strisalpha-5-minutes)
   - [str.isnumeric()](#n-strisnumeric-5-minutes)
   - [str.isalnum()](#o-stris)
   - [str.islower()](#p-strislower-5-minutes)
   - [str.isupper()](#q-strisupper-5-minutes)
2. [Interpolated String](#2-interpolated-strings-10-minutes)
3. [Escape Sequences](#3-escape-sequences-10-minutes)
4. [Slicing and Reversin](#4-slicing-and-reversing-10-minutes)
5. [Conclusion](#5-conclusion-5-minutes)

### 1. Built-in String Methods (90 minutes)

#### a. `str.upper()` (5 minutes)

- **Description**: Converts all characters in a string to uppercase.
- **Use Case**: Useful for ensuring consistent formatting or performing case-insensitive comparisons.
- **Example**:

  ```python
  text = "hello, world"
  upper_text = text.upper()  # Result: "HELLO, WORLD"
  ```

#### b. `str.lower()` (5 minutes)

- **Description**: Converts all characters in a string to lowercase.
- **Use Case**: Useful for ensuring consistent formatting or performing case-insensitive comparisons.
- **Example**:

  ```python
  text = "Hello, World"
  lower_text = text.lower()  # Result: "hello, world"
  ```

#### c. `str.capitalize()` (5 minutes)

- **Description**: Capitalizes the first character of a string and makes all others lowercase.
- **Use Case**: Useful for capitalizing names or titles.
- **Example**:

  ```python
  text = "python programming"
  capitalized_text = text.capitalize()  # Result: "Python programming"
  ```

#### d. `str.title()` (5 minutes)

- **Description**: Capitalizes the first character of each word in a string.
- **Use Case**: Useful for creating title case text.
- **Example**:

  ```python
  text = "python programming"
  title_text = text.title()  # Result: "Python Programming"
  ```

#### e. `str.strip()` (5 minutes)

- **Description**: Removes leading and trailing whitespace from a string.
- **Use Case**: Useful for cleaning user input or when working with data that may have inconsistent spacing.
- **Example**:

  ```python
  text = "  This is some text.   "
  stripped_text = text.strip()  # Result: "This is some text."
  ```

#### f. `str.startswith()` (5 minutes)

- **Description**: Checks if a string starts with a specified prefix.
- **Use Case**: Useful for filtering or categorizing strings.
- **Example**:

  ```python
  text = "Hello, World"
  starts_with_hello = text.startswith("Hello")  # Result: True
  ```

#### g. `str.endswith()` (5 minutes)

- **Description**: Checks if a string ends with a specified suffix.
- **Use Case**: Useful for filtering or categorizing strings.
- **Example**:

  ```python
  text = "Hello, World"
  ends_with_world = text.endswith("World")  # Result: True
  ```

#### h. `str.find()` (5 minutes)

- **Description**: Searches for a substring within a string and returns the index of the first occurrence (or -1 if not found).
- **Use Case**: Useful for locating and extracting specific information from text.
- **Example**:

  ```python
  text = "Python is a powerful language. Python is fun."
  index = text.find("Python")  # Result: 0
  ```

#### i. `str.count()` (5 minutes)

- **Description**: Counts the number of non-overlapping occurrences of a substring in a string.
- **Use Case**: Useful for various text analysis tasks.
- **Example**:

  ```python
  text = "Python is a popular language, and Python is versatile."
  count = text.count("Python")  # Result: 2
  ```

#### j. `str.replace()` (5 minutes)

- **Description**: Replaces all occurrences of a specified substring with another string.
- **Use Case**: Useful for text transformations and substitutions.
- **Example**:

  ```python
  text = "I like apples, but I don't like oranges."
  replaced_text = text.replace("apples", "bananas")  # Result: "I like bananas, but I don't like oranges."
  ```

#### k. `str.split()` (5 minutes)

- **Description**: Splits a string into a list of substrings based on a specified delimiter.
- **Use Case**: Useful for tokenizing text or processing data.
- **Example**:

  ```python
  text = "www.codeplatoon.org"
  items = text.split(".")  # Result: ['www', 'codeplatoon', 'org']
  ```

#### l. `str.join()` (5 minutes)

- **Description**: Joins a list of strings into a single string using the current string as a separator.
- **Use Case**: Useful for constructing formatted text from a list of elements.
- **Example**:

  ```python
  fruits = ["apple", "banana", "cherry"]
  text = ", ".join(fruits)  # Result: "apple, banana, cherry"
  ```

#### m. `str.isalpha()` (5 minutes)

- **Description**: Checks if all characters in a string are alphabetic (letters).
- **Use Case**: Useful for validating input that should contain only letters.
- **Example**:

  ```python
  text = "Python"
  is_alpha = text.isalpha()  # Result: True
  ```

#### n. `str.isnumeric()` (5 minutes)

- **Description**: Checks if all characters in a string are numeric (digits).
- **Use Case**: Useful for validating input that should contain only digits.
- **Example**:

  ```python
  number = "12345"
  is_numeric = number.isnumeric()  # Result: True
  ```

#### o. `str.is

alnum()` (5 minutes)

- **Description**: Checks if all characters in a string are alphanumeric (letters or digits).
- **Use Case**: Useful for validating input that should be a combination of letters and digits.
- **Example**:

  ```python
  text = "Python123"
  is_alnum = text.isalnum()  # Result: True
  ```

#### p. `str.islower()` (5 minutes)

- **Description**: Checks if all characters in a string are lowercase letters.
- **Use Case**: Useful for verifying that text is in lowercase.
- **Example**:

  ```python
  text = "python"
  is_lower = text.islower()  # Result: True
  ```

#### q. `str.isupper()` (5 minutes)

- **Description**: Checks if all characters in a string are uppercase letters.
- **Use Case**: Useful for verifying that text is in uppercase.
- **Example**:

  ```python
  text = "PYTHON"
  is_upper = text.isupper()  # Result: True
  ```

### 2. Interpolated Strings (10 minutes)

You can create interpolated strings using an "f-string." These allow you to embed expressions inside a string using curly braces {}. For example:

```python
name = "Alice"
greeting = f"Hello, {name}!"
```

### 3. Escape Sequences (10 minutes)

Escape sequences allow you to include special characters in strings. They start with a backslash \. Some common escape sequences include:

\n: Newline  
\t: Tab  
\: Backslash  
\": Double quote  
\': Single quote

Example with \n:

```python
multi_line = "This is a multi-line\nstring."
print(multi_line)
```

### 4. Slicing and Reversing (10 minutes)

You can use slicing to extract a part of a string. Slicing is done using square brackets []. For example:

```python
text = "Python"
substring = text[2:5]  # Results in "tho"
```

To reverse a string, you can use slicing with a step of -1:

```python
text = "Hello"
reversed_text = text[::-1]  # Results in "olleH"
```

### 5. Conclusion (5 minutes)

In this lecture, you've explored a range of built-in string methods in Python, each designed to help you manipulate and process text efficiently. Understanding when and how to use these methods is essential for working with strings in various applications, from data cleaning and formatting to text analysis and data extraction. Continue practicing and applying these methods to become proficient in text processing with Python.

This comprehensive lecture covers all the major built-in string methods in Python, providing detailed explanations, use cases, and examples for each method. It aims to help learners understand how to effectively work with strings in Python and take full advantage of these methods for various text-related tasks.

### 6. Assignments

- [Exclamations](https://replit.com/@cpadmin/exclamations#main.py)
- [Esrever](https://replit.com/@cpadmin/Reverse#main.py)
- [DNA](https://replit.com/@cpadmin/DNA#main.py)
