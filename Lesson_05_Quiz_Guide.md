# Lesson 05: Control Flow & Loops - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers conditional statements, loops, and control flow in Python programming.

## 🎯 Key Concepts to Master

### 1. Conditional Statements (if, elif, else)
- **if statement**: Execute code if condition is True
- **elif statement**: Check additional conditions if previous ones are False
- **else statement**: Execute code if all conditions are False
- **Nested conditionals**: if statements inside other if statements

### 2. Comparison Operators in Conditions
- **==**: Equal to
- **!=**: Not equal to
- **<, >, <=, >=**: Less than, greater than, etc.
- **is, is not**: Identity comparison
- **in, not in**: Membership testing

### 3. Logical Operators in Conditions
- **and**: Both conditions must be True
- **or**: At least one condition must be True
- **not**: Inverts the boolean value
- **Short-circuit evaluation**: Stops evaluating when result is determined

### 4. For Loops
- **range() function**: Generate sequence of numbers
- **Iterating over sequences**: Lists, tuples, strings
- **enumerate()**: Get both index and value
- **zip()**: Iterate over multiple sequences

### 5. While Loops
- **Condition-based looping**: Continue while condition is True
- **Infinite loops**: Loops that never terminate
- **Loop control**: break, continue, pass

### 6. Loop Control Statements
- **break**: Exit the loop immediately
- **continue**: Skip to next iteration
- **pass**: Do nothing (placeholder)

### 7. Nested Loops
- **Loops inside loops**: Multiple levels of iteration
- **Performance considerations**: O(n²) complexity

### 8. List Comprehensions (Basic)
- **Concise way to create lists**: [expression for item in iterable]
- **Conditional comprehensions**: [expression for item in iterable if condition]

## 📝 Sample MCQs with Detailed Explanations

### Question 1: Conditional Statement
**What is the output of the following code?**
```python
x = 5
if x > 3:
    print("Greater")
elif x == 3:
    print("Equal")
else:
    print("Less")
```

- A) Greater ✅
- B) Equal
- C) Less
- D) Error

**Explanation**: Since x = 5 and 5 > 3 is True, the first condition is met, so "Greater" is printed.

### Question 2: Loop Control
**Which statement is used to exit a loop early?**

- A) exit()
- B) break ✅
- C) stop()
- D) end()

**Explanation**: The break statement immediately exits the current loop.

### Question 3: Range Function
**What does `range(5)` generate?**

- A) [0, 1, 2, 3, 4, 5]
- B) [0, 1, 2, 3, 4] ✅
- C) [1, 2, 3, 4, 5]
- D) [5]

**Explanation**: range(5) generates numbers from 0 to 4 (5 numbers total), not including 5.

### Question 4: List Comprehension
**What is the output of `[x for x in range(3)]`?**

- A) [0, 1, 2] ✅
- B) [1, 2, 3]
- C) [0, 1, 2, 3]
- D) Error

**Explanation**: This creates a list with values from range(3), which are 0, 1, and 2.

### Question 5: Loop Control
**Which keyword is used to skip the current iteration in a loop?**

- A) skip
- B) continue ✅
- C) pass
- D) next

**Explanation**: continue skips the rest of the current iteration and moves to the next one.

## 🔍 Additional Practice Questions

### Question 6: Logical Operators
**What is the result of `True or False and True`?**

- A) True ✅
- B) False
- C) Error
- D) None

**Explanation**: Due to operator precedence, this is evaluated as True or (False and True) = True or False = True.

### Question 7: While Loop
**What is the output of the following code?**
```python
i = 0
while i < 3:
    print(i)
    i += 1
```

- A) 0, 1, 2 ✅
- B) 1, 2, 3
- C) 0, 1, 2, 3
- D) Infinite loop

**Explanation**: The loop prints 0, 1, 2 and stops when i becomes 3.

### Question 8: Nested Conditions
**What is the output of the following code?**
```python
x = 10
y = 5
if x > y:
    if x > 15:
        print("Very large")
    else:
        print("Medium")
else:
    print("Small")
```

- A) Very large
- B) Medium ✅
- C) Small
- D) Error

**Explanation**: x > y is True, but x > 15 is False, so "Medium" is printed.

### Question 9: For Loop with Range
**How many times does this loop execute?**
```python
for i in range(1, 5):
    print(i)
```

- A) 3 times
- B) 4 times ✅
- C) 5 times
- D) 6 times

