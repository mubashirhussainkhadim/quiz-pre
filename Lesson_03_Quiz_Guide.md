# Lesson 03: Operators, Keywords & Variables - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers Python operators, keywords, variable naming, assignment, and scope.

## 🎯 Key Concepts to Master

### 1. Arithmetic Operators
- **+**: Addition
- **-**: Subtraction
- **\***: Multiplication
- **/**: Division (returns float)
- **//**: Floor division (returns int)
- **%**: Modulo (remainder)
- **\*\***: Exponentiation

### 2. Comparison Operators
- **==**: Equal to
- **!=**: Not equal to
- **<**: Less than
- **>**: Greater than
- **<=**: Less than or equal to
- **>=**: Greater than or equal to

### 3. Logical Operators
- **and**: Logical AND
- **or**: Logical OR
- **not**: Logical NOT
- **Short-circuit evaluation**

### 4. Assignment Operators
- **=**: Simple assignment
- **+=**: Add and assign
- **-=**: Subtract and assign
- **\*=**: Multiply and assign
- **/=**: Divide and assign
- **//=**: Floor divide and assign
- **%=**: Modulo and assign
- **\*\*=**: Exponentiate and assign

### 5. Bitwise Operators
- **&**: Bitwise AND
- **|**: Bitwise OR
- **^**: Bitwise XOR
- **~**: Bitwise NOT
- **<<**: Left shift
- **>>**: Right shift

### 6. Python Keywords
- **Control flow**: if, elif, else, for, while, break, continue
- **Function**: def, return, lambda
- **Class**: class, self
- **Import**: import, from, as
- **Exception**: try, except, finally, raise
- **Logical**: and, or, not, is, in
- **Others**: True, False, None, del, global, nonlocal

### 7. Variable Naming Rules
- Must start with letter or underscore
- Can contain letters, digits, underscores
- Case sensitive
- Cannot use keywords
- Descriptive names recommended

### 8. Variable Scope
- **Local scope**: Variables defined inside functions
- **Global scope**: Variables defined at module level
- **Enclosing scope**: Variables in nested functions
- **Built-in scope**: Python's built-in names

## 📝 Sample MCQs with Detailed Explanations

### Question 1: Floor Division
**What is the output of `5 // 2`?**

- A) 2.5
- B) 2 ✅
- C) 2.0
- D) Error

**Explanation**: The // operator performs floor division, which returns the largest integer less than or equal to the division result. 5 ÷ 2 = 2.5, so floor division returns 2.

### Question 2: Exponentiation
**Which operator is used for exponentiation?**

- A) ^
- B) ** ✅
- C) pow
- D) exp

**Explanation**: The ** operator is used for exponentiation in Python. For example, 2**3 = 8.

### Question 3: Logical AND
**What is the result of `True and False`?**

- A) True
- B) False ✅
- C) None
- D) Error

**Explanation**: The logical AND operator returns True only if both operands are True. Since False is one of the operands, the result is False.

### Question 4: Variable Naming
**Which of the following is a valid variable name?**

- A) 2variable
- B) my-variable
- C) my_variable ✅
- D) class

**Explanation**: Variable names must start with a letter or underscore, can contain letters, digits, and underscores, and cannot be Python keywords. "class" is a keyword, "2variable" starts with a digit, and "my-variable" contains a hyphen.

### Question 5: Identity Operator
**What does the `is` operator check?**

- A) Value equality
- B) Identity (same object) ✅
- C) Type equality
- D) Size equality

**Explanation**: The `is` operator checks if two variables point to the same object in memory, not if they have the same value.

## 🔍 Additional Practice Questions

### Question 6: Modulo Operator
**What is the result of `17 % 5`?**

- A) 3.4
- B) 2 ✅
- C) 3
- D) Error

**Explanation**: The modulo operator returns the remainder of division. 17 ÷ 5 = 3 with remainder 2.

### Question 7: Assignment Operator
**What is the value of x after `x = 5; x += 3`?**

- A) 5
- B) 8 ✅
- C) 15
- D) Error

**Explanation**: x += 3 is equivalent to x = x + 3, so x becomes 5 + 3 = 8.

### Question 8: Comparison Chain
**What is the result of `3 < 5 < 7`?**

