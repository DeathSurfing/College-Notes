---
created: '2025-01-31T06:08:36.535087'
modified: '2025-01-31T06:08:36.535093'
source: '[[Types-of-design-patterns]]'
hierarchy:
- Software-and-System-Design
- Unit-1
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Types of design patterns:

## Context Path
Software-and-System-Design > Unit-1

## Content
> **AI Generated Content**
 # Types of Design Patterns

## Core Definitions

A design pattern is a general reusable solution to a commonly occurring problem in software design. It is not a finished design that can be transformed directly into code, but rather a description or template for how to solve a problem that can be used in many different situations. Design patterns are categorized into three main types:

1. **Creational Patterns**: These deal with object creation mechanisms, trying to create objects in a manner suitable to the situation. The basic idea is to have object creation controlled by a single class while hiding the instantiation logic from the client classes.
   - Examples include Singleton, Factory Method, Abstract Factory, Builder, and Prototype patterns.

2. **Structural Patterns**: These concern the composition of classes or objects into larger structures, while keeping these structures flexible and efficient.
   - Examples include Adapter, Bridge, Composite, Decorator, Facade, Flyweight, and Proxy patterns.

3. **Behavioral Patterns**: These are concerned with algorithms and the assignment of responsibilities between objects. They define a way to communicate between different parts of a program without specifying how these parts are implemented.
   - Examples include Chain of Responsibility, Command, Interpreter, Iterator, Mediator, Memento, Observer, State, Strategy, Template Method, and Visitor patterns.

## Practical Applications

### Creational Patterns
- **Singleton**: Ensures a class has only one instance and provides a global point of access to it. Used in logging, configuration settings, thread pool management.
- **Factory Method**: Defines an interface for creating objects but lets subclasses decide which class to instantiate. Useful in frameworks where the implementation details need to be hidden from clients.

### Structural Patterns
- **Adapter**: Allows incompatible interfaces to work together. Commonly used in legacy systems or when integrating third-party libraries.
- **Composite**: Composes objects into tree structures to represent part-whole hierarchies. Widely used in GUI development for managing a complex tree of UI components.

### Behavioral Patterns
- **Observer**: Defines a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically. Used in event-driven systems like GUIs or real-time data feeds.
- **Strategy**: Defines a family of algorithms, encapsulates each one, and makes them interchangeable. Used in sorting algorithms, compression techniques, etc.

## Relationships to Parent Concepts

Design patterns are a part of the broader field of software design principles and architectural patterns. They are closely related to:

- **Object-Oriented Design (OOD)**: Patterns often leverage OOD principles such as encapsulation, inheritance, and polymorphism.
- **Software Architecture**: Patterns can be used at various levels of software architecture, from low-level design to high-level architectural styles.
- **Design Principles**: They embody several fundamental design principles like the Open/Closed Principle (OCP), Dependency Inversion Principle (DIP), and Single Responsibility Principle (SRP).

## Simple Examples

### Singleton Pattern
```java
public class Singleton {
    private static Singleton instance;

    private Singleton() {}

    public static synchronized Singleton getInstance() {
        if (instance == null) {
            instance = new Singleton();
        }
        return instance;
    }
}
```

### Observer Pattern
```java
import java.util.ArrayList;
import java.util.List;

interface Observer {
    void update(String message);
}

class ConcreteObserver implements Observer {
    private String name;

    public ConcreteObserver(String name) {
        this.name = name;
    }

    @Override
    public void update(String message) {
        System.out.println(name + " received: " + message);
    }
}

class Subject {
    private List<Observer> observers = new ArrayList<>();

    public void attach(Observer observer) {
        observers.add(observer);
    }

    public void detach(Observer observer) {
        observers.remove(observer);
    }

    public void notifyObservers(String message) {
        for (Observer observer : observers) {
            observer.update(message);
        }
    }
}
```

### Strategy Pattern
```java
interface SortStrategy {
    void sort(int[] array);
}

class BubbleSort implements SortStrategy {
    @Override
    public void sort(int[] array) {
        // Implementation of bubble sort
    }
}

class QuickSort implements SortStrategy {
    @Override
    public void sort(int[] array) {
        // Implementation of quick sort
    }
}

class Context {
    private SortStrategy strategy;

    public void setStrategy(SortStrategy strategy) {
        this.strategy = strategy;
    }

    public void executeStrategy(int[] array) {
        strategy.sort(array);
    }
}
```

By understanding and applying these design patterns, developers can create more flexible, reusable, and maintainable software systems.

## Related Concepts
