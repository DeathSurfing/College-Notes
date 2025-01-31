---
created: '2025-01-31T05:40:46.925727'
modified: '2025-01-31T05:40:46.925733'
source: '[[Physics-Assignment-1]]'
hierarchy:
- Physics
tags: []
summary: ''
concepts: []
ai_generated: true

---

# ii)For a particle in the ground state (n = 1) of a one-dimensional infinite potential well of width L, calculate the probability of finding the particle between 0 and L/4.

## Context Path
Physics

## Content
> **AI Generated Content**
 # ii) Probability of Finding a Particle in the Ground State Between 0 and L/4 in a One-Dimensional Infinite Potential Well

## Core Definitions

### One-Dimensional Infinite Potential Well
A one-dimensional infinite potential well is a simplified model used in quantum mechanics to describe a particle confined within a certain region. The potential energy is zero inside the well and infinite outside, which means the particle cannot escape.

### Ground State
The ground state of a system is its lowest-energy state. For a one-dimensional infinite potential well of width \( L \), the ground state has quantum number \( n = 1 \).

### Wavefunction
In quantum mechanics, the wavefunction \( \psi(x) \) describes the probability amplitude of finding a particle at position \( x \). The probability density function is given by \( |\psi(x)|^2 \).

## Practical Applications

One-dimensional infinite potential wells are used to model various physical systems, such as:

- **Electrons in quantum dots**: These are small semiconductor particles that can be treated as one-dimensional infinite potential wells.
- **Particles in nanowires**: Nanowires can confine electrons or other particles within a narrow region, similar to an infinite potential well.
- **Atoms in optical lattices**: Optical lattices created by laser beams can trap atoms and mimic the behavior of particles in one-dimensional infinite potential wells.

## Relationships to Parent Concepts

### Quantum Mechanics
The concept of a particle in an infinite potential well is fundamental in quantum mechanics, illustrating key principles such as quantization of energy and the probabilistic nature of wavefunctions.

### Probability Density Function
The probability density function \( |\psi(x)|^2 \) is crucial for understanding where a particle might be found within the well. This concept extends to more complex systems, including multi-dimensional potentials and time-dependent problems.

## Simple Examples

### Ground State Wavefunction
For a particle in the ground state (\( n = 1 \)) of an infinite potential well of width \( L \):
\[ \psi_1(x) = \sqrt{\frac{2}{L}} \sin\left(\frac{\pi x}{L}\right) \]

### Probability Calculation
To find the probability of finding the particle between 0 and \( L/4 \), we integrate the probability density function over this interval:
\[ P = \int_{0}^{L/4} |\psi_1(x)|^2 \, dx \]

Substituting the ground state wavefunction:
\[ P = \int_{0}^{L/4} \left| \sqrt{\frac{2}{L}} \sin\left(\frac{\pi x}{L}\right) \right|^2 \, dx \]
\[ P = \int_{0}^{L/4} \frac{2}{L} \sin^2\left(\frac{\pi x}{L}\right) \, dx \]

Using the trigonometric identity \( \sin^2(x) = \frac{1 - \cos(2x)}{2} \):
\[ P = \int_{0}^{L/4} \frac{2}{L} \cdot \frac{1 - \cos\left(\frac{2\pi x}{L}\right)}{2} \, dx \]
\[ P = \int_{0}^{L/4} \frac{1}{L} \left( 1 - \cos\left(\frac{2\pi x}{L}\right) \right) \, dx \]

Integrating:
\[ P = \frac{1}{L} \left[ x - \frac{L}{2\pi} \sin\left(\frac{2\pi x}{L}\right) \right]_{0}^{L/4} \]
\[ P = \frac{1}{L} \left( \frac{L}{4} - 0 \right) - \frac{1}{2\pi} \left[ \sin\left(\frac{\pi}{2}\right) - \sin(0) \right] \]
\[ P = \frac{1}{4} - \frac{1}{2\pi} (1 - 0) \]
\[ P = \frac{1}{4} - \frac{1}{2\pi} \]
\[ P = \frac{\pi - 2}{4\pi} \]

Thus, the probability of finding the particle between 0 and \( L/4 \) is:
\[ P = \frac{\pi - 2}{4\pi} \approx 0.127 \]

This calculation illustrates how quantum mechanics provides a probabilistic description of particle positions within confined systems.

## Related Concepts
