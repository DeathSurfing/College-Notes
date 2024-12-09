___
## Aim
To determine the acceleration due to gravity, $g$, using the time period of a compound pendulum.

## Apparatus
- Bar pendulum
- Stopwatch
- Meter scale
- Stand for hanging the pendulum

## Theory
The experiment aims to measure the acceleration due to gravity, $g$, by observing the motion of a compound pendulum. Unlike the simple pendulum, which is an ideal case requiring a point mass and a torsionless string, the compound pendulum is a physical pendulum. A rigid body of any shape that can oscillate without friction about a vertical axis is referred to as a compound pendulum.

When displaced from equilibrium, the pendulum oscillates due to torque. The governing equation for torque is:
$$
\tau = -m g D \sin \theta
$$
For small angular displacements, $\sin \theta \approx \theta$, and the torque becomes:
$$
\tau = -m g D \theta
$$
Using the relationship between torque and angular acceleration:
$$
\tau = I \frac{d^2\theta}{dt^2}
$$
we get:
$$
I \frac{d^2\theta}{dt^2} + m g D \theta = 0
$$
This represents a simple harmonic motion with angular frequency:
$$
\omega = \sqrt{\frac{m g D}{I}}
$$
The time period of oscillation is:
$$
T = 2\pi \sqrt{\frac{I}{m g D}}
$$
Using the parallel axis theorem:
$$
I = I_G + m D^2, \quad \text{where} \quad I_G = m k^2
$$
Substituting, the time period becomes:
$$
T = 2\pi \sqrt{\frac{k^2 + D^2}{g D}}
$$
The equivalent length of the simple pendulum is:
$$
L = D + \frac{k^2}{D}
$$
The quadratic equation for $D$ is:
$$
D^2 - L D + k^2 = 0
$$
The roots are:
$$
D_1 = \frac{L + \sqrt{L^2 - 4k^2}}{2}, \quad D_2 = \frac{L - \sqrt{L^2 - 4k^2}}{2}
$$

## Formula
The acceleration due to gravity is calculated using:
$$
g = \frac{4\pi^2 L}{T^2}
$$
where $L = D + \frac{k^2}{D}$.

## Procedure
1. Identify the center of gravity ($G$) of the bar pendulum.
2. Suspend the pendulum using a metal wedge through the first hole towards end A, ensuring it oscillates with an amplitude under $10^\circ$.
3. Record the time for 20 oscillations using a stopwatch.
4. Measure the distance from the point of suspension to the center of gravity, $G$.
5. Repeat for other holes along the pendulum, noting the time for 20 oscillations and the corresponding distances.
6. After passing the midpoint of the bar, reverse the orientation and continue measurements for the other side.
7. Calculate the time period $T$ as:
   $$
   T = \frac{\text{Time for 20 oscillations}}{20}
   $$
8. Plot a graph of $D$ (distance from $G$) on the x-axis and $T$ (time period) on the y-axis.
9. Draw a horizontal line at one specific $T$ value to determine points $A$, $B$, $C$, and $D$ on the graph.
10. Compute the equivalent length $L$ as:
    $$
    L = \frac{AC + BD}{2}
    $$
11. Use the calculated $L$ and $T$ to find $g$.

## Observations:
### Table 1: End A
| Hole No. | $D$ (cm) | Time for 20 Oscillations (s) | Mean Time ($t$) (s) | Period $T = \frac{t}{20}$ (s) |
| -------- | -------- | ---------------------------- | ------------------- | ----------------------------- |
|          |          |                              |                     |                               |
|          |          |                              |                     |                               |
|          |          |                              |                     |                               |

### Table 2: End B
| Hole No. | $D$ (cm) | Time for 20 Oscillations (s) | Mean Time ($t$) (s) | Period $T = \frac{t}{20}$ (s) |
| -------- | -------- | ---------------------------- | ------------------- | ----------------------------- |
|          |          |                              |                     |                               |
|          |          |                              |                     |                               |
|          |          |                              |                     |                               |

### Table 3: Calculations
| $T$ (s) | $T^2$ (s$^2$) | $L / T^2$ | $AC$ (cm) | $BD$ (cm) | $L = \frac{AC + BD}{2}$ (cm) |
| ------- | ------------- | --------- | --------- | --------- | ---------------------------- |
|         |               |           |           |           |                              |

# Graph:


## Error Estimation
Calculate the error percentage as:
$$
\text{Error (\%)} = \frac{|\text{Measured } g - 980|}{980} \times 100
$$
