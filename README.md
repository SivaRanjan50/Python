# 🐍 Python Ultimate Cheat Sheet with Definitions

## 📋 TABLE OF CONTENTS
```
Python Basics
Data Types
Control Flow
Functions
Data Structures
Object-Oriented Programming
Error Handling
File Operations
Modules & Packages
Advanced Concepts
Useful Libraries**
```

### Variables & Assignment
```
Definition: Variables store data values. Python is dynamically typed (no need to declare type)

# Variable assignment
x = 10                    # Integer
name = "Alice"            # String
is_valid = True           # Boolean
price = 19.99             # Float

# Multiple assignment
a, b, c = 1, 2, 3        # a=1, b=2, c=3
x = y = z = 0            # All set to 0

# Swap variables
a, b = b, a              # Swap values

# Dynamic typing
variable = 10            # Now it's an integer
variable = "Hello"       # Now it's a string
```

### Input/Output
```
Definition: print() displays output, input() reads user input as string.

# Output
print("Hello")                          # Basic print
print("Hello", "World", sep=", ")       # Custom separator
print("Hello", end=" ")                 # No newline
print(f"Value: {x}")                    # f-string (Python 3.6+)
print("Value: {}".format(x))            # format method
print("Value: %d" % x)                  # Old style (avoid)

# Input
name = input("Enter your name: ")       # Returns string
age = int(input("Enter age: "))         # Convert to int
```

### Basic Operators
```
Definition: Operators perform operations on variables and values.

# Arithmetic operators
x + y      # Addition
x - y      # Subtraction
x * y      # Multiplication
x / y      # Division (float)
x // y     # Floor division (integer)
x % y      # Modulus (remainder)
x ** y     # Exponentiation
-x         # Negation

# Comparison operators
x == y     # Equal to
x != y     # Not equal to
x > y      # Greater than
x < y      # Less than
x >= y     # Greater than or equal to
x <= y     # Less than or equal to

# Logical operators
x and y    # Logical AND
x or y     # Logical OR
not x      # Logical NOT

# Identity operators
x is y     # True if same object
x is not y # True if different objects

# Membership operators
x in y     # True if x found in y
x not in y # True if x not found in y
```
## 📊 DATA TYPES
### Numeric Types
```
Definition: Numeric types store numbers. Python supports int, float, and complex numbers.

# Integers (int)
x = 10
y = -5
z = 0
large = 1_000_000  # Underscores for readability (Python 3.6+)

# Floating point (float)
pi = 3.14159
temp = -2.5
scientific = 2.5e-3  # 0.0025

# Complex numbers (complex)
comp = 3 + 4j
comp.real  # 3.0
comp.imag  # 4.0

# Type conversion
int(3.14)    # 3 (truncates)
float(5)     # 5.0
complex(2)   # (2+0j)
str(100)     # "100"

# Type checking
type(x)              # <class 'int'>
isinstance(x, int)   # True
```

### Strings
```
Definition: Strings store text as sequence of Unicode characters. Immutable.

# String creation
s1 = 'Single quotes'
s2 = "Double quotes"
s3 = '''Triple quotes for
multi-line strings'''
s4 = """Also works with
double triple quotes"""

# String operations
len("Hello")                 # 5 (length)
"Hello" + " " + "World"      # "Hello World"
"Hi" * 3                     # "HiHiHi"
"Hello"[1]                   # "e" (indexing)
"Hello"[1:4]                 # "ell" (slicing)
"Hello"[-1]                  # "o" (negative index)

# String methods
"hello".upper()              # "HELLO"
"HELLO".lower()              # "hello"
" hello ".strip()            # "hello"
"hello world".split()        # ['hello', 'world']
",".join(['a', 'b', 'c'])    # "a,b,c"
"hello".replace('l', 'x')    # "hexxo"
"hello".find('l')            # 2 (first occurrence)
"123".isdigit()              # True
"hello".startswith('he')     # True
"hello".endswith('lo')       # True

# String formatting (modern)
name = "Alice"
age = 30
f"Name: {name}, Age: {age}"          # f-string
"Name: {}, Age: {}".format(name, age) # format()
```
### Booleans
```
Definition: Booleans represent truth values: True or False. Used in conditions.

# Boolean values
True
False

# Boolean operations
True and False    # False
True or False     # True
not True          # False

# Truthy and Falsy values
bool(0)           # False
bool(1)           # True
bool("")          # False
bool("hello")     # True
bool([])          # False
bool([1, 2])      # True
bool(None)        # False
```

