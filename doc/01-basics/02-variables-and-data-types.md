# Variables & Data Types

Variables are one of the first things you learn in Python.

A variable stores a value so you can use it later.

Instead of writing the same value again and again, store it in a variable.

---

# Creating Variables

Python creates a variable automatically when you assign a value.

```python
name = "vinay"
age = 19
height = 5.9
```

No keyword is required.

Unlike C, C++, or Java, you don't need to specify the data type.

---

# How Variables Work

```python
x = 10
```

Python creates an object with value `10` and makes the variable `x` refer to that object.

Think of it like this:

```

x ───► 10

```

The variable does **not** store the value itself.

It stores a reference to the object.

---

# Printing Variables

```python
name = "india"

print(name)
```

Output

```
india
```

Multiple variables

```python
name = "india"
age = 22

print(name, age)
```

Output

```
india 22
```

---

# Reassigning Variables

Variables can change.

```python
x = 5

print(x)

x = 20

print(x)
```

Output

```
5
20
```

Python simply changes what `x` points to.

---

# Dynamic Typing

Python is dynamically typed.

This means a variable can store different types of values.

```python
x = 10

x = "Hello"

x = True
```

This is completely valid.

---

# Checking Variable Type

Use `type()`.

```python
x = 10

print(type(x))
```

Output

```
<class 'int'>
```

Example

```python
print(type(3.14))
print(type("Python"))
print(type(True))
```

Output

```
<class 'float'>
<class 'str'>
<class 'bool'>
```

---

# Naming Rules

Valid

```python
name = "vinay"

_age = 20

user1 = "india"

total_price = 100
```

Invalid

```python
1name = "vinay"

user-name = "vinay"

class = 10
```

Why?

- Cannot start with numbers
- Cannot contain spaces
- Cannot contain special symbols except `_`
- Cannot use Python keywords

---

# Variable Naming Style

Recommended

```python
student_name = "kumar"

total_marks = 500

is_logged_in = True
```

Bad

```python
a = 100

abcxyz = 10

q = "vinay"
```

Use meaningful names.

Good names make code easier to understand.

---

# Constants

Python has no real constant.

By convention, write constants in uppercase.

```python
PI = 3.14159

MAX_SPEED = 120
```

Nothing prevents changing them.

```python
PI = 10
```

This is allowed but considered bad practice.

---

# Multiple Assignment

Assign multiple variables.

```python
x, y, z = 10, 20, 30

print(x)
print(y)
print(z)
```

Output

```
10
20
30
```

---

# Assign Same Value

```python
a = b = c = 100

print(a)
print(b)
print(c)
```

Output

```
100
100
100
```

---

# Swapping Variables

Python makes swapping easy.

```python
a = 10
b = 20

a, b = b, a

print(a)
print(b)
```

Output

```
20
10
```

No temporary variable needed.

---

# Deleting Variables

Use `del`.

```python
x = 10

del x
```

Now

```python
print(x)
```

Output

```
NameError
```

---

# Variable Scope (Basic)

```python
x = 100

def show():
    print(x)

show()
```

Output

```
100
```

Local variable

```python
def test():
    x = 50
    print(x)

test()
```

Output

```
50
```

Outside the function

```python
print(x)
```

Output

```
100
```

---

# Data Types

Python has many built-in data types.

| Type | Example |
|------|---------|
| int | 10 |
| float | 3.14 |
| complex | 2+3j |
| bool | True |
| str | "Python" |
| list | [1,2,3] |
| tuple | (1,2,3) |
| set | {1,2,3} |
| dict | {"a":1} |
| range | range(5) |
| bytes | b"abc" |
| bytearray | bytearray(5) |
| memoryview | memoryview(bytes(5)) |
| NoneType | None |

---

# Integer

Whole numbers.

```python
x = 100
```

Negative numbers

```python
y = -500
```

Very large numbers

```python
z = 999999999999999999999999
```

Python integers have unlimited size.

---

# Float

Decimal numbers.

```python
price = 99.99
```

Scientific notation

```python
x = 5e3

print(x)
```

Output

```
5000.0
```

---

# Complex Numbers

