___

# Aim
To obtain the V-I characteristics of a given solar Cell

# Apparatus

| S.no | Name             | Quantity    | Remakrs                                                                             |
| ---- | ---------------- | ----------- | ----------------------------------------------------------------------------------- |
| 1    | Trainer board    | 1           | Consists of:<br>- Volt Meter(20V)<br>- Amp Meter(200mA)<br>- 2x Variable Resistance |
| 2    | Solar Cell       | 1           | N/A                                                                                 |
| 3    | Source of Light  | 1           | Variable resistance connected to bulb                                               |
| 4    | Connecting wires | as required | N/A                                                                                 |

# Formula

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


