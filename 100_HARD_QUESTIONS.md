# 100 HARD Python Questions - Lessons 01-09

## 🎯 Advanced Quiz Questions for Deep Understanding

### **LESSON 01-03: Fundamentals**

**1. What is the output of `type(type(int))`?**
- A) <class 'type'>
- B) <class 'int'>
- C) <class 'object'>
- D) Error

**2. What happens when you run `print(0.1 + 0.2 == 0.3)`?**
- A) True
- B) False
- C) Error
- D) None

**3. What is the result of `bool([]) + bool({}) + bool(0)`?**
- A) 0
- B) 1
- C) 2
- D) 3

**4. What does `isinstance(True, int)` return?**
- A) True
- B) False
- C) Error
- D) None

**5. What is the output of `print(3 * '7' + 2 * '3')`?**
- A) 77733
- B) 21
- C) 7776
- D) Error

**6. What is the result of `(1, 2, 3) + (4, 5)`?**
- A) (1, 2, 3, 4, 5)
- B) (5, 7, 3)
- C) Error
- D) (1, 2, 3)(4, 5)

**7. What does `print(2 ** 3 ** 2)` output?**
- A) 64
- B) 512
- C) 256
- D) Error

**8. What is the result of `True + False + True`?**
- A) 2
- B) True
- C) Error
- D) 3

**9. What does `print(3 < 5 < 7 < 9)` return?**
- A) True
- B) False
- C) Error
- D) (True, True, True)

**10. What is the output of `print(not not True or False)`?**
- A) True
- B) False
- C) Error
- D) None

### **LESSON 04: Strings & Type Casting**

**11. What is the result of `"hello"[::-1][::-1] == "hello"`?**
- A) True
- B) False
- C) Error
- D) None

**12. What does `print("Python".replace("", "X"))` output?**
- A) XPXyXtXhXoXnX
- B) Python
- C) Error
- D) XPythonX

**13. What is the output of `int(float("3.14"))`?**
- A) 3.14
- B) 3
- C) Error
- D) 4

**14. What does `"abc".join(["1", "2", "3"])` return?**
- A) "1abc2abc3"
- B) "abc1abc2abc3"
- C) Error
- D) "123"

**15. What is the result of `str(True) + str(False)`?**
- A) "TrueFalse"
- B) "10"
- C) Error
- D) "True"

**16. What does `print("hello".upper().lower())` output?**
- A) "hello"
- B) "HELLO"
- C) Error
- D) "Hello"

**17. What is the output of `len("Python"[1:4:2])`?**
- A) 2
- B) 3
- C) 1
- D) Error

**18. What does `"Python".split("")` return?**
- A) ['P', 'y', 't', 'h', 'o', 'n']
- B) ['Python']
- C) Error
- D) []

**19. What is the result of `bool("0")`?**
- A) True
- B) False
- C) Error
- D) None

**20. What does `print("hello" * 3 + "world" * 2)` output?**
- A) "hellohellohelloworldworld"
- B) "hello3world2"
- C) Error
- D) "hello world"

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
- A) 6
- B) 10
- C) 4
- D) 0

**22. What does this code print?**
```python
for i in range(3):
    for j in range(2):
        if i == j:
            break
        print(f"{i},{j}")
```
- A) 0,0 1,0 2,0
- B) 1,0 2,0
- C) Nothing
- D) Error

**23. What is the result of `[i for i in range(5) if i % 2 == 0]`?**
- A) [0, 2, 4]
- B) [1, 3]
- C) [0, 1, 2, 3, 4]
- D) []

**24. What does this code output?**
```python
x = 5
while x > 0:
    x -= 1
    if x == 2:
        continue
    print(x, end=" ")
```
- A) 4 3 1 0
- B) 4 3 2 1 0
- C) 4 3 1
- D) Error

**25. What is the output of `sum(i for i in range(10) if i % 3 == 0)`?**
- A) 18
- B) 27
- C) 9
- D) 0

**26. What does this code print?**
```python
for i in range(3):
    pass
else:
    print("Done")
```
- A) Nothing
- B) "Done"
- C) Error
- D) 0 1 2

