Date: 21-October-2025

## Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
#### 🧠 Dictionaries in Python
**1. Introduction to Dictionaries**\
A dictionary in Python is a collection of key–value pairs, where each key maps to a value.

**Key features of dictionaries:**
- Ordered (since Python 3.7): Items retain their insertion order.
- Mutable: You can add, remove, or change items.
- Unindexed: Access values by their keys, not by position.
- Unique keys: Each key must be unique, though values may repeat.
- 📝 Before Python 3.7, dictionaries were unordered, but now they maintain insertion order.

**2. Creating a Dictionary**\
You can create a dictionary using curly braces {} with key–value pairs separated by colons.
**Example. 01**
```
# Syntax:
dictionary = {key1: value1, key2: value2, ...}
```
**Example. 02**
```
# Creating a dictionary with personal details
person = {
    "name": "Alice",
    "age": 25,
    "visited_cities": ["New York", "Los Angeles", "Chicago"]
}
print(person)
```
You can also create a dictionary using the dict() constructor:

**Example. 04**
```
my_dict = dict(name="John", age=36, country="Norway")
print(type(my_dict), "-", my_dict)
```

**3. Accessing Dictionary Items**\
Access values using their keys:
```
print(person["name"])       # Output: Alice
print(person.get("age"))    # Output: 25
```
If the key doesn’t exist, get() returns None (or a custom default value if provided).

**4. Modifying a Dictionary**\
You can add a new key–value pair or update an existing one:
```
person["age"] = 26                  # Modify an existing value
person["city"] = "San Francisco"    # Add a new key
print(person)
```

**5. Deleting Items**\
You can remove elements using the del, pop(), or clear() methods.
```
# Remove specific key
del person["city"]

# Remove and return a value
age = person.pop("age")
print("Removed age:", age)

# Remove all items
person.clear()
```
- del does not return anything, but pop() returns the removed value.
- You can also use pop(key, default) to avoid errors if the key doesn’t exist.

**6. Dictionary Methods**
- Method	Description
- keys()	Returns all keys in the dictionary
- values()	Returns all values
- items()	Returns key–value pairs as tuples
- update()	Adds or updates multiple items
- pop()	Removes a specific key and returns its value
- popitem()	Removes the last inserted key–value pair
- clear()	Empties the entire dictionary
- copy()	Returns a shallow copy of the dictionary

**Example**
```
student = {"name": "Ali", "age": 22, "grade": "A"}

print(student.keys())     # dict_keys(['name', 'age', 'grade'])
print(student.values())   # dict_values(['Ali', 22, 'A'])
print(student.items())    # dict_items([('name', 'Ali'), ('age', 22), ('grade', 'A')])
```

**7. Looping Through a Dictionary**\
You can loop through keys, values, or both:
```
for key in student:
    print(key, ":", student[key])

# Or
for key, value in student.items():
    print(f"{key} → {value}")
```
```
for x, obj in myfamily.items():
  print(x)

  for y in obj:
    print(y + ':', obj[y])
```
**We will learn more about loops in the "Loop Chapter", how they work, and why it is important.**


**8. Nested Dictionaries**\
A dictionary can contain another dictionary inside it.
```
# Create three dictionaries, then create one dictionary that will contain the other three dictionaries:
family = {
    "child1": {"name": "Aisha", "age": 10},
    "child2": {"name": "Bilal", "age": 8}
}
print(family["child1"]["name"])  # Output: Aisha
```
```
myfamily = {
  "child1": {"name": "Emil", "year": 2004},
  "child2": {"name": "Tobias", "year": 2007},
  "child3": {"name": "Linus", "year": 2011}
}
myfamily = {
  "child1" : child1,
  "child2" : child2,
  "child3" : child3
}
print(child1)
print(child2)
print(child3)
```

**9. Copying a Dictionary in Python**\
You cannot copy a dictionary simply by writing dict2 = dict1.\
This only creates a reference to the original dictionary, meaning any changes made to dict1 will also affect dict2.

To create an actual independent copy, you can use one of the following methods:\
**✅ Method 1: Using the copy() Method**

The built-in copy() method creates a shallow copy of the dictionary.

**1. Example:**
```
thisdict = {
    "brand": "Ford",
    "model": "Mustang",
    "year": 1964
}

mydict = thisdict.copy()
print(mydict)
```

**✅ Method 2: Using the dict() Constructor**

You can also use the dict() function to make a copy of an existing dictionary.

**2. Example:**
```
thisdict = {
    "brand": "Ford",
    "model": "Mustang",
    "year": 1964
}

mydict = dict(thisdict)
print(mydict)
```

**💡 Tip: Both copy() and dict() create shallow copies.**\
If your dictionary contains nested dictionaries and you want to duplicate them as well, use the deepcopy() function from the copy module:
```
import copy
mydict = copy.deepcopy(thisdict)
```
**01. Practical Examples**\
Here are two practical examples to solidify these concepts.

**Example 1: Building a Phonebook**
```
# Create a phonebook
phonebook: dict = {
    "Abid": "123-456-7890",
    "Bbilal": "987-654-3210",
    "Chaudry": "555-555-5555",
    "Daniyal": "458-582-9999"
}

# Add a new contact
phonebook["Ehsan"] = "022-525-6444"

# Search for a contact
name: str = input("Enter a name to search: ")
if name in phonebook:
    print(f"{name}'s phone number is {phonebook[name]}.")
else:
    print(f"{name} is not in the phonebook.")
```     
**10. Dictionary Comprehensions in Python**

Dictionary comprehensions offer a concise and elegant way to create dictionaries.\
They are similar to list comprehensions, but instead of creating lists, they generate key–value pairs.

**✅ Basic Syntax**\
{key_expression: value_expression for item in iterable if condition}

This syntax allows you to loop through an iterable, apply a condition (optional), and construct key–value pairs dynamically.

**✅ Example 1: Doubling Dictionary Values**
```
original_dict = {'a': 1, 'b': 2, 'c': 3}
print("original_dict =", original_dict)

doubled_dict = {k: v * 2 for k, v in original_dict.items()}
print("doubled_dict  =", doubled_dict)
```

**🧠 Practice Exercise**

Create a dictionary comprehension that converts a list of temperatures in Celsius to Fahrenheit.\
Use the formula:\
**Example:**
```
celsius_temps = [0, 10, 20, 30, 40]

fahrenheit_temps = {str(c) + "c": str((c * 9/5) + 32) + "f" for c in celsius_temps}
print(fahrenheit_temps)
```

**💡 Tip:**\
**Dictionary comprehensions are great for transforming data, filtering items, or generating dictionaries from lists — all in a single, readable line of code.**
















