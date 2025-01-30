---
created: '2025-01-31T02:56:50.806706'
modified: '2025-01-31T02:56:50.806708'
source: '[[Energy Gap of a semi conductor]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Energy Gap of a semi conductor

___
## Aim
To determine the energy band gap ($E_g$) of a given semiconductor.

## Apparatus
- D.C Power Supply  
- Semiconductor diode (Germanium or Silicon)  
- Thermometer  
- Heating arrangement to heat the diode  
- Voltmeter  
- Micro ammeter  
- Connecting wires  

## Theory & Formula
The **Energy Gap ($E_g$)** of a material is the minimum energy required for an electron to move from the valence band to the conduction band.  

- For **metals**, $E_g = 0$ as the valence and conduction bands overlap.  
- For **insulators**, $E_g$ is very high.  
- For **semiconductors**, $E_g$ lies between metals and insulators.

The resistance of a semiconductor varies with temperature as:

$$
R = R_0 e^{\frac{E_g}{2kT}}
$$

Taking the natural logarithm:

$$
\ln R = \ln R_0 + \frac{E_g}{2kT} \tag{1}
$$

Where:  
- $R_0$: Resistance of the semiconductor at absolute zero  
- $k = 1.381 \times 10^{-23} \, \text{J/K}$: Boltzmann constant  
- $T$: Temperature in kelvins  

From Equation (1), a graph of $\ln R$ versus $1/T$ gives a straight line. The slope of this line is:

$$
\text{Slope} = \frac{E_g}{2k}
$$

Thus, the energy band gap can be calculated as:

$$
E_g = 2k \times \text{Slope} = 2 \times 1.381 \times 10^{-23} \times \text{Slope} \, \text{J} = \text{Slope} \, \times 5.785 \times 10^{-5} \, \text{eV}
$$

## Procedure
1. Connect the given semiconductor diode (Germanium or Silicon) in reverse bias to the D.C Power supply and microammeter.
2. Immerse the diode in the oil bath and insert the thermometer alongside.
3. Set the reverse bias voltage to 5V using the D.C Power supply.
4. Heat the oil bath gradually using the heating coil. Record the current ($I$) for every $5^\circ$C increase in temperature.
5. Stop heating once the temperature stabilizes around $70^\circ$C.
6. Record the current as the temperature decreases, again at $5^\circ$C intervals, until room temperature is reached.
7. Repeat the experiment for 2–3 different bias voltages.
8. Tabulate the temperature, current, resistance ($R = \frac{V}{I}$), $\ln R$, and $1/T$ values.
9. Plot a graph of $\ln R$ versus $1/T$ (in $\text{K}^{-1}$). The slope of the line will help calculate $E_g$.
## Data table:

| Temperature ($^\circ$C) | Increasing Current (μA) | Decreasing Current (μA) | Mean Current (μA) | Temperature (K) |
| ----------------------- | ----------------------- | ----------------------- | ----------------- | --------------- |
| 70                      | 343.15                  | 134                     | 238.575           | 343.15          |
| 65                      | 338.15                  | 125                     | 231.575           | 338.15          |
| 60                      | 333.15                  | 174                     | 253.575           | 333.15          |
| 55                      | 328.15                  | 132                     | 230.075           | 328.15          |
| 50                      | 323.15                  | 100                     | 211.575           | 323.15          |
| 45                      | 318.15                  | 73                      | 195.575           | 318.15          |
| 40                      | 313.15                  | 51                      | 182.075           | 313.15          |
| 35                      | 308.15                  | 53                      | 180.575           | 308.15          |

| Resistance ($\Omega$) | $\ln R$ | $1/T \, (\text{K}^{-1})$ |
| --------------------- | ------- | ------------------------ |
| 4191.55               | 8.3408  | 0.002914                 |
| 4318.26               | 8.3706  | 0.002957                 |
| 3943.61               | 8.2799  | 0.003002                 |
| 4346.41               | 8.3771  | 0.003047                 |
| 4726.46               | 8.4609  | 0.003095                 |
| 5113.13               | 8.5396  | 0.003143                 |
| 5492.24               | 8.6111  | 0.003193                 |
| 5537.87               | 8.6194  | 0.003245                 |

## Graph:
![[output.png]]

## Result
The energy band gap of the given semiconductor: **$E_g = 0.30745$ eV**

## Circuit Diagram
- Connect the diode in reverse bias with terminals:
  - A (Anode)
  - K (Cathode)
- Use:
  - Microammeter to measure current
  - Voltmeter to adjust reverse bias voltage  

## Error Estimation
The actual value of the energy band gap for Germanium ($E_g$) = $0.7 \, \text{eV}$  

Percentage Error:

$$
\text{Error (\%)} = \left| \frac{\text{Observed Value} - \text{Actual Value}}{\text{Actual Value}} \right| \times 100
$$
Error %=56.08%