**27. What is the result of `any(i % 2 == 0 for i in range(1, 6))`?**
- A) True
- B) False
- C) Error
- D) [2, 4]

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
- A) "Large"
- B) "Medium"
- C) "Small"
- D) Error

**29. What is the output of `[x for x in range(5) if x % 2 == 0 and x > 0]`?**
- A) [2, 4]
- B) [0, 2, 4]
- C) [1, 3]
- D) []

**30. What does this code print?**
```python
for i in range(3):
    for j in range(2):
        print(f"{i}{j}", end=" ")
    print()
```
- A) 00 01 10 11 20 21
- B) 00 01\n10 11\n20 21
- C) 0 1 2
- D) Error

### **LESSON 06: Lists, Tuples & Dictionary**

**31. What is the output of `[1, 2, 3] * 2`?**
- A) [2, 4, 6]
- B) [1, 2, 3, 1, 2, 3]
- C) Error
- D) [1, 2, 3, 2, 4, 6]

**32. What does `dict(zip([1, 2], [3, 4]))` create?**
- A) {1: 3, 2: 4}
- B) {3: 1, 4: 2}
- C) Error
- D) [(1, 3), (2, 4)]

**33. What is the result of `[1, 2, 3].append(4)`?**
- A) [1, 2, 3, 4]
- B) None
- C) Error
- D) 4

**34. What does `{1: 'a', 2: 'b'}.get(3, 'default')` return?**
- A) 'default'
- B) None
- C) Error
- D) KeyError

**35. What is the output of `(1, 2, 3)[1:2]`?**
- A) (2,)
- B) (1, 2)
- C) 2
- D) Error

**36. What does `[1, 2, 3].extend([4, 5])` return?**
- A) [1, 2, 3, 4, 5]
- B) None
- C) Error
- D) [4, 5]

**37. What is the result of `{1: 'a', 2: 'b'}.pop(1)`?**
- A) 'a'
- B) None
- C) Error
- D) {2: 'b'}

**38. What does `[1, 2, 3].insert(1, 4)` return?**
- A) [1, 4, 2, 3]
- B) None
- C) Error
- D) [1, 2, 3, 4]

**39. What is the output of `dict.fromkeys([1, 2, 3], 0)`?**
- A) {1: 0, 2: 0, 3: 0}
- B) {0: [1, 2, 3]}
- C) Error
- D) {1: None, 2: None, 3: None}

**40. What does `[1, 2, 3].remove(2)` return?**
- A) [1, 3]
- B) None
- C) Error
- D) 2

### **LESSON 07: Sets & Frozenset**

**41. What is the output of `{1, 2, 3} & {2, 3, 4} | {5, 6}`?**
- A) {2, 3, 5, 6}
- B) {1, 2, 3, 4, 5, 6}
- C) Error
- D) {2, 3}

**42. What does `set([1, 1, 2, 2, 3])` create?**
- A) {1, 2, 3}
- B) [1, 2, 3]
- C) Error
- D) {1, 1, 2, 2, 3}

**43. What is the result of `{1, 2, 3} - {2, 3, 4}`?**
- A) {1}
- B) {4}
- C) {1, 4}
- D) Error

**44. What does `frozenset([1, 2, 3]).add(4)` do?**
- A) Adds 4 to the frozenset
- B) Returns a new frozenset
- C) Raises AttributeError
- D) Does nothing

**45. What is the output of `{1, 2, 3} ^ {2, 3, 4}`?**
- A) {1, 4}
- B) {2, 3}
- C) {1, 2, 3, 4}
- D) Error

**46. What does `set().add(1).add(2)` return?**
- A) {1, 2}
- B) None
- C) Error
- D) {1}

**47. What is the result of `{1, 2, 3}.issubset({1, 2, 3, 4})`?**
- A) True
- B) False
- C) Error
- D) None

**48. What does `{1, 2, 3}.discard(4)` do?**
- A) Raises KeyError
- B) Removes 4 if present
- C) Does nothing
- D) Error

**49. What is the output of `len({1, 1, 2, 2, 3, 3})`?**
- A) 6
- B) 3
- C) Error
- D) 1

**50. What does `{1, 2, 3}.pop()` return?**
- A) 1
- B) 3
- C) Random element
- D) Error

