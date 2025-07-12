# 100 HARD Python Questions - ANSWERS & EXPLANATIONS

## 🎯 Complete Answer Key with Detailed Explanations

### **LESSON 01-03: Fundamentals**

**1. What is the output of `type(type(int))`?**
- **Answer: A) <class 'type'>**
- **Explanation**: `type(int)` returns `<class 'type'>` because `int` is a class, and `type()` of any class returns the `type` class itself.

**2. What happens when you run `print(0.1 + 0.2 == 0.3)`?**
- **Answer: B) False**
- **Explanation**: Due to floating-point precision issues, `0.1 + 0.2` equals `0.30000000000000004`, not exactly `0.3`.

**3. What is the result of `bool([]) + bool({}) + bool(0)`?**
- **Answer: A) 0**
- **Explanation**: All three are falsy values, so `bool([]) = 0`, `bool({}) = 0`, `bool(0) = 0`. Sum is `0 + 0 + 0 = 0`.

**4. What does `isinstance(True, int)` return?**
- **Answer: A) True**
- **Explanation**: In Python, `bool` is a subclass of `int`, so `True` is an instance of `int`.

**5. What is the output of `print(3 * '7' + 2 * '3')`?**
- **Answer: A) 77733**
- **Explanation**: String repetition: `'7' * 3 = '777'`, `'3' * 2 = '33'`, concatenated gives `'77733'`.

**6. What is the result of `(1, 2, 3) + (4, 5)`?**
- **Answer: A) (1, 2, 3, 4, 5)**
- **Explanation**: The `+` operator concatenates tuples, creating a new tuple with all elements.

**7. What does `print(2 ** 3 ** 2)` output?**
- **Answer: B) 512**
- **Explanation**: Exponentiation is right-associative, so `2 ** 3 ** 2` = `2 ** (3 ** 2)` = `2 ** 9` = `512`.

**8. What is the result of `True + False + True`?**
- **Answer: A) 2**
- **Explanation**: Boolean values are treated as integers: `True = 1`, `False = 0`, so `1 + 0 + 1 = 2`.

**9. What does `print(3 < 5 < 7 < 9)` return?**
- **Answer: A) True**
- **Explanation**: Python supports chained comparisons. This is equivalent to `(3 < 5) and (5 < 7) and (7 < 9)`, which is `True`.

**10. What is the output of `print(not not True or False)`?**
- **Answer: A) True**
- **Explanation**: `not not True` = `not False` = `True`, then `True or False` = `True`.

### **LESSON 04: Strings & Type Casting**

**11. What is the result of `"hello"[::-1][::-1] == "hello"`?**
- **Answer: A) True**
- **Explanation**: `[::-1]` reverses the string, so `"hello"[::-1]` = `"olleh"`, then `"olleh"[::-1]` = `"hello"`.

**12. What does `print("Python".replace("", "X"))` output?**
- **Answer: A) XPXyXtXhXoXnX**
- **Explanation**: Replacing empty string with "X" inserts "X" between every character.

**13. What is the output of `int(float("3.14"))`?**
- **Answer: B) 3**
- **Explanation**: `float("3.14")` = `3.14`, then `int(3.14)` truncates to `3`.

**14. What does `"abc".join(["1", "2", "3"])` return?**
- **Answer: A) "1abc2abc3"**
- **Explanation**: `join()` concatenates the list elements with the separator "abc".

**15. What is the result of `str(True) + str(False)`?**
- **Answer: A) "TrueFalse"**
- **Explanation**: `str(True)` = `"True"`, `str(False)` = `"False"`, concatenated gives `"TrueFalse"`.

**16. What does `print("hello".upper().lower())` output?**
- **Answer: A) "hello"**
- **Explanation**: `"hello".upper()` = `"HELLO"`, then `"HELLO".lower()` = `"hello"`.

**17. What is the output of `len("Python"[1:4:2])`?**
- **Answer: A) 2**
- **Explanation**: `"Python"[1:4:2]` = `"yt"` (characters at indices 1 and 3), length is 2.

**18. What does `"Python".split("")` return?**
- **Answer: C) Error**
- **Explanation**: `split()` with empty string raises `ValueError`.