### None Type
```
Definition: None is a special constant representing the absence of a value.

# None represents absence of value
x = None
if x is None:
    print("x is None")
    
# Common use cases
def function():
    return None  # Implicitly returns None
    
result = function()  # result is None
```

##  CONTROL FLOW
### Conditional Statements (if/elif/else)
```
Definition: Conditional statements execute code based on boolean conditions.

# Basic if statement
if condition:
    # code block
    pass

# If-else
if x > 10:
    print("Greater than 10")
else:
    print("10 or less")

# If-elif-else chain
if score >= 90:
    grade = "A"
elif score >= 80:
    grade = "B"
elif score >= 70:
    grade = "C"
else:
    grade = "F"

# Ternary operator
result = "Even" if x % 2 == 0 else "Odd"

# Multiple conditions
if 0 < x < 10:  # Python allows this!
    print("Between 0 and 10")
    
if x > 0 and x < 10:  # Equivalent
    print("Between 0 and 10")
```

### Loops
```
Definition: Loops repeat code execution. for loops iterate over sequences, while loops repeat while condition is true.

# For loop
for i in range(5):          # 0 to 4
    print(i)

for i in range(2, 10, 2):   # 2, 4, 6, 8
    print(i)

# Iterating over sequences
for char in "Hello":
    print(char)

for item in [1, 2, 3]:
    print(item)

# While loop
count = 0
while count < 5:
    print(count)
    count += 1

# Loop control
for i in range(10):
    if i == 3:
        continue    # Skip rest of loop for i=3
    if i == 7:
        break       # Exit loop entirely
    print(i)
else:
    # Executes if loop completes normally (no break)
    print("Loop completed")

# Enumerate (get index and value)
for index, value in enumerate(["a", "b", "c"]):
    print(f"Index {index}: {value}")

# Zip (iterate over multiple sequences)
names = ["Alice", "Bob", "Charlie"]
ages = [25, 30, 35]
for name, age in zip(names, ages):
    print(f"{name} is {age} years old")
```

### Range Function

```
Definition: range() generates sequence of numbers, efficient for memory.

range(5)            # 0, 1, 2, 3, 4
range(2, 5)         # 2, 3, 4
range(0, 10, 2)     # 0, 2, 4, 6, 8
range(10, 0, -1)    # 10, 9, 8, ..., 1

# Convert to list
list(range(5))      # [0, 1, 2, 3, 4]
```

## FUNCTIONS
### Defining Functions
```
Definition: Functions are reusable blocks of code that perform specific tasks.

# Basic function
def greet():
    print("Hello!")

# Function with parameters
def greet(name):
    print(f"Hello, {name}!")

# Function with return value
def add(a, b):
    return a + b

# Default parameters
def greet(name="Guest"):
    print(f"Hello, {name}!")

# Multiple return values
def min_max(numbers):
    return min(numbers), max(numbers)

# Type hints (Python 3.5+)
def add(a: int, b: int) -> int:
    return a + b
```

### Arguments & Parameters
```
Definition: Functions can accept different types of arguments for flexibility.

# Positional arguments
def power(base, exponent):
    return base ** exponent

power(2, 3)  # 8

# Keyword arguments
power(exponent=3, base=2)  # 8

# Mix of positional and keyword (positional first)
power(2, exponent=3)  # 8

# Variable-length arguments (*args)
def sum_all(*args):
    return sum(args)

sum_all(1, 2, 3, 4)  # 10

# Variable-length keyword arguments (**kwargs)
def print_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_info(name="Alice", age=30)

# All argument types
def complex_func(a, b, *args, c=10, **kwargs):
    print(f"a={a}, b={b}, args={args}, c={c}, kwargs={kwargs}")
```

### Lambda Functions
```
Definition: Lambda functions are anonymous, single-expression functions.

# Anonymous function
square = lambda x: x ** 2
square(5)  # 25

# Immediately invoked
(lambda x: x * 2)(10)  # 20

# Common use with map/filter
numbers = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x**2, numbers))  # [1, 4, 9, 16, 25]
evens = list(filter(lambda x: x % 2 == 0, numbers))  # [2, 4]
```

