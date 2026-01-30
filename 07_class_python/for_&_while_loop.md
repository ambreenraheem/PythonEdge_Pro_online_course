Date: 25-January-2026

### Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
#### Python Loop
#### Topic: **for, while & nested loop**

**Python Tutor:** https://pythontutor.com/  
For understanding use Python Tutor: "A best site to understand how python loop works step by step"
Loops in Python are used to repeat actions efficiently. The main types are For loops (counting through items) and While loops (based on conditions).

**For Loop**
For loops is used to iterate over a sequence such as a list, tuple, string or range. It allow to execute a block of code repeatedly, once for each item in the sequence.

**Example:01**
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
```

Example: Iterating Over List, Tuple, String and Dictionary Using for Loops in Python
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

### Understanding the `range()` function

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
```

3.  **range(start, stop, step)**: Generates numbers from `start` up to (but not including) `stop`, incrementing by `step` each time.
    *Example: `range(0, 10, 2)` will produce `0, 2, 4, 6, 8`.
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

**The break Statement**\
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

### Break in List
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








