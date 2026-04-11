Date: 05- April- 2026

## Instructor: Ambreen Abdul Raheem
#### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)

### Four Pillars of OOP:

### 01. Encapsulation
 
> **Encapsulation** means **hiding** the internal details of an object and only showing what's necessary.
 
🔐 Think of it like an ATM machine — you use the buttons and screen, but you don't see the internal wiring.
 
```python
class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.__balance = balance    # __ makes it PRIVATE (hidden)
 
    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount
            print(f"Deposited Rs.{amount}. New balance: Rs.{self.__balance}")
 
    def withdraw(self, amount):
        if amount > self.__balance:
            print("Insufficient funds!")
        else:
            self.__balance -= amount
            print(f"Withdrawn Rs.{amount}. Remaining: Rs.{self.__balance}")
 
    def get_balance(self):          # Controlled access to private data
        return self.__balance
 
account = BankAccount("Ambreen", 5000)
account.deposit(1000)              # Deposited Rs.1000. New balance: Rs.6000
account.withdraw(2000)             # Withdrawn Rs.2000. Remaining: Rs.4000
 
# Trying to access private data directly — this will FAIL:
# print(account.__balance)        # AttributeError!
 
# Correct way — use the method:
print(account.get_balance())       # 4000
```
 
> ✅ This protects your data from being accidentally changed from outside the class.
 
---
 
### 02. Inheritance
 
> **Inheritance** lets a new class **inherit** (take) properties and methods from an existing class.
 
👨‍👩‍👧 Think of it like a child inheriting traits from parents — but also having their own unique traits.
 
```python
# Parent class (Base class)
class Animal:
    def __init__(self, name):
        self.name = name
 
    def breathe(self):
        print(f"{self.name} is breathing.")
 
    def eat(self):
        print(f"{self.name} is eating.")
 
# Child class (Derived class) — inherits from Animal
class Dog(Animal):
    def bark(self):
        print(f"{self.name} says: Woof!")
 
class Cat(Animal):
    def meow(self):
        print(f"{self.name} says: Meow!")
 
# Dog gets all Animal methods PLUS its own
dog = Dog("Buddy")
dog.breathe()    # Buddy is breathing.   ← inherited from Animal
dog.eat()        # Buddy is eating.      ← inherited from Animal
dog.bark()       # Buddy says: Woof!     ← Dog's own method
 
cat = Cat("Whiskers")
cat.breathe()    # Whiskers is breathing.
cat.meow()       # Whiskers says: Meow!
```
 
#### Overriding a Parent Method:
```python
class Animal:
    def sound(self):
        print("Some generic animal sound")
 
class Lion(Animal):
    def sound(self):                         # Overriding the parent method
        print("ROAR! 🦁")
 
a = Animal()
a.sound()    # Some generic animal sound
 
l = Lion()
l.sound()    # ROAR! 🦁  ← uses its own version
```
 
---
 
### 03. Polymorphism
 
> **Polymorphism** means **"many forms"**. The same method name behaves differently depending on the object calling it.
 
```python
class Shape:
    def area(self):
        pass  # To be defined in child classes
 
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
 
    def area(self):
        return 3.14 * self.radius ** 2
 
class Rectangle(Shape):
    def __init__(self, width, height):
        self.width = width
        self.height = height
 
    def area(self):
        return self.width * self.height
 
class Triangle(Shape):
    def __init__(self, base, height):
        self.base = base
        self.height = height
 
    def area(self):
        return 0.5 * self.base * self.height
 
# Same method name "area()" — different behavior for each shape!
shapes = [Circle(5), Rectangle(4, 6), Triangle(3, 8)]
 
for shape in shapes:
    print(f"{shape.__class__.__name__} area: {shape.area()}")
 
# Output:
# Circle area: 78.5
# Rectangle area: 24
# Triangle area: 12.0
```
 
> 💡 One method name (`area`), but it behaves differently based on which object calls it. That's polymorphism!
 
---
 
### 04. Abstraction
 
> **Abstraction** means hiding **complex implementation** and showing only the **essential features**.
 
```python
from abc import ABC, abstractmethod
 
# Abstract class — cannot be used directly
class Vehicle(ABC):
    @abstractmethod
    def start_engine(self):     # Must be implemented by child classes
        pass
 
    @abstractmethod
    def stop_engine(self):
        pass
 
    def fuel_type(self):        # Normal method — shared by all
        return "Petrol/Diesel"
 
class Car(Vehicle):
    def start_engine(self):
        print("Car engine started: Vroom! 🚗")
 
    def stop_engine(self):
        print("Car engine stopped.")
 
class Motorcycle(Vehicle):
    def start_engine(self):
        print("Motorcycle engine started: Brap! 🏍️")
 
    def stop_engine(self):
        print("Motorcycle engine stopped.")
 
# v = Vehicle()     # ❌ Error! Cannot create object of abstract class
 
car = Car()
car.start_engine()      # Car engine started: Vroom! 🚗
car.stop_engine()       # Car engine stopped.
print(car.fuel_type())  # Petrol/Diesel
 
bike = Motorcycle()
bike.start_engine()     # Motorcycle engine started: Brap! 🏍️
```
 
