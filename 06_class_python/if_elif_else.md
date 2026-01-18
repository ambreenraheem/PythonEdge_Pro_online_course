### Python Conditions and If Statements

Python uses conditions to make decisions.
A condition checks whether something is True or False.
Common Conditions in Python

- Equal to: ==
- Not equal to: !=
- Less than: <
- Less than or equal to: <=
- Greater than: >
- Greater than or equal to: >=

These conditions are mainly used in if, elif, and else statements.

#### The if Statement
The if statement runs code only when a condition is true.
Example (with input)
number = int(input("Enter a number: "))
```
if number > 0:
    print("The number is positive")
```
✅ If the number is greater than 0, the message is printed.

The if and else Statement
The else block runs when the if condition is false.
Example
```
number = int(input("Enter a number: "))

if number > 0:
    print("The number is positive")
else:
    print("The number is not positive")
```
✔ One of the two messages will always be printed.

The if, elif, and else Statement
Use elif (else if) to check more than one condition.
Example
```
number = int(input("Enter a number: "))

if number > 0:
    print("The number is positive")
elif number == 0:
    print("The number is zero")
else:
    print("The number is negative")
```
How it works:

- If the first condition is true, Python runs that block.
- If not, it checks the elif condition.
- If all conditions are false, the else block runs.

##### Summary

- if → checks a condition
- elif → checks another condition
- else → runs when all conditions are false

If you want, I can give you practice questions or explain this with real-life examples 😊
##### 1️⃣ School Attendance (Real Life)

Situation:
- If a student is present → mark present
- Otherwise → mark absent
```
attendance = input("Are you present? (yes/no): ")

if attendance == "yes":
    print("You are marked present")
else:
    print("You are marked absent")
```
##### 2️⃣ Weather Clothes Choice

Situation:

- If it’s hot → wear light clothes
- If it’s cold → wear warm clothes
- Otherwise → normal clothes
```
weather = input("How is the weather? (hot/cold/normal): ")

if weather == "hot":
    print("Wear light clothes")
elif weather == "cold":
    print("Wear warm clothes")
else:
    print("Wear normal clothes")
```
##### 3️⃣ Exam Result

Situation:

- 50 or more → Pass
- Less than 50 → Fail
```
marks = int(input("Enter your marks: "))

if marks >= 50:
    print("You passed the exam")
else:
    print("You failed the exam")
```
##### 4️⃣ Traffic Light (Daily Life)

Situation:

- Red → Stop
- Yellow → Wait
- Green → Go
```
light = input("Enter traffic light color: ")

if light == "red":
    print("Stop")
elif light == "yellow":
    print("Wait")
elif light == "green":
    print("Go")
else:
    print("Invalid light")
```
##### 5️⃣ Phone Battery

Situation:

- Battery ≤ 20 → Charge phone
- Battery > 20 → Keep using
```
battery = int(input("Enter battery percentage: "))

if battery <= 20:
    print("Please charge your phone")
else:
    print("Battery is okay")
```
##### 6️⃣ Shop Discount

Situation:

- Bill ≥ 5000 → Discount
- Otherwise → No discount
```
bill = int(input("Enter total bill: "))

if bill >= 5000:
    print("You get a discount!")
else:
    print("No discount available")
```
##### 7️⃣ Alarm Clock (Morning Routine)

Situation:
- If it’s weekday → go to school
- Else → sleep more 😄
```
day = input("Is today a weekday? (yes/no): ")

if day == "yes":
    print("Wake up! Time for school")
else:
    print("Sleep more, it's a holiday!")
```
##### 8️⃣ Elevator Decision

Situation:

- Floor 0 → Ground floor
- Floor > 0 → Going up
- Floor < 0 → Basement
```
floor = int(input("Enter floor number: "))

if floor == 0:
    print("Ground floor")
elif floor > 0:
    print("Going up")
else:
    print("Basement")
```
🧠 Easy Tip to Remember:

if → first decision

elif → another decision

else → last option

#### Python else Statement
- The else Keyword

- The else keyword is used to catch all cases that are not true in the if and elif conditions.

- The code inside the else block runs only when all previous conditions are false.
```
Example
a = 200
b = 33

if b > a:
    print("b is greater than a")
elif a == b:
    print("a and b are equal")
else:
    print("a is greater than b")
```
###### Explanation

First, Python checks if b is greater than a.
❌ This is false because 33 is not greater than 200.

Then, Python checks if a is equal to b.
❌ This is also false.

Since both conditions are false, Python runs the else block.

✅ The output will be:

a is greater than b

Important Point

else does not need a condition.

It always comes at the end.

Only one else is allowed in an if statement.



