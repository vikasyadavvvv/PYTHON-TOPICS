# PYTHON-TOPICS

## 1. Variables ❎
✅ What is a Variable?

A variable is like a container that stores data (a value).
In Python, you don’t need to declare the type — it’s decided automatically.

Example:
```python
name = "Vikas"     # string
age = 20           # integer
height = 5.7       # float
is_student = True  # boolean

print(name)
print(age)
print(height)
print(is_student)

```
- ✅ Rules for Variables
- Must start with a letter or _
(✅ my_name, _age) (❌ 1name)
- Can contain letters, numbers, _ but no spaces.
- Case-sensitive (Name and name are different).
- Use snake_case in Python (first_name, total_price).

-✅ Assigning Multiple Variables
```python
x, y, z = 10, 20, 30
print(x, y, z)  # 10 20 30

#Assigning the same value:
a = b = c = 100
print(a, b, c)  # 100 100 100
```

## 2. Type Casting 💱
✅ What is Type Casting?

Type casting means converting one data type into another.
Python has built-in functions for this:

- int() → converts to integer
- float() → converts to float
- str() → converts to string
- bool() → converts to boolean
```python
# integer to float
num = 10
print(float(num))   # 10.0

# string to integer
age = "20"
print(int(age) + 5) # 25

# float to string
pi = 3.14
print("The value of pi is " + str(pi))  # The value of pi is 3.14

# boolean to integer
flag = True
print(int(flag))   # 1
```

- Practice Exercises (Type Casting)
- Ask the user for their age (input is string). Convert it to integer and print:
```python
# Ask the user for their age
age_input=input("ENTER YOUT AGE")

# Convert the string input to integer
age=int(age_input)

# Print the result
print("Your age is",age)
print(type(age_input))
print(type(age))
```

## 3. User Input ⌨️
✅ Getting Input from the User

In Python, we use input() to take input from the user.
👉 Important: input() always returns a string, so you often need type casting.

Example:
```python
name = input("Enter your name: ")
print("Hello " + name)

age = int(input("Enter your age: "))  # convert to integer
print("Next year you will be", age + 1)
price = float(input("Enter the price: "))  # convert to float
print("Price with tax:", price * 1.18)

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
print("Sum:", num1 + num2)

```

## 4. ⭐ Madlibs Game 📖
✅ What is Madlibs?
Madlibs is a word game where the program asks the user for words (like nouns, verbs, adjectives), then inserts them into a story template to create something funny.
Example:
```python
# Madlibs Game
adjective = input("Enter an adjective: ")
noun = input("Enter a noun: ")
verb = input("Enter a verb: ")

print(f"Today I saw a {adjective} {noun} that loved to {verb}!")

```


## 5. Arithmetic & Math 📐
✅ Arithmetic Operators
Python supports basic math operators:
```python
x = 10
y = 3

print(x + y)  # Addition → 13
print(x - y)  # Subtraction → 7
print(x * y)  # Multiplication → 30
print(x / y)  # Division (float) → 3.333...
print(x // y) # Floor Division → 3
print(x % y)  # Modulus (remainder) → 1
print(x ** y) # Exponentiation → 10³ = 1000

```
- ✅ Math Functions (from math module)
```python
import math

print(math.sqrt(16))    # 4.0
print(math.pow(2, 3))   # 8.0
print(math.ceil(4.3))   # 5
print(math.floor(4.7))  # 4
print(abs(-10))         # 10

import math
radius = float(input("Enter radius of a circle: "))
area = math.pi * radius ** 2
print("Area of circle:", area)

```

## 6. If Statements 🤔
✅ What is an If Statement?

It lets your program make decisions based on conditions.
Example:
```python
age = int(input("Enter your age: "))

if age >= 18:
    print("You are an adult.")
elif age > 12:
    print("You are a teenager.")
else:
    print("You are a child.")


number = int(input("Enter a number: "))
if number % 2 == 0:
    print("Even")
else:
    print("Odd")

```

## 7. Calculator Program 🧮
✅ Idea

We’ll build a simple calculator that:
- Asks the user for two numbers.
- Asks for the operation (+, -, *, /).
- Uses if statements to decide which operation to perform.
```python
# Simple Calculator
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
operation = input("Enter operation (+, -, *, /): ")

if operation == "+":
    print("Result:", num1 + num2)
elif operation == "-":
    print("Result:", num1 - num2)
elif operation == "*":
    print("Result:", num1 * num2)
elif operation == "/":
    if num2 != 0:
        print("Result:", num1 / num2)
    else:
        print("Error! Division by zero.")
else:
    print("Invalid operation.")
```


