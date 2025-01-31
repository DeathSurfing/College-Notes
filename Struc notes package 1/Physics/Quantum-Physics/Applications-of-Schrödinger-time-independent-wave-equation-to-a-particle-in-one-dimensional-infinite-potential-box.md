---
created: 2025-01-31T05:34:28.504496
modified: 2025-01-31T05:34:28.504502
source: "[[Quantum-physics]]"
hierarchy:
  - Physics
tags: []
summary: ""
concepts: []
ai_generated: false
---

# Applications of Schrödinger time independent wave equation to a particle in one dimensional infinite potential box

## Context Path
Physics

## Content


$\psi \text{ Vanishes at boundry at x=0 or L}$
$$\frac{\partial^2\psi}{\partial x^2}+\frac{4\pi^2}{h^2}\cdot 2(E-V)m\psi=0\dots1$$
$$\frac{\partial^2\psi}{\partial x^2}+k^2\psi=0\dots2$$
where $K^2=\frac{2mE}{\frac{h}{2 \pi}}$

$$\psi=ACos(kx)+BSin(kx)\dots3$$
$$\frac{2mE}{\frac{h}{2\pi}}=\frac{\pi^2n^2\frac{h}{2\pi}^2}{L^2}$$
$$E_n=\frac{\frac{h}{2\pi}^2n^2\pi^2}{2mL^2}$$



$$\int_0^L\psi^*\psi dx=1$$
$$\int_0^L(B^* sin(\frac{n\pi x}{L})\cdot Bsin(\frac{n\pi x}{L})dx=1$$
$$B^2\int_0^L \sin^2(\frac{n\pi x}{L})dx$$
$$\frac{B^2}{2}\int_0^Ldx-\int_0^L\cos(\frac{2xn\pi}{L})dx$$
$$\frac{B^2}{2}[2-0-\frac{L}{n\pi}[(\frac{\sin(\frac{2n\pi x}{L}}{2})]^L_0]$$
$$\frac{B^2L}{2}=1$$
$$B=\sqrt \frac{2}{L}$$
$$\psi=B\sin(\frac{n\pi x}{L})$$
$$\psi_n=\sqrt\frac{2}{L}\sin(\frac{n\pi x}{L})$$
$$\text{For Maximum condition}$$
$$\sin(\frac{\pi x}{L})=\sin(\frac{\pi}{2})$$
$$x=\frac{L}{2}$$


# Practice questions
___

1) 
$\lambda=\frac{\hbar}{p}$  
$\frac{\hbar}{\sqrt{2meV}}$ 
$\frac{\left(\frac{\left(6.62\cdot10^{-34}\right)}{2\pi}\right)}{\sqrt{2\cdot1.67\cdot10^{-27}\cdot1.60\cdot10^{-19}\cdot1.5\cdot10^{3}}}=7.4\cdot10^{-13}$

2) 
$\Delta X \Delta P \geq \frac{\hbar}{2}$ 
$1\cdot10^{-9}x\ge\frac{\left(\frac{6.62\cdot10^{-34}}{2\pi}\right)}{2}$
$x=5.25\cdot10^{-26}$ 

3) 
$\psi(x)=\sqrt{\frac{2}{L}}sin(\pi x L)$  

$\psi^*\psi=\frac{2}{l}\sin^2(\pi x L)$
$\int_0^L\psi^*\psi dx=1$ using gdc

4) 
$E_{n}=\frac{\pi^{2}n^{2}\left(\frac{h}{2\pi}\right)}{2mL^{2}}$
$E_{1}=1.426\cdot10^{14}$
$E_{2}=5.707\cdot10^{14}$
$E_{2}-E_{1}=4.281\times 10^{14}$ 

## Related Concepts
