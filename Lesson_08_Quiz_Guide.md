# Lesson 08: Modules & Functions - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers function definition, parameters, return values, variable scope, and module creation/importing.

## 🎯 Key Concepts to Master

### 1. Function Definition
- **def keyword**: Used to define functions
- **Function name**: Should be descriptive and follow naming conventions
- **Parameters**: Input values the function expects
- **Function body**: Code that executes when function is called
- **Return statement**: Sends value back to caller

### 2. Function Parameters
- **Required parameters**: Must be provided when calling function
- **Default parameters**: Have default values if not provided
- **Keyword arguments**: Arguments specified by parameter name
- **Positional arguments**: Arguments specified by position
- **Arbitrary arguments**: *args and **kwargs

### 3. Return Values
- **return statement**: Exits function and returns value
- **Multiple returns**: Function can have multiple return statements
- **Implicit return**: Functions return None if no return statement
- **Return multiple values**: Can return tuples, lists, etc.

### 4. Variable Scope
- **Local scope**: Variables defined inside function
- **Global scope**: Variables defined at module level
- **Enclosing scope**: Variables in nested functions
- **Built-in scope**: Python's built-in names
- **global keyword**: Modify global variables from function
- **nonlocal keyword**: Modify variables in enclosing scope

### 5. Module Creation and Importing
- **Module**: Python file containing functions, classes, variables
- **import statement**: Import entire module
- **from import**: Import specific items from module
- **as keyword**: Alias for imported items
- **Built-in modules**: math, random, datetime, os, sys