### **LESSON 08: Modules & Functions**

**51. What is the output of this function?**
```python
def func(x, y=10, z=20):
    return x + y + z
print(func(5))
```
- A) 35
- B) Error
- C) 15
- D) 25

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
- A) 1
- B) 2
- C) Error
- D) None

**53. What is the result of `lambda x: x**2(5)`?**
- A) 25
- B) Error
- C) 10
- D) None

**54. What does this function return?**
```python
def func():
    return 1, 2, 3
x, y = func()
```
- A) x=1, y=2
- B) Error
- C) x=(1,2,3), y=undefined
- D) x=1, y=(2,3)

**55. What is the output of `print(globals() is locals())`?**
- A) True
- B) False
- C) Error
- D) None

**56. What does this code print?**
```python
def func(*args, **kwargs):
    return len(args) + len(kwargs)
print(func(1, 2, a=3, b=4))
```
- A) 4
- B) 6
- C) Error
- D) 2

**57. What is the result of `import math; math.sqrt(-1)`?**
- A) 1j
- B) Error
- C) -1
- D) None

**58. What does this function do?**
```python
def func(x):
    if x <= 1:
        return 1
    return x * func(x-1)
```
- A) Calculates factorial
- B) Calculates fibonacci
- C) Error
- D) Infinite recursion

**59. What is the output of `print(__name__)`?**
- A) __main__
- B) Error
- C) None
- D) main

**60. What does this code print?**
```python
def outer(x):
    def inner(y):
        return x + y
    return inner
f = outer(10)
print(f(5))
```
- A) 15
- B) Error
- C) 10
- D) 5

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
- A) Error Done
- B) Done
- C) Error
- D) None

**62. What does this code print?**
```python
try:
    raise ValueError("test")
except Exception as e:
    print(type(e).__name__)
```
- A) ValueError
- B) Exception
- C) Error
- D) test

**63. What is the result of this code?**
```python
try:
    x = int("abc")
except ValueError:
    print("ValueError")
except TypeError:
    print("TypeError")
```
- A) ValueError
- B) TypeError
- C) Error
- D) Nothing

**64. What does this function return?**
```python
def func():
    try:
        return 1
    finally:
        return 2
```
- A) 1
- B) 2
- C) Error
- D) None

**65. What is the output of this code?**
```python
try:
    x = [1, 2, 3][10]
except IndexError:
    print("IndexError")
except Exception:
    print("Exception")
```
- A) IndexError
- B) Exception
- C) Error
- D) Nothing

**66. What does this code print?**
```python
try:
    raise Exception("test")
except Exception as e:
    print(str(e))
```
- A) test
- B) Exception
- C) Error
- D) None

**67. What is the result of this code?**
```python
try:
    x = 1 / 0
except:
    print("Caught")
else:
    print("No error")
```
- A) Caught
- B) No error
- C) Error
- D) Nothing

**68. What does this code do?**
```python
try:
    raise ValueError("test")
except ValueError:
    raise
```
- A) Catches and re-raises the exception
- B) Suppresses the exception
- C) Error
- D) Prints "test"

**69. What is the output of this code?**
```python
try:
    x = int("123")
except ValueError:
    print("Error")
else:
    print("Success")
```
- A) Error
- B) Success
- C) 123
- D) Nothing

**70. What does this code print?**
```python
try:
    x = 1 / 0
except ZeroDivisionError as e:
    print(e.__class__.__name__)
```
- A) ZeroDivisionError
- B) Exception
- C) Error
- D) None

### **MIXED TOPICS (Advanced)**

**71. What is the output of `[x for x in range(5) if x % 2 == 0 and x > 0]`?**
- A) [2, 4]
- B) [0, 2, 4]
- C) [1, 3]
- D) []

**72. What does `{k: v for k, v in zip([1,2], [3,4])}` create?**
- A) {1: 3, 2: 4}
- B) {3: 1, 4: 2}
- C) Error
- D) [(1,3), (2,4)]

**73. What is the result of `sum(i for i in range(10) if i % 3 == 0)`?**
- A) 18
- B) 27
- C) 9
- D) 0