## 8. Logical Operators 🌦️
✅ Logical Operators in Python

Used to combine multiple conditions in if statements.

- and → True if both conditions are true
- or → True if at least one condition is true
- not → Reverses the condition

✅ Examples
```python
age = 20
has_id = True

# AND
if age >= 18 and has_id:
    print("You are allowed to enter.")
else:
    print("Access denied.")

# OR
day = "Sunday"
if day == "Saturday" or day == "Sunday":
    print("It's the weekend!")
else:
    print("Weekday.")

# NOT
is_raining = False
if not is_raining:
    print("You can go outside without an umbrella.")

```

## 9. What is a Ternary Operator?

A ternary operator allows you to write an if-else condition in a single line.
It’s also called a conditional expression.
Example:
```python
age = 18
result = "Adult" if age >= 18 else "Minor"
print(result)

```


## 10. String Methods 〰️

Strings in Python come with many built-in methods that help you manipulate them easily.
Here are the most useful ones:
```python
text = "  hello world  "

# 1. Changing case
print(text.upper())     # "  HELLO WORLD  "
print(text.lower())     # "  hello world  "
print(text.title())     # "  Hello World  "

# 2. Removing extra spaces
print(text.strip())     # "hello world" (removes spaces from both ends)
print(text.lstrip())    # "hello world  " (removes from left)
print(text.rstrip())    # "  hello world" (removes from right)

# 3. Checking contents
print("hello" in text)      # True
print(text.startswith("  h"))  # True
print(text.endswith("ld  "))   # True

# 4. Finding and replacing
print(text.find("world"))   # 8 (position)
print(text.replace("world", "Python"))  # "  hello Python  "

# 5. Splitting and joining
words = text.split()        # ['hello', 'world']
print("-".join(words))      # "hello-world"

```

## 11. String Indexing ✂️

In Python, strings are sequences, so you can access them using indexes (just like lists).
Example:
```python
word = "Python"

# Positive Indexing
print(word[0])   # 'P'
print(word[1])   # 'y'
print(word[5])   # 'n'

# Negative Indexing
print(word[-1])  # 'n'
print(word[-2])  # 'o'

# Slicing
print(word[0:4])   # "Pyth"
print(word[:3])    # "Pyt"  (from start till index 2)
print(word[2:])    # "thon" (from index 2 to end)
print(word[::-1])  # "nohtyP" (reverse string)

```

## 12. While Loops ♾️
Runs until the condition becomes False.
🔹 Be careful with infinite loops (if condition never becomes false).
Example:
```python
count = 1
while count <= 5:
    print("Count:", count)
    count += 1

```

## 13. For Loop in Python
A for loop is used when you want to repeat an action a specific number of times or loop through items in a sequence (like lists, strings, or ranges).

Example 1: Loop through a range of numbers
```python
for i in range(5):
    print("Number:", i)

```

## 14. 20 Nested Loops ➿
A loop inside another loop:
Example:
```python
for i in range(1, 4):
    for j in range(1, 4):
        print(i, j)

```
## 14. Lists in Python
✅ What is a List?

A list is a collection of items (like numbers, strings, or even other lists).
It is ordered, mutable (can be changed), and allows duplicate values.

📌 Creating a List
```python
fruits = ["apple", "banana", "cherry", "mango"]
numbers = [10, 20, 30, 40, 50]
mixed = [1, "hello", 3.14, True]

# 📌 Accessing List Items
print(fruits[0])   # apple
print(fruits[-1])  # mango (last element)

# 📌 Changing Values
fruits[1] = "kiwi"
print(fruits)  # ['apple', 'kiwi', 'cherry', 'mango']

#📌 Useful List Methods
fruits.append("orange")   # add item at end
fruits.insert(1, "grapes") # add at index
fruits.remove("cherry")   # remove by value
popped = fruits.pop()     # remove last item
fruits.sort()             # sort alphabetically
fruits.reverse()          # reverse order

```

## 15. 🔹 Tuples

A tuple is an ordered, immutable collection in Python.
Defined using parentheses ().
Once created, you cannot change the elements (no add/remove/update).

Example:
```python
my_tuple = (1, 2, 3, "hello", 3.5)
print(my_tuple[0])   # 1
print(my_tuple[-1])  # 3.5

# 👉 Tuples allow duplicate values:
t = (1, 2, 2, 3)
print(t)   # (1, 2, 2, 3)

#👉 If there’s only one element, you must add a comma:
t1 = (10,)
print(type(t1))   # <class 'tuple'>

```

