# Lesson 04: Strings & Type Casting - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers string manipulation, formatting, slicing, and type casting between different data types.

## 🎯 Key Concepts to Master

### 1. String Creation and Properties
- **String literals**: Single quotes, double quotes, triple quotes
- **Immutable**: Strings cannot be modified after creation
- **Indexing**: Zero-based indexing (first character is at index 0)
- **Length**: len() function returns string length

### 2. String Methods
- **Case manipulation**: upper(), lower(), title(), capitalize()
- **Whitespace**: strip(), lstrip(), rstrip()
- **Searching**: find(), index(), count(), startswith(), endswith()
- **Splitting/Joining**: split(), join(), partition()
- **Replacement**: replace()
- **Formatting**: format(), f-strings

### 3. String Slicing
- **Syntax**: string[start:end:step]
- **Negative indexing**: -1 is last character
- **Step**: Optional third parameter for skipping characters
- **Default values**: start=0, end=len(string), step=1

### 4. String Formatting
- **f-strings** (Python 3.6+): f"Hello {name}"
- **.format()**: "Hello {}".format(name)
- **% operator**: "Hello %s" % name
- **Placeholders**: {}, {0}, {name}

### 5. Type Casting
- **int()**: Convert to integer
- **float()**: Convert to float
- **str()**: Convert to string
- **bool()**: Convert to boolean
- **list()**: Convert to list
- **tuple()**: Convert to tuple

### 6. Escape Sequences
- **\n**: New line
- **\t**: Tab
- **\\**: Backslash
- **\"**: Double quote
- **\'**: Single quote
- **\r**: Carriage return

### 7. Raw Strings
- **Prefix with r**: r"C:\path\to\file"
- **No escape processing**: Backslashes are literal

## 📝 Sample MCQs with Detailed Explanations

### Question 1: String Indexing
**What is the output of `"Hello"[1]`?**

- A) H
- B) e ✅
- C) l
- D) o

**Explanation**: String indexing starts at 0, so index 1 refers to the second character 'e'.

### Question 2: String Method
**Which method removes whitespace from both ends of a string?**

- A) trim()
- B) strip() ✅
- C) clean()
- D) remove()

**Explanation**: The strip() method removes leading and trailing whitespace characters.

### Question 3: Type Conversion Error
**What is the result of `int("3.14")`?**

- A) 3.14
- B) 3
- C) Error ✅
- D) 3.0

**Explanation**: int() cannot convert a string with a decimal point directly. You need to convert to float first: int(float("3.14")).

### Question 4: Raw String
**How do you create a raw string in Python?**

- A) r"string" ✅
- B) raw"string"
- C) @string
- D) #string

**Explanation**: Prefixing a string with 'r' makes it a raw string where backslashes are treated literally.

### Question 5: String Method
**What is the output of `"Python".upper()`?**

- A) python
- B) PYTHON ✅
- C) Python
- D) Error

**Explanation**: The upper() method converts all characters to uppercase.

## 🔍 Additional Practice Questions

### Question 6: String Slicing
**What is the output of `"Python"[1:4]`?**

- A) "Pyt"
- B) "yth" ✅
- C) "ytho"
- D) "Python"

**Explanation**: Slicing [1:4] includes characters at indices 1, 2, and 3 (but not 4), so "yth".

### Question 7: String Length
**What is the length of the string `"Hello World"`?**

- A) 10
- B) 11 ✅
- C) 12
- D) Error

**Explanation**: The string has 11 characters (including the space).

### Question 8: String Concatenation
**What is the result of `"Hello" + " " + "World"`?**

- A) "HelloWorld"
- B) "Hello World" ✅
- C) "Hello  World"
- D) Error

**Explanation**: The + operator concatenates strings, so "Hello" + " " + "World" = "Hello World".

### Question 9: String Method
**What does `"hello world".title()` return?**

- A) "Hello World" ✅
- B) "HELLO WORLD"
- C) "hello world"
- D) "Hello world"

