# Python Cheatsheet
### Introduction
Python is a high-level, interpreted programming language known for its simplicity and readability. It was created by Guido van Rossum and first released in 1991. Python emphasizes code readability with its clean and concise syntax, making it suitable for beginners and experienced programmers alike.

#### Installation and Environment Setup
- Visit the [official Python website](https://www.python.org/downloads/) to download the latest version of Python.
- Follow the installation instructions for your operating system.
- For development, consider using IDEs like PyCharm, VSCode, or Jupyter Notebook.

### Python Syntax
#### Comments
```python
# This is a single-line comment

"""
This is a 
multi-line comment
"""
```

#### Variables
```python
# Variable assignment
x = 10
name = "Alice"

# Variable naming rules
# - Must start with a letter or underscore
# - Can contain letters, numbers, and underscores
# - Case-sensitive
```

#### Data Types
```python
# Integer
age = 25

# Float
height = 5.11

# String
message = "Hello, World!"

# Boolean
is_valid = True
```

#### Expressions and Statements
```python
# Expression
result = 10 + 5

# Statement
if result > 10:
    print("Result is greater than 10")
```

#### Conditionals
```python
# if statement
if condition:
    # code block

# if-elif-else statement
if condition1:
    # code block
elif condition2:
    # code block
else:
    # code block
```

#### Loops
```python
# for loop
for item in iterable:
    # code block

# while loop
while condition:
    # code block
```

#### Functions
```python
# Function definition
def greet(name):
    return "Hello, " + name

# Function call
greeting = greet("Alice")
print(greeting)
```

#### Classes and Objects
```python
# Class definition
class Car:
    def __init__(self, make, model):
        self.make = make
        self.model = model

# Object instantiation
my_car = Car("Toyota", "Camry")
print(my_car.make, my_car.model)
```

#### Modules and Packages
```python
# Importing modules
import math
from module import function

# Creating packages
# Create a directory with __init__.py file
# Use dot notation to access modules: package.module
```

### Built-in Data Types
#### Numbers
```python
# Integer
x = 10

# Float
y = 3.14

# Complex
z = 2 + 3j
```

#### Strings
```python
# Indexing
s = "Python"
print(s[0])  # Output: 'P'

# Slicing
print(s[1:4])  # Output: 'yth'

# String methods
s = "Hello, World!"
print(s.lower())  # Output: 'hello, world!'
```

#### Lists
```python
# List creation
my_list = [1, 2, 3]

# Indexing
print(my_list[0])  # Output: 1

# List methods
my_list.append(4)
print(my_list)  # Output: [1, 2, 3, 4]
```

#### Tuples
```python
# Tuple creation
my_tuple = (1, 2, 3)

# Unpacking
a, b, c = my_tuple
```

#### Dictionaries
```python
# Dictionary creation
my_dict = {"name": "Alice", "age": 30}

# Accessing values
print(my_dict["name"])  # Output: 'Alice'

# Dictionary methods
my_dict["city"] = "New York"
print(my_dict)  # Output: {'name': 'Alice', 'age': 30, 'city': 'New York'}
```

#### Sets
```python
# Set creation
my_set = {1, 2, 3}

# Set methods
my_set.add(4)
print(my_set)  # Output: {1, 2, 3, 4}
```

### Advanced Concepts
#### List/Dict/Set Comprehension
```python
# List comprehension
squares = [x**2 for x in range(10)]

# Dict comprehension
my_dict = {x: x**2 for x in range(5)}

# Set comprehension
my_set = {x**2 for x in range(10)}
```

#### Generators and Iterators
```python
# Generator function
def my_generator(n):
    for i in range(n):
        yield i

# Iterator
my_iter = iter([1, 2, 3])
```

#### Higher Order Functions
```python
# map function
squared = list(map(lambda x: x**2, [1, 2, 3]))

# filter function
evens = list(filter(lambda x: x % 2 == 0, [1, 2, 3, 4, 5]))

# reduce function
from functools import reduce
sum = reduce(lambda x, y: x + y, [1, 2, 3, 4, 5])
```

#### Recursion
```python
# Factorial example
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)
```

#### Decorators
```python
# Decorator function
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
```

#### Exception Handling
```python
# try-except block
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Error: Division by zero")

# raise statement
x = -1
if x < 0:
    raise ValueError("x cannot be negative")
```

#### File and Directory Handling
```python
# Reading from a file
with open("file.txt", "r") as f:
    data = f.read()

# Writing to a file
with open("file.txt", "w") as f:
    f.write("Hello, World!")

# Directory handling
import os
os.mkdir("my_directory")
```

#### Regular Expressions
```python
import re

# Search for pattern
pattern = r"\b(cat)\b"
match = re.search(pattern, "The cat is here")
if match:
    print("Found")
```

### Commonly Used Modules and Libraries
#### NumPy
```python
import numpy as np

# Creating arrays
arr = np.array([1, 2, 3])

# Array operations
result = np.sum(arr)
```

#### Pandas
```python
import pandas as pd

# Creating DataFrame
df = pd.DataFrame({'Name': ['Alice', 'Bob'], 'Age': [25, 30]})

# Data manipulation
mean_age = df['Age'].mean()
```

#### Matplotlib
```python
import matplotlib.pyplot as plt

#

 Plotting
x = [1, 2, 3, 4]
y = [10, 20, 25, 30]
plt.plot(x, y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Simple Plot')
plt.show()
```

This Python cheatsheet covers the key concepts and features of the language, ranging from basic syntax to advanced topics and commonly used libraries. Practice and experimentation with these concepts will help solidify your understanding and proficiency in Python programming.

Follow: [@bhushcodes 🐦](https://twitter.com/bhushcodes) | [@16oct.01 😉](https://www.instagram.com/16oct.01/)
