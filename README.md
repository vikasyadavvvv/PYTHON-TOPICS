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
