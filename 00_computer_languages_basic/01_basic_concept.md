## 💻 What is a Computer Language?

A computer language is a means by which humans can communicate with a computer.\
Since computers only understand binary (0s and 1s), we use special languages to give them instructions.

### 🏷️ Types of Computer Languages
**01. Machine Language (Low-level)**
- Written in 0s and 1s (binary).
- Directly understood by the computer.
- Very hard for humans to write.\
Example: 10110000 01100001

**02. Assembly Language**
- Uses short codes (mnemonics) instead of 0s and 1s.
- Easier than machine code but still close to hardware.
- Needs an assembler to convert to machine language.\
Example:
```
MOV A, 5
ADD A, 2
```

**03. High-Level Language (HLL)**
- Easy to read and write (looks like English).
- Needs a compiler or interpreter to convert into machine code.
- Examples: Python, C, Java, JavaScript.\
Example (Python):
```
print("Hello, World!")
```
**📝 In short**
- Computer language = way to talk to computers.
- Low-level (machine & assembly) = fast but hard to learn.
- High-level (Python, Java, etc.) = easy for humans, converted to binary for computers.

## What is a Programming Language and a Scripting Language
**🖥️ Programming Language**
- A programming language is used to write full software or applications.
- It usually needs a compiler to convert code into machine language.
- Often used for big, complex programs (like operating systems, games, applications).\
Examples: C, C++, Java

**👉 Think of it like building a big house from scratch.**

**📜 Scripting Language**
- A scripting language is used to write small programs (scripts) that automate tasks.
- It usually runs through an interpreter (line by line, no compilation).
- Often used for automation, web tasks, and data analysis.\
Examples: Python, JavaScript, PHP, Ruby, Bash

**👉 Think of it like writing a shortcut or quick tool inside the house.**

| Feature       | Programming Language      | Scripting Language               |
| ------------- | ------------------------- | -------------------------------- |
| Execution | Compiled (before running) | Interpreted (runs line by line)  |
| Usage     | Build big software & apps | Automate tasks, control software |
| Speed     | Faster                    | Slower (but simpler)             |
| Examples  | C, C++, Java              | Python, JavaScript, PHP          |


**🎯 Super Simple Trick to Remember**
- Programming language = Build the car 🚗
- Scripting language = Drive or control the car 🕹️

## 🐍 Why Python is both a Scripting and Programming Language?
#### 🔹 Python as a Scripting Language
- Runs line by line (interpreted).
- You don’t need to compile it before running.
- Great for automation, quick tasks, data analysis, and small scripts.\
Example 01- (script):
```
fruits = ["apples", "bananas", "mango"]

for fruit in fruits:
    print("I like", fruit)
```
**Output-01**

I like apples
I like bananas
I like mango

Example 02- (script):
```
# This is a simple example of a for loop with an if-else statement in Python

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

for number in numbers:
  # Check if the number is even or odd
  if number % 2 == 0:
    print(number, "is even")
  else:
    print(number, "is odd")
```
**Output-02**

1 is odd
2 is even
3 is odd
4 is even
5 is odd
6 is even
7 is odd
8 is even
9 is odd
10 is even\
**👉 This script quickly automates a boring task.**

#### 🔹 Python as a Programming Language
- You can build large-scale applications with it.
- Supports Object-Oriented Programming (OOP), functions, error handling, libraries, etc.
- Used for web development, AI, ML, finance, game development, and more.\
Example (application):
```
class Car:
    def __init__(self, brand, speed):
        self.brand = brand
        self.speed = speed
    
    def drive(self):
        print(f"{self.brand} is driving at {self.speed} km/h")

my_car = Car("Tesla", 120)
my_car.drive()
```
**Output-03**

Tesla is driving at 120 km/h

**👉 This looks like real programming, not just a quick script.**

**⚡ In short**

Scripting Language side: Python is easy to use, interpreted, and used for automation.

On the programming language side, Python is a powerful and structured language, often used for large-scale applications.

That’s why Python is called a general-purpose language → It can be both.















