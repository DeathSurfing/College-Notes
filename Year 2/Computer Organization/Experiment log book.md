___
# Experiment 1 :Logisim-evolution tool
## Aim:
To study and understand the working of the **Logisim-evolution** tool for designing and simulating digital logic circuits.
### For Windows:
### Step 1:
Open Powershell in administrator mode
Run:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```


Restart powershell in administrator
run

```
choco install logisim-evolution
```

## For MacOS:

### Step 1:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Follow all the password entries required


### Step 2:
after home brew installs,
install logisim-evolution

```
brew install --cask logisim-evolution
```
### Step 3:
Open the app from the launcher
### Step 4:
After the prompt shows,
Go into setting 
![[Screenshot 2025-07-16 at 2.41.47 PM.png]]
Go to privacy and security and allow 

## For Linux:

Use Snap to install logisim-evolution
```
sudo snap install logisim-evolution
```



___


# Experiment 2: Exploring Logic gates
## Aim:
To study and understand the working of basic logic gates (AND, OR, NOT, NAND, NOR, XOR, XNOR) and verify their truth tables.

## And Gate
![[Screenshot 2025-07-16 at 3.04.33 PM.png]]
![[Screenshot 2025-07-16 at 2.53.03 PM.png]]
$a\cdot b=x$
## Or gate
![[Screenshot 2025-07-16 at 3.04.54 PM.png]]
![[Screenshot 2025-07-16 at 2.49.46 PM.png]]
$a+b=x$
## Not Gate
![[Screenshot 2025-07-16 at 3.05.40 PM.png]]
![[Screenshot 2025-07-16 at 3.06.04 PM.png]]
$a'=x$
![[Screenshot 2025-07-16 at 2.56.32 PM.png]]

# 2.1: Realisation of logic gates
## Aim:
To realize and implement basic logic gates (AND, OR, NOT, NAND, NOR, XOR, XNOR) using electronic components and verify their truth tables.

## Design and implement OR gate from NAND gate:
![[Screenshot 2025-07-16 at 3.41.29 PM.png]]
## Design and implement AND gate from NOR Gate:
![[Screenshot 2025-07-16 at 3.42.41 PM.png]]
## Design and implement Not gate from NOR Gate:
![[Screenshot 2025-07-16 at 3.46.41 PM.png]]
## Design and implement XOR gate from NAND gate:
![[Screenshot 2025-07-16 at 3.45.48 PM.png]]
___

# 3: Construction of Half adder and full adder
## Aim:
To design and implement **Half Adder** and **Full Adder** circuits using basic logic gates and verify their truth tables.
![[Screenshot 2025-07-23 at 11.17.21 AM.png]]

## Construction of half adder using NAND
![[Screenshot 2025-07-29 at 4.04.39 PM.png]]
## Construction of half adder using NOR
___
![[Screenshot 2025-07-29 at 4.05.32 PM.png]]


# Experiment 4 : Study and Verify Half And Full Subtractor

## Aim:
To design and implement **Half Subtractor** and **Full Subtractor** circuits using basic logic gates and verify their truth tables.
### Half Subtractor:
![[Screenshot 2025-08-25 at 11.26.39 AM.png]]
Difference = a⊕b
Borrow = ~a⋅b
![[Screenshot 2025-08-25 at 11.27.41 AM.png]]

## Full Subtractor:
![[Screenshot 2025-08-25 at 11.30.51 AM.png]]
D = A⊕B⊕Bin⊕Bin
BOut = ~(A⊕B⊕Bin)⋅Bin+~A⋅B
![[Screenshot 2025-08-25 at 11.31.16 AM.png]]

# Experiment 5 : Implementation and verification of decoder and de-multiplexer and encoder using logic gates

## Aim:
To analyse the truth table of $4 \times 2$ decoder/demultiplexer using NOT (7404) and AND (7408) logic gate IC' and $2 \times 4$ encoder using OR (7432) Logic gate IC and to understand the working of $4 \times 2$ Decoder and $2 \times 4$ encoder circuit with the help of LED's display


## $2\times 4$ Decoder
![[Screenshot 2025-08-25 at 11.58.26 AM.png]]
Q0 = ~A⋅~B
Q1 = ~A⋅B
Q2 = A⋅~B
Q3 = A⋅B
![[Screenshot 2025-08-25 at 11.55.23 AM.png]]

## $4\times2$ Encoder
![[Screenshot 2025-08-25 at 12.30.42 PM.png]]![[Screenshot 2025-08-25 at 12.31.00 PM.png]]
A = D3
B = ~D2⋅D1+D3