### Decorators
```
Definition: Decorators modify or enhance functions without changing their code.

# Basic decorator
def my_decorator(func):
    def wrapper():
        print("Before function")
        func()
        print("After function")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
# Output:
# Before function
# Hello!
# After function

# Decorator with arguments
def repeat(n):
    def decorator(func):
        def wrapper(*args, **kwargs):
            for _ in range(n):
                result = func(*args, **kwargs)
            return result
        return wrapper
    return decorator

@repeat(3)
def greet(name):
    print(f"Hello, {name}!")
```

## 📦 DATA STRUCTURES
### Lists
```
Definition: Lists are ordered, mutable collections that can contain different data types.

# List creation
numbers = [1, 2, 3, 4, 5]
mixed = [1, "hello", 3.14, True]
empty = []

# List operations
len([1, 2, 3])          # 3
[1, 2] + [3, 4]         # [1, 2, 3, 4]
["hi"] * 3              # ["hi", "hi", "hi"]
3 in [1, 2, 3]          # True

# Indexing and slicing
lst = [10, 20, 30, 40, 50]
lst[0]                  # 10 (first)
lst[-1]                 # 50 (last)
lst[1:3]                # [20, 30] (slice)
lst[:3]                 # [10, 20, 30]
lst[2:]                 # [30, 40, 50]
lst[::2]                # [10, 30, 50] (every 2nd)
lst[::-1]               # [50, 40, 30, 20, 10] (reverse)

# List methods
lst.append(60)          # Add to end
lst.insert(2, 25)       # Insert at index 2
lst.remove(30)          # Remove first occurrence of 30
lst.pop()               # Remove and return last item
lst.pop(2)              # Remove and return item at index 2
lst.index(40)           # Find index of 40
lst.count(20)           # Count occurrences of 20
lst.sort()              # Sort in place
lst.reverse()           # Reverse in place
lst.copy()              # Shallow copy
lst.clear()             # Remove all items

# List comprehension
squares = [x**2 for x in range(10)]  # [0, 1, 4, ..., 81]
evens = [x for x in range(10) if x % 2 == 0]  # [0, 2, 4, 6, 8]
pairs = [(x, y) for x in [1, 2] for y in [3, 4]]  # [(1,3), (1,4), (2,3), (2,4)]
```

### Tuples
```
Definition: Tuples are ordered, immutable collections. Faster than lists, used for fixed data.

# Tuple creation
point = (10, 20)
single = (5,)          # Note comma for single element
coordinates = 30, 40   # Parentheses optional
empty = ()

# Tuple operations (similar to lists but immutable)
point[0]               # 10
point[1:]              # (20,)
len(point)             # 2
point + (30,)          # (10, 20, 30)
point * 2              # (10, 20, 10, 20)

# Tuple unpacking
x, y = point           # x=10, y=20
a, b, c = 1, 2, 3      # Multiple assignment

# Swap using tuple unpacking
a, b = b, a

# Return multiple values from function
def get_coordinates():
    return 10, 20

x, y = get_coordinates()
```

### Sets
```
Definition: Sets are unordered collections of unique elements. Useful for membership testing and mathematical operations.

# Set creation
fruits = {"apple", "banana", "cherry"}
numbers = {1, 2, 3, 4, 5}
empty = set()          # Not {} (that's a dict)

# Set operations
len(fruits)                       # 3
"apple" in fruits                 # True
"grape" not in fruits             # True

# Set methods
fruits.add("orange")              # Add single element
fruits.update(["grape", "kiwi"])  # Add multiple
fruits.remove("banana")           # Remove, error if not exists
fruits.discard("mango")           # Remove, no error if not exists
fruits.pop()                      # Remove random element
fruits.clear()                    # Remove all

# Set operations (mathematical)
A = {1, 2, 3}
B = {3, 4, 5}

A | B        # Union: {1, 2, 3, 4, 5}
A & B        # Intersection: {3}
A - B        # Difference: {1, 2}
A ^ B        # Symmetric difference: {1, 2, 4, 5}

# Set comprehension
squares = {x**2 for x in range(5)}  # {0, 1, 4, 9, 16}

```

