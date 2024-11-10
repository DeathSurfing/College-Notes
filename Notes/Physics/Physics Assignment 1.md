___
# Q1
 
## i) Discuss the construction and working of Young’s Double slit experiment. Use it to find the position of the central bright, nth bright,

and nth dark fringe.
The experiment employs two screens: one with a single slit and the other with two slits. Because the two apertures are equidistant from the light source, the light waves that emerge from each are in phase. This converts the slits into coherent sources. 
 
The light waves from the two slits interact with one another, resulting in an interference pattern on the screen. The pattern is made up of alternating brilliant and black fringes, the former caused by constructive interference and the latter by destructive interference.

### Position of Dark Fringes
For minimum intensity, or a dark fringe to form at $P$, the path difference $\Delta z$ must be:
$$\Delta z = (2n + 1) \frac{\lambda}{2} \quad (n = 0, \pm 1, \pm 2, \dots)$$

which implies
$$x = \frac{(2n + 1) \lambda D}{2d}$$

The distance of the \( n \)-th dark fringe from the center is:
$$x_n = \frac{(2n + 1) \lambda D}{2d}$$
$$x_{n-1} = \frac{(2(n - 1) + 1) \lambda D}{2d}$$

The fringe width $\beta$ :

$$\beta = x_n - x_{n-1} = \frac{(2n + 1) \lambda D}{2d} - \frac{(2(n - 1) + 1) \lambda D}{2d} = \frac{\lambda D}{d}$$
where $n = 0$, $\pm 1$, $\pm 2$, $\dots$
### Position of Bright Fringes
For maximum intensity, or a bright fringe to form at $P$, the path difference $\Delta z$ must be:
$$\Delta z = n \lambda \quad (n = 0, \pm 1, \pm 2, \dots)$$

which implies
$$\frac{xd}{D} = n \lambda$$

or
$$x = \frac{n \lambda D}{d}$$

The distance of the \( n \)-th bright fringe from the center is:
$$x_n = \frac{n \lambda D}{d}$$

$$x_{n-1} = \frac{(n - 1) \lambda D}{d}$$
The fringe width $\beta$ :

$$
\beta = x_n - x_{n-1} = \frac{n \lambda D}{d} - \frac{(n - 1) \lambda D}{d} = \frac{\lambda D}{d}
$$

where $n = 0$, $\pm 1$, $\pm 2$, $\dots$


---
## ii)In Young’s Double slit, if D=12 m, d=0.25 cm, l=600 nm, calculate distance “y” from central maxima where intensity on screen is 75% of maximum intensity.
Given:
- $D = 12 \, \text{m}$
- $d = 0.25 \, \text{cm} = 0.0025 \, \text{m}$
- $\lambda = 600 \, \text{nm} = 600 \times 10^{-9} \, \text{m}$
- $I = 0.75 I_{\text{max}}$
   $$0.75 = \cos^2 \left( \frac{\pi y d}{\lambda D} \right)$$$$\sqrt{0.75} = \cos \left( \frac{\pi y d}{\lambda D} \right)$$
   $$\frac{\pi y d}{\lambda D} = \cos^{-1} \left( \sqrt{0.75} \right)$$
   $$y = \frac{\lambda D}{\pi d} \cos^{-1} \left( \sqrt{0.75} \right)$$
$$y=0.48 mm$$
___
# Q2

## i)Discuss the construction and working of Single slit experiment. Use it to find the positions of central bright, nth bright and nth dark fringe.

The single-slit experiment illustrates how light diffracts, resulting in an interference pattern of bright and dark fringes. The experiment is sending light through a narrow slit and then viewing the resulting pattern on a screen.

In the single slit diffraction experiment, the small angle approximation is used when the diffraction angle $\theta$ is small, typically measured in radians. The approximation is:

$\sin \theta \approx \theta$ and $\tan \theta \approx \theta$

This simplifies calculations, especially for determining fringe positions. For the **nth dark fringe**, the condition is:

$a \sin \theta_n = n \lambda$

Where  $a$ is the slit width and $\lambda$ is the wavelength. Using the small angle approximation, the position of the $n$-th dark fringe on the screen (at distance $D$) is:

$y_n \approx D \sin \theta_n$

For the **central bright fringe**, the position is $y_0 = 0$. Bright fringes occur between dark fringes but are more complex to express directly.

**Nth Bright Fringe**: The bright fringes occur between the dark fringes, and the position is approximately halfway between two dark fringes, but it's not as simple to express as a direct formula.
___
## ii)Find the width of central maxima in single slit diffraction located at 1m. Given the wavelength=500 nm and lens diameter=0.1mm.
$a \sin \theta_1 = \lambda$
Where:
- $a$ is the slit width (lens diameter),
- $\lambda$ is the wavelength of light.

$\Delta y = 2 D \sin \theta_1$

