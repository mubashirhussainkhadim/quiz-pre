# 100 LOGICAL Python MCQs with Answers

## 🧠 Logical Reasoning & Problem Solving

### **Questions 1-25: Fundamental Logic**

**1. What is the output of this code?**
```python
x = 5
y = 3
z = x if x > y else y
print(z)
```
A) 3  
B) 5  
C) 8  
D) Error

**Answer: B) 5**  
**Explanation**: Conditional expression: if x > y (5 > 3 is True), so z = x = 5.

**2. What does this code print?**
```python
numbers = [1, 2, 3, 4, 5]
result = [n * 2 for n in numbers if n % 2 == 0]
print(result)
```
A) [2, 4, 6, 8, 10]  
B) [4, 8]  
C) [2, 4]  
D) [1, 3, 5]

**Answer: B) [4, 8]**  
**Explanation**: List comprehension doubles even numbers only: 2*2=4, 4*2=8.

**3. What is the result of this logical operation?**
```python
a = True
b = False
c = True
result = (a and b) or (not c)
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: B) False**  
**Explanation**: (True and False) or (not True) = False or False = False.

**4. What does this function return?**
```python
def mystery(x, y):
    if x == 0:
        return y
    return mystery(x - 1, y + 1)
print(mystery(3, 5))
```
A) 8  
B) 5  
C) 3  
D) Error

**Answer: A) 8**  
**Explanation**: Recursive function adds x to y: 3 + 5 = 8.

**5. What is the output of this code?**
```python
data = [1, 2, 3, 4, 5]
filtered = list(filter(lambda x: x > 2, data))
print(len(filtered))
```
A) 2  
B) 3  
C) 5  
D) Error

**Answer: B) 3**  
**Explanation**: Filter keeps numbers > 2: [3, 4, 5], length = 3.

**6. What does this code print?**
```python
def func(x):
    return x + 1 if x > 0 else x - 1
print(func(0))
```
A) 0  
B) -1  
C) 1  
D) Error

**Answer: B) -1**  
**Explanation**: x = 0, so condition is False, returns x - 1 = 0 - 1 = -1.

**7. What is the result of this operation?**
```python
items = ['a', 'b', 'c']
result = items[1:] + items[:1]
print(result)
```
A) ['b', 'c', 'a']  
B) ['a', 'b', 'c']  
C) ['b', 'a']  
D) Error

**Answer: A) ['b', 'c', 'a']**  
**Explanation**: items[1:] = ['b', 'c'], items[:1] = ['a'], concatenated = ['b', 'c', 'a'].

**8. What does this code output?**
```python
x = 10
y = 20
x, y = y, x
print(x, y)
```
A) 10 20  
B) 20 10  
C) 20 20  
D) Error

**Answer: B) 20 10**  
**Explanation**: Tuple unpacking swaps values: x becomes 20, y becomes 10.

**9. What is the output of this logical test?**
```python
test = [1, 2, 3] and [4, 5, 6]
print(test)
```
A) [1, 2, 3]  
B) [4, 5, 6]  
C) True  
D) False

**Answer: B) [4, 5, 6]**  
**Explanation**: `and` returns the last truthy value, which is [4, 5, 6].

**10. What does this function calculate?**
```python
def calculate(n):
    if n <= 1:
        return n
    return calculate(n-1) + calculate(n-2)
print(calculate(5))
```
A) 5  
B) 8  
C) 13  
D) 21

**Answer: A) 5**  
**Explanation**: This is the Fibonacci sequence: 0,1,1,2,3,5. calculate(5) = 5.

**11. What is the result of this operation?**
```python
data = {'a': 1, 'b': 2, 'c': 3}
result = sum(data.values()) if len(data) > 2 else 0
print(result)
```
A) 0  
B) 6  
C) 3  
D) Error

**Answer: B) 6**  
**Explanation**: len(data) = 3 > 2, so sum of values: 1 + 2 + 3 = 6.

**12. What does this code print?**
```python
numbers = [1, 2, 3, 4, 5]
result = [x for x in numbers if x % 2 == 0 and x > 2]
print(result)
```
A) [2, 4]  
B) [4]  
C) [2]  
D) []

**Answer: B) [4]**  
**Explanation**: Only 4 is even and > 2.

**13. What is the output of this logical expression?**
```python
x = 5
y = 10
result = x < y < 15
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: Chained comparison: 5 < 10 < 15 is True.

