---
created: '2025-01-31T02:56:50.815822'
modified: '2025-01-31T02:56:50.815825'
source: '[[Particular Integral]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Particular Integral

___

$\text{General Form:}[f(D)]y=Q(x)$
$\text{Particular Integral}=\frac{1}{f(D)}\times[Q(X)]$ 


# Finding particular Integral

## Case 1: $Q(X)=e^{ax}$:
$D=a$
### Worked Example:
Solve $(d^2 +2d+1)y=e^{3x}+e^{-x}$ 
$y=CF+PI$

CF:
$m^2+2m+1=0$

$\text{C.F}:C_1e^{-x}+C_2xe^{-x}\dots$ 
PI:
$\frac{1}{d^2+2d+1}\times(e^{3x}+\frac{1}{d^2+2d+1}\times e^{-x})$
$\frac{1}{16}e^{3x}+x^2 \times \frac{e^{-x}}{2}$

Final Solution:
$c_1e^{-x}+c_2xe^{-x}+\frac{e^{3x}}{16}+\frac{x^2\times e^{-x}}{2}$ 


## Case 2: $Q(X)=\sin(ax+b)\text{ or }\cos(ax+b)$ :
$D^2=-a^2$

## Case 3:$Q(X)=x^n$:

$y_p=\frac{1}{f(D)}[x^n]$ 
Convert $f(D) = 1\pm \phi(D)$ 

### Worked Example:

Find the particular integral of the d.e of $(D^4+4d^2)y=x^2+1$ 

PI:
$\frac{1}{d^4+4d^2}[x^2+x^0]$

$4d^2[1+\frac{d^2}{4}]^{-1}[x^2+1]$

$P.I=\frac{1}{4d^2}[1-\frac{d^2}{4}+(\frac{d^2}{4})^2-(\frac{d^2}{4})^3+\dots$ 
$\frac{1}{4d^2}[1-\frac{d^2}{4}]\times[x^2+1]$ 
$\frac{1}{4}[\frac{x^3}{6}-\frac{x^2}{4}]$

## Case 4:$Q(X)=e^{ax}V$:

Take $e^{ax}$ common and make $d \text{<---}d+a$ 


### Worked example:
$[D^2+3d+2]y=e^{3x}sin(x)$



## Case 5: $Q(X)=\text{any function}$:

Substitute into $\frac{1}{d+a}Q(X)=e^{-ax}\int(e^{ax}Q(x))dx$ 