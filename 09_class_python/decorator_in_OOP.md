Date: 07- April- 2026

## Instructor: Ambreen Abdul Raheem
#### Professional Data Analyst And Web Developer (Upwork Freelancer)


### @staticmethod:

@staticmethod is a regular function that lives inside a class for organisation. It does NOT receive self or cls — it has no access to instance or class data.

> Like a calculator app on your phone — it belongs to the phone's OS but doesn't need to know your contact list to add numbers.

> - No self or cls
> - Utility functions

#### Example:01

```
class Welcome:
    @staticmethod
    def greeting():
        print("We Welcome you here!")
print(Welcome)
print(Welcome.greeting)
```

#### Example: 02

```
class MathHelper:

    @staticmethod
    def is_even(n):
        return n % 2 == 0

    @staticmethod
    def celsius_to_fahrenheit(c):
        return (c * 9/5) + 32

    @staticmethod
    def grade(marks):
        if marks >= 90: return "A+"
        if marks >= 80: return "A"
        if marks >= 70: return "B"
        return "C"

# Call without creating an object!
print(MathHelper.is_even(4))            # True
print(MathHelper.celsius_to_fahrenheit(100))  # 212.0
print(MathHelper.grade(85))             # A
```

### @classmethod:
@classmethod receives cls (the class itself) instead of self. Used to create alternative constructors or track class-level data shared across all objects.

> Like a factory that stamps products — the factory knows how many it has made total, not just one product.

> - Class-level access
> - Alternative constructors

```
@class 
```



```
class Employee:
    __count = 0                  # class variable

    def __init__(self, name, salary):
        self.name   = name
        self.salary = salary
        Employee.__count += 1

    @classmethod
    def get_count(cls):           # cls = Employee
        return cls.__count

    @classmethod
    def from_string(cls, data):  # alt constructor
        name, salary = data.split(",")
        return cls(name, int(salary))

e1 = Employee("Ambreen", 80000)
e2 = Employee.from_string("Sara,70000")
print(Employee.get_count())    # 2
```

### @propertymethod:

@property lets you access a method like an attribute — no parentheses needed. Pair it with @x.setter to add validation when a value is changed.

> Like a bank teller window — you can ask for your balance (getter) or request a deposit (setter), but you never touch the vault directly.

> - Encapsulation
> - Controlled access

```
class
```

```
class Product:
    def __init__(self, name, price):
        self.name  = name
        self.__price = price          # private

    @property
    def price(self):                 # getter
        return f"Rs.{self.__price:.2f}"

    @price.setter
    def price(self, value):          # setter
        if value < 0:
            raise ValueError("Price cannot be negative!")
        self.__price = value

p = Product("Laptop", 85000)
print(p.price)        # Rs.85000.00  ← no ()
p.price = 90000      # setter validates
print(p.price)        # Rs.90000.00
# p.price = -100    → ValueError!
```

