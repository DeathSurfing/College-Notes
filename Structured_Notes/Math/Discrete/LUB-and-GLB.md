---
created: '2025-01-31T05:53:41.238612'
modified: '2025-01-31T05:53:41.238618'
source: '[[Discrete]]'
hierarchy:
- Math
tags: []
summary: ''
concepts: []
ai_generated: true

---

# LUB and GLB

## Context Path
Math

## Content
> **AI Generated Content**
 # Lower Bound (LUB) and Greatest Lower Bound (GLB) in Mathematics

## Core Definitions

### Lower Bound (LUB)
- **Definition**: A lower bound for a set \( S \) is an element \( l \) such that for all elements \( x \in S \), \( l \leq x \).
- **Formally**: If \( S \) is a subset of real numbers, then \( l \) is a lower bound for \( S \) if \( l \leq x \) for every \( x \in S \).

### Greatest Lower Bound (GLB)
- **Definition**: The greatest lower bound (also known as the infimum or meet) of a set \( S \) is the largest element that is less than or equal to all elements in \( S \).
- **Formally**: If \( S \) is a subset of real numbers, then \( \inf(S) \) (or GLB) is defined such that:
  - \( \inf(S) \leq x \) for every \( x \in S \), and
  - There does not exist any element \( y > \inf(S) \) that satisfies the above condition.

## Practical Applications

### LUB in Optimization Problems
- **Application**: In optimization problems, finding a lower bound can help determine feasible solutions more efficiently. For example, in linear programming, lower bounds are used to prune the search space and improve computational efficiency.
- **Example**: When solving for the minimum value of a function \( f(x) \), determining a lower bound helps in narrowing down the possible values where the minimum might occur.

### GLB in Statistics and Probability
- **Application**: In statistics, the GLB is often used to estimate parameters or to determine confidence intervals. For instance, the GLB can be employed to find the maximum likelihood estimator (MLE) for a parameter.
- **Example**: Consider a set of sample means \( \{\bar{x}_1, \bar{x}_2, ..., \bar{x}_n\} \). The GLB of this set provides an estimate of the population mean that is less likely to overestimate the true mean.

## Relationships to Parent Concepts

### LUB and Supremum (Sup)
- **Relation**: The supremum of a set \( S \) is the least upper bound for \( S \), analogous to how the infimum is the greatest lower bound.
- **Formally**: If \( S \) is a subset of real numbers, then \( \sup(S) \) (or LUB) is defined such that:
  - \( x \leq \sup(S) \) for every \( x \in S \), and
  - There does not exist any element \( y < \sup(S) \) that satisfies the above condition.

### GLB and Least Upper Bound (LUB)
- **Relation**: While the GLB is concerned with finding the largest element that is less than or equal to all elements in a set, the LUB focuses on finding the smallest element that is greater than or equal to all elements in the set.
- **Formally**: For a set \( S \) and its complement \( \mathbb{R} \setminus S \), if \( l \) is the GLB of \( S \), then it is the LUB of \( \mathbb{R} \setminus S \).

## Simple Examples

### Example for LUB
- **Set**: Consider the set \( S = \{1, 2, 3\} \).
- **Lower Bound**: Any number less than or equal to all elements in \( S \) is a lower bound. For example, \( l = -1 \) since \( -1 \leq 1 \), \( -1 \leq 2 \), and \( -1 \leq 3 \).
- **Greatest Lower Bound**: The greatest lower bound for \( S \) is \( \inf(S) = 1 \) because 1 is the largest number that is less than or equal to all elements in \( S \).

### Example for GLB
- **Set**: Consider the set \( T = \{2, 3, 4\} \).
- **Upper Bound**: Any number greater than or equal to all elements in \( T \) is an upper bound. For example, \( u = 5 \) since \( 5 \geq 2 \), \( 5 \geq 3 \), and \( 5 \geq 4 \).
- **Least Upper Bound**: The least upper bound for \( T \) is \( \sup(T) = 2 \) because 2 is the smallest number that is greater than or equal to all elements in \( T \).

By understanding these core definitions, practical applications, relationships, and simple examples, one can better appreciate the roles of lower bounds and greatest lower bounds in mathematics.

## Related Concepts
