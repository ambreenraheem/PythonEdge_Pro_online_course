Date: 21-October-2025

## Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
#### 01. Tuple in Python
A tuple is an ordered and immutable (unchangeable) sequence of elements. Tuples are useful when you want to store data that should not be modified, or to store fixed collections of data.

**🔹 Key Properties of Tuples**\
**Immutable:**\
Once a tuple is created, you cannot change, add, or remove its elements.

**Ordered:**\
Tuples preserve the order of elements, meaning the order in which you store data remains the same.

**Allow Duplicates:**\
Since tuples are indexed, they can contain duplicate values.

**🔹 Why Use Tuples?**\
- Immutable: Protects data from being accidentally changed.
- Hashable: Can be used as keys in dictionaries (unlike lists).
- Performance: Faster than lists due to immutability.

**🔹 When to Use Tuples vs. Lists**\
Use Case	Data Type\
Data should not change (e.g., coordinates, constants)	Tuple\
Data needs modification (e.g., adding/removing elements)	List

**🔹 Creating Tuples**\
You can create tuples in multiple ways:
```
tuple1 = tuple(["apple", "banana", "cherry"])  # Convert list to tuple
tuple2 = (10, 20, 30)                          # Direct tuple creation
mixed_tuple = ("hello", 42, 3.14, True)        # Different data types
print(tuple1)
print(tuple2)
print(mixed_tupke)
```
**🔹 Tuple Identity and Immutability**\
Even if two tuples have identical content, Python may assign them different memory locations:
```
tuple_1 = (10, 20, 30)
tuple_2 = (10, 20, 30)

print("id(tuple_1) =", id(tuple_1))
print("id(tuple_2) =", id(tuple_2))
print("tuple_1 == tuple_2 =", tuple_1 == tuple_2)
```
💡 Note: The tuples contain the same data (== True), but they exist as separate objects in memory (different id() values).

### Why Are Tuples Immutable?
Tuples in Python are immutable — their elements cannot be changed after creation. This design choice offers several important advantages:

**🔹 1. Memory Efficiency**\
Since tuples are immutable, Python can store them in a single continuous block of memory, making them more space-efficient and faster to access than lists.

**🔹 2. Thread Safety**\
Because tuples cannot be modified, they are safe to share between multiple threads. This ensures that no thread can accidentally change the data while another is using it.

**🔹 3. Hashability**\
Tuples are hashable, which means they can be used as keys in dictionaries or elements in sets — something that mutable data types like lists cannot do.

💡 In short, tuples are immutable to improve performance, ensure data integrity, and enable safe, consistent use in hash-based data structures.

#### More Examples
**🔹 Creating Tuples**\
```
tuple1: tuple = tuple(["apple", "banana", "cherry"])   # Convert list to tuple
tuple2: tuple = (10, 20, 30)                           # Tuple of integers
mixed_tuple: tuple = ("hello", 42, 3.14, True)         # Tuple with mixed data types

print("tuple1      =", tuple1)
print("tuple2      =", tuple2)
print("mixed_tuple =", mixed_tuple)
```

**🔹 Accessing Elements**\
Tuples are indexed like lists.
```
print("tuple1[0] =", tuple1[0])  # Access the first element
```

**🔹 Tuple Slicing**\
You can extract a portion of a tuple using slicing.
```
print("tuple2[1:] =", tuple2[1:])  # Slice from index 1 to the end
```

**🔹 Finding Tuple Length**
```
print("Length of tuple1:", len(tuple1))
```

**🔹 Iterating Through a Tuple**
```
print("Iterating through tuple2:")
for item in tuple2:
    print(item)
```

**🔹 Checking if an Element Exists**
```
print("Is 20 in tuple2?", 20 in tuple2)
```

**🔹 Concatenating Tuples**\
You can join two tuples using the + operator.
```
tuple3: tuple = tuple1 + tuple2
print("tuple1 + tuple2 =", tuple3)
```

**🔹 Repeating Tuples**
```
tuple4: tuple = tuple2 * 2
print("tuple2 * 2 =", tuple4)
```

**🔹 Nested Tuples**\
Tuples can contain other tuples as elements.
```
nested_tuple = (tuple1, tuple2)
print("nested_tuple =", nested_tuple)
```

**🔹 Unpacking Tuples**\
You can assign tuple elements to variables directly.
```
a, b, c = tuple1
print("Unpacking tuple1:", a, b, c)
```

**🔹 Using Tuples as Dictionary Keys**\
Because tuples are immutable, they can be used as keys in dictionaries.
```
my_dict = {tuple1: "This is a tuple key", tuple2: "Another tuple key"}
print("Dictionary with tuple keys:", my_dict)
```

**⚠️ Attempting to Modify a Tuple**\
Trying to change a tuple element will raise a TypeError, since tuples are immutable.
```
# tuple1[0] = "watermelon"  # ❌ This will cause an error
```
Error:
TypeError: 'tuple' object does not support item assignment










