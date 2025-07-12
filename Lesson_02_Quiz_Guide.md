# Lesson 02: Data Types - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers Python's fundamental data types, their properties, type checking, and type conversion.

## 🎯 Key Concepts to Master

### 1. Numeric Data Types
- **int**: Integer numbers (whole numbers)
  - Examples: 42, -17, 0, 1000000
  - Unlimited precision in Python 3
- **float**: Floating-point numbers (decimal numbers)
  - Examples: 3.14, -0.001, 2.0, 1e-10
  - Double precision (64-bit)
- **complex**: Complex numbers
  - Examples: 3+4j, -1j, 2.5+0j
  - Real and imaginary parts

### 2. Boolean Data Type
- **bool**: True or False values
- **Truthy values**: Non-zero numbers, non-empty sequences, True
- **Falsy values**: 0, empty sequences, None, False
- **Boolean conversion**: bool() function

### 3. Type Checking and Conversion
- **type()**: Function to check data type
- **Type conversion functions**:
  - int(): Convert to integer
  - float(): Convert to float
  - str(): Convert to string
  - bool(): Convert to boolean

### 4. Memory and Mutability
- **Immutable types**: int, float, bool, str, tuple
- **Mutable types**: list, dict, set
- **Memory management**: Python handles memory automatically

## 📝 Sample MCQs with Detailed Explanations

### Question 1: Integer Identification
**Which of the following is an integer in Python?**

- A) 3.14
- B) "42"
- C) 42 ✅
- D) True

**Explanation**: 42 is a literal integer. 3.14 is a float, "42" is a string, and True is a boolean.

### Question 2: Type Function
**What is the output of `type(3.14)`?**

- A) <class 'int'>
- B) <class 'float'> ✅
- C) <class 'number'>
- D) <class 'decimal'>

**Explanation**: The type() function returns the class of the object. 3.14 is a float literal, so it returns <class 'float'>.

### Question 3: Complex Numbers
**Which data type represents complex numbers in Python?**

- A) complex ✅
- B) imaginary
- C) number
- D) real

**Explanation**: Python uses the 'complex' data type for complex numbers, which have both real and imaginary parts.

### Question 4: Boolean Conversion
**What is the result of `bool(0)`?**

- A) True
- B) False ✅
- C) 0
- D) Error

**Explanation**: The number 0 is considered falsy in Python, so bool(0) returns False.

### Question 5: Immutable Types
**Which of the following is immutable?**

- A) List
- B) Dictionary
- C) Integer ✅
- D) Set

**Explanation**: Integers are immutable - once created, their value cannot be changed. Lists, dictionaries, and sets are mutable.

## 🔍 Additional Practice Questions

### Question 6: Float Precision
**What is the output of `0.1 + 0.2`?**

- A) 0.3
- B) 0.30000000000000004 ✅
- C) 0.3 exactly
- D) Error

**Explanation**: Due to floating-point precision issues, 0.1 + 0.2 doesn't equal exactly 0.3.

### Question 7: Type Conversion
**What is the result of `int(3.9)`?**

- A) 3.9
- B) 3 ✅
- C) 4
- D) Error

**Explanation**: int() truncates decimal numbers, so int(3.9) becomes 3.

### Question 8: Boolean Truthiness
**Which of the following is considered falsy?**

- A) "Hello"
- B) [1, 2, 3]
- C) 0 ✅
- D) True

**Explanation**: 0 is considered falsy in Python, while non-empty strings, lists, and True are truthy.

### Question 9: Complex Number
**What is the real part of `3+4j`?**

- A) 3 ✅
- B) 4
- C) 5
- D) 7

**Explanation**: In a complex number a+bj, 'a' is the real part and 'b' is the imaginary part.

### Question 10: Type Checking
**What is the output of `isinstance(42, int)`?**

- A) True ✅
- B) False
- C) 42
- D) Error

**Explanation**: isinstance() checks if an object is an instance of a specified type. 42 is an integer, so it returns True.

## 📋 Important Facts to Remember

### Numeric Types
1. **int**: Unlimited precision in Python 3
2. **float**: 64-bit double precision
3. **complex**: Real and imaginary parts

### Boolean Values
1. **Truthy**: Non-zero numbers, non-empty sequences, True
2. **Falsy**: 0, empty sequences, None, False

### Type Conversion Rules
1. **int()**: Truncates decimals, converts strings if possible
2. **float()**: Converts integers and strings to float
3. **bool()**: Converts any value to boolean
4. **str()**: Converts any value to string

### Memory Characteristics
1. **Immutable**: int, float, bool, str, tuple
2. **Mutable**: list, dict, set
3. **Memory management**: Automatic garbage collection

## 🎯 Study Tips for This Lesson

1. **Practice Type Checking**: Use type() and isinstance() functions
2. **Test Conversions**: Try converting between different types
3. **Understand Boolean Logic**: Know what makes values truthy or falsy
4. **Memory Concepts**: Understand the difference between mutable and immutable
5. **Precision Awareness**: Be aware of floating-point precision issues

## 🔗 Related Resources

- [Python Numeric Types](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex)
- [Python Boolean Operations](https://docs.python.org/3/library/stdtypes.html#boolean-operations-and-or-not)
- [Python Type Conversion](https://docs.python.org/3/library/functions.html#int)

## ✅ Self-Assessment Checklist

- [ ] I can identify different numeric types (int, float, complex)
- [ ] I understand boolean values and truthiness
- [ ] I can use type() and isinstance() functions
- [ ] I know how to convert between data types
- [ ] I understand the difference between mutable and immutable types
- [ ] I can explain floating-point precision issues
- [ ] I know the rules for boolean conversion
- [ ] I understand memory management in Python

## 🧮 Practice Exercises

### Exercise 1: Type Identification
```python
# Identify the type of each value
print(type(42))        # Should be int
print(type(3.14))      # Should be float
print(type(True))      # Should be bool
print(type("Hello"))   # Should be str
print(type(3+4j))      # Should be complex
```

### Exercise 2: Type Conversion
```python
# Practice conversions
print(int(3.9))        # 3
print(float(42))       # 42.0
print(str(123))        # "123"
print(bool(0))         # False
print(bool("Hello"))   # True
```

### Exercise 3: Boolean Logic
```python
# Test truthiness
print(bool(0))         # False
print(bool(1))         # True
print(bool(""))        # False
print(bool("Hello"))   # True
print(bool([]))        # False
print(bool([1, 2]))    # True
```

**Remember**: Understanding data types is fundamental to Python programming. Master these concepts well as they form the building blocks for all other Python operations! 