Given:
- $\lambda = 500\ nm = 500 \times 10^{-9}\ m$
- Lens diameter $a = 0.1\ mm = 0.1 \times 10^{-3}\ m$
- Distance to screen $D = 1\ m$

$a \sin \theta_1 = \lambda$
$\sin \theta_1 = \frac{\lambda}{a}$
$\sin \theta_1 = \frac{500 \times 10^{-9}}{0.1 \times 10^{-3}} = 5 \times 10^{-3}$

Since $\sin \theta_1 \approx \theta_1$ for small angles, we have:

$\theta_1 \approx 5 \times 10^{-3}\ radians$

$\Delta y = 2 D \sin \theta_1 = 2 \times 1 \times 5 \times 10^{-3} = 0.01\ m = 1\ cm$
___
# Q3

## i)Describe and explain the formation of Newton’s rings in reflected light and obtain the expressions for the diameter of the nth bright and dark ring. From your results, find expressions for radius of curvature of the Plano-convex lens, wavelength of monochromatic light and refractive index of the medium.
Newton's rings are formed by the interference of light waves reflecting between a plano-convex lens and a flat glass plate. A parallel beam of monochromatic light strikes the lens, and part of the light reflects off both the top and bottom surfaces of the thin air film between the lens and plate. The interference between these reflected waves creates alternating bright and dark rings. 

**Constructive interference (bright rings)** occurs when the path difference is an integer multiple of the wavelength $(m\lambda)$, while **destructive interference (dark rings)** occurs when the path difference is an odd multiple of half the wavelength $(m+\frac{1}{2})\lambda$.

The expression for the radius $r_n$ of the nth ring is:

$r_n = \sqrt{n \lambda R}$

where $n$ is the ring number, $\lambda$ is the wavelength of light, and $R$ is the radius of curvature of the lens.

The diameter $D_n$ of the nth ring is given by:

$D_n = 2r_n = 2 \sqrt{n \lambda R}$
### From these equations:
- The **radius of curvature** of the plano-convex lens, $R$, can be obtained by rearranging the formula for $r_n$.
- The **wavelength** $\lambda$ of the monochromatic light can be determined by analyzing the ring pattern.
### To find the expressions for the radius of curvature and wavelength

1. **Radius of Curvature ($R$):**
   From the expression $r_n = \sqrt{n \lambda R}$, solving for $R$ gives:

   $R = \frac{r_n^2}{n \lambda}$

2. **Wavelength ($\lambda$)**
   $\lambda = \frac{D_n^2}{4nR}$

___
## ii)In Newton’s rings experiment the diameter of 4th and 25th rings are 0.3 cm and 0.8 cm, respectively. Find the wavelength of light. Given radius of curvature R=100 cm

Using the formula $\lambda = \frac{D_n^2}{4nR}$

Given:
- $D_4 = 0.3$ cm (diameter of the 4th ring),
- $D_{25} = 0.8$ cm (diameter of the 25th ring),
- $R = 100$ cm.

For $n = 4$, the wavelength $\lambda$ can be calculated as:

$\lambda = \frac{D_4^2}{4 \cdot 4 \cdot R}$

Substitute the values:

$\lambda = \frac{(0.3)^2}{4 \cdot 4 \cdot 100} = \frac{0.09}{1600} = 5.625 \times 10^{-5}$ cm

For $n = 25$, the wavelength $\lambda$ can be calculated as:

$\lambda = \frac{D_{25}^2}{4 \cdot 25 \cdot R}$

Substitute the values:

$\lambda = \frac{(0.8)^2}{4 \cdot 25 \cdot 100} = \frac{0.64}{10000} = 6.4 \times 10^{-5}$ cm

$\lambda_{\text{avg}} = \frac{5.625 \times 10^{-5} + 6.4 \times 10^{-5}}{2} = 6.0125 \times 10^{-5}$ cm

$\lambda \approx 6.01 \times 10^{-5}$ cm or 600 nm.

___

# Q4 Newton rings observed in reflected light of wavelength 5900A. The diameter of the 10th dark ring is 0.5cm. 

## i)Find the radius of curvature of

$r_n = \sqrt{n \lambda R}$

$r_{10} = \sqrt{10 \times (5900 \times 10^{-10}) \times R}$

Substitute the known values:

$0.0025 = \sqrt{10 \times (5900 \times 10^{-10}) \times R}$

$(0.0025)^2 = 10 \times (5900 \times 10^{-10}) \times R$

$6.25 \times 10^{-6} = 5.9 \times 10^{-9} \times R$

$R = \frac{6.25 \times 10^{-6}}{5.9 \times 10^{-9}} = 1.06 \times 10^3 \, \text{m}$

## ii)The thickness of air film

$t_n = \frac{(n - \frac{1}{2}) \lambda}{2}$

For $n = 10$:

$t_{10} = \frac{(10 - \frac{1}{2}) \times 5900 \times 10^{-10}}{2}$

