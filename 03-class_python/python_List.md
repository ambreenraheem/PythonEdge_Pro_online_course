Date: 19-October-2025
## Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
### 01. Lists in Python
In Python, lists are used to store multiple items in a single variable.\
They are one of the four built-in data types used to store collections of data — the others being Tuple, Set, and Dictionary — each with unique features and use cases.\
A list is created by placing items inside square brackets [ ].

**01 # Example:**
```
# Creating a list
my_list = ["apple", "banana", "cherry"]
print(my_list)
```

**🔹 Ordered**\
A list maintains the order of its elements. Each item has a specific index, starting from 0 for the first item, 1 for the second, and so on.\
If you add new items to a list, they are placed at the end.\
Note: Some list methods can change the order, but by default, the original order remains the same.

**🔹 Changeable**\
Lists are mutable, meaning you can modify them after creation.\
You can add, remove, or change items in a list at any time.

**🔹 Allow Duplicates**\
Since lists are indexed, they can contain duplicate values.

**02 # Example:**
```
fruit_list = ["apple", "banana", "cherry", "apple", "cherry"]
print(fruit_list)
```

**List Length**\
To find out how many items are in a list, use the len() function.

**03 # Example:**
```
fruit_list = ["apple", "banana", "cherry"]
print(len(fruit_list))
```
**🔹 List Items – Data Types**\
List elements can be of any data type — strings, integers, booleans, etc.

**04 # Examples:**
```
list1 = ["apple", "banana", "cherry"]      # String list
list2 = [1, 5, 7, 9, 3]                   # Integer list
list3 = [True, False, False]             # Boolean list
list4 = ["hello", 25, True, 5.6]         # Mixed list (You can even mix different data types in a single list)
print("Fruits:",list1)
print("Numbers:",list2)
print("Booleans:",list3)
print("Mixed:", list4)
```

**🔹Accessing List Elements**\
You can access items in a list using indexing.\
Positive indexing starts from 0 (the first element).\
Negative indexing starts from -1 (the last element) and moves backward.

**05 # Example:**
```
fruits = ["apple", "banana", "cherry"]
print(fruits[0])    # Output: apple  → first element
print(fruits[-3])   # Output: apple  → accessed from the end
```

**🔹Modifying Lists**\
Lists in Python are mutable, which means you can change their elements after the list has been created.

**06 # Example:**
```
fruits = ["apple", "banana", "cherry"]
fruits[-3] = "watermelon"   # Replace "apple" with "watermelon"
print("I modify my List of fruits:", fruits)
```
```
students = ["Faiza", "Ahmed", "Ali"]
students[-2] = "Ambreen"
print("I modify my List of students:",students)
```

### 2. Common List Methods
Python lists come with built-in methods that make it easy to add, remove, or modify elements efficiently.

**🔹 Appending and Extending Lists**\
You can add elements to a list using append() and extend().

**01 # Example:**
```
fruits = ["watermelon", "banana", "cherry"]

fruits.append("mango")  # Adds a single item to the end
print("Adds a single item to the end:", fruits)
```
```
students = ["Faiza", "Ahmed", "Ali"]

students.append("Usman")
print("Adds a single item to the end:", students)
```

**Expend: To add multiple elements at once, use extend():**
```
fruits.extend(["grape", "kiwi"])
print("I extend two more fruits:", fruits)
```
```
students.extend(["Fazal", "Raheem"])
print("I extend two more students name:", students)
```
**🔹 Removing Elements**\
Python provides two primary methods for removing elements from a list: remove() and pop().\
Although they seem similar, they work differently.

**✅ remove() Method**\
The remove() method deletes the first occurrence of a specified value.\
If the value is not found, it raises a ValueError.

**Key Points:**
- Works by value.
- Returns None.
- Raises ValueError if the item doesn’t exist.

**01 # Example:**
```
fruits.remove("banana")  # Removes 'banana' from the list
print("I deleted 'banana' from the fruits list", fruits)
```
```
students.remove("Ambreen")
print("I deleted 'Ambreen' from the students list", students)
```

**✅ pop() Method**\
The pop() method removes an item by index and returns the removed element.\
If no index is provided, it removes the last item.

**Key Points:**
- Works by index.
- Returns the removed item.
- Raises IndexError if the index is out of range.

**01 # Example:**
```
deleted = fruits.pop(1)  # Removes the element at index 1
print("Deleted element:", deleted)
print("I deleted one item (banana) from the list of fruits with 'pop() method'", fruits)
```
```
deleted = students.pop(2)  # Removes the element at index 1
print("Deleted element:", deleted)
print("I deleted one item (Ali) from the list of students with 'pop() method'", students)
```

**🔹 Sorting a List**\
You can arrange list items in different ways using the sort() and reverse() methods.

**1. Default Sorting (Ascending Order)**
```
numbers = [3, 1, 4, 1, 5, 9]
numbers.sort()
print("I sort a number of list in ascending order:", numbers)
```

**2. Descending Order (reverse=True)**
```
numbers = [4, 2, 9, 1]
numbers.sort(reverse=True)
print("I sort a number of list in descending order:", numbers)
```
**3. Sort by String Length (key=len)**
```
words = ["apple", "kiwi", "banana"]
words.sort(key=len)
print("I sort the list of fruits name by string length:", words)
```
**4. Sort by Last Character**
```
words = ["apple", "kiwi", "banana"]
words.sort(key=lambda word: word[-1])
print("I sort the list of fruits name by string length in descending order:", words)
```
**5. Reverse the List**
```
numbers = [1, 2, 5, 7, 10]
numbers.reverse()
print("Reverse the list of numbers:", numbers)
```
**3. Iterating Over Lists**\
You can use a for loop to go through each item in a list and perform operations on them.

**01 # Example:**
```
for fruit in fruits:
    print("Fruits list in loop:", fruit)
```



