**19. What is the result of `bool("0")`?**
- **Answer: A) True**
- **Explanation**: Non-empty strings are truthy, even if they contain "0".

**20. What does `print("hello" * 3 + "world" * 2)` output?**
- **Answer: A) "hellohellohelloworldworld"**
- **Explanation**: String repetition and concatenation: `"hello" * 3` = `"hellohellohello"`, `"world" * 2` = `"worldworld"`.

### **LESSON 05: Control Flow & Loops**

**21. What is the output of this code?**
```python
x = 0
for i in range(5):
    if i % 2 == 0:
        continue
    x += i
print(x)
```
- **Answer: C) 4**
- **Explanation**: Loop adds odd numbers (1, 3) to x: `0 + 1 + 3 = 4`.

**22. What does this code print?**
```python
for i in range(3):
    for j in range(2):
        if i == j:
            break
        print(f"{i},{j}")
```
- **Answer: B) 1,0 2,0**
- **Explanation**: When `i == j` (i=0,j=0), break exits inner loop. Only prints when `i != j`.

**23. What is the result of `[i for i in range(5) if i % 2 == 0]`?**
- **Answer: A) [0, 2, 4]**
- **Explanation**: List comprehension creates list of even numbers from 0 to 4.

**24. What does this code output?**
```python
x = 5
while x > 0:
    x -= 1
    if x == 2:
        continue
    print(x, end=" ")
```
- **Answer: A) 4 3 1 0**
- **Explanation**: When x=2, continue skips printing. Prints: 4, 3, 1, 0.

**25. What is the output of `sum(i for i in range(10) if i % 3 == 0)`?**
- **Answer: A) 18**
- **Explanation**: Sums numbers divisible by 3: `0 + 3 + 6 + 9 = 18`.

**26. What does this code print?**
```python
for i in range(3):
    pass
else:
    print("Done")
```
- **Answer: B) "Done"**
- **Explanation**: `else` clause executes when loop completes normally (no break).

**27. What is the result of `any(i % 2 == 0 for i in range(1, 6))`?**
- **Answer: A) True**
- **Explanation**: `any()` returns True if any element is True. Even numbers 2, 4 exist.

**28. What does this code output?**
```python
x = 10
if x > 5:
    if x > 15:
        print("Large")
    else:
        print("Medium")
else:
    print("Small")
```
- **Answer: B) "Medium"**
- **Explanation**: `x > 5` is True, but `x > 15` is False, so prints "Medium".

**29. What is the output of `[x for x in range(5) if x % 2 == 0 and x > 0]`?**
- **Answer: A) [2, 4]**
- **Explanation**: Even numbers greater than 0: 2, 4.

**30. What does this code print?**
```python
for i in range(3):
    for j in range(2):
        print(f"{i}{j}", end=" ")
    print()
```
- **Answer: B) 00 01\n10 11\n20 21**
- **Explanation**: Nested loops print each combination, with newline after each inner loop.

### **LESSON 06: Lists, Tuples & Dictionary**

**31. What is the output of `[1, 2, 3] * 2`?**
- **Answer: B) [1, 2, 3, 1, 2, 3]**
- **Explanation**: List repetition creates a new list with elements repeated.

**32. What does `dict(zip([1, 2], [3, 4]))` create?**
- **Answer: A) {1: 3, 2: 4}**
- **Explanation**: `zip()` pairs elements, `dict()` creates dictionary from pairs.

**33. What is the result of `[1, 2, 3].append(4)`?**
- **Answer: B) None**
- **Explanation**: `append()` modifies the list in-place and returns `None`.

**34. What does `{1: 'a', 2: 'b'}.get(3, 'default')` return?**
- **Answer: A) 'default'**
- **Explanation**: Key 3 doesn't exist, so returns default value 'default'.

**35. What is the output of `(1, 2, 3)[1:2]`?**
- **Answer: A) (2,)**
- **Explanation**: Slicing returns tuple with single element at index 1.

**36. What does `[1, 2, 3].extend([4, 5])` return?**
- **Answer: B) None**
- **Explanation**: `extend()` modifies list in-place and returns `None`.

**37. What is the result of `{1: 'a', 2: 'b'}.pop(1)`?**
- **Answer: A) 'a'**
- **Explanation**: `pop()` removes and returns the value for key 1.