## 16. 🔹 Sets

A set is an unordered, mutable collection of unique elements.
Defined using curly braces {}.
Duplicates are not allowed.

Example:
```python
my_set = {1, 2, 3, 4, 4, 5}
print(my_set)   # {1, 2, 3, 4, 5}  (4 is removed automatically)

# 👉 Adding & Removing:
s = {10, 20, 30}
s.add(40)
print(s)       # {40, 10, 20, 30}

s.remove(20)   # removes element
print(s)       # {40, 10, 30}

# 👉 Set Operations:
a = {1, 2, 3, 4}
b = {3, 4, 5, 6}

print(a | b)   # Union: {1, 2, 3, 4, 5, 6}
print(a & b)   # Intersection: {3, 4}
print(a - b)   # Difference: {1, 2}
print(a ^ b)   # Symmetric Difference: {1, 2, 5, 6}

```

## 17. 🔑 What is a Dictionary?

A dictionary in Python is a collection of key-value pairs.
Similar to a real dictionary (word → meaning).
It is unordered, mutable, and indexed by keys.

🛠️ Dictionary Features

- Keys must be unique.
- Keys can be of immutable types (string, number, tuple).
- Values can be of any type (string, int, list, dict, etc.).
- Dictionaries are mutable (can change after creation).

📌 Syntax:
```python
my_dict = {
    "name": "Vikas",
    "age": 20,
    "skills": ["Python", "JavaScript", "MongoDB"]
}


# Create a dictionary
student = {"name": "Vikas", "age": 20, "course": "B.Sc IT"}

# Access value by key
print(student["name"])      # Vikas

# Using get()
print(student.get("age"))   # 20

# Add a new key-value pair
student["marks"] = 85
print(student)  

# Update value
student["age"] = 21
print(student)

# Remove a key-value pair
student.pop("course")
print(student)

# Remove last inserted item (Python 3.7+ keeps insertion order)
student.popitem()
print(student)

# Check if key exists
print("name" in student)  # True



info = {"a": 1, "b": 2, "c": 3}

print(info.keys())      # dict_keys(['a', 'b', 'c'])
print(info.values())    # dict_values([1, 2, 3])
print(info.items())     # dict_items([('a', 1), ('b', 2), ('c', 3)])

# Copy
copy_dict = info.copy()

# Clear
info.clear()
print(info)   # {}


```

## 18. Functions 📞

A function is a block of reusable code that performs a specific task.
Example:
```python
def greet():
    print("Hello, World!")

greet()   # Output: Hello, World!


# 👉 Function with arguments:
def add(a, b):
    return a + b

print(add(5, 3))   # Output: 8

# 👉 Function with return value:
def square(x):
    return x * x

result = square(4)
print(result)   # Output: 16

```

## 19. #33 Default Arguments 👍

You can assign default values to function parameters. If the caller doesn’t provide a value, the default is used.
Example:
```python
def greet(name="User"):
    print(f"Hello, {name}!")

greet()          # Output: Hello, User!
greet("Vikas")   # Output: Hello, Vikas!

```

## 20. Keyword Arguments 🗝️
You can pass arguments by name, instead of relying on position.
Example:
```python
def introduce(name, age):
    print(f"My name is {name} and I am {age} years old.")

introduce(age=20, name="Vikas")
# Output: My name is Vikas and I am 20 years old.

```

## 21. *args & kwargs 📦

*args → allows you to pass multiple positional arguments.
**kwargs → allows you to pass multiple keyword arguments.

Example:
```python
def sum_all(*args):
    return sum(args)

print(sum_all(1, 2, 3, 4))   # Output: 10

def show_details(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

show_details(name="Vikas", age=20, city="Mumbai")
# Output:
# name: Vikas
# age: 20
# city: Mumbai

```

## 24. Exception Handling

Exceptions are errors that occur during runtime. Python provides try...except to handle them gracefully.

Example:
```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("You can't divide by zero!")


def divide_100_by_number():
    try:
        # Ask for a number
        number = float(input("Enter a number to divide 100 by: "))
        
        # Perform division
        result = 100 / number
        print(f"100 divided by {number} is: {result}")
        
    except ZeroDivisionError:
        print("Error: Cannot divide by zero!")
    
    except ValueError:
        print("Error: Please enter a valid number!")
    
    finally:
        print("Program finished")

# Run the program
divide_100_by_number()
```