**Explanation**: range(1, 5) generates 1, 2, 3, 4, so the loop executes 4 times.

### Question 10: Break Statement
**What is the output of the following code?**
```python
for i in range(5):
    if i == 3:
        break
    print(i)
```

- A) 0, 1, 2, 3
- B) 0, 1, 2 ✅
- C) 0, 1, 2, 3, 4
- D) 3, 4

**Explanation**: The loop prints 0, 1, 2, then breaks when i equals 3.

## 📋 Important Facts to Remember

### Conditional Statement Rules
1. **if**: First condition to check
2. **elif**: Additional conditions (can have multiple)
3. **else**: Default case (optional, only one allowed)
4. **Indentation**: Must be consistent (usually 4 spaces)

### Loop Types and Usage
1. **for**: When you know the number of iterations
2. **while**: When you don't know the number of iterations
3. **range()**: Generate sequences for for loops
4. **enumerate()**: Get index and value together

### Control Flow Keywords
1. **break**: Exit loop immediately
2. **continue**: Skip to next iteration
3. **pass**: Do nothing (placeholder)
4. **return**: Exit function (not just loop)

### List Comprehension Syntax
1. **Basic**: [expression for item in iterable]
2. **Conditional**: [expression for item in iterable if condition]
3. **Nested**: [expression for item1 in iterable1 for item2 in iterable2]

## 🎯 Study Tips for This Lesson

1. **Practice Conditions**: Write various if-elif-else structures
2. **Test Loops**: Experiment with for and while loops
3. **Use Control Statements**: Practice break, continue, and pass
4. **Understand Range**: Know how range() works with different parameters
5. **Master Comprehensions**: Practice list comprehensions

## 🔗 Related Resources

- [Python Control Flow](https://docs.python.org/3/tutorial/controlflow.html)
- [Python Loops](https://docs.python.org/3/tutorial/controlflow.html#for-statements)
- [Python List Comprehensions](https://docs.python.org/3/tutorial/datastructures.html#list-comprehensions)

## ✅ Self-Assessment Checklist

- [ ] I can write if-elif-else statements
- [ ] I understand logical operators (and, or, not)
- [ ] I can use for loops with range()
- [ ] I can use while loops
- [ ] I know how to use break and continue
- [ ] I understand nested loops
- [ ] I can write basic list comprehensions
- [ ] I know the difference between for and while loops
- [ ] I can use comparison operators in conditions
- [ ] I understand short-circuit evaluation

## 🧮 Practice Exercises

### Exercise 1: Conditional Statements
```python
# Test different conditions
x = 10
y = 5

if x > y:
    print("x is greater than y")
elif x == y:
    print("x equals y")
else:
    print("x is less than y")

# Test logical operators
if x > 5 and y < 10:
    print("Both conditions are True")
```

### Exercise 2: For Loops
```python
# Basic for loop
for i in range(5):
    print(i)  # 0, 1, 2, 3, 4

# For loop with range parameters
for i in range(1, 6):
    print(i)  # 1, 2, 3, 4, 5

# For loop with step
for i in range(0, 10, 2):
    print(i)  # 0, 2, 4, 6, 8
```

### Exercise 3: While Loops
```python
# Basic while loop
i = 0
while i < 3:
    print(i)
    i += 1

# While loop with break
i = 0
while True:
    if i >= 3:
        break
    print(i)
    i += 1
```

### Exercise 4: Loop Control
```python
# Using continue
for i in range(5):
    if i == 2:
        continue
    print(i)  # 0, 1, 3, 4

# Using break
for i in range(5):
    if i == 3:
        break
    print(i)  # 0, 1, 2
```

### Exercise 5: List Comprehensions
```python
# Basic comprehension
squares = [x**2 for x in range(5)]
print(squares)  # [0, 1, 4, 9, 16]

# Conditional comprehension
even_squares = [x**2 for x in range(10) if x % 2 == 0]
print(even_squares)  # [0, 4, 16, 36, 64]
```

### Exercise 6: Nested Loops
```python
# Nested for loops
for i in range(3):
    for j in range(2):
        print(f"i={i}, j={j}")

# Output:
# i=0, j=0
# i=0, j=1
# i=1, j=0
# i=1, j=1
# i=2, j=0
# i=2, j=1
```

**Remember**: Control flow and loops are fundamental to programming. Master these concepts as they form the backbone of program logic and iteration! 