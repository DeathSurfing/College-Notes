## Meta Data:
- The information about data (images, pictures and videos).


## Computational device:
- Any device that performs computation

## Programs:
- A set of instructions

## Software 
- A set of programs

## Package
- A set of softwares

## SRS Document:
Software requirement specification documents contains all the specifications required to create a software; these requirements are collected from a client via forms, interviews surveys etc...

## Types of Design

### High level design:
- External design
- Showcases the overall overview of the program structure

## Low Level design:
- Data Structures
- Types
- Algorithms
## Objectives of software design

Achieving optimal solutions for the pre-requisite requirements and achieving the following goals:
- Correctness
- Completness
- Efficiency
- Flexibility
- Consistency
- Maintainability


## Software Design Principles
- Manage complexity (reducing complexity to reduce effort and minimize errors)
- Decomposition/divide and conquer (Making problems smaller)
- Abstraction (Reducing details to allow focus on primary problem)
- Modularity (Separating software into manageable, self contained modules)


### Decomposition:
- Breaking a larger problem into logical sub units (smaller parts)
- Followed by finding solutions for those smaller parts (Divide and conqueror)
- Benifits:
	- Easier to understand
	- Testing modification is easier
	- Expansion is easier
- Cons:
	- Increases the complexity of the problem; due to the increase in sub problems cost and complexity would increase


### Abstraction:
#### Functional Abstraction
- The hiding of the internals of a function or method to preserve the core essence of the program to the user

#### Data Abstraction:
- Hiding data details such as class, types, etc...
#### Key Point:
- Higher level functions have no idea of what lower level functions do ; they follow a layered design


### Modularity:
- Dividing software into modules
- Will contain relevant data and methods/functions
- Benefit's
	- Facilitates Team collaboration
	- Facilitates Code Reuse
	- Facilitates Systematic testing
- Main Point:
	- Divide into relevant data and functions
	- Should have least possible interdependence 

### Modular design 
- The number of calls a module makes is fan out
- The number of calls into a module is fan in
- The Value of Fan in should ideally be low

### Functional Independence:

Modules should have:
- High Cohesion
- Low Coupling

#### Cohesion:
- The data and functions within a module should have high relation to each other

#### Coupling:
- The amount of dependencies a module has with another 

