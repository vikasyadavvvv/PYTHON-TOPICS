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
