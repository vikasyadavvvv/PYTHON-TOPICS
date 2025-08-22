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
