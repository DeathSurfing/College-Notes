---
created: '2025-01-31T03:06:12.557819'
modified: '2025-01-31T03:06:12.557834'
source: '[[Norton''s Theorem]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# ___

## Content


![[Screenshot 2024-10-25 at 9.22.26 AM.png]]
# Step 1: 
Identify the load resistance
$R_L=10\Omega$ 

# Step 2:
Remove the load resistance from the circuit and name the terminal A&B![[Screenshot 2024-10-25 at 9.23.45 AM.png]]

# Step 3:
Across the terminal A&B find out Norton's resistance($R_N$) During the time all independent sources (Voltage , current) will be replaced by their internal resistance.


$R_N=\frac{2\times6}{2+6}+5=6.5\Omega$ 

# Step 4:
Make the terminal A & B short circuit ; then find out Norton Current in branch A & B.

![[Screenshot 2024-10-25 at 9.29.20 AM.png]]

$R_{EQ}=\frac{5\times6}{5+6}+2=4.72$
$I_S=\frac{20V}{4.72\Omega}=4.23A$
$I_N=\frac{4.23\times6}{5+6}=2.31A$

# Step 5:
Draw the Norton's equivalent circuit 
![[Screenshot 2024-10-25 at 9.34.40 AM.png]]
$I_L=\frac{2.31\times6.5}{6.5+10}=0.91A$

# Question 1:
![[Screenshot 2024-10-25 at 9.36.07 AM.png]]

$R_L=10\Omega$ 
$R_N=\frac{12}{8}=1.5\Omega$
$I_S=\frac{V}{R_{EQ}}$
$R_{EQ}=2\Omega$ 
$I_S=\frac{20}{2}=10A$
$I_N=\frac{6\times10}{6+0}=10A$
$I_L=\frac{10\times1.5}{1.5+10}=1.304A$


## Connections
- [[_MOC|Main Map of Content]]
- [[_TAGS|Tag Index]]