**38. What does `[1, 2, 3].insert(1, 4)` return?**
- **Answer: B) None**
- **Explanation**: `insert()` modifies list in-place and returns `None`.

**39. What is the output of `dict.fromkeys([1, 2, 3], 0)`?**
- **Answer: A) {1: 0, 2: 0, 3: 0}**
- **Explanation**: Creates dictionary with keys from list, all values set to 0.

**40. What does `[1, 2, 3].remove(2)` return?**
- **Answer: B) None**
- **Explanation**: `remove()` modifies list in-place and returns `None`.

### **LESSON 07: Sets & Frozenset**

**41. What is the output of `{1, 2, 3} & {2, 3, 4} | {5, 6}`?**
- **Answer: A) {2, 3, 5, 6}**
- **Explanation**: `&` (intersection) = `{2, 3}`, then `|` (union) with `{5, 6}` = `{2, 3, 5, 6}`.

**42. What does `set([1, 1, 2, 2, 3])` create?**
- **Answer: A) {1, 2, 3}**
- **Explanation**: Sets only store unique elements, duplicates are removed.

**43. What is the result of `{1, 2, 3} - {2, 3, 4}`?**
- **Answer: A) {1}**
- **Explanation**: Set difference returns elements in first set but not in second.

**44. What does `frozenset([1, 2, 3]).add(4)` do?**
- **Answer: C) Raises AttributeError**
- **Explanation**: Frozensets are immutable, so `add()` method doesn't exist.

**45. What is the output of `{1, 2, 3} ^ {2, 3, 4}`?**
- **Answer: A) {1, 4}**
- **Explanation**: Symmetric difference returns elements in either set but not both.

**46. What does `set().add(1).add(2)` return?**
- **Answer: B) None**
- **Explanation**: `add()` returns `None`, so chaining returns `None`.

**47. What is the result of `{1, 2, 3}.issubset({1, 2, 3, 4})`?**
- **Answer: A) True**
- **Explanation**: All elements of first set are in second set.

**48. What does `{1, 2, 3}.discard(4)` do?**
- **Answer: C) Does nothing**
- **Explanation**: `discard()` removes element if present, does nothing if not found.

**49. What is the output of `len({1, 1, 2, 2, 3, 3})`?**
- **Answer: B) 3**
- **Explanation**: Sets only store unique elements, so length is 3.

**50. What does `{1, 2, 3}.pop()` return?**
- **Answer: C) Random element**
- **Explanation**: `pop()` removes and returns an arbitrary element.

### **LESSON 08: Modules & Functions**

**51. What is the output of this function?**
```python
def func(x, y=10, z=20):
    return x + y + z
print(func(5))
```
- **Answer: A) 35**
- **Explanation**: `func(5)` uses default values: `5 + 10 + 20 = 35`.

**52. What does this code print?**
```python
def outer():
    x = 1
    def inner():
        nonlocal x
        x = 2
    inner()
    return x
print(outer())
```
- **Answer: B) 2**
- **Explanation**: `nonlocal` allows inner function to modify outer variable.

**53. What is the result of `lambda x: x**2(5)`?**
- **Answer: B) Error**
- **Explanation**: Lambda function needs to be called: `(lambda x: x**2)(5)`.

**54. What does this function return?**
```python
def func():
    return 1, 2, 3
x, y = func()
```
- **Answer: B) Error**
- **Explanation**: Function returns 3 values but only 2 variables to unpack.

**55. What is the output of `print(globals() is locals())`?**
- **Answer: B) False**
- **Explanation**: `globals()` and `locals()` are different dictionaries.

**56. What does this code print?**
```python
def func(*args, **kwargs):
    return len(args) + len(kwargs)
print(func(1, 2, a=3, b=4))
```
- **Answer: A) 4**
- **Explanation**: 2 positional arguments + 2 keyword arguments = 4.

**57. What is the result of `import math; math.sqrt(-1)`?**
- **Answer: B) Error**
- **Explanation**: `math.sqrt()` doesn't handle complex numbers, raises `ValueError`.

**58. What does this function do?**
```python
def func(x):
    if x <= 1:
        return 1
    return x * func(x-1)
```
- **Answer: A) Calculates factorial**
- **Explanation**: This is the factorial function: `n * (n-1)!`.

