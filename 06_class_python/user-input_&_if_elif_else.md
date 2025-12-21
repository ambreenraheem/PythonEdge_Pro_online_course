Date: 20-December-2025

### Instructor: Ambreen Abdul Raheem
### Professional Power BI Data Analyst And AI Agent Developer (Upwork Freelancer)

#### Python Input Function
**What is input()?**

The input() function allows your program to receive data from the user.\
It displays a prompt message and waits for the user to type something and press Enter.
**Basic Syntax**
```
variable = input("Prompt message: ")
```

**Important Notes**
- input() always returns a string (text)
- You need to convert it to other data types if needed
- The prompt message is optional but recommended

#### Data Types
String Input (Default)
**Example:01**
```
name = input("Enter your name: ")
print(name)  # Returns as string
print(type(name))  # <class 'str'>
```
**Converting to Integer**
**Example:02**
```
age = int(input("Enter your age: "))
print(age)  # Returns as integer
print(type(age))  # <class 'int'>
```
**Converting to Float**
**Example:03**
```
height = float(input("Enter your height (m): "))
print(height)  # Returns as float
print(type(height))  # <class 'float'>
```

**Example:04 - Multiple Inputs**
```
first_name = input("Enter first name: ")
last_name = input("Enter last name: ")
age = int(input("Enter age: "))

print(f"Name: {first_name} {last_name}")
print(f"Age: {age}")
```

**Example:05 - Float Input**
```
price = float(input("Enter product price: $"))
quantity = int(input("Enter quantity: "))
total = price * quantity

print(f"Total cost: ${total:.2f}")
```
#### What are Conditional Statements?
Conditional statements allow your program to make decisions and execute different code based on different conditions. They control the flow of your program.
**The Three Types:**

  01. Statement: "if", Purpose:	"Executes code if a condition is **True**"
  02. Statement: "elif", Purpose:	"Executes code if previous conditions were False and this condition is **True**"
  03. Statement: "else", Purpose:	"Executes code if all previous conditions were **False**"

**Example:01**
```
age = input("Enter your age?")

if age >= 18:
    print("You are an adult")
```














