---
created: '2025-01-31T05:56:47.306396'
modified: '2025-01-31T05:56:47.306402'
source: '[[Discrete]]'
hierarchy:
- Math
tags: []
summary: ''
concepts: []
ai_generated: true

---

# Permutations and combinations

## Context Path
Math

## Content
> **AI Generated Content**
 # Permutations and Combinations

## Core Definitions

### Permutation
A permutation is an arrangement of objects in a specific order. The number of permutations of \( n \) distinct objects taken \( r \) at a time is given by:
\[ P(n, r) = \frac{n!}{(n-r)!} \]
where \( n! \) (n factorial) denotes the product of all positive integers up to \( n \).

### Combination
A combination is a selection of objects without regard to order. The number of combinations of \( n \) distinct objects taken \( r \) at a time is given by:
\[ C(n, r) = \frac{n!}{r!(n-r)!} \]
where \( r! \) (r factorial) denotes the product of all positive integers up to \( r \).

## Practical Applications

### Permutations
1. **Password Generation**: When creating a password, the order in which characters are entered matters. For example, if you have 26 letters and want a 3-letter password, the number of permutations is:
   \[ P(26, 3) = \frac{26!}{(26-3)!} \]

2. **Arranging Items**: If you have a collection of items and you want to know how many ways you can arrange them in order, permutations are used. For example, arranging 5 books on a shelf:
   \[ P(5, 5) = \frac{5!}{(5-5)!} \]

### Combinations
1. **Choosing a Committee**: When selecting members for a committee where the order of selection does not matter, combinations are used. For example, choosing 3 people from a group of 10:
   \[ C(10, 3) = \frac{10!}{3!(10-3)!} \]

2. **Lottery Draws**: In lotteries where the order in which numbers are drawn does not matter, combinations are applied. For example, choosing 5 winning numbers from a set of 49:
   \[ C(49, 5) = \frac{49!}{5!(49-5)!} \]

## Relationships to Parent Concepts

### Factorials
Both permutations and combinations rely heavily on the concept of factorials. The factorial of a non-negative integer \( n \) is the product of all positive integers less than or equal to \( n \). For example:
\[ 5! = 5 \times 4 \times 3 \times 2 \times 1 = 120 \]

### Binomial Coefficient
The binomial coefficient, often denoted as \( \binom{n}{r} \) or \( C(n, r) \), is a fundamental concept in combinatorics. It represents the number of ways to choose \( r \) elements from a set of \( n \) elements without regard to order.
\[ \binom{n}{r} = \frac{n!}{r!(n-r)!} \]

### Combinatorial Problems
Permutations and combinations are essential tools in solving combinatorial problems, which involve counting the number of ways certain events or arrangements can occur. These problems are common in fields such as probability theory, computer science, and operations research.

## Simple Examples

### Permutation Example
If you have 3 different books (Book A, Book B, and Book C) and you want to arrange them on a shelf, the number of possible permutations is:
\[ P(3, 3) = \frac{3!}{(3-3)!} = \frac{6}{1} = 6 \]
So, the books can be arranged in the following ways: ABC, ACB, BAC, BCA, CAB, CBA.

### Combination Example
If you have a group of 5 friends and you want to choose 2 of them to go on a trip with you, the number of possible combinations is:
\[ C(5, 2) = \frac{5!}{2!(5-2)!} = \frac{120}{2 \times 6} = 10 \]
So, there are 10 different ways to choose 2 friends out of 5.

## Related Concepts
