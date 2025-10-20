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
**Join Two Lists**\
There are several ways to join, or concatenate, two or more lists in Python.\
One of the easiest ways are by using the + operator.

**Example: Get your own Python Server**\
**Join two list:**
```
list1 = ["a", "b", "c"]
list2 = [1, 2, 3]

list3 = list1 + list2
print(list3)
```
**Another way to join two lists is by appending all the items from list2 into list1, one by one:**

**Example**\
Append list2 into list1:
```
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

for x in list2:
  list1.append(x)

print(list1)
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
## Python - Loop Lists
First of all we need to discuss (What is Loop?)

#### 🌀 What is a Loop?

A loop means doing something again and again — until you finish.

#### 👧 Example in Real Life:

Imagine your mom says:

“Pick up all your toys one by one.”

So you:
-> Pick up the first toy 🧸

-> Pick up the second toy 🚗

-> Pick up the third toy 🪀

…and keep doing it until all toys are picked up!

That’s a loop — you repeat the same action for every toy.

**🖥 In Python:**

When you tell Python to loop, it does the same thing, it repeats an action for every item in a list.

**Example:**
```
toys = ["car", "doll", "ball"]
for toy in toys:
    print(toy)
```

You can go through (or loop through) all the items in a list using a for loop.

**Example 1 – Loop Through a List**\
Print each item in the list one by one:
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
```
**Learn more about how for loops work in the Python "For Loops" chapter. "Loop" is very important chapter in python.**

**Looping Using Index Numbers**

You can also loop through a list using index numbers.\
This means you access each item by its position in the list.

Use the range() function along with len() to create a sequence of numbers that match the list’s indexes.

**Example 2 – Loop Using Index Numbers**
```
fruits = ["apple", "banana", "cherry"]
for i in range(len(fruits)):
  print(fruits[i])
```

In the example above, range(len(fruits)) creates this sequence: [0, 1, 2],
which are the index numbers of the list items.

**Using a While Loop**

You can also go through all the items in a list using a while loop.

**To do this:**

1. Use the len() function to find out how many items are in the list.
2. Start from index 0 (the first item).
3. Keep looping until you reach the end of the list.
4. Don’t forget to increase the index by 1 each time — or the loop will never stop!

**Example – Loop Through a List Using While**
```
fruits = ["apple", "banana", "cherry"]
i = 0
while i < len(fruits):
  print(fruits[i])
  i = i + 1
```
**Learn more about while loops in the Python "While Loops" chapter. "Loop" is very important chapter in python.**

### List Comprehension
List comprehension is a quick and simple way to make a new list from an existing list.\
It lets you do the same work as a normal loop — but in just one line of code!\
**Example 1 – Without List Comprehension**\
Let’s say you have a list of fruits, and you want a new list that only includes fruits containing the letter "a".\
You can do it the long way using a for loop and an if condition:
```
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = []

for x in fruits:
  if "a" in x:
    newlist.append(x)

print(newlist)
```
**Example 2 – With List Comprehension**\
You can do the same thing in just one line using list comprehension:
```
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x for x in fruits if "a" in x]
```
**Looping with List Comprehension**\
List comprehension gives you a short and clean way to loop through a list.\
You can use it to do the same thing as a for loop — but in just one line!

**Example – Short Hand For Loop**
```
fruits = ["apple", "banana", "cherry"]
[print(x) for x in fruits]
```

💡 Tip:\
List comprehension is great for creating new lists quickly and neatly, especially when filtering or changing items.

### Copying a List in Python

If you try to copy a list like this 👇
```
list2 = list1
```
it won’t actually make a new list.\
Instead, both list1 and list2 will point to the same list in memory.\
So, if you change one — the other will change too!

**✅ 1. Using the copy() Method**\
The easiest and safest way to copy a list is by using the copy() method.

**Example**
```
fruits = ["apple", "banana", "cherry"]
mylist = fruits.copy()
print(mylist)
```
**✅ 2. Using the list() Function**\
You can also copy a list using the built-in list() function.

**Example**
```
fruits = ["apple", "banana", "cherry"]
mylist = list(fruits)
print(mylist)
```
**✅ 3. Using the Slice Operator**\
Another simple way to copy a list is by using the slice operator (:).

**Example**
```
fruits = ["apple", "banana", "cherry"]
mylist = fruits[:]
print(mylist)
```
💡 Tip:\
All three methods create a new, independent copy of your list, so changes in one list won’t affect the other.

### To check how a loop or iteration works, visit this website, and do practice with it.
[PythonTutor](http://pythontutor.com)
