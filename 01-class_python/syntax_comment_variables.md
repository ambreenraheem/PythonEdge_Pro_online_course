Date:20-September-2025
## Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
### Python
**Installation:** For installation, go to the Python official site and click here: https://www.python.org/

### 01 # Python Syntax:
Python has a simple syntax similar to the English language.

**- Execute Python Syntax**
- As we learned in the previous page, Python syntax can be executed by writing directly in the Command Line:
```
print("Hello, World!")
```
**output** Hello, World!

- Or by creating a Python file on the server, using the .py file extension, and running it in the Command Line:
```
C:\Users\Your Name>python myfile.py
```

### 02 # Python Comment:
Comments can be used to explain Python code to other people and for you as well. Comments can be used to make the code more readable and understandable. Comments can be used to prevent execution when testing code.
- Creating a Comment
Comments start with a #, and Python will ignore them:

Example: Get your own Python Server
```
#This is a comment
print("Hello, World!")
```
Comments can be placed at the end of a line, and Python will ignore the rest of the line:\
Example
```
print("Hello, World!") #This is a comment
```
A comment does not have to be text that explains the code; it can also be used to prevent Python from executing code:

Example
```
#print("Hello, World!")
print("Cheers, Mate!")
```
### 03 # Python Variable:
Variables are containers for storing data values.

**i-Creating Variables**
- Python does not have a command for declaring a variable.
- A variable is created the moment you first assign a value to it.
- You don’t have to assign a specific type when declaring variables, and their type can change after being assigned.
- A variable could be in numbers or in a string as well.

**Example # 01**
```
x = "Ambreen"   # Here, "x" is a variable
y = 40          # Here, "y" is a variable
z = "Karachi"   # Here, "z" is a variable
print(x)
print(y)
print(z)
```
**OUTPUT # 01**\
Ambreen\
40\
Karachi

**Example # 02**
```
a = 235
b = 55
c = 5896
# mathematical operation
print(a + b)
print(a * b)
print(c - a)
```
**OUTPUT # 02**\
290\
12925\
5661

**Example # 03**
```
# more presentable:
h = 58
i = 654
j = 258
# again mathematical operation with string
print("This is Addition: ", i + j)
print("This is Multiplication: ", h * i)
```
**OUTPUT # 03**\
This is Addition: 912\
This is Multiplication: 37932\
**Here, with the help of a variable, you don't need to repeat the line of code again and again, if you are writing multiple strings or lines code or operators.**

**ii-class/type of a variable:**
To know which type of variable you have made, write the type, and it will show you the type or class of variable in the output.

```
print(type(x))
print(type(y))
```

**OUTPUT OF DATA TYPE**\
<class 'str'>\
<class 'int'>\
**Here <class> means the data type of the variable value.**

**iii-RULE TO ASSIGN A VARIABLE:**
- The variable should contain letters, numbers, or underscores.
- Do not start with numbers.
- Do not use special characters like:!, @, #, $, %, ^, &, *.
- Spaces are not allowed, always use "Camel Case" like: myVariableName, or "Pascal Case" like: MyVariableName, or "Snake Case" like: my_variable_name.
- Do not use keywords used in functions like (break, mean, median, test, etc)
- Short and descriptive.
- Case sensitivity (lowercase, uppercase letters- [go for lowercase letters because it is easy to remember])

**iv-Keywords in Python: (not for use of variable name):**
- False, class, Finally, return, None, def, continue, for, lambda, try, True, from, nonlocal, while, del, global, not, print, if, type.

**v-Assign Multiple Values:**\
In Python, you can assign values to multiple variables simultaneously in a single line.

**Example # 01**\
```
a, b, c = "Potatoes", "Carrots", "Peas"
print(a)
print(b)
print(c)
```

**OUTPUT # 01**\
Potatoes\
Carrots\
Peas

**Example # 02**\
```
f, g, h = "I like Fish.", "You Like Mango.", "They like to play."
print(f)
print(g)
print(h)
```

**OUTPUT # 02**
I like Fish.\
You Like Mango.\
They like to play.

**vi-One Value to Multiple Variables:**\
In Python, you can also assign the same value to multiple variables in a single line.

```
x = y = z = "Tehreem"
print(x)
print(y)
print(z)
```

**OUTPUT # 03**\
Tehreem\
Tehreem\
Tehreem

**Example # 02**\
```
i= j= k= l= "Tehreem is five years old."
print(i)
print(j)
print(k)
print(l)
```
**OUTPUT # 02**\
Tehreem is five years old.\
Tehreem is five years old.\
Tehreem is five years old.\
Tehreem is five years old.

**vii-Output variables:**\
In Python, the print() function is commonly used to display the values of variables.



 




