`Date: 23-October-2025

## Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
#### Topic: Set in Python

A set in Python is used to store multiple items in a single variable.

It is one of the four built-in data types in Python that are used to store collections of data.
The four types are:

1. List
2. Tuple
3. Dictionary
4. Set

Each of these types has its own special features and uses.
### Set
A set is a collection that is:

- Unordered → Items do not have a fixed position or index.
- Unchangeable* → Once created, the items themselves cannot be changed.
- Unindexed → You cannot access items using an index.

**Note: You can’t change the value of an existing item, but you can add new items or remove existing ones.**

**Sets are written using curly brackets {}.**

**Example: Creating a Set**
```
myset = {"apple", "banana", "cherry"}
print(myset)
```
**Note: Sets are unordered, so you cannot be sure in which order the items will appear.**

**Set Items**

Set items have three main characteristics: they are unordered, unchangeable, and do not allow duplicates.

**1. Unordered**
- “Unordered” means that the items in a set do not have a fixed order or index.
- When you print a set, the order of the items may vary each time.
- Also, you cannot access set items by index or key.

**2. Unchangeable**

- Once a set is created, its items cannot be modified directly.
- However, you can add new items or remove existing ones — just not change the value of an existing item.

**3. No Duplicates Allowed**

- Sets do not allow duplicate values.
- If you try to include duplicate items, Python will automatically ignore them.

**Example – Duplicate values are ignored:**
```
myset = {"apple", "banana", "cherry", "apple"}
print(myset)
```

**Special Note on Boolean Values**

- In Python, True and 1 are treated as the same value inside a set.
- Similarly, False and 0 are also considered the same.

**Example – True and 1 are treated as duplicates:**
```
myset = {"apple", "banana", "cherry", True, 1, 2}
print(myset)
```

**Example – False and 0 are treated as duplicates:**
```
myset = {"apple", "banana", "cherry", False, True, 0}
print(myset)
```

**Get the Length of a Set**

To find out how many items are in a set, use the len() function.

**Example:**
```
myset = {"apple", "banana", "cherry"}
print(len(myset))
```
**Set Items – Data Types**

Set items can store any type of data, including:

- Strings
- Integers
- Booleans

**Example – Different data types:**
```
set1 = {"apple", "banana", "cherry"}
set2 = {1, 5, 7, 9, 3}
set3 = {True, False, False}
```

A set can also mix different data types in one collection.

**Example – Mixed data types:**
```
set1 = {"abc", 34, True, 40, "male"}
```
**Check the Type of a Set**

From Python’s point of view, sets are objects of the set class.

**Example:**
```
myset = {"apple", "banana", "cherry"}
print(type(myset))
```
**The set() Constructor**

You can also create a set using the set() constructor.

**Example:**
```
myset = set(("apple", "banana", "cherry"))  # note the double round brackets
print(myset)
```
**Accessing Items in a Set**

- You cannot access items in a set using an index or a key, because sets are unordered.
- However, there are two common ways to work with items inside a set:

**Loop through all elements using a for loop.**

Check if a value exists using the in or not in keywords.

**1. Looping Through a Set**

You can use a for loop to go through each item in a set.

**Example:**
```
myset = {"apple", "banana", "cherry"}

for x in myset:
    print(x)
