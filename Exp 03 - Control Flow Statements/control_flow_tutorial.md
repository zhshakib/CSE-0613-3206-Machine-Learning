# Control Flow — Short Tutorial

This short page covers comparison and logical operators, conditional statements, iterators and `range`, `for` and `while` loops, and a brief functions example.

## Comparison & Logical Operators
- Comparison: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Logical: `and`, `or`, `not`

Example:

```python
x = 10
print(x > 5)         # True
print(x == 5 or x>8) # True
print(not (x < 0))   # True
```

## Conditional Statements
Use `if`, `elif`, `else` to branch logic.

```python
score = 85
if score >= 90:
    grade = 'A'
elif score >= 80:
    grade = 'B'
else:
    grade = 'C'
print(grade)  # B
```

## Iterators & `range()`
- An iterator produces values one at a time.
- `range(start, stop, step)` creates a sequence of integers (stop is exclusive).

```python
for i in range(3):    # 0,1,2
    print(i)

for i in range(1, 6, 2):  # 1,3,5
    print(i)
```

## `for` Loop
Iterate over lists, strings, ranges, generators, etc.

```python
fruits = ['apple', 'banana', 'cherry']
for f in fruits:
    print(f)
```

Use `enumerate()` for index + value:

```python
for idx, val in enumerate(fruits, start=1):
    print(idx, val)
```

## `while` Loop
Run while a condition holds; ensure it can terminate.

```python
n = 3
while n > 0:
    print(n)
    n -= 1
# prints 3,2,1
```

Use `break` to exit early and `continue` to skip to next iteration.

## Functions (at the end)
Define reusable behavior with `def`.

```python
def greet(name):
    if not name:
        return 'Hello!'
    return f'Hello, {name}!'

print(greet('Ana'))   # Hello, Ana!
print(greet(''))      # Hello!
```

That’s a compact reference — try these snippets interactively in `control_flow.ipynb` to experiment.