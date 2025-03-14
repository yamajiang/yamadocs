{This is a basic Python Review}

## Syntax
- Indention is important to indicate blocks of code in Python
- Comments: 
```python
#one line comment

""" 
Commenting for
more than 
one line
! 
""" 
```

## Variables
- There's no command for declaring a variable, so you can just do `x = 9`.
- Variables are created whenever you assign a value to them, meaning you don't need to declare a type, and you're free to change the type after it has been created.
- If you want to specify the type, you can cast it.
- If you want to find the data type of the variable, you can print it with `type()`.
- String variables can be declared with single or double quotes.
```python
#creating variables
x = 1
y = "yama"

#casting
x = int(1)  # 1
x = str(1)  # '1'
x = float(1)  # 1.0

#type
print(type(x))

#string
x = "yama"
x = 'yama'
# ^ these two are the same
```

### Names
- Variable names must start with a letter or underscore; cannot start with numbers.
- Variable names are case-sensitive (`hello`, `HELLO`, `Hello` are all different).
- Cannot be a Python keyword.
- Variable names can only contain alphanumeric characters and underscores (A-z, 0-9, and _ ).
- Variable naming conventions:
```python
#camelCase
thisIsCamelCase = "hi"

#PascalCase 
ThisIsPascalCase = "hello"

#snake_case
this_is_snake_case = "hey"
```

### Multiple Values
- You can assign multiple variables in one line:
```python
x, y, z = "apple", "orange", "cherry"
```
- If you have a list, you can unpack it to extract the values into variables:
```python
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
```

## Data Types
- Common data types:
```python
x = 5               #int
y = 5.5             #float
z = 1j              #complex
name = "yama"       #str
is_cool = True      #bool
fruits = ["apple", "banana"]  #list
tuple_example = ("apple", "banana")  #tuple
set_example = {"apple", "banana"}  #set
dict_example = {"name": "yama", "age": 20}  #dict
none_value = None   #none type
```

## Type Conversion
- Convert between data types:
```python
x = 5
x_str = str(x)  # "5"
y = "10"
y_int = int(y)  #10
```

## Operators
- Arithmetic: `+`, `-`, `*`, `/`, `%`, `**`, `//`
- Comparison: `==`, `!=`, `>`, `<`, `>=`, `<=`
- Logical: `and`, `or`, `not`
- Assignment: `=`, `+=`, `-=`, `*=`, `/=`
- Membership: `in`, `not in`
- Identity: `is`, `is not`

## Conditionals
```python
x = 10
y = 20
if x > y:
    print("x is greater")
elif x == y:
    print("x is equal to y")
else:
    print("y is greater")
```

## Loops
```python
#for loop
for i in range(5):
    print(i)

#while loop
count = 0
while count < 5:
    print(count)
    count += 1

#loop control statements
for i in range(10):
    if i == 5:
        break  # exits loop
    if i % 2 == 0:
        continue  # skips to next iteration
    print(i)
```

## Functions
```python
def greet(name):
    return "Hello " + name

print(greet("Yama"))

#function with default parameter
def greet(name="Guest"):
    return "Hello " + name

print(greet())

#lambda f unction
# -a small anonymous function defined using the 'lambda' keyword
# it can take any number of arguments but only has one expression, which is evaluated and returned
square = lambda x: x * x
print(square(5))  #output: 25
```

## Lists
- Lists are mutable (can be changed):
```python
my_list = [1, 2, 3, "apple"]
my_list.append(4)  #adds to the end
my_list.remove(2)  #removes first occurrence of 2
print(my_list)
```

## Dictionaries
```python
person = {"name": "Yama", "age": 20}
print(person["name"])  #access value
person["city"] = "Manhattan"  #add key-value pair
```

## Exception Handling
```python
try:
    print(10 / 0)
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("Execution complete")
```

## File Handling
```python
#writing to a file
with open("example.txt", "w") as f:
    f.write("hello yama!")

#reading from a file
with open("example.txt", "r") as f:
    content = f.read()
    print(content)
```

## Extras
- Input:
```python
name = input("what's your name? ")
print("hello, " + name)
```
- Importing Modules:
```python
import math
print(math.sqrt(16))  # 4.0
```
- Import with Alias:
```python
import numpy as np
```
- Random Numbers:
```python
import random
print(random.randint(1, 100))  #random number between 1 and 100
```
