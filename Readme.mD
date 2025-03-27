## Python Scripting

## Overview

Python is a versatile and easy-to-learn programming language widely used for automation, deep learning, natural language processing, and web development.

## Key Topics

## 1. Variables and Data Types

Variables act as containers for storing values. Python is dynamically typed, meaning variable types do not need to be explicitly defined.

Examples:

```
# Dynamic Typing
x = 42      # Integer
b = True    # Boolean
c = "DevOps" # String
```

## Data Types:

* Integer

* Boolean

* Strings

* Float

* List

* Tuple

* Set

* Dictionary

Python is case-sensitive, meaning devops and DevOps are treated as different variables.

## 2. Conditions

Conditional statements allow execution of specific blocks of code based on conditions.

Example:
```
x = 10
if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is 5")
else:
    print("x is less than 5")
```
## 3. Loops

Loops are used for iteration.

Example (For Loop):
```
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
## 4. Functions

Functions allow code reuse and modularization.

Example:
```
def greet(name):
    return f"Hello, {name}!"

print(greet("DevOps Engineer"))
```
## 5. Use Cases

* Automation

* Deep Learning Applications

* Natural Language Processing (e.g., ChatGPT, Gemini, GitHub Copilot)

* Web Development (Django, Flask)

## Static vs Dynamic Typed Languages

### Static Typed Languages (Require explicit type definitions)

Examples: Java, C, C++, C#, Golang
```
int a = 42;
float b = 45.35;
```
### Dynamic Typed Languages (No explicit type definition required)

Example: Python
```
a = 42
b = True
c = "DevOps"
```
## Installation

Python can be installed and used in AWS CloudShell or we can use in VS code or Pycharm etc.

## Commenting in Python

* Single-line comment: 

```
# This is a single-line comment
```
* Multi-line comment:
```
"""
This is a 
multi-line comment
"""
```
## Naming Conventions

* snake_case (Recommended)

* camelCase (Common in JavaScript and Java)

* CONSTANTS (Written in uppercase)

* Incorrect Naming: snake-case

## Additional Code Examples

```
# Define a variable
a = 42 # This is an integer variable

# Print the value that is stored inside the variable
print(a)

# Float value
b = 42.345
print(b)

# Boolean
c = True 

# Strings
d = 'This is a string'
e = "This is also a string"
f = """
This is a multi-line string
"""

# Handling special characters
d = 'Today\'s weather is nice'
print(d)

d = "Today's weather is nice"
print(d)

# List
test_list = ["hello", "world", "python"]
print(test_list)

# Tuple
test_tuple = ("hello", "world", "python")
print(test_tuple)

# Dictionary
test_dict = {'a': 1, 'b': 2}
print(test_dict)

# Set
test_set = {'a', 'b', "abc"}
print(test_set)

# type() function -> prints the datatype of the variable
print(type(test_dict))
print(type(print))

# Operations
# Add, Subtract, Multiply, Divide, Integer division, Modulo division

a = 42
b = 45.32
c = a + b
print(c)

d = a - b
print(d)

e = a * b
print(e)

f = 12
g = 3
h = f / g
print(h, type(h))

# Integer division
h = f // g
print(h)

# Modulo division
i = f % g
print(i)

# String concatenation
a = "42"
b = "43"
print(a + b) 

# Power operation
a = 10
print(a**2) # a²

# Comparison operators
a = 10
b = 20
res = a > b
res_1 = a < b
res_2 = a != b
res_3 = a == b
print(res, res_1, res_2, res_3)

# Logical operators (AND, OR, NOT)
a = True
b = False

res = a and b
res_1 = a or b
res_2 = not a
res_3 = not b
print(res, res_1, res_2, res_3)
```


## Functions
Reusable blocks of code.

#### Example:
```
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
```

## Exception Handling

Used for error management.
#### Example:
```
try:
    result = 10 / 0  # This will cause a ZeroDivisionError
except ZeroDivisionError:
    print("Cannot divide by zero.")
finally:
    print("Execution completed.")
```

## Built-in Functions

Python provides built-in functions for common tasks.

#### Example:
```
print(len("Hello"))  # Output: 5
print(abs(-10))       # Output: 10
print(sum([1, 2, 3])) # Output: 6
print(max(4, 7, 1))   # Output: 7
print(min(4, 7, 1))   # Output: 1
print(round(3.14159, 2)) # Output: 3.14
```

### Explanation:

* len(obj): Returns length of an object.

* abs(number): Returns absolute value.

* sum(iterable): Returns the sum of all elements.

* max(iterable or args): Returns the maximum value.

* min(iterable or args): Returns the minimum value.

* round(number, ndigits): Rounds a number to the given decimal places.

## File Handling

### Writing to a File:
```
with open("example.txt", "w") as file:
    file.write("Hello, File!")
```

### Reading from a File:
```
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

###  Classes and Objects

Object-oriented programming in Python.

#### Example:
```
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        return f"Hello, my name is {self.name} and I am {self.age} years old."

p1 = Person("Alice", 25)
print(p1.greet())
```


## Additional Notes

Python scripts are saved with the .py extension.

By default, division returns a float value.

Happy Coding! 🚀