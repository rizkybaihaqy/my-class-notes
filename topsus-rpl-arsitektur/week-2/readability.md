# Readability

## Aspect of Readability

- Well-written
  - simple syntax
  - well-known features & idioms
  - clear & concise logic
  - meaningfull names
- Well-Documented
  - Tells clearly what a piece of code does
  - Its input
  - Its return (if any)
  - External library or API (if any)
- Well-formatted
  - keeps up with comunity guidelines on aspects such as indentation and formatting

### Readability in Python

```python
for idx in range(len(seq)):
    item = seq[idx]
    print(idx, '=>', item)
```

```python
for idx, item in enumerate(seq):
    print(idx, '=>', item)
```

In this case, the second version is closer to the way Python programmers would write code to solve the problem. The first way would be considered less Pythonic than the second one.

## Antipatterns

- Code with little or no comment
- Code which breaks best practices of the language
- Programming antipatterns
  - Spaghetti code: complex logic, lots of unconditional jumps
  - Big ball of mud: no overall structure, usually patched-up
  - Copy-Paste programming: stackoverflow syndrome
  - Ego programming: Cool Driven Development(CDD)

### Antipatterns in Python

- Mixed Indentation: mixing `\t` with space
- Mixing string literal types: mixing `'`, `"`, and `'''` or `"""`
- Overuse of functional constructs: overuse `map()`, `reduce()`, and `filter()`

## Techniques For Readability

### Document your code

- Inline documentation
- External documentation: `README` and `CHANGELOG`
- User Manuals: Formal document

### Follow Coding And Style Guidelines

In Python we follows PEP-8

- Code is read more than it is written. Providing a guideline would help
- Consistency within a project is important. However, __consistency within a module or package is more important__.
- Know when to ignore a guideline. For example, this may happen if adopting the guideline makes your code less readable, breaks the surrounding code, or breaks backward compatibility of the code.
- If a guideline is not directly applicable or useful for your organization, customize it.

### Review and refactor code

Reviews should be done with engineers who are familiar with the application, but
ideally, who are not working on the same code and do refactor if needed.

### Commenting the code

- Comments should be descriptive
- Code comments should be written in the block we are commenting on. __DON'T DO THIS PLEASE__:

```python
squares = map(lambda x: x*x, varray)
# The above code calculates the sum of squares of velocities
```

- Inline comments should be used as little as possible.
- Try to avoid comments that are superfluous and add little value. __The second comment is useless__:

```python
# The following code iterates through odd numbers
for number in numbers:
    # Skip if number is odd
    if number % 2 == 0: continue
```
