# What Are Data Types?
Data types are classifications that specify what kind of
value a variable can hold and what operations can be performed on it.
## 1.Numeric Data Types 
Used to store numbers. They support arithemetic operations.<br>
**int**: Whole numbers(positive, negative, or zero)
```python 
x = 10
y = -5
```
**float**: Decimal numbers
```python
price = 19.99
```
**complex**: Complex numbers with real and imaginary part
```python
z = 3+4j
```
## 2.Sequence Data Types
Used to store collection of items.<br>
**str**: Strings(text)
```python
name = "Alice"
```
**list**: Ordered, mutable (changeable) collection of items.
```python
numbers = [1, 2, 3, 4]
```
**tuple**: Ordered, immutable collection of items.
```python
coordinates = (10, 20)
```
## 3.Set Data Types
Used to store unordered collections of unique items.
**set**: Mutable set of unique items.
```python
fruits = {"apple", "banana", "orange"}
```
**frozen**: Immutable set.
```python
frozen = frozenset([1, 2, 3])
```
## 4.Mapping Data Type
Used to store data in key_value pairs.
**dict**: Dictionary
```python
person = {"name": "Alice" , "age" : 25}
```
## 5.Boolean Type
Represents **True** or **False** values.
```python
is_active = True
is_admin = False
```
## 6.None Type
Represents the absence of a value.
```python
result = None
```
## point
- Python is dynamically typed, so don’t need to declare the type explicitly; it’s inferred automatically.
- It can be checked the type of a variable using **type()**.
```python
x = 10
print(type(x))  # <class 'int'>
```
