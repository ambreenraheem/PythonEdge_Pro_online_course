Date: 25-January-2026

### Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
#### Lops in Python
#### Topic: **for, while & nested loop**

**Python Tutor:** https://pythontutor.com/ 

For understanding use Python Tutor: "A best site to understand how python loop works step by step"\
**Loops in Python are used to repeat actions efficiently. The main types are For loops (counting through items) and While loops (based on conditions).**

#### For Loop
For loops is used to iterate over a sequence such as a list, tuple, string or range. It allow to execute a block of code repeatedly, once for each item in the sequence.

**Example:01**
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
```

**Example: Iterating Over List, Tuple, String and Dictionary Using for Loops in Python**
```
# List
girls = ["Shina", "Fariya", "Abida"]
for x in girls:
    print(x)
```

```
# Tuple
Vegetables= ("garlic", "onion", "carrot")
for x in vegetables:
    print(x)
```

```
# Letters of Strings
s = "PythonEdge Pro"
for x in s:
    print(x)
```

```
# Dictionary
d = dict({'Mariya':89, 'Daniyal':54,'Ahmed': 77})
for x in d:
    print("%s  %d" % (x, d[x]))
```

```
# Set
set = {10, 30, 20}
for x in set:
    print(x),
```

#### Understanding the `range()` function

The `range()` function is often used in `for` loops in Python to generate a sequence of numbers. It's very flexible and can be used in a few ways:

1.  **range(stop)**: Generates numbers from `0` up to (but not including) `stop`. 
    *Example: range(5) will produce `0, 1, 2, 3, 4`.

```
# Example # 01- range(5) will count from 0, 1, 2, 3, 4
print("Using range(5):")
for num in range(5):
    print(num)
```

```
n = 4
for i in range(0, n):
    print(i)
```

2.  **range(start, stop)**: Generates numbers from `start` up to (but not including) `stop`. 
    *Example: range(1, 11) will produce `1, 2, 3, 4, 5, 6, 7, 8, 9, 10`. This is what we used in the multiplication table example.

In the multiplication table, `for i in range(1, 11):` means that the loop variable `i` will take on values from `1` up to `10`, allowing us to calculate `N * 1`, `N * 2`, ..., `N * 10`.

```
# Example: 02- Multiplication Table

N = int(input("Enter the number for which you want the multiplication table: "))
print(f"\nMultiplication Table for {N}:")
for i in range(1, 11): # Loop from 1 to 10 (inclusive)
    product = N * i
    print(f"{N} x {i} = {product}")
else:
    print("Enter your number in integer")
```

3.  **range(start, stop, step)**: Generates numbers from `start` up to (but not including) `stop`, incrementing by `step` each time.

    Example: `range(0, 10, 2)` will produce `0, 2, 4, 6, 8`.
```
# Example: 03.a- range(0, 10, 2) will count from 0, 2, 4, 6, 8
print("\nUsing range(0, 10, 2):")
for num in range(0, 10, 2):
    print(num)
```

```
# Example: 03.b- range(5, 0, -1) will count backwards from 5, 4, 3, 2, 1
print("\nUsing range(5, 0, -1) (counting backwards):")
for num in range(5, 0, -1):
    print(num)
```

#### The break Statement
The break statement is used to terminate the loop entirely. When break is encountered inside a loop (either for or while), the loop is immediately exited, and program control resumes at the statement immediately following the loop. It's often used when an external condition is met or a specific item is found within the loop.

```
# Example: Using 'break' to stop a loop when a condition is met
print("Counting from 1 to 10, but stopping at 5:")
for i in range(1, 11):
    if i == 5:
        print(f"Found {i}! Breaking the loop.")
        break # Exit the loop when i is 5
    print(i)

print("Loop finished.")
```

#### Break in List
**Example:01**
```
fruits = ["apple", "banana", "cherry", "date", "fig"]
search_item = "cherry"
found = False

print(f"Searching for '{search_item}' in the list: {fruits}")
for fruit in fruits:
    print(f"Checking: {fruit}")
    if fruit == search_item:
        print(f"Found '{search_item}'! Stopping the search.")
        found = True
        break

if found:
    print("Search successful.")
else:
    print("Item not found.")
```

**Example:02**
```
Exit the loop when x is "banana":

