___
## Python interpreter
A Python interpreter is a computer program that translates Python code into machine code that a computer can understand and execute

## Modes of python Interpreter
- CPython
- PyPy
- IronPython
- JyThon
## Values, and data types
- Python figures out variable types on it's own; it doesn't require explicit types and inferences types from it.

Naming Rules:
- Must start with a letter or underscore
- Can contain letters, numbers and underscores
- Case-sensitive
- (PREFERIBLE CAMLECASE)




## Variables


## Keywords
### The function that gives complete list of all keywords in python
```py
import keyword
print(keyword.kwlist)
```


## Identifiers

## Statements & Expressions
- For Numbers + - * / %
- Special use case for + for string concatenation and % for formating
- Logical operator words (and , or, not)

## Input and output
Using Input() Function reads user input as a string:

```py
name = input("What is your Name?")
```
- Type Conversion: Type casting to convert input to other types

```py
age=int(input("Enter your age: "))
```

Formatted output: use f-strings or format() for displaying variables 
```py
name = "Alice"

score=95

print(f"Student {name} Scored {score}in the exam")
```


## Comments 


Single line comments : 
```py
# This is a comment
```

Multi Line Comments:
```py
""" This is a multi line
Comment and can span multiple
lines
"""
```


## Docstring
- Special comments that describe the purpose and usage of functions, classes or modules
- Provide documentation that can be accessed via help()
- Use a consistent format
- provides standardised across codebases.

## Assignment 2:
```py
x=34-23
y="Hello"
z=3.45
if z==3.45 or y=="Hello":
	x=x+1
	y=y+" World"

print(x)
print(y)
```
Output:
12
Hello World
### REPL
Read 
Evaluate
Print
Loop