### Dictionaries
```
Definition: Dictionaries store key-value pairs. Keys must be immutable (strings, numbers, tuples), values can be any type.

# Dictionary creation
person = {"name": "Alice", "age": 30, "city": "NYC"}
empty = {}
from_keys = dict.fromkeys(["a", "b", "c"], 0)  # {'a': 0, 'b': 0, 'c': 0}

# Access elements
person["name"]                 # "Alice"
person.get("age")              # 30
person.get("country", "USA")   # "USA" (default if key doesn't exist)

# Add/update elements
person["email"] = "alice@email.com"   # Add new key
person["age"] = 31                    # Update existing

# Dictionary operations
len(person)                    # 3
"name" in person               # True
list(person.keys())            # ['name', 'age', 'city']
list(person.values())          # ['Alice', 30, 'NYC']
list(person.items())           # [('name', 'Alice'), ('age', 30), ('city', 'NYC')]

# Dictionary methods
person.copy()                  # Shallow copy
person.pop("age")              # Remove key and return value
person.popitem()               # Remove last inserted item
person.update({"country": "USA", "age": 32})  # Merge dictionaries
person.clear()                 # Remove all items

# Dictionary comprehension
squares = {x: x**2 for x in range(5)}  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
even_squares = {x: x**2 for x in range(10) if x % 2 == 0}
```
### Collections Module
```
Definition: The collections module provides specialized container datatypes.

from collections import defaultdict, Counter, deque, namedtuple

# defaultdict (dictionary with default factory)
dd = defaultdict(list)        # Default value is empty list
dd["key1"].append(1)          # Works even if key1 doesn't exist

# Counter (count hashable objects)
counter = Counter(["apple", "banana", "apple", "orange"])
counter["apple"]              # 2
counter.most_common(2)        # [('apple', 2), ('banana', 1)]

# deque (double-ended queue)
dq = deque([1, 2, 3])
dq.append(4)                  # [1, 2, 3, 4]
dq.appendleft(0)              # [0, 1, 2, 3, 4]
dq.pop()                      # 4
dq.popleft()                  # 0

# namedtuple (tuple with named fields)
Point = namedtuple("Point", ["x", "y"])
p = Point(10, 20)
p.x                           # 10
p.y                           # 20
```


## 🏗️ OBJECT-ORIENTED PROGRAMMING
### Classes & Objects
```
Definition: Classes are blueprints for creating objects (instances). Objects bundle data and methods.

# Basic class
class Dog:
    # Class attribute (shared by all instances)
    species = "Canis familiaris"
    
    # Initializer (constructor)
    def __init__(self, name, age):
        # Instance attributes
        self.name = name
        self.age = age
    
    # Instance method
    def bark(self):
        return f"{self.name} says woof!"
    
    # Another instance method
    def description(self):
        return f"{self.name} is {self.age} years old"

# Create instances (objects)
dog1 = Dog("Buddy", 5)
dog2 = Dog("Lucy", 3)

# Access attributes and methods
dog1.name                     # "Buddy"
dog1.bark()                   # "Buddy says woof!"
dog1.description()            # "Buddy is 5 years old"
Dog.species                   # "Canis familiaris"
```

### Inheritance
```
Definition: Inheritance allows creating new classes that reuse, extend, or modify behavior of existing classes.

# Parent class
class Animal:
    def __init__(self, name):
        self.name = name
    
    def speak(self):
        raise NotImplementedError("Subclass must implement")

# Child class
class Dog(Animal):
    def speak(self):
        return f"{self.name} says woof!"

class Cat(Animal):
    def speak(self):
        return f"{self.name} says meow!"

# Using inheritance
dog = Dog("Buddy")
cat = Cat("Whiskers")
dog.speak()  # "Buddy says woof!"
cat.speak()  # "Whiskers says meow!"

# Multiple inheritance
class A:
    pass

class B:
    pass

class C(A, B):  # Inherits from both A and B
    pass
```

### Special Methods (Dunder/Magic Methods)
```
Definition: Special methods (dunder methods) allow customizing behavior of objects for operations like +, *, len(), etc.

class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    # String representation
    def __str__(self):
        return f"Vector({self.x}, {self.y})"
    
    def __repr__(self):
        return f"Vector({self.x}, {self.y})"
    
    # Arithmetic operations
    def __add__(self, other):
        return Vector(self.x + other.x, self.y + other.y)
    
    def __mul__(self, scalar):
        return Vector(self.x * scalar, self.y * scalar)
    
    # Comparison
    def __eq__(self, other):
        return self.x == other.x and self.y == other.y
    
    # Length
    def __len__(self):
        return 2
    
    # Container protocol
    def __getitem__(self, index):
        if index == 0:
            return self.x
        elif index == 1:
            return self.y
        else:
            raise IndexError("Index out of range")

# Using special methods
v1 = Vector(2, 3)
v2 = Vector(4, 5)
v3 = v1 + v2        # Calls __add__
v4 = v1 * 3         # Calls __mul__
str(v1)             # Calls __str__
v1 == v2            # Calls __eq__
v1[0]               # Calls __getitem__
```

