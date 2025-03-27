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

## String Operations
 ### Example:

```
sample_str = "This-is-a-sample-string"
print(sample_str)

# How to access individual characters from a string
print(sample_str[8])

# Slicing
sub_str = sample_str[2:7]
print(sub_str)

sub_str = sample_str[:]
print(sub_str)

sub_str = sample_str[1:]
print(sub_str)

sub_str = sample_str[:5]
print(sub_str)

sub_str = sample_str[::2]
print(sub_str)

# Reverse a string
sub_str = sample_str[::-1]
print("Reversed string:", sub_str)

# Length of a string
len_str = len(sample_str)
print("Length of a string:", len_str)

# String Methods
sample_str = "hello"
print(sample_str.capitalize()) # "Hello"

# split(), join(), format(), count(), strip(), lstrip(), rstrip()
sample_str = "This is a sample string"
str_split = sample_str.split() # output: list
print(str_split, type(str_split))

join_split_str = " ".join(str_split)
print(join_split_str, type(join_split_str))

count_a = sample_str.count('a')
print(count_a)

sample_str = "    devops is a very good career choice   "
strip_str = sample_str.strip()
print(strip_str)

# Strings are immutable
sample_str = "This is a sample string"
sample_str[-1] = 'G'  # This will raise an error
print(sample_str)
```

# Python Tuples

### Introduction

A tuple is an immutable, ordered collection of elements in Python. Once created, its elements cannot be changed. Tuples are commonly used when we need to store related items together and ensure their integrity.

### Creating a Tuple

There are two ways to create a tuple:

Using parentheses ()
```sh
sample_tuple = ("Ansible", "Terraform", "Jenkins", "Docker", "K8s")
```
Using the tuple() constructor
```sh
sample_tuple = tuple(["Ansible", "Terraform", "Jenkins", "Docker", "K8s"])
```

### Accessing Elements

Tuples support indexing just like lists.
```
sample_ele = sample_tuple[1]  # Accessing by index
print(sample_ele)  # Output: Terraform

sample_ele = sample_tuple[-1]  # Accessing last element
print(sample_ele)  # Output: K8s
```

## Slicing Tuples

Tuples can be sliced to create sub-tuples.
```sh
sliced_tuple = sample_tuple[1:3]  # Extract elements from index 1 to 2
print(sliced_tuple)  # Output: ('Terraform', 'Jenkins')

sliced_tuple_len = len(sliced_tuple)  # Getting the length of a sliced tuple
print(sliced_tuple_len)  # Output: 2
```

## Tuple Immutability

Tuples do not support item assignment.
```
# sample_tuple[1] = "Shell"  # Uncommenting this line will cause an error
```
Error:
```
TypeError: 'tuple' object does not support item assignment
```

## Tuple Operations

### Concatenation

Tuples can be concatenated using +:

```sh
res_tuple = sample_tuple + sliced_tuple
print(res_tuple)  # ('Ansible', 'Terraform', 'Jenkins', 'Docker', 'K8s', 'Terraform', 'Jenkins')
```

### Repetition

Tuples can be repeated using *:
```
res_tuple_1 = sliced_tuple * 2
print(res_tuple_1)  # ('Terraform', 'Jenkins', 'Terraform', 'Jenkins')
```
## Tuple Methods

### Finding an Index

To find the index of an element in a tuple:
```
k8s_idx = res_tuple.index("K8s")
print(k8s_idx)  # Output: 4
```
If the element does not exist, an error is raised:
```
# k8s_idx = res_tuple.index("k8s")  # Uncommenting this will cause an error
```
Error:
```
ValueError: tuple.index(x): x not in tuple
```
### Tuple Unpacking

Tuples allow unpacking of elements into individual variables.
```sh
ansible, terraform, jenkins, docker, k8s = ("Ansible", "Terraform", "Jenkins", "Docker", "K8s")
print(ansible, terraform, jenkins, docker, k8s)
```
Using * for flexible unpacking:
```sh
ansible, *tools, orchestrator = ("Ansible", "Terraform", "Jenkins", "Docker", "K8s", "DevOps")
print(ansible, tools, orchestrator)
print(*tools)  # Output: Terraform Jenkins Docker K8s
```
#### Summary

* Tuples are immutable and ordered.

* Created using () or tuple().

* Elements are accessed via indexing and slicing.

* They support concatenation, repetition, and some useful methods.

* Tuple unpacking allows easy assignment of values.

* Tuples are an efficient data structure when immutability is required!


# Python Lists

## Overview

A list in Python is a mutable, ordered collection of elements. It allows duplicate values and supports various operations such as indexing, slicing, appending, and extending.

### Creating a List
```
sample_list = ["Ansible", "Terraform", "Jenkins", "Docker", "K8s"]
```
### Indexing and Slicing

#### Accessing Elements
```
sample_ele = sample_list[1]
print(sample_ele)  # Output: Terraform
```
#### Handling Index Errors
```
# sample_ele = sample_list[5]  # IndexError: list index out of range
```
#### Accessing the Last Element
```
sample_ele = sample_list[-1]  # Equivalent to sample_list[len(sample_list) - 1]
print(sample_ele)  # Output: K8s
```
#### Slicing a List
```
sliced_list = sample_list[1:3]  # Extracts elements from index 1 to 2
print(sliced_list)  # Output: ['Terraform', 'Jenkins']
```
#### Length of Sliced List
```
sliced_list_len = len(sliced_list)
print(sliced_list_len)  # Output: 2
```
### Mutability of Lists

Lists are mutable, meaning elements can be modified after creation.
```
sample_list[1] = "Shell"
print(sample_list)  # Output: ['Ansible', 'Shell', 'Jenkins', 'Docker', 'K8s']
```
## List Operations

#### Append an Element
```
sample_list.append("Shell")  # Adds 'Shell' to the end of the list
print(sample_list)
```
#### Append a List to Itself
```
sample_list.append(sample_list)
print(len(sample_list))  # Output increases due to nesting
```
#### Extend a List
```
sample_list = [1, 2, 'sample', True]
sample_list.extend(sample_list)
print(len(sample_list), sample_list)
```
### Membership Operators

Checking if an element exists in a list:
```
is_elem = 2 in sample_list
print(is_elem)  # Output: True
```
### Summary

Python lists provide dynamic storage with various functionalities such as indexing, slicing, mutability, and built-in operations like append and extend. Understanding these operations is essential for efficient list manipulation in Python.



## Additional Notes

Python scripts are saved with the .py extension.

By default, division returns a float value.

Happy Coding! 🚀