---
created: '2025-01-31T06:13:35.409529'
modified: '2025-01-31T06:13:35.409535'
source: '[[Software-Design-Principles]]'
hierarchy:
- Software-and-System-Design
- Unit-1
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Software Design Principles

## Context Path
Software-and-System-Design > Unit-1

## Content
> **AI Generated Content**
 # Software Design Principles

## Core Definitions

Software design principles are fundamental guidelines that help developers create robust, maintainable, and efficient software systems. These principles provide a framework for making decisions about the architecture, structure, and implementation of software. They ensure that the software is not only functional but also scalable, adaptable, and easy to understand.

### Key Principles

1. **Single Responsibility Principle (SRP)**
   - A class should have only one reason to change.
   - Ensures that a class has a single responsibility, making the system easier to maintain and modify.

2. **Open-Closed Principle (OCP)**
   - Software entities should be open for extension but closed for modification.
   - Encourages the use of abstraction to allow new functionality without altering existing code.

3. **Liskov Substitution Principle (LSP)**
   - Objects of a superclass should be replaceable with objects of a subclass without affecting the correctness of the program.
   - Ensures that inheritance hierarchies are used correctly and safely.

4. **Interface Segregation Principle (ISP)**
   - Clients should not be forced to depend on interfaces they do not use.
   - Promotes the creation of small, focused interfaces tailored to specific client needs.

5. **Dependency Inversion Principle (DIP)**
   - High-level modules should not depend on low-level modules; both should depend on abstractions.
   - Reduces coupling and increases modularity by depending on abstractions rather than concrete implementations.

6. **Don't Repeat Yourself (DRY) Principle**
   - Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.
   - Prevents redundancy and promotes code reuse.

7. **You Aren't Gonna Need It (YAGNI)**
   - Implement something only when you need it.
   - Avoids unnecessary complexity by focusing on current requirements rather than future possibilities.

8. **Keep It Simple, Stupid (KISS) Principle**
   - The simplest solution is usually the best.
   - Encourages straightforward and clear design to improve maintainability and readability.

## Practical Applications

### Example: Designing a User Management System

- **Single Responsibility Principle (SRP)**: Create separate classes for user authentication, user profile management, and user notification. Each class has a single responsibility.

  ```python
  class AuthenticationService:
      def login(self):
          pass

      def logout(self):
          pass

  class ProfileService:
      def update_profile(self):
          pass

      def get_profile(self):
          pass

  class NotificationService:
      def send_notification(self):
          pass
  ```

- **Open-Closed Principle (OCP)**: Define an abstract base class for notifications and extend it for different types of notifications.

  ```python
  from abc import ABC, abstractmethod

  class Notification(ABC):
      @abstractmethod
      def send(self):
          pass

  class EmailNotification(Notification):
      def send(self):
          print("Sending email notification")

  class SMSNotification(Notification):
      def send(self):
          print("Sending SMS notification")
  ```

- **Liskov Substitution Principle (LSP)**: Ensure that a `User` object can be replaced with a `PremiumUser` object without breaking functionality.

  ```python
  class User:
      def get_discount(self):
          return 0

  class PremiumUser(User):
      def get_discount(self):
          return 10
  ```

- **Interface Segregation Principle (ISP)**: Create specific interfaces for different client needs.

  ```python
  from abc import ABC, abstractmethod

  class ReadOnlyInterface(ABC):
      @abstractmethod
      def read(self):
          pass

  class WriteOnlyInterface(ABC):
      @abstractmethod
      def write(self):
          pass
  ```

- **Dependency Inversion Principle (DIP)**: Use abstractions to define dependencies.

  ```python
  from abc import ABC, abstractmethod

  class PaymentProcessor(ABC):
      @abstractmethod
      def process_payment(self, amount):
          pass

  class PayPalPaymentProcessor(PaymentProcessor):
      def process_payment(self, amount):
          print(f"Processing payment of {amount} via PayPal")

  class CreditCardPaymentProcessor(PaymentProcessor):
      def process_payment(self, amount):
          print(f"Processing payment of {amount} via Credit Card")
  ```

## Relationships to Parent Concepts

### Software and System Design

Software design principles are a critical part of the broader field of software and system design. They help in creating well-structured, maintainable, and efficient systems. By adhering to these principles, developers can ensure that their software is scalable, adaptable, and easy to understand. This leads to better collaboration among team members and easier maintenance over time.

### Unit-1: Foundations of Software Design

In the context of a unit on foundations of software design, these principles provide the basic framework for creating robust and maintainable code. Understanding and applying these principles helps developers build a solid foundation upon which more complex systems can be constructed. This unit serves as an introduction to the essential practices that guide software development.

## Simple Examples

### Example: Building a Simple Calculator

- **Single Responsibility Principle (SRP)**: Create separate classes for addition, subtraction, multiplication, and division.

  ```python
  class Addition:
      def calculate(self, a, b):
          return a + b

  class Subtraction:
      def calculate(self, a, b):
          return a - b

  class Multiplication:
      def calculate(self, a, b):
          return a * b

  class Division:
      def calculate(self, a, b):
          if b == 0:
              raise ValueError("Cannot divide by zero")
          return a / b
  ```

- **Open-Closed Principle (OCP)**: Use a base class for operations and extend it for specific calculations.

  ```python
  from abc import ABC, abstractmethod

  class Operation(ABC):
      @abstractmethod
      def calculate(self, a, b):
          pass

  class Addition(Operation):
      def calculate(self, a, b):
          return a + b

  class Subtraction(Operation):
      def calculate(self, a, b):
          return a - b
  ```

- **Liskov Substitution Principle (LSP)**: Ensure that a `Calculator` object can be replaced with a `ScientificCalculator` object without breaking functionality.

  ```python
  class Calculator:
      def add(self, a, b):
          return a + b

      def subtract(self, a, b):
          return a - b

  class ScientificCalculator(Calculator):
      def multiply(self, a, b):
          return a * b

      def divide(self, a, b):
          if b == 0:
              raise ValueError("Cannot divide by zero")
          return a / b
  ```

By understanding and applying these software design principles, developers can create more reliable, maintainable, and scalable systems.

## Related Concepts
