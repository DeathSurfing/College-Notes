---
created: '2025-01-31T06:18:30.090143'
modified: '2025-01-31T06:18:30.090149'
source: '[[Functional-Independence]]'
hierarchy:
- Software-and-System-Design
- Unit-1
- Design-Principles
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Cohesion:

## Context Path
Software-and-System-Design > Unit-1 > Design-Principles

## Content
> **AI Generated Content**
 # Cohesion

## Core Definitions

Cohesion is a fundamental concept in software and system design that refers to the degree to which the responsibilities of a single module or class form a logical group. High cohesion indicates that the module or class has a well-defined purpose, making it easier to understand, maintain, and test. Conversely, low cohesion suggests that the module or class is responsible for multiple, unrelated tasks, leading to increased complexity and potential for errors.

## Practical Applications

### 1. **Software Development**
In software development, high cohesion is essential for creating maintainable and scalable codebases. By ensuring that each module or class has a single, well-defined responsibility, developers can:
   - **Improve Readability**: Code with high cohesion is easier to read and understand because it focuses on a specific task.
   - **Enhance Maintainability**: Changes in one part of the system are less likely to affect other parts, reducing the risk of introducing bugs.
   - **Simplify Testing**: Highly cohesive modules can be tested independently, making it easier to identify and fix issues.

### 2. **System Design**
In system design, cohesion helps in organizing components effectively:
   - **Microservices Architecture**: Each microservice should have high cohesion, focusing on a specific business capability or function.
   - **Database Normalization**: Tables with high cohesion contain data that is closely related, reducing redundancy and improving data integrity.

## Relationships to Parent Concepts

### 1. **Software-and-System-Design**
Cohesion is a critical principle within the broader context of software and system design. It directly influences other principles such as:
   - **Modularity**: High cohesion supports modularity by ensuring that each module has a clear boundary and purpose.
   - **Encapsulation**: Cohesive modules encapsulate their data and behavior, promoting information hiding and reducing dependencies.

### 2. **Design Principles**
Cohesion is closely related to other design principles:
   - **Single Responsibility Principle (SRP)**: SRP states that a class should have only one reason to change, which aligns with the goal of high cohesion.
   - **Open-Closed Principle (OCP)**: Cohesive modules are easier to extend without modification, adhering to OCP.

## Simple Examples

### 1. **Low Cohesion Example**
```java
public class Employee {
    public void calculateSalary() {
        // Calculates salary
    }

    public void saveToDatabase() {
        // Saves employee data to the database
    }

    public void sendEmailNotification() {
        // Sends email notifications
    }
}
```
In this example, the `Employee` class has multiple responsibilities: calculating salary, saving data, and sending emails. This results in low cohesion and makes the class difficult to maintain.

### 2. **High Cohesion Example**
```java
public class SalaryCalculator {
    public void calculateSalary(Employee employee) {
        // Calculates salary for the given employee
    }
}

public class DatabaseManager {
    public void saveToDatabase(Employee employee) {
        // Saves employee data to the database
    }
}

public class NotificationService {
    public void sendEmailNotification(Employee employee) {
        // Sends email notifications for the given employee
    }
}
```
In this improved example, each class has a single responsibility: calculating salary, saving data, and sending emails. This high cohesion makes the code more modular, maintainable, and easier to understand.

## Related Concepts
