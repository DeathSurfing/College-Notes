---
created: 2025-01-31T05:33:25.692743
modified: 2025-01-31T05:33:25.692749
source: "[[Quantum-physics]]"
hierarchy:
  - Physics
tags: []
summary: ""
concepts: []
ai_generated: true
---

# Schrödinger wave equation:

## Context Path
Physics

## Content
> **AI Generated Content**
 # The Schrödinger Wave Equation

## Core Definitions

The Schrödinger wave equation is a fundamental equation in quantum mechanics that describes the time evolution of a quantum system. It was formulated by Erwin Schrödinger in 1926 and provides a way to understand how quantum states change over time.

### Time-Dependent Schrödinger Equation
The time-dependent Schrödinger equation is given by:
\[ i\hbar \frac{\partial}{\partial t} \Psi(\mathbf{r},t) = \hat{H} \Psi(\mathbf{r},t), \]
where:
- \(i\) is the imaginary unit,
- \(\hbar\) is the reduced Planck constant,
- \(\Psi(\mathbf{r},t)\) is the wave function, which describes the quantum state of the system,
- \(\hat{H}\) is the Hamiltonian operator, representing the total energy of the system.

### Time-Independent Schrödinger Equation
The time-independent Schrödinger equation is a special case where the wave function can be separated into spatial and temporal parts:
\[ \Psi(\mathbf{r},t) = \psi(\mathbf{r}) \phi(t), \]
leading to the equations:
\[ i\hbar \frac{\partial}{\partial t} \phi(t) = E \phi(t), \]
and
\[ \hat{H} \psi(\mathbf{r}) = E \psi(\mathbf{r}), \]
where \(E\) is the energy eigenvalue.

## Practical Applications

### Quantum Mechanics
The Schrödinger equation is central to quantum mechanics, providing a framework for solving problems in atomic and molecular physics. It allows physicists to calculate the probability distributions of particles and predict their behavior under various conditions.

### Chemistry
In chemistry, the Schrödinger equation is used to model the electronic structure of molecules and atoms, enabling calculations of molecular orbitals, bonding, and reaction mechanisms. This is particularly important in computational chemistry for understanding chemical reactions and properties at a quantum level.

### Materials Science
The equation plays a crucial role in materials science by helping to understand the behavior of electrons in solids. It aids in the development of new materials with desired electronic properties, such as semiconductors and superconductors.

## Relationships to Parent Concepts

### Quantum Mechanics
The Schrödinger equation is derived from the principles of quantum mechanics, particularly the wave-particle duality and Heisenberg's uncertainty principle. It provides a way to describe the probabilistic nature of quantum states and their evolution over time.

### Hamiltonian Mechanics
The Hamiltonian operator \(\hat{H}\) in the Schrödinger equation is derived from classical Hamiltonian mechanics, where it represents the total energy of a system. The transition from classical to quantum mechanics involves replacing classical variables with operators and using commutation relations.

## Simple Examples

### Particle in a Box
Consider a particle confined to a one-dimensional box of length \(L\). The time-independent Schrödinger equation for this system is:
\[ -\frac{\hbar^2}{2m} \frac{d^2 \psi(x)}{dx^2} = E \psi(x), \]
with boundary conditions \(\psi(0) = \psi(L) = 0\). The solutions are standing waves of the form:
\[ \psi_n(x) = \sqrt{\frac{2}{L}} \sin\left(\frac{n\pi x}{L}\right), \]
where \(n\) is a positive integer, and the energy eigenvalues are:
\[ E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2}. \]

### Harmonic Oscillator
For a one-dimensional harmonic oscillator with potential \(V(x) = \frac{1}{2} m \omega^2 x^2\), the time-independent Schrödinger equation is:
\[ -\frac{\hbar^2}{2m} \frac{d^2 \psi(x)}{dx^2} + \frac{1}{2} m \omega^2 x^2 \psi(x) = E \psi(x). \]
The solutions are Hermite polynomials, and the energy eigenvalues are:
\[ E_n = \hbar \omega \left( n + \frac{1}{2} \right), \]
where \(n\) is a non-negative integer.

## Related Concepts
