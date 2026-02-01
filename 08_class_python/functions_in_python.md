Date:28-January-2026

### Instructor: Ambreen Abdul Raheem
#### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)
#### Functions in Python

Python Tutor: https://pythontutor.com/

### Functions in Python
A function is a block of organized, reusable code that is used to perform a single, related action.\
Functions provide better modularity for your application and a high degree of code reusing.

#### Defining a Function
In Python, you define a function using the `def` keyword, followed by the function's name, parentheses `()`, and a colon `:`.\
Any input parameters or arguments should be placed within these parentheses. The code block within every function starts with a colon (`:`) and is indented.

**In this example:**
- `def greet():` defines a function named `greet` that takes no arguments.
- The string `"""This function prints a simple greeting."""` is a docstring, which is a brief explanation of what the function does. It's good practice to include docstrings.
- `print("Hello, Python functions!")` is the body of the function, the code that gets executed when the function is called.
- `greet()` calls the function, executing its code block.

### A simple function definition
```
def greet():
    """This function prints a simple greeting."""
    print("Hello, Python functions!")

# Calling the function
greet()
```

**Note: The code inside the function must be indented. Python uses indentation to define code blocks.**

**Function names are crucial for several reasons:**  

- Identification: A function name gives a unique identity to a block of code. Without it, you wouldn't be able to refer to or call that specific set of instructions.
- Readability and Clarity: A well-chosen function name describes what the function does. This makes your code much easier to read and understand, both for yourself and for other developers.
- Reusability: The name allows you to call the function repeatedly from different parts of your program without rewriting the code. It's like giving a specific tool a name so you can ask for it when you need it.
- Organization: Names help organize your code into logical units, making it easier to manage and navigate larger programs.
  
**In essence, a function name is its label, telling you what it is and how to use it.**

When writing function names in Python, it's important to follow certain conventions and best practices for readability and maintainability:

- Lowercase with underscores (snake_case): This is the most common and recommended convention for function names in Python. For example: calculate_sum, get_user_data, print_hello.
- Descriptive and concise: The name should clearly indicate what the function does. Avoid overly short or ambiguous names. For example, add_two_numbers is better than add if the function specifically adds two numbers.
- Use verbs: Function names often start with a verb because functions perform actions. Examples: get_, set_, calculate_, print_, is_.
- Avoid keywords: Do not use Python's reserved keywords (like def, class, if, for, while, return) as function names.
- Be consistent: Once you choose a naming style, stick to it throughout your project.
- Here are some examples of good and bad function names:

**Good: calculate_average(), is_valid_email(), fetch_data_from_api()**

**Bad: avg(), check(), getData() (uses camelCase, not idiomatic Python), _f1() (too generic)**

![image]("C:\Users\HOME\Downloads\function-python.png")
 
### Functions with Arguments

Functions can take input values, called arguments, which are specified in the parentheses when defining the function.
These arguments act as variables within the function's scope.

**For more understanding: Think of arguments like ingredients for a recipe. When you make a cake (your function), you need flour, sugar, and eggs (your arguments).
You pass these 'ingredients' to the function so it knows what to work with. Inside the function, these ingredients are called 'parameters'.
So, when you call a function, you supply the arguments, and the function uses its parameters to receive those arguments and perform its task.**

```
# A function with one argument:
def my_function(fname):
  print(fname + " Khan") # fname means first name

my_function("Fasiullah")  
my_function("Mehwish")
my_function("Sehrish")
```

**In the `greet_name` example:**
- `name` is a parameter that acts as a placeholder for the value you pass when calling the function.
- When you call `greet_name("Kashif")`, "Kashif" is the argument passed to the `name` parameter.

**In the `add_numbers` example:**
- `num1` and `num2` are parameters.
- The function calculates their sum and uses the `return` keyword to send the result back to the caller.

```
# First function that takes one argument
def greet_name(name):
    """This function greets the person passed in as an argument."""
    print(f"Hello, {name}!")

# Calling the function with an argument
greet_name("Kashif")
greet_name("Ahmed")

# Second function that takes multiple arguments
def add_numbers(num1, num2):
    """This function takes two numbers and returns their sum."""
    return num1 + num2

# Calling the function and storing the result
result = add_numbers(5, 3)
print(f"The sum is: {result}")

print(f"Another sum: {add_numbers(10, 20)}")
```
```
# Third function that takes multiple arguments 
def my_function(animal, name):
  print("I have a", animal)
  print("My", animal + "'s name is", name)

my_function(animal = "dog", name = "Buddy")
```

### Parameters vs Arguments
The terms parameter and argument can be used for the same thing: information that are passed into a function.

From a function's perspective:
- **A parameter** is the variable listed inside the parentheses in the function definition.
- **An argument** is the actual value that is sent to the function when it is called.

**For Example:**
```
def my_function(name): # name is a parameter
  print("Hello! I am ", name)

my_function("Shazia") # "Shazia" is an argument
```

### Function with User Input
```
def greet_user_input():
    """Prompts the user for their name and prints a personalized greeting."""
    user_name = input("Please enter your name: ")
    print(f"Hello, {user_name}! Welcome to Python functions.")

# Call the function to get user input and greet them
greet_user_input()
```















