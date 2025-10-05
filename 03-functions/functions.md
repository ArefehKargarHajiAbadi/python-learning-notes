# Functions in Python
A **Function** is a block of code that runs when it is 
called.
## Syntax
```python
def function_name(parameters):
  """docstring (optional)"""
  # code block
  return value
```

## Parameters and Arguments

**Parameters** are variables that a function **expects** when it is defined.  
**Arguments** are the actual values you **pass** to the function when you call it.

### Example:

```python
# Function with parameters
def greet(name, age):
   print(f"Hello {name}, you are {age} years old!")

# Calling the function with arguments
greet("Ali", 25)
# Output: Hello Ali, you are 25 years old!
```
## Return Values

A function can **return a value** back to the caller using the `return` statement.  
If a function does not have a `return` statement, it returns `None` by default.

### Example:

```python
# Function that returns a value
def add(a, b):
   return a + b

result = add(5, 3)
print(result)
# Output: 8
```

## Default and Keyword Arguments

### Default Arguments
You can provide **default values** for parameters.  
If the caller does not provide a value, the default is used.

```python
def greet(name="Guest"):
   print(f"Hello {name}!")

greet("Ali")  # Output: Hello Ali!
greet()       # Output: Hello Guest!
```
### Keyword Arguments

You can call a function by **explicitly naming the arguments**, regardless of their order.
```python
def describe_person(name, age, city):
   print(f"{name} is {age} years old and lives in {city}.")

# Using keyword arguments
describe_person(age=30, city="Tehran", name="Sara")
# Output: Sara is 30 years old and lives in Tehran.
```
## Lambda Functions

**Lambda functions** are small, anonymous functions defined using the `lambda` keyword.  
They are usually used for **short, simple operations** and can take any number of arguments but only **one expression**.

### Syntax:
```python
lambda arguments: expression
```
### Example:
```python
square_lambda = lambda x: x ** 2
print(square_lambda(5)) # output: 25
```

## Scope (Local vs Global)

**Scope** defines where a variable can be accessed in your code.  

### Local Scope
Variables defined **inside a function** are **local** to that function and cannot be accessed outside.

```python
def my_function():
   local_var = 10
   print("Inside function:", local_var)

my_function()            # Output: Inside function: 10
# print(local_var)       # Error! local_var is not defined outside
```
### Global Scope 
Variables defined **outside all functions** are **global** and can be accessed anywhere in the file.
```python
global_var = 20

def show_var():
    print("Inside function:", global_var)

show_var()               # Output: Inside function: 20
print("Outside function:", global_var)  # Output: Outside function: 20
```
## Docstrings and Best Practices
