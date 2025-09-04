___
# Experiment 1 :Logisim-evolution tool
## Introduction
Digital logic design forms the foundation of modern computing systems, requiring specialized tools for circuit design, simulation, and verification. Logisim-evolution is an open-source educational tool that provides an intuitive graphical interface for designing and simulating digital logic circuits. This powerful simulation environment allows students and engineers to construct complex digital systems using basic logic gates, analyze their behavior through interactive simulation, and verify circuit functionality before physical implementation. The tool supports a wide range of components including basic logic gates, flip-flops, multiplexers, memory elements, and custom subcircuits, making it an essential platform for understanding digital logic principles and circuit design methodologies.
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
## Introduction:
Logic gates are the fundamental building blocks of all digital electronic systems, performing basic logical operations on binary inputs to produce binary outputs. These electronic switches implement Boolean algebra in hardware form, enabling the construction of complex digital circuits from simple logical operations. The seven basic logic gates - AND, OR, NOT, NAND, NOR, XOR, and XNOR - each perform specific logical functions that correspond to mathematical operations in Boolean algebra. Understanding the behavior and truth tables of these gates is crucial for digital system design, as they form the basis for more complex circuits including arithmetic units, memory systems, and control logic. Each gate can be characterized by its unique truth table, Boolean expression, and electrical behavior, providing the foundation for digital circuit analysis and synthesis.
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
## Introduction
Universal logic gates, specifically NAND and NOR gates, possess the remarkable property of functional completeness, meaning any Boolean function can be implemented using only these gates. This universality makes them particularly valuable in digital integrated circuit design, as manufacturing processes can be optimized for a single gate type while maintaining full logical capability. The realization of basic logic gates using universal gates demonstrates important principles of digital design including gate minimization, circuit equivalence, and the mathematical relationships between different Boolean operations. This approach also reflects practical considerations in VLSI design, where NAND and NOR gates are often the primitive elements available in standard cell libraries, requiring designers to synthesize other logical functions from these fundamental building blocks.
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
## Introduction:
Binary arithmetic forms the core of all digital computation, with addition being the most fundamental arithmetic operation in digital systems. Half adders and full adders are specialized combinational logic circuits designed to perform binary addition, serving as the basic building blocks for more complex arithmetic units in processors and digital signal processors. A half adder performs addition of two single-bit binary numbers, generating a sum and carry output, while a full adder extends this capability to include a carry input from previous stages, enabling the construction of multi-bit adders through cascading. These circuits demonstrate the practical application of Boolean algebra in implementing mathematical operations using logic gates, and their design principles extend to other arithmetic operations including subtraction, multiplication, and division in digital systems.
## Aim:
To design and implement **Half Adder** and **Full Adder** circuits using basic logic gates and verify their truth tables.
![[Screenshot 2025-07-23 at 11.17.21 AM.png]]

## Construction of half adder using NAND
![[Screenshot 2025-07-29 at 4.04.39 PM.png]]
## Construction of half adder using NOR
___
![[Screenshot 2025-07-29 at 4.05.32 PM.png]]


# Experiment 4 : Study and Verify Half And Full Subtractor
## Introduction
Binary subtraction is a fundamental arithmetic operation in digital systems, requiring specialized combinational logic circuits to handle the complexities of borrowing in binary number representation. Half subtractors and full subtractors complement addition circuits by performing binary subtraction operations, generating difference and borrow outputs that correspond to the mathematical process of binary subtraction. The half subtractor handles subtraction of two single-bit numbers, while the full subtractor includes borrow input functionality, enabling the construction of multi-bit subtraction circuits. These circuits illustrate important concepts in digital arithmetic including two's complement representation, borrow propagation, and the duality between addition and subtraction operations. Understanding subtractor design is essential for implementing complete arithmetic logic units (ALUs) that can perform both addition and subtraction operations in digital processors.
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

## Introduction
Data routing and code conversion are essential functions in digital systems, enabling efficient information processing and communication between different system components. Encoders, decoders, and multiplexers/de-multiplexers represent fundamental combinational logic circuits that perform these critical functions. Binary code systems use N digits to represent 2^N distinct elements of coded information, forming the basis for efficient data representation and transmission. Encoders convert 2^N input lines into an N-bit binary code, effectively compressing information for storage or transmission. Conversely, decoders perform the inverse operation, converting N-bit codes back into 2^N output lines, enabling selective activation of system components. De-multiplexers extend decoder functionality by routing data from a single input to one of multiple outputs based on select inputs. These circuits are fundamental to computer architecture, forming the basis for memory addressing, instruction decoding, and data routing in digital systems.
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
