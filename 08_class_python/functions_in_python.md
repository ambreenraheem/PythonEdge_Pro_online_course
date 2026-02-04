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

### Types of Function Arguments

Python supports various types of arguments that can be passed at the time of the function call. In Python, we have the following function argument types in Python, Let's study more:

**1. Default Arguments**\
You can provide default values for arguments. If a value is not provided during the function call, the default value is used.\

```
def myFun(x, y=50):
    print("x: ", x)
    print("y: ", y)
```

```
def greet_language(name, language="English"):
    """This function greets a person in a specified language, with English as default."""
    if language == "English":
        print(f"Hello, {name}!")
    elif language == "Spanish":
        print(f"Hola, {name}!")
    elif language == "French":
        print(f"Bonjour, {name}!")
    else:
        print(f"Greetings, {name}! (in {language})")

# Calling with default argument
greet_language("Shazia")

# Calling with a specified argument
greet_language("Raheem", "Spanish")
greet_language("Farooq", "French")
```

**Default Arguments with User Input:**\
A default argument is a parameter that assumes a default value if a value is not provided in the function call for that argument.

This example demonstrates a function that takes user input for a name and uses a default argument for the greeting language. The user can optionally specify a different language.

```
def greet_with_options(name, language="English"):
    """Greets a person by name in a specified language, defaulting to English."""
    if language.lower() == "english":
        return f"Hello, {name}!"
    elif language.lower() == "spanish":
        return f"Hola, {name}!"
    elif language.lower() == "french":
        return f"Bonjour, {name}!"
    else:
        return f"Greetings, {name}! (in {language})"

# Get name from user
user_name_input = input("Please enter your name: ")

# Ask if user wants to specify a language (optional)
language_choice = input("Enter a language (e.g., Spanish, French) or leave blank for English: ")

# Call the function with user input and handle the optional language
if language_choice:
    greeting = greet_with_options(user_name_input, language=language_choice)
else:
    greeting = greet_with_options(user_name_input)

print(greeting)
```
**2. Keyword Arguments:**\
Function using **keyword arguments**, allows us to specify the parameter names, so the order no longer matters.
```
# Example: 01
def student(fname, lname):
    print(fname, lname)

student(fname='PythonEdge-Pro', lname='Practice')
student(lname='Practice', fname='PythonEdge-Pro')
```
```
# Example: 02
def greet(name, message):
    print(f"Hello, {name}! {message}")

# Calling with keyword arguments (order does not matter)
greet(name="Bob", message="Nice to meet you!")

# Calling with keyword arguments in a different order
greet(message="Hope you're having a good day!", name="Dawood")
```

**3. Positional Arguments**\
In positional arguments, values are assigned to parameters based on their order in the function call.

You can also combine positional and keyword arguments. The rule is that all positional arguments must come before any keyword arguments.
```
# Example: 01
# Calling with mixed arguments (positional first, then keyword)
greet("Rashid", message="Hello there!")

# This would cause a syntax error: keyword argument cannot precede a positional argument
# greet(message="Hi!", "Saleem")
```
```
# Example: 02
def nameAge(name, age):
    print("Hi, I am", name)
    print("My age is ", age)

print("Case-1:")
nameAge("Sajid", 27)

print("\nCase-2:")
nameAge(27, "Sajid")
```

**4. Arbitrary Arguments**\
In Python Arbitrary Keyword Arguments, *args and **kwargs can pass a variable number of arguments to a function using special symbols. There are two special symbols:

- *args in Python (Non-Keyword Arguments)
- **kwargs in Python (Keyword Arguments)
This code separately shows non-keyword (*args) and keyword (**kwargs) arguments in the same function.
```
def func_with_arbitrary_args(arg1, *args, **kwargs):
    print(f"First argument: {arg1}")
    if args:
        print(f"Non-keyword arguments (*args): {args}")
    if kwargs:
        print(f"Keyword arguments (**kwargs): {kwargs}")

# Calling the function with arbitrary arguments
func_with_arbitrary_args("Hello", 1, 2, 3, key1="value1", key2="value2")

print("\n")
func_with_arbitrary_args("Greetings", "a", "b", greeting="Hi", farewell="Bye")

print("\n")
func_with_arbitrary_args("Only positional arg")

print("\n")
func_with_arbitrary_args("Only keyword args (after positional)", city="New York", temp=25)
```

### Function Within Functions (Inner/Nested Function) — Definition

A function within a function is called an inner or nested function. It is a function created inside another function and can use the variables and data from the outer (enclosing) function’s scope. This technique is used to hide implementation details, protect logic from outside access, and keep related code structured and organized.

**In easy words:**

A function within a function means putting one function inside another function.\
The inside function can use the things (like variables) from the outside function.

We do this to keep code private, keep things neat, and group related work together.

#### Python Inner Functions (Nested Functions) — Simple Explanation

In Python, an inner function is a function written inside another function.

They are useful for:

- Encapsulation – Keeping helper code hidden so it can't be used from outside.
- Better organization – Placing related code together makes programs easier to read.
- Using outer variables – Inner functions can use data from the outer function.
- Closures & decorators – Used in advanced Python features where functions remember values.

This helps make programs cleaner, safer, and easier to manage.

**Example 1: Simple Inner Function**
```
def outer_function():
    message = "Hello from outer function!"

    def inner_function():
        print(message)  # Using variable from outer function

    inner_function()  # Calling inner function

outer_function()
```

The inner function can use the message variable from the outer function.

**Example 2: Inner Function as Helper**

