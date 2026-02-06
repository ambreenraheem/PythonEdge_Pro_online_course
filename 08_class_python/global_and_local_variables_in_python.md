🔹 Local Variables in Python

A local variable is a variable that is defined inside a function. Its scope (area where it can be used) is limited only to that function.

Key characteristics:

Created when the function starts execution

Destroyed when the function finishes

Not accessible outside the function

Each function call gets its own copy

✅ Example 1 — Valid Use of a Local Variable
def greet():
    msg = "Hello from inside the function!"
    print(msg)

greet()
