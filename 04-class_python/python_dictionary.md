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
**Example. 03**
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
You can remove elements using del, pop(), or clear().
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