### 6. Function Documentation
- **Docstrings**: String literals that document functions
- **Triple quotes**: """ or ''' for multi-line docstrings
- **help() function**: Display function documentation
- **__doc__ attribute**: Access function documentation

## 📝 Sample MCQs with Detailed Explanations

### Question 1: Function Definition
**How do you define a function in Python?**

- A) function name():
- B) def name(): ✅
- C) func name():
- D) define name():

**Explanation**: The def keyword is used to define functions in Python.

### Question 2: Function Output
**What is the output of the following function?**
```python
def add(x, y):
    return x + y
print(add(2, 3))
```

- A) 5 ✅
- B) 23
- C) Error
- D) None

**Explanation**: The function returns the sum of x and y, so add(2, 3) returns 5.

### Question 3: Module Import
**Which keyword is used to import a module?**

- A) include
- B) import ✅
- C) require
- D) using

**Explanation**: The import keyword is used to import modules in Python.

### Question 4: Function Documentation
**What is a docstring?**

- A) A comment
- B) A string literal that documents a function ✅
- C) A variable name
- D) A module name

**Explanation**: A docstring is a string literal that serves as documentation for functions, classes, or modules.

### Question 5: Variable Scope
**What is the scope of a variable defined inside a function?**

- A) Global
- B) Local ✅
- C) Universal
- D) Module-level

**Explanation**: Variables defined inside a function have local scope and are only accessible within that function.

## 🔍 Additional Practice Questions

### Question 6: Default Parameters
**What is the output of the following function call?**
```python
def greet(name="World"):
    return f"Hello, {name}!"
print(greet())
```

- A) Hello, !
- B) Hello, World! ✅
- C) Error
- D) None

**Explanation**: Since no argument is provided, the default parameter "World" is used.

### Question 7: Return Statement
**What does a function return if it has no return statement?**

- A) 0
- B) None ✅
- C) Error
- D) Empty string

**Explanation**: Functions without a return statement implicitly return None.

### Question 8: Global Variable
**What is the output of the following code?**
```python
x = 10
def func():
    global x
    x = 20
func()
print(x)
```

- A) 10
- B) 20 ✅
- C) Error
- D) None

**Explanation**: The global keyword allows the function to modify the global variable x.

### Question 9: Function Parameters
**How many parameters does this function accept?**
```python
def func(a, b, c=10, d=20):
    pass
```

- A) 2
- B) 4
- C) 2 to 4 ✅
- D) Error

**Explanation**: The function has 2 required parameters (a, b) and 2 default parameters (c, d), so it can accept 2 to 4 arguments.

### Question 10: Module Import
**What is the correct way to import only the sqrt function from math module?**

- A) import sqrt from math
- B) from math import sqrt ✅
- C) import math.sqrt
- D) from sqrt import math

**Explanation**: The from...import syntax imports specific items from a module.

## 📋 Important Facts to Remember

### Function Definition Rules
1. **def keyword**: Must start with def
2. **Function name**: Should be descriptive and follow snake_case
3. **Parameters**: Can have multiple parameters
4. **Function body**: Must be indented
5. **Return statement**: Optional, returns None if missing

### Parameter Types
1. **Required**: Must be provided
2. **Default**: Have default values
3. **Keyword**: Specified by name
4. **Positional**: Specified by position
5. **Arbitrary**: *args (tuple) and **kwargs (dict)

### Variable Scope Rules
1. **Local**: Variables inside function
2. **Global**: Variables at module level
3. **Enclosing**: Variables in nested functions
4. **Built-in**: Python's built-in names
5. **LEGB**: Local → Enclosing → Global → Built-in

### Import Methods
1. **import module**: Import entire module
2. **from module import item**: Import specific item
3. **from module import item as alias**: Import with alias
4. **import module as alias**: Import module with alias

## 🎯 Study Tips for This Lesson

1. **Practice Function Writing**: Write functions with different parameter types
2. **Test Variable Scope**: Experiment with local and global variables
3. **Use Built-in Modules**: Practice importing and using common modules
4. **Write Docstrings**: Document your functions properly
5. **Understand Return Values**: Know what functions return

## 🔗 Related Resources

- [Python Functions](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)
- [Python Modules](https://docs.python.org/3/tutorial/modules.html)
- [Python Built-in Functions](https://docs.python.org/3/library/functions.html)

## ✅ Self-Assessment Checklist

- [ ] I can define functions with parameters
- [ ] I understand different parameter types
- [ ] I know how to use return statements
- [ ] I understand variable scope (local vs global)
- [ ] I can import modules and specific functions
- [ ] I can write docstrings for functions
- [ ] I know how to use default parameters
- [ ] I understand keyword arguments
- [ ] I can use the global and nonlocal keywords
- [ ] I know common built-in modules

## 🧮 Practice Exercises

### Exercise 1: Basic Function Definition
```python
# Define a simple function
def greet(name):
    return f"Hello, {name}!"

# Call the function
print(greet("Alice"))       # Hello, Alice!

# Function with multiple parameters
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 3)
print(result)               # 8
```

### Exercise 2: Default Parameters
```python
# Function with default parameters
def greet_with_title(name, title="Mr."):
    return f"Hello, {title} {name}!"

print(greet_with_title("Smith"))           # Hello, Mr. Smith!
print(greet_with_title("Johnson", "Dr."))  # Hello, Dr. Johnson!

# Multiple default parameters
def create_profile(name, age=25, city="Unknown"):
    return f"Name: {name}, Age: {age}, City: {city}"

print(create_profile("Alice"))             # Name: Alice, Age: 25, City: Unknown
print(create_profile("Bob", 30, "NYC"))    # Name: Bob, Age: 30, City: NYC
```

### Exercise 3: Return Values
```python
# Function returning multiple values
def get_name_and_age():
    return "Alice", 25

name, age = get_name_and_age()
print(f"{name} is {age} years old")        # Alice is 25 years old

# Function with conditional return
def absolute_value(x):
    if x >= 0:
        return x
    else:
        return -x

print(absolute_value(5))    # 5
print(absolute_value(-3))   # 3
```

### Exercise 4: Variable Scope
```python
# Global variable
global_var = "I'm global"

def test_scope():
    local_var = "I'm local"
    print(local_var)        # I'm local
    print(global_var)       # I'm global

test_scope()
# print(local_var)          # NameError: name 'local_var' is not defined

# Modifying global variable
counter = 0

def increment():
    global counter
    counter += 1
    return counter

print(increment())          # 1
print(increment())          # 2
```

### Exercise 5: Module Importing
```python
# Import entire module
import math
print(math.sqrt(16))        # 4.0
print(math.pi)              # 3.141592653589793

# Import specific functions
from random import randint, choice
print(randint(1, 10))       # Random number between 1 and 10
print(choice(['a', 'b', 'c']))  # Random choice from list

# Import with alias
import datetime as dt
now = dt.datetime.now()
print(now.year)             # Current year
```

### Exercise 6: Function Documentation
```python
def calculate_area(length, width):
    """
    Calculate the area of a rectangle.
    
    Args:
        length (float): The length of the rectangle
        width (float): The width of the rectangle
    
    Returns:
        float: The area of the rectangle
    """
    return length * width

# Access documentation
print(calculate_area.__doc__)
help(calculate_area)

# Test the function
area = calculate_area(5, 3)
print(f"Area: {area}")      # Area: 15
```

### Exercise 7: Arbitrary Arguments
```python
# *args for variable number of arguments
def sum_all(*args):
    return sum(args)

print(sum_all(1, 2, 3, 4, 5))  # 15

# **kwargs for keyword arguments
def print_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_info(name="Alice", age=25, city="NYC")
# name: Alice
# age: 25
# city: NYC
```

### Exercise 8: Lambda Functions
```python
# Lambda function (anonymous function)
square = lambda x: x**2
print(square(5))            # 25

# Lambda with multiple parameters
add = lambda x, y: x + y
print(add(3, 4))            # 7

# Lambda in built-in functions
numbers = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x**2, numbers))
print(squared)              # [1, 4, 9, 16, 25]
```

**Remember**: Functions are the building blocks of modular programming. Master function definition, parameters, and scope as they are essential for writing clean, reusable code! 