**14. What does this function return?**
```python
def process(data):
    return [x * 2 for x in data if x > 0]
print(process([-1, 0, 1, 2, 3]))
```
A) [2, 4, 6]  
B) [1, 2, 3]  
C) [-2, 0, 2, 4, 6]  
D) []

**Answer: A) [2, 4, 6]**  
**Explanation**: Filters positive numbers, then doubles them: 1*2=2, 2*2=4, 3*2=6.

**15. What is the result of this operation?**
```python
text = "hello"
result = text[::-1] == text
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: B) False**  
**Explanation**: "hello"[::-1] = "olleh", "olleh" != "hello".

**16. What does this code output?**
```python
def mystery(x):
    return x if x % 2 == 0 else x + 1
print(mystery(7))
```
A) 7  
B) 8  
C) 6  
D) Error

**Answer: B) 8**  
**Explanation**: 7 is odd, so returns 7 + 1 = 8.

**17. What is the output of this logical test?**
```python
test = [] or {} or [1, 2, 3]
print(test)
```
A) []  
B) {}  
C) [1, 2, 3]  
D) True

**Answer: C) [1, 2, 3]**  
**Explanation**: `or` returns the first truthy value, which is [1, 2, 3].

**18. What does this function calculate?**
```python
def calculate(n):
    return n * (n + 1) // 2
print(calculate(4))
```
A) 6  
B) 10  
C) 8  
D) 12

**Answer: B) 10**  
**Explanation**: Sum of first n natural numbers: 4 * 5 // 2 = 20 // 2 = 10.

**19. What is the result of this operation?**
```python
data = [1, 2, 3, 4, 5]
result = data[::2] + data[1::2]
print(result)
```
A) [1, 3, 5, 2, 4]  
B) [1, 2, 3, 4, 5]  
C) [2, 4, 1, 3, 5]  
D) Error

**Answer: A) [1, 3, 5, 2, 4]**  
**Explanation**: data[::2] = [1, 3, 5], data[1::2] = [2, 4], concatenated.

**20. What does this code print?**
```python
x = 15
y = 3
result = x // y if x % y == 0 else x % y
print(result)
```
A) 5  
B) 0  
C) 3  
D) 15

**Answer: A) 5**  
**Explanation**: 15 % 3 = 0, so returns 15 // 3 = 5.

**21. What is the output of this logical expression?**
```python
a = True
b = False
result = (a or b) and (not b)
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: (True or False) and (not False) = True and True = True.

**22. What does this function return?**
```python
def process(items):
    return [item for item in items if item not in [2, 4, 6]]
print(process([1, 2, 3, 4, 5, 6, 7]))
```
A) [1, 3, 5, 7]  
B) [2, 4, 6]  
C) [1, 2, 3, 4, 5, 6, 7]  
D) []

**Answer: A) [1, 3, 5, 7]**  
**Explanation**: Filters out 2, 4, 6, keeping 1, 3, 5, 7.

**23. What is the result of this operation?**
```python
text = "python"
result = len(text) % 2 == 0
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: len("python") = 6, 6 % 2 = 0, so True.

**24. What does this code output?**
```python
def mystery(x, y):
    return x if x > y else y if x < y else x + y
print(mystery(3, 3))
```
A) 3  
B) 6  
C) 0  
D) Error

**Answer: B) 6**  
**Explanation**: x == y, so returns x + y = 3 + 3 = 6.

**25. What is the output of this logical test?**
```python
test = 0 and 1 or 2
print(test)
```
A) 0  
B) 1  
C) 2  
D) True

**Answer: C) 2**  
**Explanation**: 0 and 1 = 0, then 0 or 2 = 2.

---

## 🎯 **Key Logical Concepts Tested:**

1. **Conditional Expressions**: Ternary operators and their logic
2. **List Comprehensions**: Filtering and transforming data
3. **Logical Operators**: and, or, not precedence and short-circuiting
4. **Recursion**: Understanding recursive function calls
5. **Lambda Functions**: Anonymous function behavior
6. **String Operations**: Slicing and manipulation
7. **Data Structure Operations**: List, dict, set operations
8. **Variable Swapping**: Tuple unpacking
9. **Mathematical Logic**: Number theory and calculations
10. **Control Flow**: Complex conditional logic

---

**Continue with next batch...**

### **Questions 26-50: Advanced Logic & Data Structures**

**26. What is the output of this code?**
```python
def process(data):
    return {k: v * 2 for k, v in data.items() if v > 0}
