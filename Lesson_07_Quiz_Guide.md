# Lesson 07: Sets & Frozenset - Quiz Preparation Guide

## 📚 Lesson Overview
This lesson covers Python sets (mutable unordered collections of unique elements) and frozensets (immutable sets).

## 🎯 Key Concepts to Master

### 1. Sets
- **Unordered collection**: No indexing or slicing
- **Unique elements**: No duplicates allowed
- **Mutable**: Can be modified after creation
- **Heterogeneous**: Can contain different data types
- **Mathematical operations**: Union, intersection, difference, symmetric difference

### 2. Set Operations
- **Union (|)**: Elements in either set
- **Intersection (&)**: Elements in both sets
- **Difference (-)**: Elements in first set but not second
- **Symmetric Difference (^)**: Elements in either set but not both
- **Subset (<=)**: All elements of first set in second
- **Superset (>=)**: All elements of second set in first

### 3. Set Methods
- **Adding**: add(), update()
- **Removing**: remove(), discard(), pop(), clear()
- **Checking**: issubset(), issuperset(), isdisjoint()
- **Copying**: copy()

### 4. Frozensets
- **Immutable sets**: Cannot be modified after creation
- **Same operations**: All set operations except modification
- **Hashable**: Can be used as dictionary keys or set elements
- **Creation**: frozenset() constructor

### 5. Set vs Other Data Structures
- **vs Lists**: No duplicates, no order, faster membership testing
- **vs Tuples**: Mutable, no duplicates, no order
- **vs Dictionaries**: No key-value pairs, just values

## 📝 Sample MCQs with Detailed Explanations

### Question 1: Set Creation
**Which of the following creates a set?**

- A) {1, 2, 3} ✅
- B) [1, 2, 3]
- C) (1, 2, 3)
- D) "1, 2, 3"

**Explanation**: Curly braces {} create a set. Square brackets [] create a list, parentheses () create a tuple.

### Question 2: Set Intersection
**What is the output of `{1, 2, 3} & {2, 3, 4}`?**

- A) {1, 2, 3, 4}
- B) {2, 3} ✅
- C) {1, 4}
- D) Error

**Explanation**: The & operator performs set intersection, returning elements that are in both sets.

### Question 3: Set Operation
**Which set operation removes common elements?**

- A) Union
- B) Intersection
- C) Difference ✅
- D) Symmetric difference

**Explanation**: The difference operation (-) returns elements that are in the first set but not in the second.

### Question 4: Frozenset
**What is a frozenset?**

- A) An immutable set ✅
- B) A frozen list
- C) A set with no elements
- D) A set that cannot be created

**Explanation**: A frozenset is an immutable version of a set - it cannot be modified after creation.

### Question 5: Set Length
**What is the result of `len({1, 1, 2, 2, 3})`?**

- A) 5
- B) 3 ✅
- C) Error
- D) 1

**Explanation**: Sets only store unique elements, so {1, 1, 2, 2, 3} becomes {1, 2, 3}, which has length 3.

## 🔍 Additional Practice Questions

### Question 6: Set Union
**What is the output of `{1, 2, 3} | {3, 4, 5}`?**

- A) {1, 2, 3, 4, 5} ✅
- B) {3}
- C) {1, 2, 4, 5}
- D) Error

**Explanation**: The | operator performs set union, combining all unique elements from both sets.

### Question 7: Set Method
**Which method adds an element to a set?**

- A) append()
- B) add() ✅
- C) insert()
- D) extend()

**Explanation**: add() adds a single element to a set. append() is for lists, insert() is for lists, extend() is for lists.

### Question 8: Set Membership
**What is the result of `3 in {1, 2, 3}`?**

- A) True ✅
- B) False
- C) Error
- D) 3

**Explanation**: The in operator checks if an element is in the set. Since 3 is in {1, 2, 3}, it returns True.

### Question 9: Set Difference
**What is the output of `{1, 2, 3, 4} - {2, 4}`?**

- A) {1, 3} ✅
- B) {2, 4}
- C) {1, 2, 3, 4}
- D) Error

**Explanation**: The - operator performs set difference, returning elements in the first set but not in the second.

### Question 10: Frozenset Creation
**How do you create a frozenset?**

- A) {1, 2, 3}
- B) frozenset([1, 2, 3]) ✅
- C) set([1, 2, 3])
- D) tuple([1, 2, 3])

**Explanation**: Use the frozenset() constructor with an iterable to create a frozenset.

## 📋 Important Facts to Remember

### Set Properties
1. **Unordered**: No guaranteed order of elements
2. **Unique**: No duplicate elements allowed
3. **Mutable**: Can be modified (except frozensets)
4. **Heterogeneous**: Can contain different data types
5. **Fast membership**: O(1) average case for in operator

### Set Operations
1. **Union (|)**: Elements in either set
2. **Intersection (&)**: Elements in both sets
3. **Difference (-)**: Elements in first set but not second
4. **Symmetric Difference (^)**: Elements in either set but not both

