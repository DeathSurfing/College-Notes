---
created: '2025-01-31T04:48:40.276957'
modified: '2025-01-31T04:48:40.276962'
source: '[[Object-Oriented-Programming]]'
hierarchy:
- Object-Oriented-Programming
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Interfaces

## Context Path
Object-Oriented-Programming

## Content
> **AI Generated Content**
 # Interfaces in Object-Oriented Programming

## Core Definitions

In object-oriented programming (OOP), an interface is a construct that defines a contract between classes. It specifies a set of methods and properties that implementing classes must provide, without including any implementation details. This allows for the creation of flexible and reusable code structures.

Key points about interfaces:
- **Abstract**: Interfaces cannot be instantiated directly; they are implemented by concrete classes.
- **Multiple Inheritance**: Unlike classes, a class can implement multiple interfaces, enabling polymorphism.
- **Method Signatures**: An interface defines method signatures (method names and parameters) but not their bodies.
- **Default Methods**: Some languages allow the inclusion of default methods with bodies within interfaces.

## Practical Applications

Interfaces are widely used in various programming scenarios:

### Dependency Injection
Interfaces facilitate dependency injection, a technique where an object's dependencies are provided by an external source rather than being created or managed internally. This promotes loose coupling and testability.

```java
public interface Logger {
    void log(String message);
}

public class ConsoleLogger implements Logger {
    public void log(String message) {
        System.out.println("Console: " + message);
    }
}

public class Application {
    private Logger logger;

    public Application(Logger logger) {
        this.logger = logger;
    }

    public void run() {
        // application logic
        logger.log("Application is running");
    }
}
```

### Plugin Architecture
Interfaces are essential for creating plugin architectures, allowing different components to be developed independently and then integrated seamlessly.

```csharp
public interface IPlugin {
    void Execute();
}

public class SamplePlugin : IPlugin {
    public void Execute() {
        Console.WriteLine("Sample Plugin Executed");
    }
}

public class PluginManager {
    private List<IPlugin> plugins = new List<IPlugin>();

    public void AddPlugin(IPlugin plugin) {
        plugins.Add(plugin);
    }

    public void RunPlugins() {
        foreach (var plugin in plugins) {
            plugin.Execute();
        }
    }
}
```

## Relationships to Parent Concepts

### Abstract Classes
- **Similarity**: Both interfaces and abstract classes can define abstract methods that must be implemented by subclasses.
- **Difference**: Interfaces are purely declarative, while abstract classes can provide partial implementations.

### Polymorphism
Interfaces support polymorphism by allowing objects of different classes to be treated as objects of a common interface type. This is achieved through method overriding and dynamic method dispatch.

```java
public interface Animal {
    void makeSound();
}

public class Dog implements Animal {
    public void makeSound() {
        System.out.println("Woof!");
    }
}

public class Cat implements Animal {
    public void makeSound() {
        System.out.println("Meow!");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal myDog = new Dog();
        Animal myCat = new Cat();

        myDog.makeSound(); // Outputs: Woof!
        myCat.makeSound(); // Outputs: Meow!
    }
}
```

### Inheritance
Interfaces do not support inheritance in the traditional sense but can extend other interfaces, creating a hierarchical relationship. This allows for the composition of behaviors from multiple sources.

```java
public interface Flyable {
    void fly();
}

public interface Swimmable {
    void swim();
}

public interface Duck extends Flyable, Swimmable {
    // Additional methods specific to ducks can be added here
}
```

## Simple Examples

### Java
```java
interface Vehicle {
    void start();
    void stop();
}

class Car implements Vehicle {
    public void start() {
        System.out.println("Car started");
    }

    public void stop() {
        System.out.println("Car stopped");
    }
}
```

### Python
```python
from abc import ABC, abstractmethod

class Vehicle(ABC):
    @abstractmethod
    def start(self):
        pass

    @abstractmethod
    def stop(self):
        pass

class Car(Vehicle):
    def start(self):
        print("Car started")

    def stop(self):
        print("Car stopped")
```

### C#
```csharp
public interface IVehicle {
    void Start();
    void Stop();
}

public class Car : IVehicle {
    public void Start() {
        Console.WriteLine("Car started");
    }

    public void Stop() {
        Console.WriteLine("Car stopped");
    }
}
```

Interfaces are a powerful feature in object-oriented programming, enabling the creation of flexible and maintainable code by promoting abstraction and decoupling.

## Related Concepts