---
 
## Real-World Example: Bank Account System
 
Let's combine everything we've learned into a complete mini-project!
 
```python
from abc import ABC, abstractmethod
 
# Abstract Base Class
class Account(ABC):
    def __init__(self, account_number, owner):
        self.account_number = account_number
        self.owner = owner
        self.__balance = 0               # Private attribute
 
    @abstractmethod
    def account_type(self):
        pass
 
    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount
            print(f"✅ Rs.{amount} deposited. Balance: Rs.{self.__balance}")
        else:
            print("❌ Invalid amount.")
 
    def withdraw(self, amount):
        if amount > self.__balance:
            print("❌ Insufficient funds!")
        elif amount <= 0:
            print("❌ Invalid amount.")
        else:
            self.__balance -= amount
            print(f"✅ Rs.{amount} withdrawn. Balance: Rs.{self.__balance}")
 
    def get_balance(self):
        return self.__balance
 
    def show_info(self):
        print(f"\n{'='*40}")
        print(f"  Account Type   : {self.account_type()}")
        print(f"  Account Number : {self.account_number}")
        print(f"  Owner          : {self.owner}")
        print(f"  Balance        : Rs.{self.get_balance()}")
        print(f"{'='*40}\n")
 
 
# Savings Account — inherits from Account
class SavingsAccount(Account):
    def __init__(self, account_number, owner):
        super().__init__(account_number, owner)
        self.interest_rate = 0.05       # 5% interest
 
    def account_type(self):
        return "Savings Account"
 
    def add_interest(self):
        interest = self.get_balance() * self.interest_rate
        self.deposit(interest)
        print(f"💰 Interest of Rs.{interest:.2f} added!")
 
 
# Current Account — inherits from Account
class CurrentAccount(Account):
    def __init__(self, account_number, owner, overdraft_limit):
        super().__init__(account_number, owner)
        self.overdraft_limit = overdraft_limit
 
    def account_type(self):
        return "Current Account"
 
    def withdraw(self, amount):                          # Polymorphism!
        available = self.get_balance() + self.overdraft_limit
        if amount > available:
            print(f"❌ Exceeds overdraft limit of Rs.{self.overdraft_limit}!")
        else:
            print(f"✅ Rs.{amount} withdrawn (overdraft may apply).")
 
 
# ---- Testing the System ----
 
savings = SavingsAccount("SAV-001", "Ambreen")
savings.deposit(10000)
savings.deposit(5000)
savings.add_interest()
savings.withdraw(2000)
savings.show_info()
 
current = CurrentAccount("CUR-001", "Sara", overdraft_limit=3000)
current.deposit(2000)
current.withdraw(4000)    # Allowed due to overdraft
current.show_info()
```
 
**Output:**
```
✅ Rs.10000 deposited. Balance: Rs.10000
✅ Rs.5000 deposited. Balance: Rs.15000
✅ Rs.750.0 deposited. Balance: Rs.15750.0
💰 Interest of Rs.750.00 added!
✅ Rs.2000 withdrawn. Balance: Rs.13750.0
 
========================================
  Account Type   : Savings Account
  Account Number : SAV-001
  Owner          : Ambreen
  Balance        : Rs.13750.0
========================================
 
✅ Rs.2000 deposited. Balance: Rs.2000
✅ Rs.4000 withdrawn (overdraft may apply).
 
========================================
  Account Type   : Current Account
  Account Number : CUR-001
  Owner          : Sara
  Balance        : Rs.2000
========================================
```
 
---
 
## Summary Cheat Sheet
 
| Concept | What it means | Keyword/Symbol |
|---|---|---|
| **Class** | Blueprint/Template | `class MyClass:` |
| **Object** | Real instance of class | `obj = MyClass()` |
| **`__init__`** | Auto-runs when object is created | `def __init__(self):` |
| **`self`** | Refers to the current object | Used in every method |
| **Encapsulation** | Hiding data with private attributes | `self.__attribute` |
| **Inheritance** | Child class gets parent class features | `class Child(Parent):` |
| **Polymorphism** | Same method, different behavior | Override methods |
| **Abstraction** | Show only essentials, hide complexity | `ABC`, `@abstractmethod` |
 
---
 
> 💡 **Pro Tip for Beginners:** Don't try to memorize OOP all at once. Start by creating simple classes (like `Student`, `Car`, `Product`), then gradually add inheritance and other concepts as you build more projects.
 
