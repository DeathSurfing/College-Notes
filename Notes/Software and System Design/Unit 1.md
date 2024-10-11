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
## Types of design patterns:

### Functional design:
- A design paradigm that focuses on the functions and treats every thing as a function and focuses on the implementation
- Top down approach
- Showcased in the form of DFD's
- Data dictionary
- Flow chart
- Pseudo code

### Object Oriented Design:
- Treats every person or function as a object 
- Bottom up approach
- Consists of 6 parts:
	- Polymorphism
	- Inheritance
	- Abstraction
	- Encapsulation
	- Class
	- Object

## Software development cycle
-  A structured approach to software development
![[Pasted image 20241008141843.png]]
- Planning
- Analysis
- Design
- Implementation
- Testing and integration
- Maintenance


### Types of SLCM:
- Classical waterfall model
	- Proceed with the phases sequentially
		- Easy to manage
		- Rigid and less flexible
		- improper resource utilisation
		- no outcomes until the end
- Iterative water model
	- Allows to go back to any phase at any time to fix issues
	- Similar to water fall
		- Better handling of changes
		- More flexible compared to classical waterfall 
	- suitable for projects with changing requirements
	- Improper utilisation of resources
	- no outcomes until the end
- Prototyping Model
	- Implement a model with limited functional capabilities to represent the problem in the bigger picture
	- Has low reliability 
	- Inefficient performance
	- Provides a basic overview and showcases an early version that can be iterated over
- Evolutionary Model
	- Develop the core modules of the system
	- Provide updates and add new features to develop the software
	- The initial product skeleton is refined to add new functionalities in newer versions
		- High flexibility
		- Suitable for projects with unclear requirements
- Spiral Model
	- Divide the projects into sectors or quadrants
		- Identify resolve and risks
		- Determine Objectives
		- Customer evaluation of prototype
		- Develop next levels of products
	- Iterate over these quadrants until the loop is over
		- Highly Flexible and adaptable
		- Suitable for large and complex projects