### Common Set Methods
1. **Adding**: add(), update()
2. **Removing**: remove(), discard(), pop(), clear()
3. **Checking**: issubset(), issuperset(), isdisjoint()
4. **Copying**: copy()

### Frozenset Characteristics
1. **Immutable**: Cannot be modified after creation
2. **Hashable**: Can be used as dictionary keys
3. **Same operations**: All set operations except modification
4. **Memory efficient**: Slightly more memory efficient than sets

## 🎯 Study Tips for This Lesson

1. **Practice Set Operations**: Try all mathematical operations
2. **Understand Uniqueness**: Know that sets only store unique elements
3. **Test Membership**: Use the in operator frequently
4. **Compare with Other Types**: Understand when to use sets vs lists/dicts
5. **Learn Frozensets**: Know when immutability is needed

## 🔗 Related Resources

- [Python Sets](https://docs.python.org/3/tutorial/datastructures.html#sets)
- [Python Set Methods](https://docs.python.org/3/library/stdtypes.html#set-types-set-frozenset)
- [Python Set Operations](https://docs.python.org/3/library/stdtypes.html#set)

## ✅ Self-Assessment Checklist

- [ ] I can create and manipulate sets
- [ ] I understand set operations (union, intersection, difference)
- [ ] I know set methods (add, remove, etc.)
- [ ] I can use set membership testing
- [ ] I understand that sets only store unique elements
- [ ] I can create and use frozensets
- [ ] I know the difference between sets and frozensets
- [ ] I can perform mathematical set operations
- [ ] I understand when to use sets vs other data structures
- [ ] I know that sets are unordered

## 🧮 Practice Exercises

### Exercise 1: Set Creation and Basic Operations
```python
# Create sets
set1 = {1, 2, 3, 4, 5}
set2 = {4, 5, 6, 7, 8}

print(set1)                 # {1, 2, 3, 4, 5}
print(len(set1))           # 5

# Test uniqueness
duplicate_set = {1, 1, 2, 2, 3}
print(duplicate_set)        # {1, 2, 3}
```

### Exercise 2: Set Operations
```python
# Set operations
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

print(set1 | set2)          # Union: {1, 2, 3, 4, 5, 6}
print(set1 & set2)          # Intersection: {3, 4}
print(set1 - set2)          # Difference: {1, 2}
print(set1 ^ set2)          # Symmetric difference: {1, 2, 5, 6}
```

### Exercise 3: Set Methods
```python
# Set methods
my_set = {1, 2, 3}

# Adding elements
my_set.add(4)               # {1, 2, 3, 4}
my_set.update([5, 6])       # {1, 2, 3, 4, 5, 6}

# Removing elements
my_set.remove(1)            # {2, 3, 4, 5, 6}
my_set.discard(10)          # No error if element doesn't exist
popped = my_set.pop()       # Removes and returns arbitrary element

print(my_set)
```

### Exercise 4: Set Membership and Comparison
```python
# Membership testing
numbers = {1, 2, 3, 4, 5}
print(3 in numbers)         # True
print(6 in numbers)         # False

# Set comparisons
set1 = {1, 2, 3}
set2 = {1, 2, 3, 4, 5}
print(set1.issubset(set2))  # True
print(set2.issuperset(set1)) # True
print(set1.isdisjoint({6, 7, 8})) # True
```

### Exercise 5: Frozensets
```python
# Create frozenset
frozen = frozenset([1, 2, 3, 4])
print(frozen)               # frozenset({1, 2, 3, 4})

# Frozenset operations (read-only)
print(len(frozen))          # 4
print(2 in frozen)          # True

# Can't modify frozenset
# frozen.add(5)             # AttributeError

# Use frozenset as dictionary key
dict_with_frozen = {frozen: "value"}
print(dict_with_frozen)
```

### Exercise 6: Set Applications
```python
# Remove duplicates from list
numbers = [1, 2, 2, 3, 3, 4, 5, 5]
unique_numbers = list(set(numbers))
print(unique_numbers)       # [1, 2, 3, 4, 5]

# Find common elements
list1 = [1, 2, 3, 4, 5]
list2 = [4, 5, 6, 7, 8]
common = set(list1) & set(list2)
print(common)               # {4, 5}

# Find unique elements
unique = set(list1) ^ set(list2)
print(unique)               # {1, 2, 3, 6, 7, 8}
```

### Exercise 7: Set Comprehension
```python
# Set comprehension
squares = {x**2 for x in range(5)}
print(squares)              # {0, 1, 4, 9, 16}

# Conditional set comprehension
even_squares = {x**2 for x in range(10) if x % 2 == 0}
print(even_squares)         # {0, 4, 16, 36, 64}
```

**Remember**: Sets are excellent for removing duplicates, testing membership, and performing mathematical set operations. Use them when you need unique, unordered collections! 