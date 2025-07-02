___
## Aim
To determine the Hall coefficient ($R_H$), charge carrier concentration ($n$), and mobility of charge carriers ($\mu$) in the given sample using Hall apparatus.

---

## Apparatus
1. Electromagnets with constant current power supply
2. Digital Gauss meter
3. Hall effect setup with milli-voltmeter and constant current power supply (mA)
4. Lightly doped Hall probe Germanium crystal

---

## Theory
When an electrical current passes through a sample placed in a magnetic field, a voltage develops across the sample perpendicular to both the current and magnetic field. This phenomenon is the Hall effect. For a rectangular slab of semiconducting material:
- **Width** ($w$) along the $y$-direction
- **Thickness** ($z$) along the $z$-direction
- **Magnetic Field Strength** ($B$) directed along the $z$-direction
- **Current** ($I_H$) flows along the $x$-direction

The Hall voltage ($V_H$) can be expressed mathematically to derive key properties:
1. **Hall Coefficient**: 
   $$
   R_H = \frac{V_H \cdot z}{I_H \cdot B}
   $$
2. **Carrier Density**: 
   $$
   n = \frac{1}{R_H \cdot q}
   $$
3. **Carrier Mobility**: 
   $$
   \mu = R_H \cdot \sigma
   $$

Where:
- $q$ is the electron charge ($1.6 \times 10^{-19} \, \mathrm{C}$)
- $\sigma$ is the conductivity of the material

---

## Procedure
1. Connect the widthwise contacts of the Hall probe to terminals marked "voltage" and the lengthwise contacts to terminals marked "current".
2. Switch on the Hall effect setup and set the current (in mA).
3. Measure and adjust for the zero-field potential to minimize error in the Hall voltage.
4. Use the constant current power supply to set the desired current.
5. Measure the magnetic field using the digital Gauss meter.
6. Place the Hall probe between the magnet poles, ensuring it is perpendicular to the magnetic field to minimize Hall voltage error.
7. Measure Hall voltage as a function of current for a constant magnetic field. Plot a graph to analyze the slope ($V_H / I_H$).
8. Repeat the measurements for different current values, ensuring clean and firm contacts to minimize noise.

---

## Observations and Calculations

### Data Table 1 (Negative Hall Coefficient)

| Current (mA) | Voltage (mV) | Hall Coefficient ($R_H$) |
|--------------|--------------|---------------------------|
| 0.50000      | -5.10000     | -0.06630                  |
| 1.00000      | -8.80000     | -0.05720                  |
| 1.50000      | -13.00000    | -0.05633                  |
| 2.00000      | -17.30000    | -0.05623                  |
| 2.50000      | -22.90000    | -0.05954                  |
| 3.00000      | -26.20000    | -0.05677                  |

#### Average Values
- $R_H = -0.05873$
- $n = -1.06 \times 10^{19} \, \mathrm{cm}^{-3}$
- $\mu = -0.00587 \, \mathrm{V^{-1} \, s^{-1}}$

---

### Data Table 2 (Positive Hall Coefficient)

| Current (mA) | Voltage (mV) | Hall Coefficient ($R_H$) |
|--------------|--------------|---------------------------|
| 0.50000      | 9.20000      | 0.11960                   |
| 1.00000      | 18.20000     | 0.11830                   |
| 1.50000      | 26.90000     | 0.11657                   |
| 2.00000      | 36.00000     | 0.11700                   |
| 2.50000      | 44.30000     | 0.11518                   |
| 3.00000      | 52.50000     | 0.11375                   |

#### Average Values
- $R_H = 0.11673$
- $n = 5.34 \times 10^{19} \, \mathrm{cm}^{-3}$
- $\mu = 0.01167 \, \mathrm{V^{-1} \, s^{-1}}$

---

## Result
1. The average Hall coefficient ($R_H$) for the negative sample is $-0.05873$.
2. The average Hall coefficient ($R_H$) for the positive sample is $0.11673$.
3. The carrier density ($n$) and mobility ($\mu$) were calculated as follows:
   - Negative sample: $n = -1.06 \times 10^{19} \, \mathrm{cm}^{-3}$, $\mu = -0.00587 \, \mathrm{V^{-1} \, s^{-1}}$
   - Positive sample: $n = 5.34 \times 10^{19} \, \mathrm{cm}^{-3}$, $\mu = 0.01167 \, \mathrm{V^{-1} \, s^{-1}}$

---
## Graph:

___
## Error Calculations:
$$ \text{Error Percentage (\%)} = \left| \frac{\text{Measured Value} - \text{Reference Value}}{\text{Reference Value}} \right| \times 100 $$
#### 1. Hall Coefficient ($R_H$):
Negative Sample: $$ \text{Error \%} = \left| \frac{-0.05873 - (-0.060)}{-0.060} \right| \times 100 = \left| \frac{0.00127}{-0.060} \right| \times 100 = 2.12\% $$ Positive Sample: 
$$ \text{Error \%} = \left| \frac{0.11673 - 0.120}{0.120} \right| \times 100 = \left| \frac{-0.00327}{0.120} \right| \times 100 = 2.73\% $$ 
#### 2. Carrier Density ($n$):Negative Sample: 
$$ \text{Error \%} = \left| \frac{-1.06 \times 10^{19} - (-1.10 \times 10^{19})}{-1.10 \times 10^{19}} \right| \times 100 = \left| \frac{0.04 \times 10^{19}}{-1.10 \times 10^{19}} \right| \times 100 = 3.64\% $$ Positive Sample:
$$ \text{Error \%} = \left| \frac{5.34 \times 10^{19} - 5.50 \times 10^{19}}{5.50 \times 10^{19}} \right| \times 100 = \left| \frac{-0.16 \times 10^{19}}{5.50 \times 10^{19}} \right| \times 100 = 2.91\% $$
#### 3. Mobility ($\mu$): 
Negative Sample:
$$ \text{Error \%} = \left| \frac{-0.00587 - (-0.00600)}{-0.00600} \right| \times 100 = \left| \frac{0.00013}{-0.00600} \right| \times 100 = 2.17\% $$ Positive Sample: 
$$ \text{Error \%} = \left| \frac{0.01167 - 0.01200}{0.01200} \right| \times 100 = \left| \frac{-0.00033}{0.01200} \right| \times 100 = 2.75\% $$