### Properties & Descriptors
```
Definition: Properties allow controlled access to attributes with getter, setter, and deleter methods.

class Person:
    def __init__(self, name):
        self._name = name  # Private convention
    
    # Getter property
    @property
    def name(self):
        return self._name
    
    # Setter property
    @name.setter
    def name(self, value):
        if not value:
            raise ValueError("Name cannot be empty")
        self._name = value
    
    # Deleter property
    @name.deleter
    def name(self):
        print("Deleting name...")
        del self._name

# Using properties
person = Person("Alice")
person.name                     # "Alice" (uses getter)
person.name = "Bob"             # Uses setter
del person.name                 # Uses deleter
```

##  ERROR HANDLING
### Try/Except Blocks
```
Definition: Try-except blocks handle runtime errors gracefully without crashing the program

# Basic try-except
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")

# Multiple exceptions
try:
    value = int("not a number")
except (ValueError, TypeError) as e:
    print(f"Error: {e}")

# Specific exception handling
try:
    file = open("nonexistent.txt", "r")
except FileNotFoundError:
    print("File not found")
except PermissionError:
    print("Permission denied")
except Exception as e:  # Catch-all
    print(f"Unexpected error: {e}")

# Else clause (runs if no exception)
try:
    result = 10 / 2
except ZeroDivisionError:
    print("Division by zero")
else:
    print(f"Result: {result}")

# Finally clause (always runs)
try:
    file = open("data.txt", "r")
    data = file.read()
except FileNotFoundError:
    print("File not found")
finally:
    print("Cleaning up...")
    file.close() if 'file' in locals() else None
```

## 📁 FILE OPERATIONS
### Reading Files
```
# Read entire file
with open("file.txt", "r") as f:
    content = f.read()          # Entire file as string

# Read line by line
with open("file.txt", "r") as f:
    for line in f:
        print(line.strip())

# Read all lines into list
with open("file.txt", "r") as f:
    lines = f.readlines()       # List of lines

# Read with encoding
with open("file.txt", "r", encoding="utf-8") as f:
    content = f.read()
```

### Writing Files
```
# Write to file (overwrites)
with open("output.txt", "w") as f:
    f.write("Hello, World!\n")
    f.write("Second line\n")

# Append to file
with open("output.txt", "a") as f:
    f.write("Appended line\n")

# Write multiple lines
lines = ["Line 1\n", "Line 2\n", "Line 3\n"]
with open("output.txt", "w") as f:
    f.writelines(lines)
```

### File Modes
```
"r"     # Read (default)
"w"     # Write (truncates)
"x"     # Exclusive creation (fails if exists)
"a"     # Append
"b"     # Binary mode
"t"     # Text mode (default)
"+"     # Read and write

# Examples
"rb"    # Read binary
"wb"    # Write binary
"r+"    # Read and write
"a+"    # Append and read
```
```
File operations allow reading from and writing to files. Use with statement for automatic closing.
```

### Working with Paths
```
Definition: pathlib provides object-oriented filesystem paths.

from pathlib import Path  # Modern approach (Python 3.4+)

# Create Path object
path = Path("folder/file.txt")

# Common operations
path.exists()           # Check if exists
path.is_file()          # Check if file
path.is_dir()           # Check if directory
path.name               # "file.txt"
path.stem               # "file" (without extension)
path.suffix             # ".txt"
path.parent             # Path("folder")
path.with_suffix(".csv") # Change extension

# Read/write with Path
content = path.read_text()
path.write_text("New content")

# List directory
for item in Path(".").iterdir():
    print(item.name)

# Find files
list(Path(".").glob("*.py"))          # All Python files
list(Path(".").glob("**/*.py"))       # Recursive
```

