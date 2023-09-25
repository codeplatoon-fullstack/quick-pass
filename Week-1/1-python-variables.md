# Python Variable

## Introduction

In this lesson you will learn how to run a Python script, what different types of Python variables can be created, when to use different types of variables.

## Running/Creating a Python script

Unlike other languages, Python scripts are extremely simple to run. To create a Python script you'll need to follow these steps:

- Open Visual Studio Code.
- Within Visual Studio Code open/create a folder that will hold all your code.
- Once you've opened up said folder create a file that is pre-pended with `.py` for example `my_file.py`.

Typically, when naming Python files and variables you'll want to follow a concept named snake casing. This concept is basically stating that all letters within the name will be lower case and spaces between words will be accentuated by "_". For example `My File` should be written as `my_file`.

## Python Variables and Types

In python there are many types that you can utilize to declare a value. These types are as follows: string, integer,list, dictionary, float, boolean, tuple, and set. Each one of these types have different built in methods, behaviors that can be applied to manipulate the value of a variable, we will learn to utilize these methods in detail later on in this program.

Lets go ahead and take a look at a couple of different examples for creating types and variables. To create a variable with a value you'll have to start by declaring a `variable` which is essentially a reference point for a `value`. You will give a value to this variable by using the `=` operator, otherwise Python will think you are trying to reference a pre-existing value rather than trying to create a new one.

```python
# variable  operator    value
    six        =          6
```

Variable names should be descriptive of the value they hold. This will make it easier for you as a programmer to identify which variable you need to utilize and when to utilize it.

```python
# STRING
string = "Hello I am a string"
string = 'Hello I am also a string, notice that I can use either double or single quotes but still count as a string'
string = """I am a rare kind of string that is wrapped by three sets of double quotes. I will explain my purpose later on"""
f_string = f"I am a string that is prepended by an 'f', for now just remember I exist. I will explain my purpose later on"
not_a_string = I am not a string because I am not wrapped by either single nor double quotes

# INTEGERS
integer = 3
integer = -3
integer = 0
not_an_integer ="3"
not_an_integer = '3'

# FLOAT
float = 1.12482
float = 3749.0
float = 0.0
not_a_float = 1
not_a_float = 2
not_a_float = "0.0"

# BOOLEAN
boolean = True
boolean = False 
```