result = process({'a': 1, 'b': -2, 'c': 3, 'd': 0})
print(len(result))
```
A) 1  
B) 2  
C) 3  
D) 4

**Answer: B) 2**  
**Explanation**: Only 'a' and 'c' have positive values, so 2 items in result.

**27. What does this code print?**
```python
numbers = [1, 2, 3, 4, 5]
result = [x for x in numbers if x % 2 == 0 or x % 3 == 0]
print(len(result))
```
A) 2  
B) 3  
C) 4  
D) 5

**Answer: C) 4**  
**Explanation**: Numbers divisible by 2 or 3: 2, 3, 4 (2,4 are even; 3 is divisible by 3).

**28. What is the result of this operation?**
```python
text = "programming"
result = text[::2] + text[1::2]
print(result == text)
```
A) True  
B) False  
C) Error  
D) None

**Answer: B) False**  
**Explanation**: text[::2] = "pormig", text[1::2] = "rgamn", concatenated ≠ original.

**29. What does this function return?**
```python
def mystery(x, y):
    if x == 0:
        return 0
    return y + mystery(x - 1, y)
print(mystery(3, 4))
```
A) 7  
B) 12  
C) 4  
D) Error

**Answer: B) 12**  
**Explanation**: Recursive multiplication: 4 + 4 + 4 = 12 (3 times).

**30. What is the output of this logical test?**
```python
data = [1, 2, 3, 4, 5]
result = all(x > 0 for x in data) and any(x % 2 == 0 for x in data)
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: All numbers > 0 (True) and any even numbers exist (True), so True.

**31. What does this code print?**
```python
def func(x):
    return x if isinstance(x, int) else len(x)
print(func("hello"))
```
A) "hello"  
B) 5  
C) Error  
D) None

**Answer: B) 5**  
**Explanation**: "hello" is not int, so returns len("hello") = 5.

**32. What is the result of this operation?**
```python
items = ['a', 'b', 'c', 'd']
result = items[1:3] + items[0:1]
print(result)
```
A) ['b', 'c', 'a']  
B) ['a', 'b', 'c']  
C) ['b', 'c', 'd']  
D) Error

**Answer: A) ['b', 'c', 'a']**  
**Explanation**: items[1:3] = ['b', 'c'], items[0:1] = ['a'], concatenated.

**33. What does this function calculate?**
```python
def calculate(n):
    return sum(range(1, n + 1))
print(calculate(5))
```
A) 10  
B) 15  
C) 20  
D) 25

**Answer: B) 15**  
**Explanation**: Sum of 1 to 5: 1 + 2 + 3 + 4 + 5 = 15.

**34. What is the output of this logical expression?**
```python
x = 10
y = 5
result = x > y and x % y == 0
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: 10 > 5 (True) and 10 % 5 == 0 (True), so True.

**35. What does this code output?**
```python
data = {'a': 1, 'b': 2, 'c': 3}
result = [k for k, v in data.items() if v % 2 == 1]
print(result)
```
A) ['a', 'c']  
B) ['b']  
C) [1, 3]  
D) []

**Answer: A) ['a', 'c']**  
**Explanation**: Keys with odd values: 'a' (1), 'c' (3).

**36. What is the result of this operation?**
```python
text = "python"
result = text[1:4] == text[-4:-1]
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: text[1:4] = "yth", text[-4:-1] = "yth", so True.

**37. What does this function return?**
```python
def process(items):
    return [x for x in items if x not in [1, 3, 5]]
print(process([1, 2, 3, 4, 5, 6]))
```
A) [2, 4, 6]  
B) [1, 3, 5]  
C) [1, 2, 3, 4, 5, 6]  
D) []

