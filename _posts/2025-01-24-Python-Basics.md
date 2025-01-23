---
title: "Python Basics"
date: "2025-01-24 00:00:00 +0800"
categories: [Python]
tags: [code]
---
# Python Basics

Python, in my experience, is a high-level, interpreted programming language that’s super versatile. I’ve found it really beginner-friendly because of its simple and clean syntax—it’s easy to pick up and understand, even if you’re new to programming.

One thing I like about Python is that it’s dynamically typed, so I don’t have to worry about declaring variable types—it just figures it out as the program runs. Plus, it’s interpreted, meaning it executes code line by line, which has been great for debugging and testing ideas quickly.

What makes Python stand out to me is how versatile it is. You can use it on pretty much any platform—Windows, macOS, Linux—and it’s widely used in so many areas. For example, I’ve seen it used in web development, data analysis, AI/ML, and even for automating repetitive tasks.

Another thing I’ve really appreciated is the massive library ecosystem. Whether it’s NumPy and pandas for data analysis or Django and Flask for web development, there’s probably a library or framework for whatever you want to do. And the Python community? Honestly, it’s one of the best—there are so many tutorials, forums, and resources out there to help you get unstuck.

For me, Python has become my go-to for projects because it strikes a great balance between being simple enough for quick scripts but powerful enough for complex applications. Have you ever tried using Python for something specific?

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

Example:
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(f"I like {fruit}")
Output:
I like apple  
I like banana  
I like cherry  
While Loops
A while loop continues to execute as long as a specified condition is True. Be careful to include a condition that eventually stops the loop to avoid infinite loops.

Example:
count = 0

while count < 3:
    print(f"The count is {count}")
    count += 1
Output:

The count is 0  
The count is 1  
The count is 2  
Functions in Python
Functions are blocks of reusable code that perform a specific task. They help make your code modular and easier to understand.

Defining and Calling a Function
To define a function, use the def keyword, followed by the function name and parentheses. You can also pass arguments to the function.

Example:
def greet(name):
    print(f"Hello, {name}!")

greet("Vallerio")
Output:
Hello, Vallerio!
Function with Return Value
If you want your function to return a value, use the return keyword.

Example:
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 7)
print(f"The sum is {result}")
Output:

The sum is 12
Lists in Python
A list is a versatile data structure in Python that allows you to store multiple items in a single variable. Lists are mutable, meaning you can modify them after creation.

Basic List Operations
Example:
my_list = [1, 2, 3, 4, 5]

# Access elements
print(my_list[0])  # Output: 1

# Append an element
my_list.append(6)

# Remove an element
my_list.remove(3)

# Iterate through the list
for item in my_list:
    print(item)