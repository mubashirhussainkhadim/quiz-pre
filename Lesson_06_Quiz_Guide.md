# Lesson 06: Lists, Tuples & Dictionary - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers Python's sequence data types: lists (mutable), tuples (immutable), and dictionaries (key-value pairs).

## 🎯 Key Concepts to Master

### 1. Lists
- **Mutable sequence**: Can be modified after creation
- **Heterogeneous**: Can contain different data types
- **Indexed**: Zero-based indexing
- **Methods**: append(), extend(), insert(), remove(), pop(), clear()
- **Slicing**: [start:end:step]
- **Concatenation**: + operator
- **Repetition**: * operator

### 2. Tuples
- **Immutable sequence**: Cannot be modified after creation
- **Heterogeneous**: Can contain different data types
- **Indexed**: Zero-based indexing
- **Methods**: count(), index()
- **Slicing**: [start:end:step]
- **Packing/Unpacking**: Multiple assignment
- **Single element**: Need trailing comma

### 3. Dictionaries
- **Key-value pairs**: Unordered collection
- **Mutable**: Can be modified after creation
- **Keys**: Must be immutable (strings, numbers, tuples)
- **Values**: Can be any data type
- **Methods**: keys(), values(), items(), get(), update(), pop()
- **Access**: dict[key] or dict.get(key)

### 4. Common Operations
- **Length**: len() function
- **Membership**: in operator
- **Iteration**: for loops
- **Nesting**: Lists/tuples/dicts inside each other

## 📝 Sample MCQs with Detailed Explanations

### Question 1: Mutability
**Which of the following is mutable?**

- A) Tuple
- B) List ✅
- C) String
- D) Integer

**Explanation**: Lists are mutable - they can be modified after creation. Tuples, strings, and integers are immutable.

### Question 2: List Concatenation
**What is the output of `[1, 2, 3] + [4, 5]`?**

- A) [1, 2, 3, 4, 5] ✅
- B) [5, 7, 3]
- C) Error
- D) [1, 2, 3][4, 5]

**Explanation**: The + operator concatenates lists, creating a new list with all elements.

### Question 3: Dictionary Access
**How do you access a value in a dictionary?**

- A) dict.value(key)
- B) dict[key] ✅
- C) dict.get(key)
- D) Both B and C

**Explanation**: Both dict[key] and dict.get(key) can access values, but dict[key] raises KeyError if key doesn't exist.

### Question 4: Tuple Indexing
**What is the result of `(1, 2, 3)[1]`?**

- A) 1
- B) 2 ✅
- C) 3
- D) Error

**Explanation**: Tuple indexing starts at 0, so index 1 refers to the second element (2).

### Question 5: List Method
**Which method adds an element to the end of a list?**

- A) add()
- B) append() ✅
- C) insert()
- D) extend()

**Explanation**: append() adds a single element to the end of a list.

## 🔍 Additional Practice Questions

### Question 6: List Slicing
**What is the output of `[1, 2, 3, 4, 5][1:4]`?**

- A) [1, 2, 3]
- B) [2, 3, 4] ✅
- C) [1, 2, 3, 4]
- D) [2, 3, 4, 5]

**Explanation**: Slicing [1:4] includes elements at indices 1, 2, and 3 (but not 4).

### Question 7: Dictionary Keys
**Which of the following can be a dictionary key?**

- A) List
- B) Tuple ✅
- C) Dictionary
- D) Set

**Explanation**: Dictionary keys must be immutable. Tuples are immutable, while lists, dictionaries, and sets are mutable.

### Question 8: List Method
**What does `[1, 2, 3].pop()` return?**

- A) 1
- B) 2
- C) 3 ✅
- D) [1, 2]

**Explanation**: pop() without arguments removes and returns the last element (3).

### Question 9: Tuple Creation
**How do you create a tuple with one element?**

- A) (1)
- B) (1,) ✅
- C) tuple(1)
- D) [1]

**Explanation**: A trailing comma is needed to distinguish a single-element tuple from a parenthesized expression.

### Question 10: Dictionary Method
**What does `dict.get(key, default)` do?**

- A) Returns the value for key, or raises KeyError
- B) Returns the value for key, or default if key doesn't exist ✅
- C) Adds key with default value if key doesn't exist
- D) Removes key and returns its value

**Explanation**: get() returns the value for the key if it exists, otherwise returns the default value.

## 📋 Important Facts to Remember

### List Characteristics
1. **Mutable**: Can be modified after creation
2. **Ordered**: Elements maintain their order
3. **Indexed**: Access elements by position
4. **Heterogeneous**: Can contain different types
5. **Dynamic**: Can grow or shrink