## 📦 MODULES & PACKAGES
### Importing Modules
```
Definition: Modules are Python files containing code. Packages are directories containing modules.

# Import entire module
import math
math.sqrt(16)  # 4.0

# Import with alias
import numpy as np
np.array([1, 2, 3])

# Import specific functions
from math import sqrt, pi
sqrt(16)  # 4.0

# Import all (generally discouraged)
from math import *

# Import from package
from sklearn.linear_model import LinearRegression

# Relative imports (within package)
from . import module_in_same_package
from .. import module_in_parent_package
```

### Creating Modules & Packages
```
Definition: __name__ == "__main__" allows code to run when file is executed directly, not when imported.

"""
my_module.py
"""
# Module code
def greet(name):
    return f"Hello, {name}!"

class Calculator:
    def add(self, a, b):
        return a + b

# Special variables
__all__ = ["greet"]  # Controls what gets imported with "from module import *"
__version__ = "1.0.0"

# Test code (runs when module is executed directly)
if __name__ == "__main__":
    print(greet("World"))

"""
Package structure:
my_package/
    __init__.py      # Package initialization
    module1.py
    module2.py
    subpackage/
        __init__.py
        module3.py
"""
```

### Virtual Environments
```
Definition: Virtual environments isolate project dependencies.

# Create virtual environment
python -m venv venv

# Activate (Windows)
venv\Scripts\activate

# Activate (macOS/Linux)
source venv/bin/activate

# Deactivate
deactivate

# Requirements file
# requirements.txt
# numpy==1.21.0
# pandas>=1.3.0
# matplotlib

# Install from requirements
pip install -r requirements.txt

# Generate requirements
pip freeze > requirements.txt
```

## 🚀 ADVANCED CONCEPTS
### Generators
```
Definition: Generators produce values lazily (one at a time), saving memory.
# Generator function
def count_up_to(max):
    count = 1
    while count <= max:
        yield count  # Pauses here, resumes on next()
        count += 1

# Use generator
counter = count_up_to(5)
next(counter)  # 1
next(counter)  # 2
list(counter)  # [3, 4, 5]

# Generator expression
squares = (x**2 for x in range(10))
sum(squares)  # 285

# Infinite generator
def infinite_sequence():
    num = 0
    while True:
        yield num
        num += 1
```
### Context Managers
```
Definition: Context managers handle setup and teardown of resources (files, locks, connections).

# Using with statement
with open("file.txt", "r") as f:
    content = f.read()
# File automatically closed

# Create custom context manager
from contextlib import contextmanager

@contextmanager
def timer():
    import time
    start = time.time()
    try:
        yield
    finally:
        end = time.time()
        print(f"Elapsed: {end - start:.2f}s")

# Use custom context manager
with timer():
    # Do something time-consuming
    sum(range(1000000))
```

### Decorators (Advanced)
```
# Decorator with arguments
def repeat(n):
    def decorator(func):
        def wrapper(*args, **kwargs):
            for _ in range(n):
                result = func(*args, **kwargs)
            return result
        return wrapper
    return decorator

@repeat(3)
def say_hello():
    print("Hello")

# Class decorator
def add_method(cls):
    def new_method(self):
        return "New method"
    cls.new_method = new_method
    return cls

@add_method
class MyClass:
    pass

obj = MyClass()
obj.new_method()  # "New method"
```

## 📚 USEFUL LIBRARIES
### Built-in Modules
```
# math - Mathematical functions
import math
math.sqrt(16), math.pi, math.sin(math.radians(30))

# random - Random numbers
import random
random.random(), random.randint(1, 10), random.choice(["a", "b", "c"])

# datetime - Dates and times
from datetime import datetime, date, timedelta
datetime.now(), date.today(), timedelta(days=7)

# json - JSON processing
import json
json_string = '{"name": "Alice", "age": 30}'
data = json.loads(json_string)  # String to dict
json.dumps(data)                # Dict to string

# re - Regular expressions
import re
re.findall(r'\d+', "Hello 123 World 456")  # ['123', '456']
re.search(r'^Hello', "Hello World")        # Match object

# os - Operating system interface
import os
os.getcwd(), os.listdir('.'), os.path.join('folder', 'file.txt')

# sys - System-specific parameters
import sys
sys.version, sys.argv, sys.exit(0)

# itertools - Iterator tools
import itertools
list(itertools.permutations([1, 2, 3], 2))

# collections - Container datatypes
from collections import Counter, defaultdict, deque

# functools - Higher-order functions
from functools import lru_cache, partial, reduce

# typing - Type hints
from typing import List, Dict, Optional, Union
```