$t_{10} = \frac{9.5 \times 5900 \times 10^{-10}}{2} = 2.8025 \times 10^{-6} \, \text{m} = 2.8025 \, \mu\text{m}$

___
# Q5)State and explain Malus' law. How is it used to calculate the intensity of polarized light after passing through a polarizer?

describes the behavior of light intensity when polarized light passes through a polarizing filter. It states that the intensity of polarized light after passing through a polarizer is proportional to the cosine square of the angle (𝜃) between the light's polarization direction and the axis of the polarizer.

![[Screenshot 2024-11-10 at 7.32.55 PM.png]]
The diagram above is assuming source of light as unpolarized
The mathematical formula for Mauls law is:$I = I_0 \cos^2(\theta)$
___
# Q6)What is the Broglie hypothesis? Derive the expression for the deBroglie wavelength of a particle and explain its significance. Find the deBroglie wavelength of an electron moving with a speed of $1×10^6$ m/s.


De Broglie's Hypothesis says that Matter consists of both the particle nature as well as wave nature.
De Broglie wavelength $\lambda$ is given as $\lambda=\frac{h}{p}$, where p represents the particle momentum and can be written as
$p=mv$ 
making,
$\lambda=\frac{h}{mv}$ 
### Significance of De Broglie's hypothesis:
- **Wave-particle duality**: It shows that particles have wave-like characteristics, and these waves can be observed under specific conditions, particularly for small particles like electrons.
- **Electron diffraction**: The concept was crucial in explaining phenomena such as electron diffraction, where electrons, behaving like waves, can produce interference patterns.
- **Quantum mechanics**: The de Broglie wavelength played a key role in the development of quantum mechanics, particularly in the understanding of the behavior of electrons in atoms.

Given:
- Mass of electron, $m = 9.11 \times 10^{-31} \, \text{kg}$
- Speed of electron, $v = 1 \times 10^6 \, \text{m/s}$
- Planck's constant, $h = 6.626 \times 10^{-34} \, \text{J·s}$

Momentum of electron:
$p = mv = (9.11 \times 10^{-31} \, \text{kg}) \times (1 \times 10^6 \, \text{m/s}) = 9.11 \times 10^{-25} \, \text{kg·m/s}$

de Broglie wavelength:
$\lambda = \frac{h}{p} = \frac{6.626 \times 10^{-34}}{9.11 \times 10^{-25}} = 7.28 \times 10^{-10} \, \text{m} \, (0.728 \, \text{nm})$
___
# Q7) Define Wave function. Explain Physical Significance of the wave function. Also, list out the properties of wave function.

A wave function refers to a mathematical description of a particle's quantum state as a function of spin, time, momentum, and position.
Wave functions are denoted by the letter $\psi$ 

Wave functions are a complex function $\psi=A+Bi$
#### Normalised condition
$\int\psi^*\psi dx=1$
#### Orthogonal condition: 
$\int\psi^*\psi dx=0$
### Properties of the wave function:
- $\psi$ must be finite
- $\psi$ must be continuous
- $\psi$ must be a single value
- $\psi$ must be square integrable
___
# Q8) Define Schrödinger time-independent wave equation. Derive the Schrödinger time-independent wave equation

The time-independent Schrödinger wave equation is a differential equation that describes a quantum particle's wave nature in a stationary state, depending only on its position.

$$\frac{\partial^2\psi}{\partial x^2}=\frac{1}{v^2}\cdot \frac{\partial^2\psi}{\partial t^2}\dots_{1}$$

$$\psi=\psi_{0}e^{-i\omega t}\dots_{2}$$
$$\frac{\partial^2t}{\partial t^2}=-w^2\psi_{0}e^{-i\omega t}$$
$$\frac{\partial^2\psi}{\partial t^2}=-\omega^2\psi\dots_{3}$$
Where $v=velocity$
From Equation 1 and 3
$$\frac{\partial^2\psi}{\partial x^2}=-\frac{1}{v^2}\omega^2\psi$$
$$\omega =2\pi \nu$$
$$v=\lambda \nu$$
$$\frac{\omega ^2}{v^2}=\frac{4\pi^2}{\lambda^2}$$
$$\frac{\partial^2\psi}{\partial x^2}+\frac{4\pi^2}{h^2}+m^2v^2\psi=0$$
If E & V is total energy 
$$E=\frac{1}{2}mv^2+V$$
$$E-V=\frac{1}{2}mv^2$$
$$2(E-V)m=m^2v^2$$
## Schrödinger equation time independent: 
$$\frac{\partial^2\psi}{\partial x^2}+\frac{4\pi^2}{h^2}\cdot 2(E-V)m\psi=0$$
$$\frac{\partial \psi^2}{\partial x^2}+\frac{8\pi^2m(E-V)\psi}{\left( \frac{h}{2\pi} \right)^2}=0$$
$$\frac{\partial^2\psi}{\partial x^2}+\frac{2m(E-V)\psi}{\hbar^2}=0$$    


