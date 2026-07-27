# Operators in Python

Operators are symbols or keywords that perform operations on values and variables.

Example:

```python
10 + 5
```

Here, `+` is an operator.

Operators are used in almost every Python program.

---

# Types of Operators

Python provides the following operator categories:

- Arithmetic Operators
- Assignment Operators
- Comparison Operators
- Logical Operators
- Identity Operators
- Membership Operators
- Bitwise Operators
- Conditional (Ternary) Expression

---

# 1. Arithmetic Operators

Arithmetic operators perform mathematical calculations.

| Operator | Meaning | Example |
|----------|---------|---------|
| + | Addition | 5 + 2 |
| - | Subtraction | 5 - 2 |
| * | Multiplication | 5 * 2 |
| / | Division | 5 / 2 |
| // | Floor Division | 5 // 2 |
| % | Modulus | 5 % 2 |
| ** | Exponent | 5 ** 2 |

---

## Addition (+)

```python
a = 10
b = 20

print(a + b)
```

Output

```
30
```

Addition also works with strings.

```python
print("Hello " + "World")
```

Output

```
Hello World
```

---

## Subtraction (-)

```python
print(20 - 5)
```

Output

```
15
```

---

## Multiplication (*)

```python
print(6 * 4)
```

Output

```
24
```

Strings can also be multiplied.

```python
print("Hi " * 3)
```

Output

```
Hi Hi Hi
```

---

## Division (/)

Always returns a float.

```python
print(10 / 2)
```

Output

```
5.0
```

Even if both numbers are integers.

```python
print(9 / 3)
```

Output

```
3.0
```

---

## Floor Division (//)

Returns only the integer part.

```python
print(10 // 3)
```

Output

```
3
```

Another example

```python
print(17 // 5)
```

Output

```
3
```

---

## Modulus (%)

Returns the remainder.

```python
print(10 % 3)
```

Output

```
1
```

Useful for checking even and odd numbers.

```python
number = 8

print(number % 2 == 0)
```

Output

```
True
```

---

## Exponent (**)

Raises a number to a power.

```python
print(2 ** 3)
```

Output

```
8
```

Example

```python
print(10 ** 4)
```

Output

```
10000
```

---

# Arithmetic Operator Precedence

Python follows mathematical precedence.

```python
print(2 + 3 * 4)
```

Output

```
14
```

Because multiplication happens first.

Use parentheses to change the order.

```python
print((2 + 3) * 4)
```

Output

```
20
```

---

# 2. Assignment Operators

Assignment operators assign values to variables.

| Operator | Example | Same As |
|----------|---------|---------|
| = | x = 5 | Assign value |
| += | x += 2 | x = x + 2 |
| -= | x -= 2 | x = x - 2 |
| *= | x *= 2 | x = x * 2 |
| /= | x /= 2 | x = x / 2 |
| //= | x //= 2 | x = x // 2 |
| %= | x %= 2 | x = x % 2 |
| **= | x **= 2 | x = x ** 2 |

---

## =

```python
x = 100
```

Assigns a value.

---

## +=

```python
x = 10

x += 5

print(x)
```

Output

```
15
```

---

## -=

```python
x = 20

x -= 4

print(x)
```

Output

```
16
```

---

## *=

```python
x = 5

x *= 4

print(x)
```

Output

```
20
```

---

## /=

```python
x = 10

x /= 2

print(x)
```

Output

```
5.0
```

---

## //=

```python
x = 11

x //= 2

print(x)
```

Output

```
5
```

---

## %=

```python
x = 11

x %= 4

print(x)
```

Output

```
3
```

---

## **=

```python
x = 3

x **= 2

print(x)
```

Output

```
9
```

---

# 3. Comparison Operators

Comparison operators compare values.

They always return either:

- True
- False

| Operator | Meaning |
|----------|---------|
| == | Equal |
| != | Not Equal |
| > | Greater Than |
| < | Less Than |
| >= | Greater Than or Equal |
| <= | Less Than or Equal |

---

## ==

```python
print(10 == 10)
```

Output

```
True
```

---

## !=

```python
print(10 != 5)
```

Output

```
True
```

---

## >

```python
print(15 > 8)
```

Output

```
True
```

---

## <

```python
print(2 < 5)
```

Output

```
True
```

---

## >=

```python
print(5 >= 5)
```

Output

```
True
```

---

## <=

```python
print(4 <= 3)
```

Output

```
False
```

---

# Chained Comparisons

Python allows multiple comparisons together.

```python
x = 10

print(5 < x < 20)
```

Output

```
True
```

Equivalent to

```python
5 < x and x < 20
```

---

# 4. Logical Operators

Logical operators combine conditions.

| Operator | Meaning |
|----------|---------|
| and | Both must be True |
| or | At least one True |
| not | Reverses result |