### Tuple Characteristics
1. **Immutable**: Cannot be modified after creation
2. **Ordered**: Elements maintain their order
3. **Indexed**: Access elements by position
4. **Heterogeneous**: Can contain different types
5. **Faster**: Slightly faster than lists

### Dictionary Characteristics
1. **Mutable**: Can be modified after creation
2. **Unordered**: Order not guaranteed (Python 3.7+ maintains insertion order)
3. **Key-based**: Access by keys, not position
4. **Unique keys**: Each key can appear only once
5. **Heterogeneous values**: Values can be any type

### Common Methods
1. **List**: append(), extend(), insert(), remove(), pop(), clear()
2. **Tuple**: count(), index()
3. **Dictionary**: keys(), values(), items(), get(), update(), pop()

## 🎯 Study Tips for This Lesson

1. **Practice List Operations**: Try all list methods
2. **Understand Mutability**: Know which types are mutable/immutable
3. **Master Dictionary Access**: Use both [] and get() methods
4. **Test Slicing**: Practice with different slice parameters
5. **Learn Nesting**: Create nested data structures

## 🔗 Related Resources

- [Python Lists](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)
- [Python Tuples](https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences)
- [Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)

## ✅ Self-Assessment Checklist

- [ ] I can create and manipulate lists
- [ ] I understand list methods (append, extend, insert, etc.)
- [ ] I can create and use tuples
- [ ] I understand tuple immutability
- [ ] I can create and access dictionaries
- [ ] I know dictionary methods (keys, values, items, get)
- [ ] I understand the difference between mutable and immutable types
- [ ] I can use slicing on lists and tuples
- [ ] I can iterate over lists, tuples, and dictionaries
- [ ] I understand nested data structures

## 🧮 Practice Exercises

### Exercise 1: List Operations
```python
# Create and manipulate lists
my_list = [1, 2, 3]
my_list.append(4)          # [1, 2, 3, 4]
my_list.extend([5, 6])     # [1, 2, 3, 4, 5, 6]
my_list.insert(0, 0)       # [0, 1, 2, 3, 4, 5, 6]
my_list.remove(3)          # [0, 1, 2, 4, 5, 6]
popped = my_list.pop()     # popped = 6, list = [0, 1, 2, 4, 5]
print(my_list)
```

### Exercise 2: Tuple Operations
```python
# Create and use tuples
my_tuple = (1, 2, 3, 2, 4)
print(len(my_tuple))       # 5
print(my_tuple.count(2))   # 2
print(my_tuple.index(2))   # 1

# Tuple unpacking
a, b, c = (1, 2, 3)
print(a, b, c)             # 1 2 3

# Single element tuple
single = (1,)
print(type(single))        # <class 'tuple'>
```

### Exercise 3: Dictionary Operations
```python
# Create and manipulate dictionaries
my_dict = {'name': 'Alice', 'age': 25}
print(my_dict['name'])     # Alice
print(my_dict.get('age'))  # 25
print(my_dict.get('city', 'Unknown'))  # Unknown

# Dictionary methods
print(my_dict.keys())      # dict_keys(['name', 'age'])
print(my_dict.values())    # dict_values(['Alice', 25])
print(my_dict.items())     # dict_items([('name', 'Alice'), ('age', 25)])

# Update dictionary
my_dict.update({'city': 'New York'})
print(my_dict)
```

### Exercise 4: Slicing
```python
# List slicing
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
print(numbers[1:5])        # [1, 2, 3, 4]
print(numbers[::2])        # [0, 2, 4, 6, 8]
print(numbers[::-1])       # [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]

# Tuple slicing
my_tuple = (1, 2, 3, 4, 5)
print(my_tuple[1:4])       # (2, 3, 4)
```

### Exercise 5: Nested Data Structures
```python
# Nested list
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(matrix[1][1])        # 5

# List of tuples
points = [(1, 2), (3, 4), (5, 6)]
for x, y in points:
    print(f"Point: ({x}, {y})")

# Dictionary with lists
student = {
    'name': 'Bob',
    'grades': [85, 90, 78, 92],
    'subjects': ['Math', 'Science', 'English']
}
print(f"Average grade: {sum(student['grades']) / len(student['grades'])}")
```

### Exercise 6: Iteration
```python
# Iterate over different data types
# List iteration
for item in [1, 2, 3, 4, 5]:
    print(item, end=' ')   # 1 2 3 4 5

# Tuple iteration
for item in (1, 2, 3):
    print(item, end=' ')   # 1 2 3

# Dictionary iteration
my_dict = {'a': 1, 'b': 2, 'c': 3}
for key in my_dict:
    print(f"{key}: {my_dict[key]}")

# Dictionary items iteration
for key, value in my_dict.items():
    print(f"{key}: {value}")
```

**Remember**: Lists, tuples, and dictionaries are fundamental data structures in Python. Master their operations and understand when to use each one! 