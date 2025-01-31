---
created: '2025-01-31T06:09:32.896121'
modified: '2025-01-31T06:09:32.896127'
source: '[[Types-of-design-patterns]]'
hierarchy:
- Software-and-System-Design
- Unit-1
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Object Oriented Design:

## Context Path
Software-and-System-Design > Unit-1

## Content
> **AI Generated Content**
 # Object Oriented Design (OOD)

## Core Definitions

Object-Oriented Design (OOD) is a paradigm for designing software that focuses on data rather than process. It provides a clear modular structure for programs by using "objects" – instances of classes – which can contain data and code: data in the form of fields, and code, in the form of procedures.

### Key Concepts

1. **Class**: A blueprint or template that defines the properties (attributes) and behaviors (methods) of an object.
2. **Object**: An instance of a class. Objects are created dynamically at runtime.
3. **Inheritance**: A mechanism where one class can inherit attributes and methods from another class, promoting code reuse and hierarchical classification.
4. **Encapsulation**: The bundling of data with the methods that operate on that data. It restricts direct access to some of an object's components, which is a means of preventing accidental interference and misuse of the properties of an object in the class.
5. **Polymorphism**: Allows objects to be treated as instances of their parent class rather than their actual class. The most common use of polymorphism is to have a parent class reference that can call a method of either the parent or child classes.
6. **Abstraction**: Hides the complexity and only shows the essential features of the object. It helps in reducing programming complexity and effort.

## Practical Applications

Object-Oriented Design has been widely adopted in various fields due to its flexibility, scalability, and reusability. Some practical applications include:

1. **Software Development**: OOD is used extensively in developing software applications, such as desktop applications, web applications, and mobile applications.
2. **Game Development**: Games often require complex interactions between various entities (e.g., characters, items), which can be effectively managed using object-oriented principles.
3. **Simulation Systems**: Objects can represent real-world entities in simulations, making OOD suitable for creating realistic models.
4. **Enterprise Applications**: Large enterprise applications benefit from the modularity and reusability provided by OOD.
5. **Artificial Intelligence (AI) and Machine Learning (ML)**: AI/ML systems often involve complex data structures and behaviors that can be effectively modeled using objects.

## Relationships to Parent Concepts

Object-Oriented Design is a subset of Software Design, which itself is part of the broader field of System Design. The relationships can be summarized as follows:

1. **System Design**: Focuses on the architecture and structure of an entire system, including hardware and software components. It deals with high-level decisions about how different parts of a system should work together.
2. **Software Design**: Concentrates on the organization of software systems into modules or units that can be developed, tested, and maintained independently.
3. **Object-Oriented Design (OOD)**: A specific approach within Software Design that structures software around data, grouped into objects. It emphasizes modularity, reusability, and maintainability.

## Simple Examples

### Example 1: Bank Account System

```python
class Account:
    def __init__(self, account_number, balance=0):
        self.account_number = account_number
        self.balance = balance

    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"Deposited {amount}. New balance is {self.balance}.")
        else:
            print("Invalid deposit amount.")

    def withdraw(self, amount):
        if 0 < amount <= self.balance:
            self.balance -= amount
            print(f"Withdrew {amount}. New balance is {self.balance}.")
        else:
            print("Insufficient funds or invalid amount.")

    def get_balance(self):
        return self.balance

# Create an account object
account = Account("123456", 1000)

# Perform transactions
account.deposit(500)
account.withdraw(200)
print(f"Current balance: {account.get_balance()}")
```

### Example 2: Shape Hierarchy

```python
class Shape:
    def __init__(self, color):
        self.color = color

    def set_color(self, color):
        self.color = color

    def get_color(self):
        return self.color

    def area(self):
        raise NotImplementedError("Subclass must implement abstract method")

class Circle(Shape):
    def __init__(self, color, radius):
        super().__init__(color)
        self.radius = radius

    def area(self):
        return 3.14 * self.radius ** 2

class Rectangle(Shape):
    def __init__(self, color, width, height):
        super().__init__(color)
        self.width = width
        self.height = height

    def area(self):
        return self.width * self.height

# Create shape objects
circle = Circle("red", 5)
rectangle = Rectangle("blue", 4, 6)

# Calculate areas
print(f"Circle Area: {circle.area()}")
print(f"Rectangle Area: {rectangle.area()}")
```

These examples demonstrate the core principles of Object-Oriented Design, including encapsulation, inheritance, and polymorphism.

## Related Concepts
