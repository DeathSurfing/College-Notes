---
created: '2025-01-31T03:06:43.252182'
modified: '2025-01-31T03:06:43.252188'
source: '[[Superpostion Theorem]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Question 1:

## Content
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




## Connections
- [[_MOC|Main Map of Content]]
- [[_TAGS|Tag Index]]