---

## and

```python
age = 20

print(age > 18 and age < 30)
```

Output

```
True
```

---

## or

```python
print(False or True)
```

Output

```
True
```

---

## not

```python
print(not True)
```

Output

```
False
```

---

# Short-Circuit Evaluation

Python stops checking as soon as the result is known.

```python
False and print("Hello")
```

Nothing is printed.

Because the result is already False.

Example

```python
True or print("Hello")
```

Nothing is printed.

Because the result is already True.

---

# 5. Identity Operators

Identity operators compare whether two variables refer to the same object.

| Operator | Meaning |
|----------|---------|
| is | Same object |
| is not | Different object |

---

## is

```python
a = [1, 2]
b = a

print(a is b)
```

Output

```
True
```

Both variables point to the same object.

---

## is not

```python
a = [1]
b = [1]

print(a is not b)
```

Output

```
True
```

Values are equal, but objects are different.

---

## Difference Between == and is

```python
a = [1, 2]
b = [1, 2]

print(a == b)
print(a is b)
```

Output

```
True
False
```

`==` compares values.

`is` compares object identity.

---

# 6. Membership Operators

Membership operators check whether a value exists inside a collection.

| Operator | Meaning |
|----------|---------|
| in | Exists |
| not in | Doesn't exist |

---

## in

```python
numbers = [10, 20, 30]

print(20 in numbers)
```

Output

```
True
```

---

## not in

```python
print(50 not in numbers)
```

Output

```
True
```

Works with strings too.

```python
print("Py" in "Python")
```

Output

```
True
```

---

# 7. Bitwise Operators

Bitwise operators work on binary numbers.

| Operator | Meaning |
|----------|---------|
| & | AND |
| \| | OR |
| ^ | XOR |
| ~ | NOT |
| << | Left Shift |
| >> | Right Shift |

---

## Bitwise AND (&)

```python
print(5 & 3)
```

Output

```
1
```

Binary

```
5 = 101
3 = 011
---------
    001
```

---

## Bitwise OR (|)

```python
print(5 | 3)
```

Output

```
7
```

---

## Bitwise XOR (^)

```python
print(5 ^ 3)
```

Output

```
6
```

---

## Bitwise NOT (~)

```python
print(~5)
```

Output

```
-6
```

---

## Left Shift (<<)

```python
print(5 << 1)
```

Output

```
10
```

Equivalent to multiplying by 2.

---

## Right Shift (>>)

```python
print(8 >> 2)
```

Output

```
2
```

Equivalent to dividing by 4.

---

# 8. Conditional (Ternary) Expression

A shorter way to write an `if...else`.

Syntax

```python
value_if_true if condition else value_if_false
```

Example

```python
age = 20

status = "Adult" if age >= 18 else "Minor"

print(status)
```

Output

```
Adult
```

---

# Operator Precedence

Higher precedence operators are evaluated first.

| Priority | Operators |
|-----------|-----------|
| Highest | () |
| | ** |
| | +x, -x, ~x |
| | *, /, //, % |
| | +, - |
| | <<, >> |
| | & |
| | ^ |
| | \| |
| | ==, !=, >, <, >=, <= |
| | not |
| | and |
| Lowest | or |

Example

```python
result = 10 + 2 * 5 > 15 and True

print(result)
```

Output

```
True
```

---

# Common Beginner Mistakes

## Using = Instead of ==

Wrong

```python
if x = 10:
    pass
```

Correct

```python
if x == 10:
    pass
```

---

## Using is Instead of ==

Wrong

```python
if a is 10:
```

Correct

```python
if a == 10:
```

Use `is` only for object identity (or comparisons with `None`).

---

## Dividing Integers

```python
print(5 / 2)
```

Output

```
2.5
```

Use `//` if you need an integer result.

---

## Forgetting Parentheses

Bad

```python
2 + 3 * 4
```

Better

```python
(2 + 3) * 4
```

Makes your code easier to read.

---

# Best Practices

- Use `==` for value comparison.
- Use `is` only for identity checks.
- Use parentheses to improve readability.
- Prefer meaningful expressions over clever ones.
- Don't overuse nested logical operators.

---

# Quick Summary

You learned:

- Arithmetic Operators
- Assignment Operators
- Comparison Operators
- Logical Operators
- Identity Operators
- Membership Operators
- Bitwise Operators
- Conditional (Ternary) Expression
- Operator Precedence
- Common Mistakes
- Best Practices

Operators are the building blocks of calculations, comparisons, and decision-making in Python. Mastering them will make writing conditions, loops, and algorithms much easier.

---

# Next Topic

➡️ **Input & Output**

You will learn:

- `print()`
- `input()`
- Formatting Output
- f-Strings
- Escape Characters
- End and Separator Parameters
- Reading Different Data Types
```