fruits = ["apple","apricot", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
```

**Examole:03**
```
Exit the loop when x is "banana", but this time the break comes before the print:

fruits = ["apple", "apricot", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    break
  print(x)
```

#### The continue Statement

The continue statement is used to skip the rest of the code inside a loop for the current iteration only. The loop does not terminate; it proceeds to the next iteration.

It's useful when you want to bypass certain parts of the loop's body based on a condition, but still want the loop to continue its execution.

**Example 1: Using continue to skip a specific number.**

```
# Example: Using 'continue' to skip printing the number 5
print("Counting from 1 to 10, but skipping 5:")
for i in range(1, 11):
    if i == 5:
        print(f"Skipping {i}...")
        continue # Skip the rest of the current iteration when i is 5
    print(i)

print("Loop finished.")
```

**Example 2: Using continue to print only even numbers.**

```
# Example: Using 'continue' to print only even numbers
print("Printing only even numbers from 1 to 10:")
for i in range(1, 11):
    if i % 2 != 0: # If i is odd
        continue # Skip to the next iteration
    print(i)

print("Loop finished.")
```

```
# Example
Do not print banana:

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    continue
  print(x)
```

#### while Loop
A while loop in programming is used to repeatedly execute a block of code as long as a specified condition is true. The loop continues to run until the condition becomes false. It's important to ensure that the condition eventually becomes false to avoid an infinite loop.

**In this example:**
- `count = 0` initializes a variable `count`.
- `while count < 5:` sets the condition for the loop. The code inside the loop will execute as long as `count` is less than 5.
- `print(f"The count is: {count}")` is the code block that gets executed in each iteration.
- `count += 1` increments the `count` variable in each iteration. This is crucial because it ensures that `count` will eventually reach 5, making the condition `count < 5` false and terminating the loop.

```
# Example of a while loop

count = 0
while count < 5:
    print(f"The count is: {count}")
    count += 1 # Increment count to eventually make the condition false

print("Loop finished.")
```

#### `break` statement in a `while` loop
The `break` statement is used to exit a loop immediately, regardless of whether the loop's condition is still true. It transfers control to the statement immediately following the loop.

**In this example:**
- The loop is set to run as long as num < 10.
- However, when num becomes 5, the if num == 5: condition is met.
- The break statement is executed, causing the loop to terminate immediately, and the program continues with the statement after the loop.

```
# Example of 'break' in a while loop

num = 0
while num < 10:
    if num == 5:
        print(f"Breaking the loop when num is {num}")
        break  # Exit the loop
    print(f"Current number: {num}")
    num += 1

print("Loop terminated by break.")
```

#### `continue` statement in a `while` loop
The `continue` statement is used to skip the rest of the current iteration of the loop and move to the next iteration. The loop's condition is re-evaluated before the next iteration begins.

**In this example:**
- The loop iterates from i=1 to i=5.
- When i is 3, the if i == 3: condition is met.
- The continue statement is executed, causing the print(f"Current value of i: {i}") line to be skipped for that iteration, and the loop proceeds to the next iteration.

```
# Example of 'continue' in a while loop

i = 0
while i < 5:
    i += 1  # Increment i first to avoid infinite loop if continue is the first statement
    if i == 3:
        print(f"Skipping iteration when i is {i}")
        continue  # Skip the rest of this iteration
    print(f"Current value of i: {i}")

print("Loop finished using continue.")
```

#### Nested Loop
```
# Example of nested while loops for a multiplication table

i = 1
while i <= 3:  # Outer loop for rows
    j = 1
    while j <= 3:  # Inner loop for columns
        product = i * j
        print(f"{i} * {j} = {product}\t", end='') # \t for tab spacing
        j += 1
    print() # Newline after each row
    i += 1

print("Multiplication table complete.")
```

**This example shows how to use nested loops to process data stored in a list where each element is a dictionary.**

**In this example:**
- The outer for loop iterates through the students list. In each iteration, student is a dictionary containing information for one student.
- student["name"] is used to access the student's name.
- The inner for loop iterates through the key-value pairs (subject, grade) within the grades dictionary of the current student.
- This structure allows you to neatly display each student's name and their corresponding grades for each subject.

```
# Example of nested loops with a list of dictionaries

students = [
    {"name": "Alice", "grades": {"math": 90, "science": 85}},
    {"name": "Bob", "grades": {"math": 78, "science": 92}},
    {"name": "Charlie", "grades": {"math": 95, "science": 88}}
]

print("Student Grades:")
for student in students:  # Outer loop iterates through each student dictionary in the list
    student_name = student["name"]
    print(f"  {student_name}:")
    for subject, grade in student["grades"].items():  # Inner loop iterates through subjects and grades in each student's 'grades' dictionary
        print(f"    - {subject.capitalize()}: {grade}")
```

**This example demonstrates how to use nested loops to list items under different categories, where the categories themselves are stored in a list of dictionaries.**

**In this example:**
- The outer for loop iterates through the categories list. In each iteration, category is a dictionary with a 'name' and an 'items' key.
- The inner for loop iterates through the items list (which is the value associated with the 'items' key) of the current category dictionary.
- This effectively prints each category name followed by its associated items.

```
# Example of a simple nested loop with a list of dictionaries

categories = [
    {"name": "Fruits", "items": ["Apple", "Banana", "Orange"]},
    {"name": "Vegetables", "items": ["Carrot", "Spinach", "Broccoli"]}
]

print("Listing categories and their items:")
for category in categories:  # Outer loop iterates through each category dictionary
    category_name = category["name"]
    print(f"Category: {category_name}")
    for item in category["items"]:  # Inner loop iterates through the list of items for the current category
        print(f"  - {item}")
```














 