**59. What is the output of `print(__name__)`?**
- **Answer: A) __main__**
- **Explanation**: When script is run directly, `__name__` is `"__main__"`.

**60. What does this code print?**
```python
def outer(x):
    def inner(y):
        return x + y
    return inner
f = outer(10)
print(f(5))
```
- **Answer: A) 15**
- **Explanation**: Closure captures `x=10`, then `inner(5)` returns `10 + 5 = 15`.

### **LESSON 09: Exception Handling**

**61. What is the output of this code?**
```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Error")
finally:
    print("Done")
```
- **Answer: A) Error Done**
- **Explanation**: Exception occurs, except block prints "Error", finally always executes.

**62. What does this code print?**
```python
try:
    raise ValueError("test")
except Exception as e:
    print(type(e).__name__)
```
- **Answer: A) ValueError**
- **Explanation**: `type(e).__name__` gets the exception class name.

**63. What is the result of this code?**
```python
try:
    x = int("abc")
except ValueError:
    print("ValueError")
except TypeError:
    print("TypeError")
```
- **Answer: A) ValueError**
- **Explanation**: `int("abc")` raises `ValueError`, caught by first except.

**64. What does this function return?**
```python
def func():
    try:
        return 1
    finally:
        return 2
```
- **Answer: B) 2**
- **Explanation**: Finally block executes even after return, overriding the return value.

**65. What is the output of this code?**
```python
try:
    x = [1, 2, 3][10]
except IndexError:
    print("IndexError")
except Exception:
    print("Exception")
```
- **Answer: A) IndexError**
- **Explanation**: Index 10 doesn't exist, raises `IndexError`, caught by first except.

**66. What does this code print?**
```python
try:
    raise Exception("test")
except Exception as e:
    print(str(e))
```
- **Answer: A) test**
- **Explanation**: `str(e)` converts exception to string, prints the message.

**67. What is the result of this code?**
```python
try:
    x = 1 / 0
except:
    print("Caught")
else:
    print("No error")
```
- **Answer: A) Caught**
- **Explanation**: Exception occurs, so except block executes, else block doesn't.

**68. What does this code do?**
```python
try:
    raise ValueError("test")
except ValueError:
    raise
```
- **Answer: A) Catches and re-raises the exception**
- **Explanation**: `raise` without arguments re-raises the current exception.

**69. What is the output of this code?**
```python
try:
    x = int("123")
except ValueError:
    print("Error")
else:
    print("Success")
```
- **Answer: B) Success**
- **Explanation**: No exception occurs, so else block executes.

**70. What does this code print?**
```python
try:
    x = 1 / 0
except ZeroDivisionError as e:
    print(e.__class__.__name__)
```
- **Answer: A) ZeroDivisionError**
- **Explanation**: `e.__class__.__name__` gets the exception class name.

### **MIXED TOPICS (Advanced)**

**71-100. [Same answers as questions 21-50 above]**
- **Explanation**: These questions are repeated from earlier sections for mixed topic practice.

---

## 🎯 **KEY LEARNING POINTS**

### **Critical Concepts Tested:**
1. **Type System**: Understanding `bool` as subclass of `int`
2. **Floating Point**: Precision issues with decimal arithmetic
3. **Operator Precedence**: Exponentiation associativity
4. **String Operations**: Slicing, methods, concatenation
5. **Control Flow**: Loop behavior, break/continue
6. **Data Structures**: Mutability, methods, operations
7. **Function Scope**: Local vs global, closures
8. **Exception Handling**: Try/except/finally flow
9. **List Comprehensions**: Conditional filtering
10. **Set Operations**: Mathematical set operations

### **Common Pitfalls:**
- Method return values (many return `None`)
- Floating-point precision
- Operator precedence and associativity
- Exception handling flow
- Variable scope in nested functions
- Immutable vs mutable types
- String slicing with step
- Boolean arithmetic

### **Advanced Topics:**
- Metaclasses and type system
- Closure and lexical scoping
- Exception chaining and re-raising
- Generator expressions
- Set theory operations
- Function decorators (implied)
- Context managers (implied)

---

**These questions test deep understanding of Python's behavior and edge cases. Master these concepts for advanced Python programming! 🐍✨** 