# Lesson 09: Exception Handling - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers Python exception handling, including try-except blocks, different exception types, and error management.

## 🎯 Key Concepts to Master

### 1. What are Exceptions?
- **Runtime errors**: Errors that occur during program execution
- **Exception objects**: Python objects that represent errors
- **Exception hierarchy**: Built-in exception classes
- **Raise exceptions**: When errors occur, exceptions are raised
- **Handle exceptions**: Catch and process exceptions

### 2. Try-Except Blocks
- **try block**: Code that might raise an exception
- **except block**: Code that handles the exception
- **Multiple except clauses**: Handle different exception types
- **Exception types**: Specify which exceptions to catch
- **Generic except**: Catch all exceptions (use sparingly)

### 3. Exception Types
- **ValueError**: Invalid value for operation
- **TypeError**: Invalid type for operation
- **IndexError**: Invalid index for sequence
- **KeyError**: Invalid key for dictionary
- **ZeroDivisionError**: Division by zero
- **FileNotFoundError**: File not found
- **AttributeError**: Invalid attribute access

### 4. Finally Clause
- **Cleanup code**: Code that always executes
- **Resource management**: Close files, connections
- **Exception or not**: Executes regardless of exception
- **Return statements**: Finally executes even after return

### 5. Raise Statement
- **Manual exception raising**: raise Exception("message")
- **Re-raising exceptions**: raise without arguments
- **Custom exceptions**: Create your own exception classes
- **Exception chaining**: Preserve original exception

### 6. Exception Hierarchy
- **BaseException**: Root of exception hierarchy
- **Exception**: Base class for built-in exceptions
- **SystemExit**: Exit interpreter
- **KeyboardInterrupt**: User interrupts program
- **Custom exceptions**: Inherit from Exception

## 📝 Sample MCQs with Detailed Explanations

### Question 1: Exception Handling Block
**Which block is used to handle exceptions?**

- A) try-except ✅
- B) if-else
- C) for-while
- D) def-return

**Explanation**: The try-except block is specifically designed to catch and handle exceptions in Python.

### Question 2: Finally Clause Purpose
**What is the purpose of the `finally` clause?**

- A) To handle exceptions
- B) To execute code regardless of exceptions ✅
- C) To raise exceptions
- D) To define functions

**Explanation**: The finally clause executes its code whether an exception occurs or not, making it perfect for cleanup operations.

### Question 3: Division by Zero
**Which exception is raised when dividing by zero?**

- A) ValueError
- B) TypeError
- C) ZeroDivisionError ✅
- D) ArithmeticError

**Explanation**: ZeroDivisionError is raised when attempting to divide by zero.

### Question 4: Manual Exception Raising
**How do you raise an exception manually?**

- A) throw exception
- B) raise exception ✅
- C) catch exception
- D) handle exception

**Explanation**: The raise statement is used to manually raise exceptions in Python.

### Question 5: Try-Except-Finally Output
**What is the output of the following code?**
```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Error")
finally:
    print("Done")
```

- A) Error
- B) Done
- C) Error Done ✅
- D) None

**Explanation**: The except block prints "Error", then the finally block prints "Done" regardless of the exception.

## 🔍 Additional Practice Questions

### Question 6: Exception Type
**What exception is raised when accessing a non-existent list index?**

- A) KeyError
- B) IndexError ✅
- C) ValueError
- D) TypeError

**Explanation**: IndexError is raised when trying to access an index that doesn't exist in a sequence.

### Question 7: Multiple Except Clauses
**What is the output of the following code?**
```python
try:
    x = int("abc")
except ValueError:
    print("Value error")
except TypeError:
    print("Type error")
```

- A) Value error ✅
- B) Type error
- C) No output
- D) Error

**Explanation**: int("abc") raises a ValueError, which is caught by the first except clause.

### Question 8: Exception Hierarchy
**Which is the base class for all built-in exceptions?**

- A) BaseException
- B) Exception ✅
- C) Error
- D) RuntimeError

**Explanation**: Exception is the base class for all built-in, non-system-exiting exceptions.

### Question 9: Finally Execution
**What happens to the finally block if a return statement is in the try block?**

- A) Finally doesn't execute
- B) Finally executes before return ✅
- C) Finally executes after return
- D) Error occurs

**Explanation**: The finally block always executes, even if there's a return statement in the try block.

### Question 10: Generic Exception Handling
**What is the output of the following code?**
```python
try:
    x = 10 / 0
except:
    print("Caught exception")
```

- A) Caught exception ✅
- B) ZeroDivisionError
- C) No output
- D) Error

**Explanation**: The generic except clause catches all exceptions, including ZeroDivisionError.

## 📋 Important Facts to Remember

### Exception Handling Rules
1. **try**: Code that might raise an exception
2. **except**: Handle specific exceptions
3. **else**: Execute if no exception occurs
4. **finally**: Always execute (cleanup)
5. **raise**: Manually raise exceptions

### Common Exception Types
1. **ValueError**: Invalid value
2. **TypeError**: Invalid type
3. **IndexError**: Invalid index
4. **KeyError**: Invalid dictionary key
5. **ZeroDivisionError**: Division by zero
6. **FileNotFoundError**: File not found
7. **AttributeError**: Invalid attribute

### Best Practices
1. **Specific exceptions**: Catch specific exception types
2. **Avoid bare except**: Don't use except: without specifying type
3. **Cleanup in finally**: Use finally for resource cleanup
4. **Meaningful messages**: Provide clear error messages
5. **Log exceptions**: Log exceptions for debugging

