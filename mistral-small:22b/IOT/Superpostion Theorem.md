---
created: '2025-01-31T02:56:50.739327'
modified: '2025-01-31T02:56:50.739330'
source: '[[Superpostion Theorem]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Superpostion Theorem

___
## Question 1:
![[Screenshot 2024-10-04 at 11.23.19 AM.png]]
- Can only be applied on 2 source (Voltage , current) are required

If you are going to consider 1 source it may be voltage/current source that time other sources will be replaced by their internal resistance 
	- The internal resistance of the current source is infinite , means resistance will act as a open circuit
	- The internal resistance of voltage source is $0 \Omega$, means resistance will act as a short circuit!

Step wise:
- Consider 5v source
	- [[Screenshot 2024-10-04 at 11.39.57 AM.png]]
	- ![[Screenshot 2024-10-04 at 11.41.29 AM.png]]
	- $R_{eq}=4.33\Omega$
	- $I=\frac{V}{R_{eq}}\to \frac{5}{4.33}=1.15A$
	- $I^{'}_{s}=\frac{1.15\times_{2}}{4+2}\to \frac{2.30}{6}=0.38A$


- Consider 6V Source:
	- ![[Screenshot 2024-10-04 at 11.51.11 AM.png]]
	- $R_{eq}=\frac{ 3\times 4}{3+4}=\frac{12}{7}+2=3.71\Omega$
	- $I_{S}=\frac{6}{3.71}=1.61A$
	- $I^{''}=\frac{1.61\times 3}{4+3}=0.69A$


$Total\ Current=I^{'}+I^{''}$
$I=0.38+0.69$
$I=1.07A$



## Question 2:
![[Screenshot 2024-10-04 at 11.58.41 AM.png]]

- Step 1 Consider 8V:
	- ![[Screenshot 2024-10-04 at 12.00.29 PM.png]]
	- ![[Screenshot 2024-10-04 at 12.00.57 PM.png]]
	- $I_{s}=\frac{V}{R_{eq}}$
	- $R_{eq}=3+4=7\Omega$
	- $I^{'}=\frac{V}{R_{eq}}=\frac{8}{7}=1.14A$

- Step 2 Consider 6 A Source:
	- ![[Screenshot 2024-10-04 at 12.04.05 PM 1.png]]
	- $I^{''}=\frac{6\times 3}{3+4}=\frac{18}{7}=2.57A$

$I =I^{'}+I^{''}$
$I=1.14+2.57$
$I=3.71A$$

### Question 2:

![[Screenshot 2024-10-08 at 1.25.27 PM.png]]

Taking 4v as active:

$\frac{12\times 8}{12+8}=4.8\Omega$
$\frac{14.8\times 5}{14.8+5}=3.73\Omega$
$3.73+5=8.73\Omega$

# Defination:
In any linear or bilateral network or circuit having more than one independent source, the response of an element will be equal to the algebraic sum of the responses of that element by considering one source at a time.