**Answer: A) [2, 4, 6]**  
**Explanation**: Filters out 1, 3, 5, keeping 2, 4, 6.

**38. What is the output of this logical test?**
```python
test = 1 and 2 and 3 or 4
print(test)
```
A) 1  
B) 2  
C) 3  
D) 4

**Answer: C) 3**  
**Explanation**: 1 and 2 and 3 = 3, then 3 or 4 = 3.

**39. What does this code print?**
```python
def mystery(x):
    return x * 2 if x > 0 else abs(x)
print(mystery(-3))
```
A) -6  
B) 3  
C) 6  
D) Error

**Answer: B) 3**  
**Explanation**: x = -3 < 0, so returns abs(-3) = 3.

**40. What is the result of this operation?**
```python
data = [1, 2, 3, 4, 5]
result = [x for x in data if x % 2 == 0 and x < 5]
print(result)
```
A) [2, 4]  
B) [2]  
C) [4]  
D) []

**Answer: A) [2, 4]**  
**Explanation**: Even numbers < 5: 2, 4.

**41. What does this function calculate?**
```python
def calculate(n):
    if n <= 1:
        return 1
    return n * calculate(n - 1)
print(calculate(4))
```
A) 10  
B) 24  
C) 16  
D) 8

**Answer: B) 24**  
**Explanation**: Factorial: 4 * 3 * 2 * 1 = 24.

**42. What is the output of this logical expression?**
```python
x = 15
y = 3
result = x // y == 5 and x % y == 0
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: 15 // 3 == 5 (True) and 15 % 3 == 0 (True), so True.

**43. What does this code output?**
```python
text = "hello world"
result = len(text.split()) > 1
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: text.split() = ['hello', 'world'], len = 2 > 1, so True.

**44. What is the result of this operation?**
```python
data = {'a': 1, 'b': 2, 'c': 3}
result = sum(v for v in data.values() if v % 2 == 0)
print(result)
```
A) 2  
B) 4  
C) 6  
D) 0

**Answer: A) 2**  
**Explanation**: Sum of even values: only 2 is even, so sum = 2.

**45. What does this function return?**
```python
def process(items):
    return [x for x in items if isinstance(x, int) and x > 0]
print(process([1, -2, 3, "hello", 4]))
```
A) [1, 3, 4]  
B) [1, -2, 3, 4]  
C) [1, 2, 3, 4]  
D) []

**Answer: A) [1, 3, 4]**  
**Explanation**: Positive integers only: 1, 3, 4.

**46. What is the output of this logical test?**
```python
test = [] or 0 or "hello"
print(test)
```
A) []  
B) 0  
C) "hello"  
D) True

**Answer: C) "hello"**  
**Explanation**: `or` returns first truthy value: "hello".

**47. What does this code print?**
```python
def mystery(x, y):
    return x if x == y else mystery(x - 1, y) if x > y else mystery(x + 1, y)
print(mystery(3, 5))
```
A) 3  
B) 5  
C) 4  
D) Error

**Answer: B) 5**  
**Explanation**: Recursively increments x until x == y: 3→4→5.

**48. What is the result of this operation?**
```python
data = [1, 2, 3, 4, 5]
result = [x for x in data if x % 2 == 1 and x < 4]
print(result)
```
A) [1, 3]  
B) [1, 3, 5]  
C) [1]  
D) []

**Answer: A) [1, 3]**  
**Explanation**: Odd numbers < 4: 1, 3.

**49. What does this function calculate?**
```python
def calculate(n):
    return sum(range(0, n + 1, 2))
print(calculate(6))
```
A) 6  
B) 12  
C) 18  
D) 24

**Answer: B) 12**  
**Explanation**: Sum of even numbers 0 to 6: 0 + 2 + 4 + 6 = 12.

**50. What is the output of this logical expression?**
```python
x = 20
y = 4
result = x % y == 0 and x // y > 3
print(result)
```
A) True  
B) False  
C) Error  
D) None

**Answer: A) True**  
**Explanation**: 20 % 4 == 0 (True) and 20 // 4 > 3 (5 > 3 is True), so True. 