Used in scientific computing.

```python
x = 3 + 4j

print(type(x))
```

Output

```
<class 'complex'>
```

---

# Boolean

Only two values.

```python
True

False
```

Example

```python
is_admin = True
```

Booleans are heavily used in conditions.

---

# Strings

A string stores text.

```python
name = "Python"
```

Single quotes

```python
'Hello'
```

Double quotes

```python
"Hello"
```

Triple quotes

```python
"""Multiple
Lines"""
```

---

# List

Ordered

Mutable

Allows duplicates

```python
numbers = [1,2,3]
```

Change value

```python
numbers[0] = 100
```

Output

```
[100,2,3]
```

---

# Tuple

Ordered

Immutable

```python
point = (10,20)
```

Trying to change

```python
point[0] = 100
```

Output

```
TypeError
```

---

# Set

Unordered

Unique values only.

```python
items = {1,2,3,2,1}
```

Output

```
{1,2,3}
```

Duplicates are removed automatically.

---

# Dictionary

Stores key-value pairs.

```python
student = {
    "name":"vinay",
    "age":20
}
```

Access value

```python
print(student["name"])
```

Output

```
vinay
```

---

# Range

Generates numbers.

```python
range(5)
```

Example

```python
for i in range(5):
    print(i)
```

Output

```
0
1
2
3
4
```

---

# None

Represents "no value".

```python
x = None
```

Useful when a variable has no value yet.

---

# Mutable vs Immutable

## Mutable

Can change after creation.

- list
- dict
- set
- bytearray

Example

```python
numbers = [1,2,3]

numbers.append(4)
```

---

## Immutable

Cannot change after creation.

- int
- float
- bool
- str
- tuple
- bytes

Example

```python
name = "Python"

name[0] = "J"
```

Output

```
TypeError
```

---

# Type Conversion

## Implicit Conversion

Python converts automatically.

```python
x = 5
y = 2.5

print(x + y)
```

Output

```
7.5
```

---

## Explicit Conversion

You convert manually.

```python
age = "20"

print(int(age))
```

Output

```
20
```

Examples

```python
float(10)

str(100)

bool(1)

list("abc")

tuple([1,2])

set([1,2,2,3])
```

---

# Truthy and Falsy Values

Falsy values

```python
False
None
0
0.0
''
[]
{}
()
set()
```

Everything else is generally Truthy.

Example

```python
if []:
    print("Yes")
else:
    print("No")
```

Output

```
No
```

---

# Object Identity

Every object has an identity.

```python
x = 10

print(id(x))
```

`id()` returns the object's unique identity.

---

# Copying Variables

```python
a = [1,2,3]

b = a
```

Both variables refer to the same object.

```python
b.append(4)

print(a)
```

Output

```
[1,2,3,4]
```

To create a new list

```python
b = a.copy()
```

---

# Common Beginner Mistakes

## Using Undefined Variable

```python
print(age)
```

Error

```
NameError
```

---

## Wrong Variable Name

```python
my-name = "vinay"
```

Error

```
SyntaxError
```

---

## Forgetting Quotes

Wrong

```python
name = Python
```

Correct

```python
name = "Python"
```

---

## Confusing '=' and '=='

Assignment

```python
x = 10
```

Comparison

```python
x == 10
```

---

# Best Practices

- Use meaningful variable names.
- Follow snake_case naming.
- Keep variable names short but descriptive.
- Use uppercase for constants.
- Don't overwrite built-in names.

Bad

```python
list = [1,2,3]
```

Good

```python
numbers = [1,2,3]
```

---

# Quick Summary

You learned:

- What variables are
- How Python stores variables
- Variable naming rules
- Dynamic typing
- Built-in data types
- Mutable vs immutable objects
- Type conversion
- Truthy and falsy values
- Object identity
- Copying variables
- Common mistakes
- Best practices

You now understand how Python stores and manages data, which is the foundation for writing real Python programs.

---

# Next Topic

➡️ Operators

You will learn:

- Arithmetic operators
- Comparison operators
- Assignment operators
- Logical operators
- Bitwise operators
- Membership operators
- Identity operators
- Operator precedence