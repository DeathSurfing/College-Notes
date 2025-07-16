___
# Experiment 1 :Logisim-evolution tool

## For Windows:
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
