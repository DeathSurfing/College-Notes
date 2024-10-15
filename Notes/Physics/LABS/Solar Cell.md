___

# Aim:
To obtain the V-I characteristics of a given solar Cell
# Apparatus:

| S.no | Name             | Quantity    | Remakrs                                                                             |
| ---- | ---------------- | ----------- | ----------------------------------------------------------------------------------- |
| 1    | Trainer board    | 1           | Consists of:<br>- Volt Meter(20V)<br>- Amp Meter(200mA)<br>- 2x Variable Resistance |
| 2    | Solar Cell       | 1           | N/A                                                                                 |
| 3    | Source of Light  | 1           | Variable resistance connected to bulb                                               |
| 4    | Connecting wires | as required | N/A                                                                                 |
# Theory:
A solar cell is a two-terminal p-n junction device that absorbs photons and converts them into electrical signals or power for external circuits.
Therefore, it is required to understand the physics of semiconductor p-n junction diodes, which convert optical radiation into electrical signals. Doped semiconductors are classified into two types: p and n, based on the charge carrier nature. In n-type semiconductors, free carriers are electrons, while p-type semiconductors have positive charge carriers, which are holes. Doped semiconductors have the same amount of free carriers as lattice ions due to their electrical neutrality.

A solar cell is illuminated by light having photon energy greater than the band gap energy
of the solar cell. Then, using a proper circuit, the open circuit voltage, short circuit
current and power drawn from the solar cell are measured.


# Procedure:
- Complete the circuit as shown in the diagram.
- Illuminate the solar cell. Adjust $R_{h}$ to zero volt reading on the voltmeter and maximum current on the ammeter. Record this short-circuit current $I_{SC}$.
- Slowly increase $R_{h}$ and note current and voltage readings until maximum voltage is reached, ensuring at least 5–10 readings.
- Disconnect **Rh** and record the open-circuit voltage $V_{OC}$.
- Repeat the experiment with a different illumination intensity.
- Tabulate all readings. Calculate power using $P=V\times I$.
- Plot **I vs. V**, marking $I_{SC}$ at zero volts and $V_{OC}$ at zero current.
- Identify the maximum power point **Pm** on the plot. Calculate series resistance $R_{s}=\frac{\Delta V}{\Delta I} \Omega$
- Calculate the fill factor (**FF**) using $F_{F}=\frac{P_{max}}{I_{SC}\times V_{OC}}$.
- Record the voltmeter, ammeter, and $R_{h}$ values for each distance. Tabulate all readings.
# Formula:

## Fill factor($F_{f}$)
$F_{F}=\frac{P_{max}}{I_{SC}\times V_{OC}}$
*Where ;*
$P_{max}: \text{is the maximum power value }$ 
$I_{SC}: \text{Current at short circuit (0 resistance)}$ 
$V_{OC} :\text{Voltage at Open circuit (infinite resistance)}$ 

## Series Resistance ($R_{s}$)

$R_{s}=\frac{\Delta V}{\Delta I} \Omega$
*Where ;*
$\Delta V:\text{Change in Voltage }$
$\Delta I:\text{Change in Current}$


# Circuit Diagram:
![[Screenshot 2024-10-15 at 11.52.36 AM.png]]

# Model Graph:
![[Screenshot 2024-10-15 at 11.57.18 AM.png]]

# Processed data:
## Table 1 (Low Intensity of light):

| S.no | Voltage(V) | Current(mA) | Power(mW) |
| ---- | ---------- | ----------- | --------- |
| 1    | 0          | 5.8         | 0         |
| 2    | 0.5        | 5.8         | 2.9       |
| 3    | 1          | 5.3         | 5.3       |
| 4    | 1.5        | 4.7         | 7.05      |
| 5    | 2          | 4.1         | 8.2       |
| 6    | 2.5        | 2.2         | 5.5       |
| 7    | 2.65       | 0.2         | 0.53      |
| 8    | 2.7        | 0           | 0         |
## Table 2 (High Intensity of light):

| S.no | Voltage(V) | Current(mA) | Power(mW) |
| ---- | ---------- | ----------- | --------- |
| 1    | 0          | 26.2        | 0         |
| 2    | 0.5        | 24.8        | 12.4      |
| 3    | 1          | 23.8        | 23.8      |
| 4    | 1.5        | 22.8        | 34.2      |
| 5    | 2          | 22.1        | 44.2      |
| 6    | 2.5        | 18.8        | 47        |
| 7    | 2.92       | 0.2         | 0.584     |
| 8    | 3          | 0           | 0         |
# Calculations:

### Fill factor for low Intensity:
$F_{f}=\frac{8.2}{5.8\times 2.7}=0.524$
### Fill factor for high Intensity:
$F_{f}=\frac{47}{26.2 \times 3}=0.6$

