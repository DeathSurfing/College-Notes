___

![[Screenshot 2024-10-17 at 1.44.55 PM.png]]

## Step 1:
Find out the Load resistance of the Circuit diagram
$R_L=9\Omega$ 

## Step 2:
Remove the Load resistance $R_L$ from the circuit diagram
give the terminal name as A & B
![[Screenshot 2024-10-17 at 1.48.22 PM.png]]

## Step 3:
![[Screenshot 2024-10-17 at 1.52.57 PM.png]]
Find out Thevenin Resistance ($R_{th}$) across terminal A and B; that time all sources (current and voltage) will be replaced by their internal resistance.

$R_{TH} =\frac{10\times8}{10+8}+12=16.4 \Omega$


## Step 4:
Find Thevenin Voltage($V_{th}$) across the terminal A&B
![[Screenshot 2024-10-17 at 1.54.46 PM.png]]
$I=\frac{25}{18}=1.38A$
$V_{th}=V_{AB}=V_{CD}$
$V_{CD}=8\times 1.38=11.04V$

## Step 5:
Draw the Thevenin equivalence  circuit diagram
![[Screenshot 2024-10-17 at 2.00.31 PM.png]]
$I_L= \frac{V_{TH}}{R_{TH}+R_L}$
$\frac{11.04}{16.4+9}=0.435A$


## Question 1:
![[Screenshot 2024-10-17 at 2.06.32 PM.png]]

$R_{L}=8\Omega$ 
$R_{TH}=12.5\Omega$
$I=25A$
$V_{th}=125-75=50V$
$I_L=\frac{50}{12.5+8}=2.439A$



## Question 2:
![[Screenshot 2024-10-22 at 10.15.24 AM.png]]![[Screenshot 2024-10-22 at 10.16.16 AM.png]]
![[Screenshot 2024-10-22 at 10.17.31 AM.png]]
$R_{TH}=\frac{10}{3}=3.33\Omega$ 
![[Screenshot 2024-10-22 at 10.20.13 AM.png]]
$-40+5I_1+20+10I_1=0$ 
$I=1.33A$
$R_L=2\Omega$

$-10+13.33+V_{TH}=0$
$V_{TH}=23.33V$ 

$I_L=\frac{V_{tH}}{R_{TH}+R_L}$ 
$I_L=\frac{23.33}{2+3.33}$
$I_L=\frac{23.33}{5.33}=4.38A$

## Question 3:
![[Screenshot 2024-10-22 at 10.33.23 AM.png]]
![[Screenshot 2024-10-22 at 10.34.55 AM.png]]

$R_{TH}=\frac{10}{11}\Omega$
![[Screenshot 2024-10-22 at 10.37.42 AM.png]]

$4+2I_2 + 1I_2 + I_1 + I_2=0$   
$-2+2I_1+I_1+I_2=0$

$I_1=\frac{-14}{11}$
$I_2=\frac{12}{11}$

$-V_{TH}+3I_1+4=0$ 
$-V_{TH}=-3.82-4$
$V_{TH}=-7.82V$

$I_L=\frac{-7.82}{2+\frac{10}{11}}$
$I_L=-2.69A$
