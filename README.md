# Python Data Structures

This document provides a comprehensive overview of essential data structures in Python. It covers the theory, key differences, use cases, and hands-on practice examples for each type.

# What are Data Structures, and Why Are They Important?

Data structures are ways to organize and store data in a computer so that it can be accessed and modified efficiently. They are essential for:

Optimizing performance
Managing large amounts of data
Ensuring scalability and flexibility
Enabling efficient algorithms

# Mutable vs Immutable Data Types

**Mutable**: Can be changed after creation.
**Immutable**: Cannot be changed once created.

**Example (Mutable):**

```python
my_list = [1, 2, 3]
my_list[0] = 10
print(my_list)  # Output: [10, 2, 3]
```

**Example (Immutable):**

```python
my_tuple = (1, 2, 3)
my_tuple[0] = 4  # Error: Tuples are immutable
```

# List vs Tuple

| Feature      | List    | Tuple     |
| ------------ | ------- | --------- |
| Mutability   | Mutable | Immutable |
| Syntax       | `[]`    | `()`      |
| Performance  | Slower  | Faster    |
| Memory Usage | Higher  | Lower     |

# How Dictionaries Store Data

Dictionaries store data in key-value pairs, using a hash table behind the scenes.

**Example:**

```python
my_dict = {"apple": 1, "banana": 2, "cherry": 3}
```

# Why Use a Set Instead of a List?

Removes duplicates automatically
Faster membership tests using hashing
Supports set operations (union, intersection, etc.)

# String vs List

**String**: Immutable sequence of characters
**List**: Mutable collection that can contain any data type

# How Tuples Ensure Data Integrity

Tuples are immutable, which means their contents cannot be changed. This makes them ideal for storing constant data and preventing accidental modification.

# Hash Tables and Dictionaries

A hash table maps keys to values using a hash function. Python's `dict` is implemented using hash tables, which allows constant-time (O(1)) lookup and insertion.

# Can Lists Contain Different Data Types?

Yes.
**Example:**

```python
my_list = [1, "hello", 3.14, [1, 2], {"key": "value"}]
```

# Why Are Strings Immutable?

Efficiency in memory usage
Thread safety
Enables consistent hash values for use in dictionaries

# Advantages of Dictionaries Over Lists

Fast access using keys
Easy to map related data (e.g., student name → grade)

# When to Prefer Tuples Over Lists

Data should not change (e.g., coordinates)
Faster performance in read-only scenarios

# How Sets Handle Duplicates

Sets automatically eliminate duplicates.
**Example:**

```python
my_set = {1, 2, 3, 1}
print(my_set)  # Output: {1, 2, 3}
```

# `"in"` Keyword: List vs Dictionary

* **List**: Checks for presence of a value
* **Dictionary**: Checks for presence of a key

# Can You Modify Tuple Elements?

No. Tuples are immutable and cannot be changed after creation.

# What Is a Nested Dictionary?

A dictionary within another dictionary.

**Example:**
```python
students = {
    "John": {"age": 20, "grade": "A"},
    "Alice": {"age": 22, "grade": "B"}
}
print(students["John"]["age"])  # Output: 20
```

# Time Complexity of Accessing Dictionary Elements

**Average case**: O(1) (constant time)
Due to use of hash tables

# When Are Lists Preferred Over Dictionaries?

When order matters
When storing simple sequences of values
When position-based access is needed

# Are Dictionaries Ordered?

Prior to Python 3.7: Unordered
From Python 3.7 onward: Insertion order is preserved

# List vs Dictionary: Data Retrieval

**List**: Access via index (e.g., `my_list[0]`)
**Dictionary**: Access via key (e.g., `my_dict["key"]`)

# Practice Questions (Python Code)
# Strings

```python
my_name = "John"
print(my_name)  # John

string = "Hello World"
print(len(string))  # 11

string = "Python Programming"
print(string[:3])  # Pyt

print("hello".upper())  # HELLO

string = "I like apple"
print(string.replace("apple", "orange"))  # I like orange
```

# Lists

```python
my_list = [1, 2, 3, 4, 5]
print(my_list)

my_list = [1, 2, 3, 4]
my_list.append(10)
print(my_list)  # [1, 2, 3, 4, 10]

my_list = [1, 2, 3, 4, 5]
my_list.remove(3)
print(my_list)  # [1, 2, 4, 5]

my_list = ['a', 'b', 'c', 'd']
print(my_list[1])  # b

my_list = [10, 20, 30, 40, 50]
print(my_list[::-1])  # [50, 40, 30, 20, 10]
```

# Tuples

```python
my_tuple = (10, 20, 30)
print(my_tuple)

my_tuple = ('apple', 'banana', 'cherry')
print(my_tuple[0])  # apple

my_tuple = (1, 2, 3, 2, 4, 2)
print(my_tuple.count(2))  # 3

my_tuple = ('dog', 'cat', 'rabbit')
print(my_tuple.index('cat'))  # 1

my_tuple = ('apple', 'orange', 'banana')
print('banana' in my_tuple)  # True
```

# Sets

```python
my_set = {1, 2, 3, 4, 5}
print(my_set)

my_set = {1, 2, 3, 4}
my_set.add(6)
print(my_set)  # {1, 2, 3, 4, 6}
```
