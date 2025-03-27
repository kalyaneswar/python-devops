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

## Additional Notes

Python scripts are saved with the .py extension.

By default, division returns a float value.

Happy Coding! 🚀