### Popular Third-party Libraries
```
"""
Data Science & Analytics:
- numpy: Numerical computing
- pandas: Data manipulation
- matplotlib: Plotting
- seaborn: Statistical visualization
- scikit-learn: Machine learning
- scipy: Scientific computing
- tensorflow/pytorch: Deep learning

Web Development:
- flask/django: Web frameworks
- requests: HTTP requests
- beautifulsoup4: Web scraping
- fastapi: Modern API framework

Automation & Testing:
- selenium: Web automation
- pytest: Testing framework
- celery: Task queue

DevOps & Deployment:
- docker: Containerization
- kubernetes: Orchestration
- airflow: Workflow management

Database:
- sqlalchemy: ORM
- psycopg2: PostgreSQL adapter
- pymongo: MongoDB driver
"""
```

## QUICK REFERENCE
### Common Patterns
```
# List comprehension
[x**2 for x in range(10) if x % 2 == 0]

# Dictionary comprehension
{x: x**2 for x in range(5)}

# Set comprehension
{x**2 for x in range(5)}

# Generator expression
(x**2 for x in range(10))

# Lambda function
lambda x: x * 2

# Map/Filter/Reduce
list(map(lambda x: x*2, [1, 2, 3]))
list(filter(lambda x: x > 0, [-1, 0, 1, 2]))
from functools import reduce
reduce(lambda x, y: x + y, [1, 2, 3, 4])

# Enumerate
for i, value in enumerate(["a", "b", "c"]):
    print(i, value)

# Zip
for a, b in zip([1, 2, 3], ["a", "b", "c"]):
    print(a, b)
```
```
Term	                Definition
Python	              High-level, interpreted programming language
Variable	            Named reference to a value
Data Type	            Classification of data (int, str, list, etc.)
Immutable	            Cannot be changed after creation (str, tuple)
Mutable	              Can be changed after creation (list, dict)
Function	            Reusable block of code
Method	              Function associated with an object
Class	                Blueprint for creating objects
Object	              Instance of a class
Module	              Python file containing code
Package	              Directory containing modules
Import	              Bring code from module/package into current scope
Exception	            Runtime error that can be caught and handled
Iterable	            Object that can return its elements one at a time
Iterator	            Object with next() method
Generator	            Function that yields values lazily
Decorator	            Function that modifies another function
Context Manager	      Object with enter() and exit() methods
Lambda	              Anonymous, single-expression function
List Comprehension	  Compact way to create lists
Dunder Methods	      Special methods with double underscores
PEP	                  Python Enhancement Proposal (standards)
Virtual Environment	  Isolated Python environment
```

```
Python - A high-level, interpreted programming language known for its readability and simplicity.

Variable - A named reference or container that stores a value in memory.

Data Type - A classification that specifies what type of value a variable can hold (like integer, string, list, etc.).

Immutable - An object whose value cannot be changed after it is created (examples: strings, tuples).

Mutable - An object whose value can be changed after it is created (examples: lists, dictionaries).

Function - A reusable block of code that performs a specific task and can be called multiple times.

Method - A function that is associated with an object and defined inside a class.

Class - A blueprint or template for creating objects that defines attributes and methods.

Object - An instance of a class that contains both data (attributes) and behavior (methods).

Module - A Python file containing code, including functions, classes, and variables.

Package - A directory containing multiple modules and a special init.py file.

Import - A statement that brings code from a module or package into the current scope for use.

Exception - A runtime error that can be caught and handled gracefully without crashing the program.

Iterable - An object that can return its elements one at a time (can be looped over).

Iterator - An object with a next() method that returns the next item in a sequence.

Generator - A special type of function that yields values lazily, one at a time, using the yield keyword.

Decorator - A function that modifies or enhances another function without changing its source code.

Context Manager - An object with enter() and exit() methods, used with the 'with' statement for resource management.

Lambda - An anonymous, single-expression function defined using the lambda keyword.

List Comprehension - A compact way to create lists by applying an expression to each item in an iterable.

Dunder Methods - Special methods with double underscores (like init, str) that enable operator overloading and other features.

PEP - Python Enhancement Proposal, a design document that describes new features or processes for Python.

Virtual Environment - An isolated Python environment that allows projects to have their own dependencies without conflicts.
```







