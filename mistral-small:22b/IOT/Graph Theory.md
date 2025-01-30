---
created: '2025-01-31T02:56:50.742025'
modified: '2025-01-31T02:56:50.742028'
source: '[[Graph Theory]]'
tags: []
aliases: []
summary: ''
category: ''
links:
  outgoing: []
  backlinks: []

---

# Graph Theory

___
Is the pictorial representation of set of objects connected by the links.


1. By replacing all the independent voltage source form the short circuit.
2. All Passive element like resistance($R$),Capacitance($C$) and inductance($L$) will be replaced by short circuit
3. All the independent current source will be replaced by open circuit


## Active and Passive elements:
There are two types of elements,
### Active Element:
- Generate supply
### Passive element:
- Absorb the supply
# Directed graphs
- Have incoming and outgoing current
- Showcases the flow of current
# Non-directed graphs
- Don't have outgoing current and incoming current
- Do not showcase the flow of current
# Rank of a graph:
Let n be the number of nodes
$rank=n-1$
# Degree of node
- The number of incoming branches

# Degree of a graph:
- Number of branches in the graph
- The sum of degrees of all nodes

# Incidence matrix:

| Node/Branch | a   | b   | c   | d   | e   | f   |
| ----------- | --- | --- | --- | --- | --- | --- |
| 1           | 1   | 0   | 0   | -1  | 0   | -1  |
| 2           | 0   | 1   | 0   | 1   | -1  | 0   |
| 3           | 0   | 0   | 1   | 0   | 1   | 1   |
| 4           | -1  | -1  | -1  | 0   | 0   | 0   |

The sum of columns in any incidence matrix must be 0

# Reduced Incidence matrix:
Eliminate any one row from the incidence matrix 