```

**(Note: The order may vary each time since sets are unordered.)**

**2. Check if an Item Exists in a Set**

You can use the in keyword to test if an item exists in the set.

**Example – Check if an item exists:**
```
myset = {"apple", "banana", "cherry"}
print("banana" in 2. Check if an Item Exists in a Set

You can use the in keyword to test if an item exists in the set.

Example – Check if an item exists:

myset = {"apple", "banana", "cherry"}
print("banana" in myset)
```
**3. Check if an Item Does NOT Exist in a Set**

You can also use not in to check if an item is not in the set.

**Example – Check if an item is missing:**
```
myset = {"apple", "banana", "cherry"}
print("banana" not in myset)
```
**Adding Items to a Set**

You can add new items to a set using the add() or update() methods.

**1. Add a Single Item**

To add one new element to a set, use the add() method.

**Example:**
```
myset = {"apple", "banana", "cherry"}

myset.add("orange")

print(thisset)
```
**2. Add Multiple Items (from Another Set)**

To add multiple items from another set, use the update() method.

**Example:**
```
myset = {"apple", "banana", "cherry"}
tropical = {"pineapple", "mango", "papaya"}

myset.update(tropical)

print(thisset)
```
**3. Add Items from Any Iterable**

- The update() method can also take any iterable (not just a set).
- This means you can add elements from lists, tuples, or even dictionaries.

**Example:**
```
myset = {"apple", "banana", "cherry"}
mylist = ["kiwi", "orange"]
myset.update(mylist)
print(myset)
```
**✅ Tip: The update() method is perfect when you want to combine multiple collections into one set.**

**Removing Items from a Set**

You can remove items from a set using several different methods.

Each behaves slightly differently depending on your needs.

**1. Using remove()**

The remove() method deletes a specific item from the set.

**Example:**
```
myset = {"apple", "banana", "cherry"}
myset.remove("banana")
print(myset)
```
**⚠️ Note: If the item doesn’t exist, remove() will raise an error.**

**2. Using discard()**

The discard() method also removes a specific item, but it does not raise an error if the item is not found.

**Example:**
```
myset = {"apple", "banana", "cherry"}
myset.discard("banana")
print(myset)
```
**3. Using pop()**

- The pop() method removes and returns a random item from the set.
- Since sets are unordered, you cannot predict which item will be removed.

**Example:**
```
myset = {"apple", "banana", "cherry"}
x = myset.pop()
print(x)        # The removed item
print(myset)  # Remaining items
```
**⚠️ Each time you run it, a different item may be removed.**

**4. Using clear()**

The clear() method removes all items from the set, leaving it empty.

**Example:**
```
myset = {"apple", "banana", "cherry"}
myset.clear()
print(myset)
```
**5. Using del**

The del keyword deletes the entire set completely.

**Example:**
```
myset = {"apple", "banana", "cherry"}
del myset
print(myset)  # This will cause an error
```
**⚠️ Once deleted, the set no longer exists — it cannot be accessed again.**

**Loop Items**
You can loop through the set items by using a for loop:

**Example: Get your own Python Server**
Loop through the set, and print the values:
```
myset = {"apple", "banana", "cherry"}

for x in myset:
  print(x)
```
**Joining Sets**

- You can combine two or more sets in Python using different methods.
- Each method serves a specific purpose, depending on how you want to handle duplicates.

**Overview of Joining Methods**

| Method                       | Description                                                    |
| ---------------------------- | -------------------------------------------------------------- | 
| **`union()` / `**            | Combines all items from both sets                              |
| **`update()`**               | Adds items from one set to another (modifies the original set) |
| **`intersection()`**         | Keeps only the items found in both sets                        |
| **`difference()`**           | Keeps items from the first set that aren’t in the other set(s) | 
| **`symmetric_difference()`** | Keeps all items *except* those that appear in both sets        |

 

**1. Union**

The union() method returns a new set that contains all unique items from both sets.

**Example:**
```
set1 = {"a", "b", "c"}
set2 = {1, 2, 3}

set3 = set1.union(set2)
print(set3)
```
**Using the | Operator**

You can use the | symbol instead of union() — both give the same result.

**Example:**
```
set1 = {"a", "b", "c"}
set2 = {1, 2, 3}

set3 = set1 | set2
print(set3)
```

**2. Join Multiple Sets**

You can join more than two sets at once using either union() or the | operator.

**Using union() method:**
```
set1 = {"a", "b", "c"}
set2 = {1, 2, 3}
set3 = {"John", "Elena"}
set4 = {"apple", "banana", "cherry"}

myset = set1.union(set2, set3, set4)
print(myset)
```
**Using | operator:**
```
set1 = {"a", "b", "c"}
set2 = {1, 2, 3}
set3 = {"John", "Elena"}
set4 = {"apple", "banana", "cherry"}

myset = set1 | set2 | set3 | set4
print(myset)
```
**3. Join a Set with a Tuple**

- The union() method can also combine a set with other iterable types, such as lists or tuples.
- However, the | operator works only with sets.

**Example:**
```
x = {"a", "b", "c"}
y = (1, 2, 3)

z = x.union(y)
print(z)
```
**⚠️ Note:
The | operator only works between sets.
To join a set with other types (like tuples or lists), use the union() method.**

**🧩 1. union() → Combines sets (no duplicates)**
```
a = {1, 2, 3}
b = {3, 4, 5}

print(a.union(b))  # {1, 2, 3, 4, 5}
print(a | b)       # same result
```

🟢 Returns a new set
🟠 Doesn’t change the original

**🧩 2. update() → Adds items from another set**
```
a = {1, 2, 3}
b = {3, 4, 5}

a.update(b)
print(a)  # {1, 2, 3, 4, 5}
```

🟢 Changes the original set
🟠 No new set created

**🧩 3. intersection() → Keeps common items**
```
a = {1, 2, 3}
b = {2, 3, 4}

print(a.intersection(b))  # {2, 3}
print(a & b)              # same result
```

🟢 Returns only duplicates (common values)
🟠 Doesn’t change the original set

**🧩 4. intersection_update() → Keeps common items (in-place)**
```
a = {1, 2, 3}
b = {2, 3, 4}

a.intersection_update(b)
print(a)  # {2, 3}
```

🟢 Modifies the original set

**🧩 5. difference() → Items only in the first set**
```
a = {1, 2, 3}
b = {2, 3, 4}

print(a.difference(b))  # {1}
print(a - b)            # same result
```

🟢 Returns a new set
🟠 Keeps only elements unique to the first set

**🧩 6. difference_update() → Removes common items (in-place)**
```
a = {1, 2, 3}
b = {2, 3, 4}

a.difference_update(b)
print(a)  # {1}
```

🟢 Changes the original set

**🧩 7. symmetric_difference() → Keeps all except duplicates**
```
a = {1, 2, 3}
b = {2, 3, 4}

print(a.symmetric_difference(b))  # {1, 4}
print(a ^ b)                      # same result
```

🟢 Returns items that are not common

**🧩 8. symmetric_difference_update() → Same as above, but modifies**
```
a = {1, 2, 3}
b = {2, 3, 4}

a.symmetric_difference_update(b)
print(a)  # {1, 4}
```

🟢 Updates the original set

**🧊 Python frozenset**

A frozenset is an immutable (unchangeable) version of a set.

Like normal sets, a frozenset:

- Contains unique elements (no duplicates)
- Is unordered (no index)
- Is unchangeable (but normal sets are mutable)

The key difference:

✅ You can’t add or remove elements from a frozenset.

**🪄 Creating a FrozenSet**

Use the frozenset() constructor to create one from any iterable (like a list, tuple, or set).
```
x = frozenset({"apple", "banana", "cherry"})
print(x)
print(type(x))
```
**🧩 Frozenset Methods**

Even though frozenset objects are immutable, they still support all non-modifying set operations.

| Method                   | Shortcut    | Description                                            |
| ------------------------ | ----------- | ------------------------------------------------------ | 
| `copy()`                 | —           | Returns a shallow copy                                 |  
| `difference()`           | `-`         | Returns elements in one frozenset but not the other    | 
| `intersection()`         | `&`         | Returns common elements between frozensets             |  
| `isdisjoint()`           | —           | Returns True if no common elements                     |  
| `issubset()`             | `<=` or `<` | Returns True if one frozenset is a subset of another   | 
| `issuperset()`           | `>=` or `>` | Returns True if one frozenset is a superset of another | 
| `symmetric_difference()` | `^`         | Returns elements that are not common                   |                  
| `union()`                | ``|``       | Combines all elements from both frozensets             |

**🧠 Example:**
```
a = frozenset({1, 2, 3})
b = frozenset({3, 4, 5})

print(a.union(b))              # frozenset({1, 2, 3, 4, 5})
print(a.intersection(b))       # frozenset({3})
print(a.difference(b))         # frozenset({1, 2})
print(a.symmetric_difference(b))  # frozenset({1, 2, 4, 5})
```

**🧺 Python Set Methods**
- Python provides several built-in methods that you can use to work with sets.
- These methods help you add, remove, copy, and compare elements easily.
**🧩 List of Set Methods**

| **Method**                      | **Shortcut** | **Description**                                                       |
| ------------------------------- | ------------ | --------------------------------------------------------------------- | 
| `add()`                         | —            | Adds an element to the set                                            | 
| `clear()`                       | —            | Removes all elements from the set                                     |
| `copy()`                        | —            | Returns a copy of the set                                             |
| `difference()`                  | `-`          | Returns elements that are in one set but not in another               | 
| `difference_update()`           | `-=`         | Removes elements found in another specified set                       | 
| `discard()`                     | —            | Removes a specified element (no error if element doesn’t exist)       |
| `intersection()`                | `&`          | Returns only elements found in both sets                              |
| `intersection_update()`         | `&=`         | Keeps only items present in both sets (changes the original set)      |
| `isdisjoint()`                  | —            | Returns True if two sets have no elements in common                   |
| `issubset()`                    | `<=` or `<`  | Returns True if all elements of this set are present in another set   | 
| `issuperset()`                  | `>=` or `>`  | Returns True if this set contains all elements of another set         |
| `pop()`                         | —            | Removes and returns a random element from the set                     |
| `remove()`                      | —            | Removes a specified element (raises an error if it doesn’t exist)     | 
| `symmetric_difference()`        | `^`          | Returns elements that are in either set, but not in both              |  
| `symmetric_difference_update()` | `^=`         | Keeps only elements not found in both sets (updates the original set) | 
| `union()`                       | ``|``        | Combines all elements from both sets (returns a new set)              |
| `update()`                      | ``|=``       | Adds elements from another set (updates the original set)             |




















