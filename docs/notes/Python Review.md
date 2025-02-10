{Review Notes made with W3 Schools}
## Syntax
- Indention is important to indicate blocks of codes in Python
- Comments: 
```
# one line comment 

""" 
commenting for
more than 
one line 
!
""" 
```
## Variables
- There's no command for declaring a variable, so you can just do x=9 
- Variables are created whenever you assign a value to it meaning you don't need to declare it as a type & you're free to change the type after its been created
- If you want to specify the type, you can cast it  
- If you want to find the data type of the variable, you can print it with type()
- String variables can be declared with single or double quotes 
```
  # creating variables
  x = 1
  y = "yama"
  
  # casting
  x = (int)1  # 1
  x = (str)1  # '1'
  x = (float)1  # 1.0

  # type
  print(type(x))

  # string
  x= "yama" 
  x= 'yama'
  # ^ these two are the same
```

### Names
- Variable names must start with a letter or underscore - cannot start with numbers
- Variable names are case sensitive (hello, HELLO, Hello)
- Cannot be a python keyword
- Variable name can only contain alpha numeric characters and underscores (A-z, 0-9, and _ )
- Variable naming conversions
```
# camelCase
thisIsCamelCase = "hi"

# PascalCase 
ThisIsPascalCase = "hello"

# snake_case
this_is_snake_case = "hey"


```
### Multiple Values
- You can assign multiple variables in one line 
```
x,y,x= "apple", "orange", "cherry"
```
- If you have a list, you can unpack it to extract the values into variables
```
fruits= ["apple", "banana", "cherry"]  
x, y, z = fruits
```