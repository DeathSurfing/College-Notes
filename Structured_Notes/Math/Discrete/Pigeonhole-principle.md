---
created: '2025-01-31T05:56:21.670650'
modified: '2025-01-31T05:56:21.670656'
source: '[[Discrete]]'
hierarchy:
- Math
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Pigeonhole principle

## Context Path
Math

## Content
> **AI Generated Content**
 # The Pigeonhole Principle

## Core Definitions

The Pigeonhole Principle is a fundamental concept in combinatorics and discrete mathematics. It states that if \( n \) items are put into \( m \) containers, with \( n > m \), then at least one container must contain more than one item. This principle is often used to establish simple bounds on the number of elements required for certain properties to hold.

### Formal Statement

Let's formalize the Pigeonhole Principle:

- **Containers (Pigeonholes):** A set \( C \) with \( m \) distinct elements.
- **Items (Pigeons):** A set \( I \) with \( n \) distinct elements where \( n > m \).
- **Mapping:** A function \( f: I \to C \) that maps each item to a container.

By the Pigeonhole Principle, there exists at least one container \( c \in C \) such that \( |f^{-1}(c)| > 1 \).

## Practical Applications

The Pigeonhole Principle has numerous applications in various fields of mathematics and computer science. Here are a few notable examples:

### 1. Combinatorial Designs

In the construction of combinatorial designs like balanced incomplete block designs (BIBDs), the principle ensures that certain configurations must exist given specific constraints.

### 2. Computer Science

- **Hashing:** In hash tables, the Pigeonhole Principle helps understand the likelihood of collisions when more items are hashed than there are available buckets.
- **Error Detection:** It can be used to establish bounds on error detection codes and algorithms.

### 3. Graph Theory

The principle is often applied in graph theory to prove properties about graphs, such as the existence of certain subgraphs or the minimum number of edges required for a graph to have specific characteristics.

## Relationships to Parent Concepts

The Pigeonhole Principle is closely related to several fundamental concepts in mathematics:

### 1. Combinatorics

It is a cornerstone in combinatorial reasoning, often used to derive bounds and establish the existence of certain configurations.

### 2. Set Theory

The principle can be seen as an application of basic set theory, particularly when dealing with partitions of sets and mappings between them.

### 3. Discrete Mathematics

In discrete mathematics, it is used to prove theorems related to counting and partitioning problems.

## Simple Examples

To illustrate the Pigeonhole Principle, consider the following examples:

### Example 1: Distributing Books

Suppose you have 5 books and 3 shelves. If you distribute the books across the shelves, at least one shelf must contain more than one book. This is because \( n = 5 \) (books) and \( m = 3 \) (shelves), with \( n > m \).

### Example 2: Birthdays in a Group

In a group of 10 people, there are only 12 months in a year. By the Pigeonhole Principle, at least two people must share the same birthday month because \( n = 10 \) (people) and \( m = 12 \) (months), with \( n > m \).

### Example 3: Coloring a Graph

Consider a graph with 6 vertices, each connected to every other vertex. If you attempt to color this graph using only 5 colors, the Pigeonhole Principle guarantees that at least two adjacent vertices will have the same color. Here, \( n = 6 \) (vertices) and \( m = 5 \) (colors), with \( n > m \).

## Conclusion

The Pigeonhole Principle is a powerful and intuitive tool in mathematics that finds applications across various domains. Its simplicity belies its utility in proving complex properties and establishing bounds in combinatorial problems.

## Related Concepts