**74. What does this code print?**
```python
x = [1, 2, 3]
y = x
y.append(4)
print(x)
```
- A) [1, 2, 3]
- B) [1, 2, 3, 4]
- C) Error
- D) [4, 1, 2, 3]

**75. What is the output of `bool([]) + bool({}) + bool(0)`?**
- A) 0
- B) 1
- C) 2
- D) 3

**76. What does `print(0.1 + 0.2 == 0.3)` output?**
- A) True
- B) False
- C) Error
- D) None

**77. What is the result of `(1, 2, 3) + (4, 5)`?**
- A) (1, 2, 3, 4, 5)
- B) (5, 7, 3)
- C) Error
- D) (1, 2, 3)(4, 5)

**78. What does `print(2 ** 3 ** 2)` output?**
- A) 64
- B) 512
- C) 256
- D) Error

**79. What is the output of `True + False + True`?**
- A) 2
- B) True
- C) Error
- D) 3

**80. What does `print(3 < 5 < 7 < 9)` return?**
- A) True
- B) False
- C) Error
- D) (True, True, True)

**81. What is the result of `not not True or False`?**
- A) True
- B) False
- C) Error
- D) None

**82. What does `"hello"[::-1][::-1] == "hello"` return?**
- A) True
- B) False
- C) Error
- D) None

**83. What is the output of `int(float("3.14"))`?**
- A) 3.14
- B) 3
- C) Error
- D) 4

**84. What does `"abc".join(["1", "2", "3"])` return?**
- A) "1abc2abc3"
- B) "abc1abc2abc3"
- C) Error
- D) "123"

**85. What is the result of `str(True) + str(False)`?**
- A) "TrueFalse"
- B) "10"
- C) Error
- D) "True"

**86. What does `print("hello".upper().lower())` output?**
- A) "hello"
- B) "HELLO"
- C) Error
- D) "Hello"

**87. What is the output of `len("Python"[1:4:2])`?**
- A) 2
- B) 3
- C) 1
- D) Error

**88. What does `bool("0")` return?**
- A) True
- B) False
- C) Error
- D) None

**89. What is the result of `{1, 2, 3} & {2, 3, 4} | {5, 6}`?**
- A) {2, 3, 5, 6}
- B) {1, 2, 3, 4, 5, 6}
- C) Error
- D) {2, 3}

**90. What does `set([1, 1, 2, 2, 3])` create?**
- A) {1, 2, 3}
- B) [1, 2, 3]
- C) Error
- D) {1, 1, 2, 2, 3}

**91. What is the output of `{1, 2, 3} - {2, 3, 4}`?**
- A) {1}
- B) {4}
- C) {1, 4}
- D) Error

**92. What does `frozenset([1, 2, 3]).add(4)` do?**
- A) Adds 4 to the frozenset
- B) Returns a new frozenset
- C) Raises AttributeError
- D) Does nothing

**93. What is the result of `{1, 2, 3} ^ {2, 3, 4}`?**
- A) {1, 4}
- B) {2, 3}
- C) {1, 2, 3, 4}
- D) Error

**94. What does `set().add(1).add(2)` return?**
- A) {1, 2}
- B) None
- C) Error
- D) {1}

**95. What is the output of `{1, 2, 3}.issubset({1, 2, 3, 4})`?**
- A) True
- B) False
- C) Error
- D) None

**96. What does `{1, 2, 3}.discard(4)` do?**
- A) Raises KeyError
- B) Removes 4 if present
- C) Does nothing
- D) Error

**97. What is the result of `len({1, 1, 2, 2, 3, 3})`?**
- A) 6
- B) 3
- C) Error
- D) 1

**98. What does `{1, 2, 3}.pop()` return?**
- A) 1
- B) 3
- C) Random element
- D) Error

**99. What is the output of this function?**
```python
def func(x, y=10, z=20):
    return x + y + z
print(func(5))
```
- A) 35
- B) Error
- C) 15
- D) 25

**100. What does this code print?**
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
- A) 1
- B) 2
- C) Error
- D) None

---

## 🎯 **ANSWERS WILL BE PROVIDED SEPARATELY**

These questions test deep understanding of Python concepts. Take your time to think through each one carefully! 