## Average Fill factor:
$Average \ Fill \ Factor=\frac{0.524+0.6}{2}=0.562$

$Error\%= \frac{\text{Actual Value}-\text{Experimental Value}}{\text{Actual Value}}\times 100$
$Error\%=\frac{0.70-0.562}{0.7}\times 100=19.71\%$

## Series Resistance:

$\frac{2.5-2}{18.8-4.1}=34\Omega$


![[Desmos Graph.png]]

# Results:

### Fill Factor:

$0.562$
### Series Resistance:
$34\Omega$

# Error Propagation and Calculations

## Error in Measurement Devices
- The error in both the voltmeter and ammeter was \(0.005\).

## Error Propagation for Fill Factor (\(F_F\))

The formula for \(F_F\) is:
$$
F_F = \frac{P_{max}}{I_{SC} \times V_{OC}}
$$

### Given Values
- $P_{max} = 8.2 \, \text{mW}$
- $I_{SC} = 5.8 \, \text{mA}$ 
- $V_{OC} = 2.7 \, \text{V}$ 

### Uncertainties
- $\sigma_{P_{max}} = 0.005 \, \text{mW}$
- $sigma_{I_{SC}} = 0.005 \, \text{mA}$
- $sigma_{V_{OC}} = 0.005 \, \text{V}$

### Calculating Relative Uncertainties
- $$\frac{\sigma_{P_{max}}}{P_{max}} = \frac{0.005}{8.2} \approx 0.000610$$
- $$\frac{\sigma_{I_{SC}}}{I_{SC}} = \frac{0.005}{5.8} \approx 0.000862$$
- $$\frac{\sigma_{V_{OC}}}{V_{OC}} = \frac{0.005}{2.7} \approx 0.001852$$

### Combining Relative Uncertainties
$$
\frac{\sigma_{F_F}}{F_F} = \sqrt{\left(0.000610\right)^2 + \left(0.000862\right)^2 + \left(0.001852\right)^2}
$$

### Calculation Steps
1. $$(0.000610)^2 \approx 3.721 \times 10^{-7}$$
2. $$(0.000862)^2 \approx 7.434 \times 10^{-7}$$
3. $$(0.001852)^2 \approx 3.429 \times 10^{-6}$$

Adding them up:
$$
3.721 \times 10^{-7} + 7.434 \times 10^{-7} + 3.429 \times 10^{-6} \approx 4.080 \times 10^{-6}
$$

Taking the square root:
$$
\sqrt{4.080 \times 10^{-6}} \approx 0.002020
$$

Calculating \(F_F\):
$$
F_F = 0.524 
$$

Calculating propagated error:
$$
\sigma_{F_F} = F_F \times 0.002020 \approx 0.524 \times 0.002020 \approx 0.001057
$$

## Error Propagation for Series Resistance ($R_s$)

Using the formula:
$$
R_s = \frac{\Delta V}{\Delta I}
$$

### Given Changes
- $$\Delta V = 2.5 - 2 = 0.5 \, \text{V}$$
- $$\Delta I = 18.8 - 4.1 = 14.7 \, \text{mA}$$

### Uncertainties
- $$\sigma_{\Delta V} = 0.005 \, \text{V}$$
- $$\sigma_{\Delta I} = 0.005 \, \text{mA}$$

### Calculating Relative Uncertainties
$$
\frac{\sigma_{R_s}}{R_s} = \sqrt{\left(\frac{\sigma_{\Delta V}}{\Delta V}\right)^2 + \left(\frac{\sigma_{\Delta I}}{\Delta I}\right)^2}
$$

### Calculate ($R_s$)
$$
R_s = \frac{0.5 \, \text{V}}{14.7 \, \text{mA}} = \frac{0.5}{0.0147} \approx 34.01 \, \Omega
$$

### Calculating Relative Uncertainties
- $$\frac{\sigma_{\Delta V}}{\Delta V} = \frac{0.005}{0.5} = 0.01$$
- $$\frac{\sigma_{\Delta I}}{\Delta I} = \frac{0.005}{14.7} \approx 0.00034$$

### Combining Relative Uncertainties
$$
\frac{\sigma_{R_s}}{R_s} = \sqrt{(0.01)^2 + (0.00034)^2} \approx 0.01
$$

### Final Calculation of Uncertainty in ($R_s$)
$$
\sigma_{R_s} = R_s \times 0.01 \approx 34.01 \times 0.01 \approx 0.3401 \, \Omega
$$

## Summary of Results
- **Fill Factor:** 
  - $$F_F = 0.562 \pm 0.0011$$ 
- **Series Resistance:** 
  - $$R_s = 34 \pm 0.34 \, \Omega$$