### Exception Flow
1. **Exception occurs**: In try block
2. **Exception raised**: Python creates exception object
3. **Exception caught**: By except block
4. **Exception handled**: Code in except block executes
5. **Finally executes**: Cleanup code runs
6. **Program continues**: After exception handling

## 🎯 Study Tips for This Lesson

1. **Practice Exception Handling**: Write code that raises and catches exceptions
2. **Understand Exception Types**: Know when different exceptions are raised
3. **Use Finally**: Practice cleanup operations
4. **Test Different Scenarios**: Try various error conditions
5. **Read Error Messages**: Understand what different exceptions mean

## 🔗 Related Resources

- [Python Exception Handling](https://docs.python.org/3/tutorial/errors.html)
- [Python Built-in Exceptions](https://docs.python.org/3/library/exceptions.html)
- [Python Exception Hierarchy](https://docs.python.org/3/library/exceptions.html#exception-hierarchy)

## ✅ Self-Assessment Checklist

- [ ] I can write try-except blocks
- [ ] I understand different exception types
- [ ] I know how to use the finally clause
- [ ] I can raise exceptions manually
- [ ] I understand exception hierarchy
- [ ] I can handle multiple exception types
- [ ] I know when to use specific vs generic exception handling
- [ ] I can create custom exceptions
- [ ] I understand the flow of exception handling
- [ ] I can use exception handling for robust code

## 🧮 Practice Exercises

### Exercise 1: Basic Exception Handling
```python
# Basic try-except block
try:
    x = int(input("Enter a number: "))
    result = 10 / x
    print(f"Result: {result}")
except ValueError:
    print("Invalid input. Please enter a number.")
except ZeroDivisionError:
    print("Cannot divide by zero.")
except Exception as e:
    print(f"An error occurred: {e}")
```

### Exercise 2: Multiple Exception Types
```python
# Handle different exception types
def safe_divide(a, b):
    try:
        return a / b
    except TypeError:
        print("Both arguments must be numbers")
        return None
    except ZeroDivisionError:
        print("Cannot divide by zero")
        return None

print(safe_divide(10, 2))    # 5.0
print(safe_divide(10, 0))    # Cannot divide by zero, None
print(safe_divide("10", 2))  # Both arguments must be numbers, None
```

### Exercise 3: Finally Clause
```python
# Using finally for cleanup
def read_file(filename):
    file = None
    try:
        file = open(filename, 'r')
        content = file.read()
        return content
    except FileNotFoundError:
        print(f"File {filename} not found")
        return None
    finally:
        if file:
            file.close()
            print("File closed")

# Test with existing and non-existing files
read_file("existing_file.txt")
read_file("non_existing_file.txt")
```

### Exercise 4: Raising Exceptions
```python
# Manual exception raising
def validate_age(age):
    if not isinstance(age, int):
        raise TypeError("Age must be an integer")
    if age < 0:
        raise ValueError("Age cannot be negative")
    if age > 150:
        raise ValueError("Age seems unrealistic")
    return True

# Test the function
try:
    validate_age(25)         # Valid
    validate_age(-5)         # ValueError
    validate_age("25")       # TypeError
except (ValueError, TypeError) as e:
    print(f"Validation error: {e}")
```

### Exercise 5: Custom Exceptions
```python
# Create custom exception
class InsufficientFundsError(Exception):
    """Raised when account has insufficient funds"""
    pass

class BankAccount:
    def __init__(self, balance):
        self.balance = balance
    
    def withdraw(self, amount):
        if amount > self.balance:
            raise InsufficientFundsError(f"Insufficient funds. Balance: {self.balance}")
        self.balance -= amount
        return amount

# Test custom exception
account = BankAccount(100)
try:
    account.withdraw(150)
except InsufficientFundsError as e:
    print(f"Error: {e}")
```

### Exercise 6: Exception Chaining
```python
# Exception chaining
def process_data(data):
    try:
        return int(data)
    except ValueError as e:
        raise RuntimeError(f"Failed to process data: {data}") from e

try:
    result = process_data("abc")
except RuntimeError as e:
    print(f"Runtime error: {e}")
    print(f"Original error: {e.__cause__}")
```

### Exercise 7: Try-Except-Else-Finally
```python
# Complete exception handling structure
def divide_numbers(a, b):
    try:
        result = a / b
    except ZeroDivisionError:
        print("Cannot divide by zero")
        return None
    except TypeError:
        print("Both arguments must be numbers")
        return None
    else:
        print("Division successful")
        return result
    finally:
        print("Division operation completed")

# Test the function
print(divide_numbers(10, 2))     # Division successful, 5.0, Division operation completed
print(divide_numbers(10, 0))     # Cannot divide by zero, None, Division operation completed
print(divide_numbers("10", 2))   # Both arguments must be numbers, None, Division operation completed
```

### Exercise 8: Context Managers (with statement)
```python
# Using context managers for automatic resource management
def read_file_safely(filename):
    try:
        with open(filename, 'r') as file:
            return file.read()
    except FileNotFoundError:
        print(f"File {filename} not found")
        return None
    except PermissionError:
        print(f"Permission denied to read {filename}")
        return None

# The 'with' statement automatically handles file closing
content = read_file_safely("example.txt")
```

**Remember**: Exception handling is crucial for writing robust, production-ready code. Always handle exceptions appropriately and provide meaningful error messages! 