Date:28-September-2025

## Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)

#### 🔤 What is a string?
A string is just text inside quotes.
- It can have letters, numbers, or symbols.
- Use single ' or double " quotes.
- Assigning a string to a variable is done with the variable name followed by an equal sign and the string:
```
name = 'ambreen'
greetings = "Hello "
print(greetings,name)
```
**Quotes Inside Quotes**\
You can use quotes inside a string, as long as they don't match the quotes surrounding the string:
```
print("It's my car.")
print("I am working with 'Ahmed'.")
print('"Tehreem" is my friend.')
```
**Multiline Strings**\
You can assign a multiline string to a variable by using three quotes or three single quotes and just print that variable:
```
intro = """Hi, this is ambreen.
I am teaching Python from the basic to the advanced level.
I am a Data Analyst."""
print(intro)
```
```
intro = '''Hi, this is ambreen.
I am teaching Python from the basic to the advanced level.
I am a Data Analyst.'''
print(intro)
```
#### F-Strings in Python

F-Strings were introduced in Python 3.6 and are now the recommended way to format strings.

To make an f-string, just put the letter f before your string and use curly brackets {} inside the string to insert variables, expressions, or operations.
**Example 1 – Basic F-String**
```
age = 36
txt = f"My name is John, I am {age}"
print(txt)
```

**Placeholders and Modifiers**\
Inside the curly brackets, you can put:

- Variables
- Math operations
- Functions
- Or formatting modifiers

**Example 2 – Using a Variable**
```
price = 59
txt = f"The price is {price} dollars"
print(txt)
```

**Example 3 – Using a Modifier**\
You can add a modifier after a colon : to format the value.\
For example, .2f means “show as a number with 2 decimal places”.
```
price = 59
txt = f"The price is {price:.2f} dollars"
print(txt)
```

**Example 4 – Doing Math Inside an F-String**\
You can even perform calculations directly inside {}:
```
txt = f"The price is {20 * 59} dollars"
print(txt)
```




















