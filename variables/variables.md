## Variables
- In Python, a variable is a container that stores data values, such as numbers, strings, or lists.
- variables are similar to those in algebra, but they can represent a wider range of information

here is hyperlink - [link for w3schools]("https://www.w3schools.com/python/python_variables.asp")

## Creating Variables

- Python has no command for declaring a variable.

- A variable is created the moment you first assign a value to it.

### Example
```
x = 5
y = "John"
print(x)
print(y)
```
## Casting
- If you want to specify the data type of a variable, this can be done with casting.

### Example
```
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
```

## Variable Names
- A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume). Rules for Python variables:
- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive (age, Age and AGE are three different variables)
- A variable name cannot be any of the Python keywords.

## Example
#### Legal variable names:
```
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```

## Mulitiple variables- Many Values to Multiple Variables
- Python allows you to assign values to multiple variables in one line:

### Example
```
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```
## Unpack a Collection
- If you have a collection of values in a list, tuple etc. Python allows you to extract the values into variables. This is called unpacking.

### Example
#### Unpack a list:
```
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
```
## Output Variables
- The Python print() function is often used to output variables.

### Example
```
x = "Python is awesome"
print(x)
```

- In the print() function, you output multiple variables, separated by a comma:

### Example
```
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
```

- You can also use the + operator to output multiple variables:

### Example
```
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)
```

- Notice the space character after "Python " and "is ", without them the result would be "Pythonisawesome".

#### For numbers, the + character works as a mathematical operator:

### Example
```
x = 5
y = 10
print(x + y)
```
## Global Variables

**Variables that are created outside of a function (as in all of the examples in the previous pages) are known as global variables.**

- Global variables can be used by everyone, both inside of functions and outside.

### Example
- Create a variable outside of a function, and use it inside the function
```
x = "awesome"

def myfunc():
  print("Python is " + x)

myfunc()
```
## The global Keyword
**Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.***

To create a global variable inside a function, you can use the global keyword.

### Example
- If you use the global keyword, the variable belongs to the global scope:
```
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```
