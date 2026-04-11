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


