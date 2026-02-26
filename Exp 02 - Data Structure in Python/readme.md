# Using Python Data Structures

## Class Overview

This class introduces core Python data structures—**lists, tuples, dictionaries, and NumPy arrays**—and shows how to store, access, and organize data efficiently. These structures are foundational for data handling and Machine Learning workflows.

---

## Learning Objectives

By the end of this class, students will be able to:

* Understand different Python data structures and their use cases
* Store and organize data using lists, tuples, dictionaries, and NumPy arrays
* Choose appropriate data structures for specific problems
* Perform basic operations on each data structure

---

## 1. Lists

### What is a List?

A **list** is an ordered, mutable collection that can store multiple data types.

### Example

```python
marks = [78, 85, 90, 66]
print(marks)
```

### Common Operations

```python
marks.append(92)      # Add element
marks.remove(66)      # Remove element
marks.sort()          # Sort list
print(max(marks))     # Maximum value
print(sum(marks)/len(marks))  # Average
```

### Use Cases

* Storing datasets
* Collecting feature values
* Maintaining ordered records

---

## 2. Tuples

### What is a Tuple?

A **tuple** is an ordered, immutable collection. Once created, it cannot be modified.

### Example

```python
student = (101, "Ali", 20)
print(student)
```

### Immutability Demonstration

```python
student[1] = "Rahim"  # This will raise an error
```

### When to Use Tuples

* Fixed data (coordinates, configuration values)
* Data that should not change

---

## 3. Dictionaries

### What is a Dictionary?

A **dictionary** stores data as key–value pairs, allowing fast access using keys.

### Example

```python
student = {
    "name": "Ali",
    "roll": 101,
    "marks": 85
}
```

### Accessing and Updating Values

```python
print(student["name"])
student["marks"] = 90
student["grade"] = "A"
```

### Iterating Through a Dictionary

```python
for key, value in student.items():
    print(key, value)
```

### Use Cases

* Storing structured data
* Label mappings in ML
* Configuration settings

---

## 4. NumPy Arrays

### Why NumPy?

NumPy arrays are faster and more memory-efficient than lists for numerical operations, making them ideal for Machine Learning.

### Creating a NumPy Array

```python
import numpy as np

arr = np.array([10, 20, 30, 40])
print(arr)
```

### Common Operations

```python
print(arr + 5)           # Element-wise addition
print(arr.mean())        # Mean
print(arr.reshape(2,2))  # Reshape
```

### Use Cases

* Numerical computations
* Matrix operations
* ML feature storage

---

## 5. Comparison of Data Structures

| Structure   | Ordered        | Mutable | Best For             |
| ----------- | -------------- | ------- | -------------------- |
| List        | Yes            | Yes     | General data storage |
| Tuple       | Yes            | No      | Fixed data           |
| Dictionary  | No (key-based) | Yes     | Structured data      |
| NumPy Array | Yes            | Yes     | Numerical & ML data  |

---

## 6. Practice Tasks

### Task 1

Create a list of 5 numbers and:

* Add one number
* Remove one number
* Find maximum and average

### Task 3

Create a dictionary for a student and:

* Update values
* Add a new key
* Print all key–value pairs

### Task 4

Create a NumPy array and:

* Perform element-wise multiplication
* Calculate mean

---
