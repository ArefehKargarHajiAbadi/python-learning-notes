# Loops in Python

Loops let us run the same block of code multiple times.  
There are two main types of loops in Python: **for loops** and **while loops**.

---

## 1. For Loop
Used when you want to iterate over a sequence (list, string, range, etc.).

### Example: Range
```python
for i in range(5):
    print(i)
```
### Example: List
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
## 2. While Loop

Repeats as long as the condition is True.
```python
count = 0
while count < 5:
    print(count) # Output: 0 1 2 3 4
```
### If the condition never becomes False, an infinte loop has been created.
## 3.Break and Continue
- break : exit the loop early
- continue : skip to the next iteration
```python
for i in range(10):
    if i == 5:
        break   # stop loop completely
    if i % 2 == 0:
        continue  # skip even numbers
    print(i)
```
### 4.Nested Loops
A loop inside another loop.
```python
for i in range(3):
  for j in range(2):
    print(i, j)
