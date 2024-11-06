___

## Introduction:
### Classical Physics:
- Deals with larger sized objects and consists of mostly newtonian physics
### Quantum physics:
- Deals with small sized objects closer to the Planck length object and mostly deals with Special theory of relativity.
### Dual nature of light:
- Light acts as both wave and particle in circumstances
- For example
	- Light acts as a particle in the photoelectric effect
		- $h\nu=K.E+W$
		- Where $W=h\nu_{0}$
		- Which is same as $K.E=h(\nu-\nu_{0})$
	- Light acts as a wave in interference (Young double slits experiment)


### Compton scattering:
$\lambda_{f}-\lambda_{i}=\Delta \lambda=\frac{h}{m_{0}c}(1-\cos \theta)$

## De-Broglie hypothesis
$$\lambda=\frac{h}{p}$$
Where p is the momentum
$\lambda$ is the wavelength
h is Planck constant ($6.62607015×10^{-34}JHz^{-1}$)


## Basic postulates of quantum mechanics


## Heisenbergs uncertainty principle
Both position and momentum cant be figured out simultaneously for microscopic(Quantum) objects.
$$\Delta x\Delta px\geq \frac{h}{4\pi}$$
## Wave function
- Denoted by the letter $\psi$ 
- Is a complex function

$$\psi=A+Bi$$
$\psi^*=|\psi|$
$\psi^{*}=A-BI$
$|\psi|^2=|\psi*\psi|$ is the probability of 
$|\psi^2|=A^2+B^2$

#### Normalised condition
$\int\psi^*\psi dx=1$

#### Orthogonal condition: 
$\int\psi^*\psi dx=0$

### Properties of the wave function:
- $\psi$ must be finite
- $\psi$ must be continuous
- $\psi$ must be a single value
- $\psi$ must be square integrable

### Schrödinger wave equation:

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


##### De-broglie hypothesis
$$p=\frac{h}{\lambda}$$
$$\lambda=\frac{h}{mv}$$

$$\frac{\partial^2\psi}{\partial x^2}+\frac{4\pi^2}{h^2}+m^2v^2\psi=0$$
If E & V is total energy 
$$E=\frac{1}{2}mv^2+V$$
$$E-V=\frac{1}{2}mv^2$$
$$2(E-V)m=m^2v^2$$

## Schrödinger equation time independent: 
$$\frac{\partial^2\psi}{\partial x^2}+\frac{4\pi^2}{h^2}\cdot 2(E-V)m\psi=0$$
$$\frac{\partial \psi^2}{\partial x^2}+\frac{8\pi^2m(E-V)\psi}{\left( \frac{h}{2\pi} \right)^2}=0$$

$$\frac{\partial^2\psi}{\partial x^2}+\frac{2m(E-V)\psi}{\hbar^2}=0$$     
## Applications of Schrödinger time independent wave equation to a particle in one dimensional infinite potential box


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