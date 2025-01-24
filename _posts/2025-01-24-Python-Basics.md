---
title: "Python Basics"
layout: post
date: "2025-01-24 00:00:00 +0800"
categories: [Python]
tags: [code]
---
# Python Basics

Python, in my experience, is a high-level, interpreted programming language that’s super versatile. I’ve found it really beginner-friendly because of its simple and clean syntax—it’s easy to pick up and understand, even if you’re new to programming.

One thing I like about Python is that it's dynamically typed, so I don’t have to worry about declaring variable types—it just figures it out as the program runs. Plus, it’s interpreted, meaning it executes code line by line, which has been great for debugging and testing ideas quickly.

What makes Python stand out to me is how versatile it is. You can use it on pretty much any platform—Windows, macOS, Linux—and it’s widely used in so many areas. For example, I’ve seen it used in web development, data analysis, AI/ML, and even for automating repetitive tasks.

Another thing I’ve really appreciated is the massive library ecosystem. Whether it’s NumPy and pandas for data analysis or Django and Flask for web development, there’s probably a library or framework for whatever you want to do. And the Python community? Honestly, it’s one of the best—there are so many tutorials, forums, and resources out there to help you get unstuck.

For me, Python has become my go-to for projects because it strikes a great balance between being simple enough for quick scripts but powerful enough for complex applications.

Here are a few things I have learned about Python throughout my first semester.

# If Statements
`if` statements are used to perform a specific action when a certain condition is met.

### Example:

```python
ayam = 2

if ayam == 1:
    print("You have less than 2 chickens")
elif ayam == 2:
    print("You have exactly 2 chickens")
else:
    print("You have more than 2 chickens")
```

# Loops in Python
Loops are incredibly useful in Python when you need to repeat a block of code multiple times. Python supports two main types of loops: for loops and while loops.

# For Loops
A for loop is used to iterate over a sequence (like a list, tuple, or string) or any iterable object.

### Example:
```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(f"I like {fruit}")
Output:
I like apple  
I like banana  
I like cherry
```

# While Loops
A while loop continues to execute as long as a specified condition is True. Be careful to include a condition that eventually stops the loop to avoid infinite loops.

### Example:
```python
count = 0

while count < 3:
    print(f"The count is {count}")
    count += 1

#Output:
#The count is 0  
#The count is 1  
#The count is 2  
```

# Functions in Python
Functions are blocks of reusable code that perform a specific task. They help make your code modular and easier to understand.

* Defining and Calling a Function
To define a function, use the def keyword, followed by the function name and parentheses. You can also pass arguments to the function.

### Example:
```python
def greet(name):
    print(f"Hello, {name}!")

greet("Vallerio") 

#Output: 
#Hello, Vallerio!
```
Function with Return Value
If you want your function to return a value, use the return keyword.

### Example:
```python
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 7)
print(f"The sum is {result}") 

#Output: 
#The sum is 12
```
# Lists in Python
Lists are a fundamental part of Python and are incredibly useful for managing collections of data. Below, we’ll explore some common list operations with detailed examples and explanations.

Accessing Elements in a List
Lists in Python are zero-indexed, meaning the first element has an index of 0. You can use square brackets [] to access elements by their position in the list.

### Example:
```python
my_list = [1, 2, 3, 4, 5]
```

### Access the first element
```python
print(my_list[0])  

#Output: 1
```

### Access the last element
```python
print(my_list[-1])  

#Output: 5
```

### Access a range of elements (slicing)
```python
print(my_list[1:4])  

#Output: [2, 3, 4]
```
Explanation:
my_list[0] gives the first element.
my_list[-1] accesses the last element using a negative index.
my_list[1:4] retrieves elements from index 1 to 3 (4 is excluded).
Appending Elements to a List
The append() method adds a single element to the end of the list. It’s useful when you need to grow a list dynamically.

### Example:
```python
my_list = [1, 2, 3]
my_list.append(4)
print(my_list)  

#Output: [1, 2, 3, 4]
```

Explanation:
After calling my_list.append(4), the number 4 is added to the end of the list.
This operation modifies the original list in place.
Removing Elements from a List
The remove() method removes the first occurrence of a specified value from the list. If the value doesn’t exist, Python will raise a ValueError.

### Example:
```python
my_list = [1, 2, 3, 4, 5]
my_list.remove(3)  # Removes the value 3 from the list
print(my_list)  

#Output: [1, 2, 4, 5]
```
Explanation:
After calling my_list.remove(3), the first occurrence of 3 is removed.
If you try my_list.remove(6) and 6 isn’t in the list, Python will raise an error.
Iterating Through a List
You can use a for loop to go through each element in a list. This is particularly helpful when you need to process or print all elements in the list.

### Example:
```python
my_list = ["apple", "banana", "cherry"]

for item in my_list:
    print(f"I like {item}")
```

```
Output:
I like apple
I like banana
I like cherry
```
Explanation:
The for loop iterates over each item in the list, assigning it to the variable item for use in the loop body.
You can perform any operation on item inside the loop, such as printing, modifying, or applying calculations.
Additional List Tips
Check if an item exists in a list:

```python
if "banana" in my_list:
    print("Banana is in the list!")
# Get the length of a list:
```

```python
print(len(my_list))  

#Output: 3

Combine two lists:
list1 = [1, 2, 3]
list2 = [4, 5, 6]

combined = list1 + list2
print(combined)  

#Output: [1, 2, 3, 4, 5, 6]
```