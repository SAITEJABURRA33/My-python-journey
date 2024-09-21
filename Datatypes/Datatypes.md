## Built-in Data Types
In programming, data type is an important concept.

- Variables can store data of different types, and different types can do different things.

- Python has the following data types built-in by default, in these categories:
```
Text Type     :	str
Numeric Types :	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type  :	dict
Set Types     :	set, frozenset
Boolean Type  :	bool
Binary Types  :	bytes, bytearray, memoryview
None Type     :	NoneType
```
## Setting the Data Type
****In Python, the data type is set when you assign a value to a variable****
```
Example	Data Type	
x = "Hello World"	                            str	
x = 20	                                        int	
x = 20.5	                                    float	
x = 1j	                                        complex	
x = ["apple", "banana", "cherry"]	            list	
x = ("apple", "banana", "cherry")	            tuple	
x = range(6)	                                range	
x = {"name" : "John", "age" : 36}	            dict	
x = {"apple", "banana", "cherry"}	            set	
x = frozenset({"apple", "banana", "cherry"})    frozenset	
x = True	                                    bool	
x = b"Hello"	                                bytes	
x = bytearray(5)	                            bytearray	
x = memoryview(bytes(5))	                    memoryview	
x = None	                                    NoneType	

```

## Python Numbers
There are three numeric types in Python:

- int
- float
- complex

Variables of numeric types are created when you assign a value to them:

Example
Integers:
```

x = 1
y = 35656222554887711
z = -3255522

print(type(x))
print(type(y))
print(type(z))
```

## Float

Float, or "floating point number" is a number, positive or negative, containing one or more decimals.

**Example**

Floats:
```
x = 1.10
y = 1.0
z = -35.59

print(type(x))
print(type(y))
print(type(z))
```

Float can also be scientific numbers with an "e" to indicate the power of 10.

## Example

**Floats:**
```
x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))
```

## Complex
Complex numbers are written with a "j" as the imaginary part:

## Example
**Complex:**
```
x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))
```

## Type Conversion

You can convert from one type to another with the int(), float(), and complex() methods:

## Example

**Convert from one type to another**
```
x = 1    # int
y = 2.8  # float
z = 1j   # complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
```
**NOTE: You cannot convert complex numbers into another number type.**

## Random Number

Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers:

## Example
Import the random module, and display a random number between 1 and 9:

```
import random

print(random.randrange(1, 10))
```