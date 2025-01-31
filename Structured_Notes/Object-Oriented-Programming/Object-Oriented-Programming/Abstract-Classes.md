---
created: '2025-01-31T04:44:24.316524'
modified: '2025-01-31T04:44:24.316530'
source: '[[Object-Oriented-Programming]]'
hierarchy:
- Object-Oriented-Programming
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Abstract Classes

## Context Path
Object-Oriented-Programming

## Content
> **AI Generated Content**
 # Abstract Classes in Object-Oriented Programming

## Core Definitions

### What is an Abstract Class?
An abstract class in object-oriented programming (OOP) is a class that cannot be instantiated. It acts as a blueprint for other classes and can contain both abstract methods (methods without a body) and concrete methods (methods with a body). The primary purpose of an abstract class is to provide a common interface or base functionality for its subclasses while allowing them to implement specific details.

### Key Features of Abstract Classes
1. **Abstract Methods**: These are methods declared in the abstract class but do not have an implementation. Subclasses must provide an implementation for these methods.
2. **Concrete Methods**: These are regular methods with a body, which can be called directly from the subclass.
3. **Instantiation**: Abstract classes cannot be instantiated directly; they serve as templates for other classes.
4. **Access Modifiers**: Abstract classes and methods can have access modifiers such as public, protected, or private to control their visibility.

## Practical Applications

### Use Cases
1. **Framework Development**: Abstract classes are often used in frameworks where a common interface is needed but specific implementations vary.
2. **Polymorphism**: They enable polymorphic behavior by providing a common method signature that subclasses must adhere to, allowing for dynamic method dispatch.
3. **Code Reusability**: Abstract classes promote code reuse by encapsulating shared functionality and leaving the specific implementation details to subclasses.
4. **Template Method Pattern**: This design pattern uses an abstract class with a template method that defines the skeleton of an algorithm, calling abstract methods for steps that can vary.

### Example Scenarios
1. **Database Connections**: An abstract class `DBConnection` might have methods like `connect()`, `disconnect()`, and an abstract method `executeQuery(String query)`. Subclasses such as `MySQLConnection` or `PostgreSQLConnection` would provide specific implementations for `executeQuery`.
2. **Graphical User Interfaces (GUIs)**: An abstract class `Button` could define common behavior, while subclasses like `OKButton`, `CancelButton`, and `HelpButton` could implement specific functionalities.

## Relationships to Parent Concepts

### Inheritance
Abstract classes are a form of inheritance where a subclass inherits the abstract methods and concrete methods from its parent class. The subclass must provide implementations for all abstract methods inherited from the abstract class.

### Polymorphism
Polymorphism allows objects of different classes to be treated as objects of a common superclass, typically an abstract class. This is achieved through method overriding in subclasses.

### Encapsulation
Abstract classes can encapsulate common behavior and attributes, providing a clear interface for subclasses while hiding the implementation details from external clients.

## Simple Examples

### Example 1: Abstract Class in Java
```java
abstract class Animal {
    abstract void makeSound(); // Abstract method

    void sleep() {
        System.out.println("Sleeping..."); // Concrete method
    }
}

class Dog extends Animal {
    @Override
    void makeSound() {
        System.out.println("Bark"); // Implementation of abstract method
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.makeSound(); // Output: Bark
        dog.sleep();     // Output: Sleeping...
    }
}
```

### Example 2: Abstract Class in Python
```python
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def make_sound(self):
        pass

    def sleep(self):
        print("Sleeping...")

class Dog(Animal):
    def make_sound(self):
        print("Bark")

if __name__ == "__main__":
    dog = Dog()
    dog.make_sound()  # Output: Bark
    dog.sleep()       # Output: Sleeping...
```

## Conclusion
Abstract classes are a fundamental concept in object-oriented programming, enabling the creation of a common interface for subclasses while promoting code reuse and maintainability. By understanding abstract classes and their applications, developers can design more flexible and scalable systems.

## Related Concepts