**Explanation**: title() capitalizes the first letter of each word.

### Question 10: Type Casting
**What is the output of `str(123) + "456"`?**

- A) 579
- B) "123456" ✅
- C) Error
- D) 123456

**Explanation**: str(123) converts 123 to "123", then concatenates with "456" to get "123456".

## 📋 Important Facts to Remember

### String Properties
1. **Immutable**: Cannot be changed after creation
2. **Indexed**: Zero-based indexing
3. **Sliced**: Can extract portions using [start:end:step]
4. **Methods**: Many built-in methods for manipulation

### Common String Methods
1. **Case**: upper(), lower(), title(), capitalize()
2. **Whitespace**: strip(), lstrip(), rstrip()
3. **Search**: find(), index(), count()
4. **Split/Join**: split(), join()
5. **Replace**: replace()

### Type Casting Rules
1. **int()**: Truncates floats, converts valid string numbers
2. **float()**: Converts integers and valid string numbers
3. **str()**: Converts any object to string representation
4. **bool()**: Converts to True/False based on truthiness

### String Formatting Methods
1. **f-strings**: Most readable and efficient (Python 3.6+)
2. **.format()**: Flexible and powerful
3. **% operator**: Older style, still supported

## 🎯 Study Tips for This Lesson

1. **Practice String Methods**: Try all string methods on sample strings
2. **Master Slicing**: Understand start, end, and step parameters
3. **Learn Formatting**: Practice different string formatting methods
4. **Test Type Casting**: Convert between different data types
5. **Understand Immutability**: Know that strings cannot be modified in place

## 🔗 Related Resources

- [Python String Methods](https://docs.python.org/3/library/stdtypes.html#string-methods)
- [Python String Formatting](https://docs.python.org/3/library/string.html#format-string-syntax)
- [Python Type Conversion](https://docs.python.org/3/library/functions.html#int)

## ✅ Self-Assessment Checklist

- [ ] I can create and manipulate strings
- [ ] I understand string indexing and slicing
- [ ] I can use common string methods
- [ ] I know different string formatting methods
- [ ] I can convert between data types
- [ ] I understand string immutability
- [ ] I can use escape sequences
- [ ] I know how to create raw strings
- [ ] I can concatenate strings
- [ ] I understand string length and indexing

## 🧮 Practice Exercises

### Exercise 1: String Methods
```python
# Test string methods
text = "  Hello World  "
print(text.strip())        # "Hello World"
print(text.upper())        # "  HELLO WORLD  "
print(text.lower())        # "  hello world  "
print(text.title())        # "  Hello World  "
print(len(text))           # 15
```

### Exercise 2: String Slicing
```python
# Test string slicing
text = "Python Programming"
print(text[0:6])           # "Python"
print(text[7:])            # "Programming"
print(text[-11:])          # "Programming"
print(text[::2])           # "Pto rgamn"
print(text[::-1])          # "gnimmargorP nohtyP"
```

### Exercise 3: String Formatting
```python
# Test string formatting
name = "Alice"
age = 25

# f-string (recommended)
print(f"My name is {name} and I am {age} years old")

# .format() method
print("My name is {} and I am {} years old".format(name, age))

# % operator
print("My name is %s and I am %d years old" % (name, age))
```

### Exercise 4: Type Casting
```python
# Test type casting
print(int(3.9))            # 3
print(float(42))           # 42.0
print(str(123))            # "123"
print(bool(0))             # False
print(bool("Hello"))       # True
print(list("Python"))      # ['P', 'y', 't', 'h', 'o', 'n']
```

### Exercise 5: String Operations
```python
# Test string operations
text = "Python is awesome"
print(text.split())        # ['Python', 'is', 'awesome']
print(" ".join(['Hello', 'World']))  # "Hello World"
print(text.replace("awesome", "great"))  # "Python is great"
print(text.count("o"))     # 2
print(text.find("is"))     # 7
```

**Remember**: Strings are one of the most commonly used data types in Python. Master string manipulation as it's essential for text processing and data handling! 