Date:30-January-2026

### Instructor: Ambreen Abdul Raheem
#### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)

#### Functions in Python
Python Tutor: https://pythontutor.com/

### Python pass Statement — Simple Explanation

- The pass statement is a do-nothing placeholder.
- When Python runs it, nothing happens, but it keeps the code syntactically correct.
We use pass when a block of code is required, but we don’t want to write the logic yet.

**1. In Functions**\
Used when a function is planned but not written yet.
```
def fun():
    pass

fun()
```

The function exists, but it does nothing.

**2. In Conditional Statements**\
Used when a condition needs a block, but no action is needed.
```
x = 10

if x > 5:
    pass  # Nothing happens here
else:
    print("x is 5 or less")
```

If x > 5, the program simply moves on.

**3. In Loops**\
Used when you want the loop structure but no action for some case.
```
for i in range(5):
    if i == 3:
        pass
    else:
        print(i)
```

When i is 3, nothing happens.

**4. In Classes**\
Used to create empty classes or methods as placeholders.
```
class EmptyClass:
    pass

class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        pass
```

The structure is ready, even if logic is not added yet.

**In Simple Words**
- pass means “I will write this code later.”
- It keeps programs error-free while building the structure.