- A) True ✅
- B) False
- C) Error
- D) None

**Explanation**: Python supports chained comparisons. This is equivalent to (3 < 5) and (5 < 7), which is True.

### Question 9: Bitwise Operation
**What is the output of `5 & 3`?**

- A) 8
- B) 1 ✅
- C) 7
- D) 2

**Explanation**: 5 in binary is 101, 3 is 011. Bitwise AND: 101 & 011 = 001 = 1.

### Question 10: Variable Scope
**What is the output of the following code?**
```python
x = 10
def func():
    x = 20
    print(x)
func()
print(x)
```

- A) 20, 20
- B) 20, 10 ✅
- C) 10, 20
- D) 10, 10

**Explanation**: The x inside the function is a local variable, while the x outside is global. They are different variables.

## 📋 Important Facts to Remember

### Operator Precedence (from highest to lowest)
1. **()**: Parentheses
2. **\*\***: Exponentiation
3. **+x, -x, ~x**: Unary operators
4. **\*, /, //, %**: Multiplication, division, floor division, modulo
5. **+, -**: Addition, subtraction
6. **<<, >>**: Bitwise shifts
7. **&**: Bitwise AND
8. **^**: Bitwise XOR
9. **|**: Bitwise OR
10. **==, !=, <, >, <=, >=**: Comparisons
11. **is, is not**: Identity
12. **in, not in**: Membership
13. **not**: Logical NOT
14. **and**: Logical AND
15. **or**: Logical OR

### Variable Naming Conventions
1. **snake_case**: For variables and functions
2. **UPPER_CASE**: For constants
3. **PascalCase**: For classes
4. **Descriptive names**: Avoid single letters except for counters

### Keywords to Remember
- **Control**: if, elif, else, for, while, break, continue, pass
- **Function**: def, return, lambda
- **Import**: import, from, as
- **Exception**: try, except, finally, raise
- **Scope**: global, nonlocal
- **Logic**: and, or, not, is, in

## 🎯 Study Tips for This Lesson

1. **Practice Operators**: Write code to test each operator
2. **Understand Precedence**: Know which operations happen first
3. **Test Variable Scope**: Experiment with local and global variables
4. **Learn Keywords**: Memorize common Python keywords
5. **Follow Naming Conventions**: Use descriptive variable names

## 🔗 Related Resources

- [Python Operators](https://docs.python.org/3/reference/expressions.html#operator-precedence)
- [Python Keywords](https://docs.python.org/3/reference/lexical_analysis.html#keywords)
- [Python Variable Scope](https://docs.python.org/3/tutorial/classes.html#python-scopes-and-namespaces)

## ✅ Self-Assessment Checklist

- [ ] I can use all arithmetic operators correctly
- [ ] I understand comparison and logical operators
- [ ] I know how assignment operators work
- [ ] I can perform bitwise operations
- [ ] I understand operator precedence
- [ ] I know Python keywords and their usage
- [ ] I can create valid variable names
- [ ] I understand variable scope (local vs global)
- [ ] I can use the identity and membership operators
- [ ] I follow Python naming conventions

## 🧮 Practice Exercises

### Exercise 1: Arithmetic Operations
```python
# Test arithmetic operators
print(10 + 5)    # 15
print(10 - 5)    # 5
print(10 * 5)    # 50
print(10 / 5)    # 2.0
print(10 // 3)   # 3
print(10 % 3)    # 1
print(2 ** 3)    # 8
```

### Exercise 2: Comparison and Logical
```python
# Test comparison and logical operators
print(5 > 3)           # True
print(5 == 5)          # True
print(True and False)  # False
print(True or False)   # True
print(not True)        # False
```

### Exercise 3: Assignment Operators
```python
# Test assignment operators
x = 10
x += 5    # x = 15
x *= 2    # x = 30
x //= 3   # x = 10
print(x)  # 10
```

### Exercise 4: Variable Scope
```python
# Test variable scope
global_var = "I'm global"

def test_scope():
    local_var = "I'm local"
    print(local_var)
    print(global_var)

test_scope()
# print(local_var)  # This would cause an error
```

**Remember**: Operators and variables are the building blocks of Python programming. Master these concepts as they are used in every Python program! 