```
def calculate_square(number):

    def multiply(n):
        return n * n   # Helper function

    result = multiply(number)
    print("Square is:", result)

calculate_square(5)
```

Here, multiply() is hidden inside calculate_square() because it's only needed there.

**Example 3: Closure (Function Remembering Value)**

```
def outer(x):

    def inner(y):
        return x + y  # Remembers x

    return inner

add_five = outer(5)
print(add_five(3))
```

Even though outer() finished, the inner function remembers x = 5. This is called a closure.

**Inner functions help keep code private, organized, and powerful.**

**In this example:**

- inner_function is defined inside outer_function.
- inner_function can access message (passed to outer_function) and greeting (defined within outer_function).
- When outer_function is called, it returns inner_function. This returned function (e.g., my_greeting) remembers the message and greeting from when outer_function was executed, forming a closure.

```
def outer_function(message):
    # This is a variable in the outer function's scope
    greeting = "Hello from outer function!"

    def inner_function(name):
        # inner_function can access 'greeting' and 'message' from outer_function's scope
        print(f"{greeting} {message}, {name}!")

    # The outer function returns the inner function
    return inner_function

# Call the outer function, which returns the inner function
my_greeting = outer_function("Welcome")

# Now, call the returned inner function
my_greeting("Alice")
my_greeting("Bob")

# Another example with a different message
another_greeting = outer_function("Good to see you")
another_greeting("Charlie")
```

**Scope of Variables in Inner Functions**

Inner (nested) functions follow Python’s LEGB rule for finding variables:

- L → Local (inside the inner function)
- E → Enclosing (inside the outer function)
- G → Global (file-level variables)
- B → Built-in (Python’s reserved names like print, len)

**An inner function can read variables from the outer function.
To change them, we use the keyword nonlocal.**

**Example 1: Accessing Outer Variable**

```
def outer():
    message = "Hello from outer"

    def inner():
        print(message)  # Using outer variable

    inner()

outer()
```

The inner function can use message because it belongs to the enclosing scope.

**Example 2: Changing Outer Variable (nonlocal)**

```
def outer():
    a = 10

    def inner():
        nonlocal a
        a = 20
        print("Inside inner:", a)

    inner()
    print("Inside outer:", a)

outer()
```

nonlocal tells Python to modify the outer variable instead of creating a new local one.

**Example 3: Closure (Remembering Value)**

```
def outer(text):

    def inner():
        print(text)

    return inner

my_func = outer("Closures are powerful!")
my_func()
```

Even after outer() finishes, inner() remembers text. This is called a closure.

**Real-World Uses of Inner Functions**

```
# 1. Encapsulation (Hidden Helper Function)
def process_data(data):

    def clean():
        return [item.strip() for item in data]

    return clean()

print(process_data(["  Python  ", "  Code  "]))
```

The helper function clean() is hidden inside process_data().

```
# 2. Wrappers (Logging / Decorators)
def logger(func):

    def wrapper(*args, **kwargs):
        print(f"Calling {func.__name__} with {args} {kwargs}")
        return func(*args, **kwargs)

    return wrapper

@logger
def add(a, b):
    return a + b

print(add(3, 4))
```

The inner function wrapper() runs before the real function — this idea is used in decorators.

### Return Statement in Python Functions

The return statement stops a function and sends a value back to where the function was called.

A function can return:

- A number
- A string
- A list

Multiple values (as a tuple)\
Or nothing (then it returns None)

```
Example
def square_value(num):
    return num ** 2

print(square_value(2))
print(square_value(-4))
```

The function calculates the square and returns the result.

**Pass by Reference vs Pass by Value (Python Behavior)**

In Python, variables point to objects. What happens inside a function depends on the object type.

Mutable Objects (can change)

```
# Examples: list, dictionary, set
# Changes inside the function affect the original object.

def change_list(x):
    x[0] = 20

lst = [10, 11, 12]
change_list(lst)
print(lst)
```
The list changed.

Immutable Objects (cannot change)

```
# Examples: int, float, string, tuple

Changes inside the function do not affect the original value.

def change_number(x):
    x = 20

a = 10
change_number(a)
print(a)
```

The number stayed the same.

**Note: Python actually uses pass-by-object-reference.**

**Recursive Functions**

A recursive function is a function that calls itself.\
It must have a base case (a stopping condition), or it will run forever.

```
# Example: Factorial

Factorial of 4 = 4 × 3 × 2 × 1

def factorial(n):
    if n == 0:      # Base case
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(4))
```

The function keeps calling itself until it reaches the base case (n == 0).

### Anonymous Functions (Lambda Functions) in Python
An anonymous function is a function without a name.\
In Python, we create them using the lambda keyword instead of def.

They are usually used for short, simple tasks where writing a full function is not necessary.

```
def cube(x): return x*x*x   # without lambda
cube_l = lambda x : x*x*x  # with lambda
​
print(cube(7))
print(cube_l(7))
```
```
# Normal Function (using def)
def cube(x):
    return x * x * x

print(cube(7))
```

**Anonymous Function (using lambda)**
```
cube_l = lambda x: x * x * x

print(cube_l(7))
```

Both functions do the same work, but lambda lets us write it in one line.

**Where Lambda is Commonly Used**

Lambda functions are often used with functions like:
- map() – apply a function to every item
- filter() – select items based on a condition
- sorted() – sort with custom rules
```
# Example with map()
numbers = [1, 2, 3, 4]
squares = list(map(lambda x: x**2, numbers))
print(squares)
```
**In simple words**\
**A lambda function is a small, one-line function without a name, used when we need quick, simple.**
























