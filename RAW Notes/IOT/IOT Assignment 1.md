___
### **Q1: Electrical Hazard Conditions in the Campus**

1. **Exposed Electrical Cables**
    
    - **Risk**: Electrical shocks from exposed wires.
    - **Control**: Regular maintenance, proper insulation.
2. **Damaged Electrical Equipment**
    
    - **Risk**: Malfunction causing fire/shock.
    - **Control**: Frequent checks, repair/replace damaged equipment.
3. **Electrical Equipment near Water**
    
    - **Risk**: Electrocution risk near water.
    - **Control**: Keep away from water, use GFCIs.
4. **Overloaded Sockets**
    
    - **Risk**: Overheating leading to fire.
    - **Control**: Balance loads, use surge protectors.

**Importance**: Prevent injury, death, and property damage.

**Response to Shock**:

- Disconnect power.
- Assess the situation.
- Administer first aid if trained.
- Seek medical help.

---

### **Q2: Kirchhoff's Voltage Law (KVL)**

# Solution for Question 2

Given circuit:
- Loop 1: $R_1 = 20 \Omega$, $R_2 = 80 \Omega$, $V_1 = 400 V$
- Loop 2: $R_3 = 15 \Omega$, $R_4 = 90 \Omega$, $R_2$ (shared with Loop 1)
- Loop 3: $R_5 = 10 \Omega$, $V_2 = 200 V$, $R_4$ (shared with Loop 2)

## i. Write and solve the KVL equations for each loop

### Loop 1:
$$ V_1 - I_1R_1 - I_1R_2 + I_2R_2 = 0 $$
$$ 400 - 20I_1 - 80I_1 + 80I_2 = 0 $$
$$ 400 - 100I_1 + 80I_2 = 0 $$

### Loop 2:
$$ -I_2R_3 - I_2R_4 - I_2R_2 + I_1R_2 + I_3R_4 = 0 $$
$$ -15I_2 - 90I_2 - 80I_2 + 80I_1 + 90I_3 = 0 $$
$$ 80I_1 - 185I_2 + 90I_3 = 0  $$

### Loop 3:
$$ V_2 - I_3R_5 - I_3R_4 + I_2R_4 = 0 $$
$$ 200 - 10I_3 - 90I_3 + 90I_2 = 0 $$
$$ 200 + 90I_2 - 100I_3 = 0  $$

## Solve the system of equations:

From (1): 
$$ I_1 = 4 + 0.8I_2 $$

Substituting in (2):
$$ 80(4 + 0.8I_2) - 185I_2 + 90I_3 = 0 $$
$$ 320 + 64I_2 - 185I_2 + 90I_3 = 0 $$
$$ 320 - 121I_2 + 90I_3 = 0  $$

From (3): 
$$ I_3 = 2 + 0.9I_2 $$

Substituting in (4):
$$ 320 - 121I_2 + 90(2 + 0.9I_2) = 0 $$
$$ 320 - 121I_2 + 180 + 81I_2 = 0 $$
$$ 500 - 40I_2 = 0 $$
$$ I_2 = 12.5 A $$

Now we can find $I_1$ and $I_3$:
$$ I_1 = 4 + 0.8(12.5) = 14 A $$
$$ I_3 = 2 + 0.9(12.5) = 13.25 A $$

## ii. Calculate the current through each resistor

- Current through $R_1$: $I_1 = 14 A$
- Current through $R_2$: $I_1 - I_2 = 14 - 12.5 = 1.5 A$
- Current through $R_3$: $I_2 = 12.5 A$
- Current through $R_4$: $I_2 - I_3 = 12.5 - 13.25 = -0.75 A$ (flowing in opposite direction)
- Current through $R_5$: $I_3 = 13.25 A$


---

### **Q3: Superposition Theorem**

1. **Step 1 (V1 Active)**:  
$$I_{V1} = \frac{12V}{R_1 + R_2} = \frac{12}{5 + 2} = \frac{12}{7} = 1.71A$$

2. **Step 2 (V2 Active)**: 
    $$I_{V2} = \frac{6V}{R_2 + R_3} = \frac{6}{2 + 6+1} = \frac{6}{9} = 0.66A$$
3. $I_{1}=3A$:
4. **Step 4:Super position of currents:**
	$I_{total\ through\ 5\Omega }=1.71-3=-1.286A$
Current through $5\Omega$ resistor = 1.286A


