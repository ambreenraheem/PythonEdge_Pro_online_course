Date:28-January-2026

## Instructor: Ambreen Abdul Raheem
#### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)

#### OOPs in Python

### Object-Oriented Programming (OOP) in Python
#### A Complete Beginner's Guide

### What is OOP?
OOP (Object-Oriented Programming) is a way of writing code by organizing it around real-world things called objects.\
Instead of writing a long list of instructions (like a recipe), OOP lets you model your program like the real world, with things (objects) that have properties (data) and behaviors (actions).



### Before OOP — Procedural Style:
```
# Managing a student without OOP

student_name = "Ambreen"
student_age = 22
student_grade = "A"

def show_student(name, age, grade):
    print(f"Name: {name}, Age: {age}, Grade: {grade}")

show_student(student_name, student_age, student_grade)
```

⚠️ Problem: If you have 100 students, you'd need 300 variables. It becomes messy fast!

In OOP, we organize our code around objects, which are like little self-contained units. These objects are created from classes, which act like blueprints or cookie cutters.

Let's break down the main ideas:
- Classes and Objects: Imagine a 'Car' blueprint (the class). From this blueprint, you can build many different 'Car' models (the objects), like a 'red sports car' or a 'blue family sedan'. Each car object has its own features (like color, speed, model – these are attributes) and things it can do (like accelerate, brake, turn on lights – these are methods).
- Encapsulation: This is like putting all the car's engine parts, wires, and controls inside the car's body. You don't need to know exactly how the engine works to drive the car; you just use the steering wheel and pedals. Encapsulation keeps an object's internal workings private and tidy, only letting you interact with it through defined methods.
- Inheritance: Imagine you have a 'Vehicle' blueprint. Instead of starting from scratch for a 'Car' blueprint, you can say, "A Car is a type of Vehicle." This means the 'Car' blueprint automatically gets all the basic features and abilities of a 'Vehicle' (like having wheels, being able to move) and then you just add the specific 'Car' stuff. This saves time and makes your code reusable.
- Polymorphism: This means "many forms." It allows different objects to respond to the same command in their own way. For example, if you tell a 'Car' object to start(), it might turn on an engine. If you tell an 'ElectricCar' object to start(), it might power up a battery. The command start() is the same, but the action is different depending on the type of car.
- By using these ideas, OOP helps us build programs that are more organized, easier to fix, and can be expanded more easily without breaking everything else. It makes coding feel more like managing a team of specialized workers than a giant, tangled ball of yarn!

Example # 01:
```
class Student:
    """Here we have created class."""
    name= "ABC College" # class attribute
    
    # created method function
    def show_name():
        print(f"Welcome to my college!")

print(Student.name)
Student.show_name()
```

## Why Do We Need OOP?
 
| Problem Without OOP | How OOP Solves It |
|---|---|
| Code becomes very long and hard to read | OOP groups related data and functions together |
| Hard to reuse code | Inheritance lets you reuse existing code |
| Hard to maintain large projects | Each class is independent and manageable |
| Data is not protected | Encapsulation hides sensitive data |
| Same function behaves differently in different contexts | Polymorphism handles this cleanly |

## Core Concepts of OOP
 
### 1. Class & Object
 
> A **Class** is like a **blueprint** (template).  
> An **Object** is a **real thing** made from that blueprint.
 
🏠 Think of it like: A class is the architectural plan of a house. Objects are the actual houses built from that plan.
 
```python
# Blueprint (Class)
class Car:
    color = "Red"
    brand = "Toyota"
 
# Object (Real thing)
my_car = Car()           # Creating an object from the class
print(my_car.color)      # Red
print(my_car.brand)      # Toyota
 
your_car = Car()
your_car.color = "Blue"  # Changing this object's color only
print(your_car.color)    # Blue
print(my_car.color)      # Red (my_car is not affected)
```
 
### 2. Attributes & Methods
 
**Attributes** = Data stored in a class (variables)  
**Methods** = Actions a class can perform (functions inside a class)
 ```
class Dog:
    # Attribute
    species = "Canine"
 
    # Method (action)
    def bark(self):
        print("Woof! Woof!")
 
    def fetch(self, item):
        print(f"Fetching the {item}!")
 
# Creating an object
my_dog = Dog()
print(my_dog.species)    # Canine  ← accessing attribute
my_dog.bark()            # Woof! Woof!  ← calling method
my_dog.fetch("ball")     # Fetching the ball!
```
 
💡 **What is `self`?**\  
 `self` refers to the **current object**. When you call `my_dog.bark()`, Python automatically passes `my_dog` as `self`. It's how the method knows which object it belongs to.
 
### 3. The `__init__` Constructor
 
> `__init__` is a **special method** that runs **automatically** when you create an object. It's used to set up initial values.
 
```
class Person:
    def __init__(self, name, age):  # Constructor
        self.name = name            # Setting attribute
        self.age = age              # Setting attribute
 
    def greet(self):
        print(f"Hi! I'm {self.name} and I'm {self.age} years old.")
 
# When we create a Person object, __init__ runs automatically
p1 = Person("Ambreen", 22)
p2 = Person("Sara", 25)
 
p1.greet()   # Hi! I'm Ambreen and I'm 22 years old.
p2.greet()   # Hi! I'm Sara and I'm 25 years old.
```

