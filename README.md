# unit-2
# Python Programming Assignment (Unit 2)
**Name:** Abhijeet Sunil Dahifale 
**Class:** FY CSE SOC-09
**Subject:** Programming Language (II) – Python Programming
**Unit:** II – Sequence Types and Operators

---

## Q1. List the Python sequence data types and state one key characteristic of each with respect to mutability or ordering.

**Answer:**
Python sequence data types include:

* **List:** Ordered and mutable (elements can be changed)
* **Tuple:** Ordered and immutable (cannot be changed after creation)
* **String:** Ordered and immutable (sequence of characters)
* **Range:** Ordered and immutable (represents sequence of numbers)

---

## Q2. Explain how indexing and slicing work in Python sequences. Illustrate how they differ when applied to strings and lists.

**Answer:**

* **Indexing:** Used to access a single element using its position. Index starts from 0.
* **Slicing:** Used to access a range of elements using syntax `[start:end:step]`.

**Example:**

```python
string = "Python"
print(string[0])      # P
print(string[1:4])    # yth

list1 = [1, 2, 3, 4]
list1[0] = 10
print(list1)          # [10, 2, 3, 4]
```

**Difference:**

* Strings are **immutable** (cannot modify elements)
* Lists are **mutable** (can modify elements)

---

## Q3. Write a Python program that uses indexing and slicing on a string or list, and applies at least two built-in functions to display meaningful results.

**Answer (Program):**

```python
s = "HelloWorld"

print("First character:", s[0])
print("Last character:", s[-1])
print("Slice (1:5):", s[1:5])

print("Length:", len(s))
print("Uppercase:", s.upper())
```

---

## Q4. Analyze the difference between equality (==) and identity (is) when used with sequence types. Discuss how object mutability and memory reference affect program behaviour.

**Answer:**

* `==` checks whether the **values are equal**
* `is` checks whether both variables refer to the **same memory location**

**Example:**

```python
a = [1, 2, 3]
b = [1, 2, 3]

print(a == b)   # True (values are same)
print(a is b)   # False (different memory locations)
```

**Explanation:**

* Mutable objects (like lists) can exist in different memory locations even if values are same
* Identity depends on reference, not value

---

## Q5. Evaluate the suitability of lists, sets, and dictionaries for storing and managing unique student records. Justify which data structure is most efficient and why.

**Answer:**

* **List:** Ordered, allows duplicates → not suitable for unique records
* **Set:** Stores unique elements but unordered → not ideal for structured records
* **Dictionary:** Stores data in key-value pairs → best suited

**Conclusion:**
Dictionary is most efficient because:

* Each student can have a unique key (like ID)
* Fast access and retrieval
* Well-structured data storage

---

## Q6. Design and implement a Python program that uses appropriate sequence types, indexing or slicing, and built-in functions to manage and process student data efficiently.

**Answer (Program):**

```python
students = {
    1: "Abhi",
    2: "Rahul",
    3: "Sneha"
}

print("All Students:", students)
print("Student with ID 1:", students[1])

names = list(students.values())
print("First Student:", names[0])
print("Total Students:", len(students))
```

---

# LAB PROGRAMS (Q7 to Q10)

## Q7. Write a program to print the first and last character of a string.

**Algorithm:**

1. Start
2. Input a string
3. Display first character using index 0
4. Display last character using index -1
5. End

**Program:**

```python
s = input("Enter string: ")
print("First character:", s[0])
print("Last character:", s[-1])
```

---

## Q8. Write a program to create a list, tuple, set and dictionary.

**Algorithm:**

1. Start
2. Create list, tuple, set, dictionary
3. Print all
4. End

**Program:**

```python
list1 = [1, 2, 3]
tuple1 = (1, 2, 3)
set1 = {1, 2, 3}
dict1 = {1: "A", 2: "B"}

print("List:", list1)
print("Tuple:", tuple1)
print("Set:", set1)
print("Dictionary:", dict1)
```

---

## Q9. Write a program to understand the concept of indexing.

**Algorithm:**

1. Start
2. Create a list
3. Access elements using index
4. Print values
5. End

**Program:**

```python
list1 = [10, 20, 30, 40]

print("First element:", list1[0])
print("Last element:", list1[-1])
```

---

## Q10. Write a program to understand the concept of built-in function.

**Algorithm:**

1. Start
2. Create a list
3. Use built-in functions like len, max, min
4. Display results
5. End

**Program:**

```python
list1 = [5, 10, 15]

print("Length:", len(list1))
print("Maximum:", max(list1))
print("Minimum:", min(list1))
```



