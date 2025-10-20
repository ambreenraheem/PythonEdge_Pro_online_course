Date: 19-October-2025
## Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
### Lists in Python
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
print(fruits)
```
```
students = ["Faiza", "Ahmed", "Ali"]
students[-2] = "Ambreen"
print("I modify my List:",students)
```



















