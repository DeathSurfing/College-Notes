___
# Unit 1 :
## Prior knowledge:

### Set forms:
- Roster A= { 1,a,2,b,... } 
- Builder $$x/ 0\leq x\leq1,x\in\mathbb{R}$$
- Vendiagram


### Cardinality:
The cardinal number of a set is defined as the number of elements in a finite set.
#### Represented by:
$$Card(A)\ or\ n(A) \ or\ (A)$$
### Empty set:
Empty set or null set is represented by $$ \phi $$
### Property of sets:
- Repetitions are not allowed . {1,1,1,1,1} is not allowed
- In a set order doesn't matter . {1 ,2} or {2,1} are the same


### Books recommended for Discrete Math course:
- Discrete mathematics by K.H Rosen
- Schum outlines  

### Mathematical symbols:
$$\exists=There \ Exists$$
$$\in=Belongs\ to$$
$$\backepsilon=Such \ That$$
$$\forall=For\ all$$
### Mathematical representation of Subsets
When can we say $$A\subseteq B$$
When
$$\forall x\in A\implies x\in B$$
Then
$$A\subseteq B$$
### Proper Subset : 
$$A\subset B$$
When all the elements are properly contained within B


### When are two sets equal?

$$A\subset B\ and \ b\subset A$$
$$A=B$$


### Set of factors of 12 and 2
$$A=\left\{12,6,4,3,2,1\right\}$$
$$B=\left\{1,2\right\}$$
$$B\subseteq A\subseteq \phi$$
### Union
- Combining of two or more sets
$$x=A \cup B$$
$$\forall x\in A \ \vee \ x\in B$$
### Intersection
$$x=A\cap B $$
$$\forall x\in A\ \wedge \ x\in B$$

### Union and intersection repetition notation 
#### Union:
$$A_1\cup A_2...A_n=\cup^n_{i=1}A_i$$
$$\cup^n_{i=1}A_i=A_1$$
#### Intersection
$$A_1\cap A_2...A_n=\cap^n_{i=1}A_i$$
$$\cap^n_{i=1}A_i=A_n$$

### Operations on sets
$$Card(A \cup B)=Card(A)+Card(B)-Card(A\cap B) $$
$$Card(A\cup B \ \cup C)=Card(A)+Card(B)+Card(C)-Card(A\cap B)-Card(B\cap C)+Card(C\cap A)+Card(A\cap B \cap C)$$
- Difference
	- $$A \setminus B$$
	- $$\forall x\in A ,x\notin B$$
- Symmetrical difference
	- $$A\Delta B$$
	- $$(A\setminus B)\cup(B\setminus A)=(A\cap B)\setminus(A\cup B)$$
- Complement
	- $$A^C \ or\ A^{'}$$
	- $$\forall x\in A,x \notin U$$


#### Practice Problem:
100 students
M:50
P:40
C:25
$$M \cap C=10$$
$$P \cap C=10$$
$$M \cap P =10 $$
$$M \cap P \cap C=5$$



### Laws of sets:

___

### De Morgan's theorem 

$$(A \cup B)' = A'\cap B'$$
$$or$$
$$(A\cap B)'=A'\cup B'$$
![[Screenshot 2024-09-17 at 3.27.02 PM.png]]


### Home work:

### Solved Problems

#### 1.1 
Which of these sets are equal: \( \{x, y, z\}, \{z, y, x\}, \{y, z, x\}, \{z, y, z\}, \{y, z, y\} \)?

They are equal because order and repetition do not change a set.

#### 1.2 
List the elements of each set where \(N = \{1, 2, 3, \dots\}\):

(a) $$ A = \{ x \in N \mid 3 \leq x \leq 9 \}$$
(b) $$ B = \{ x \in N \mid x \text{ is even} \land x < 11 \} $$
(c) $$C = \{ x \in N \mid 4n + x = 3 \}$$

**Ans:**

(a) A consists of the positive integers between 3 and 9; hence \( A = \{ 3, 4, 5, 6, 7, 8, 9 \} \).

(b) B consists of the even positive integers less than 11; hence \( B = \{ 2, 4, 6, 8, 10 \} \).

(c) No positive integer satisfies \( 4n + x = 3 \); hence \( C = \emptyset \), the empty set.

#### 1.3 
Let $$A = \{ 2, 3, 4, 5 \} $$:

(a) Show that \( A \) is not a subset of
$$B = \{ x \in N \mid x \text{ is even} \} $$.

(b) Show that \( A \) is a proper subset of 
$$ C = \{ 1, 2, 3, 4, 5, 6, 7, 8, 9 \} $$.

**Ans:**

(a) It is necessary to show that at least one element in \( A \) does not belong to \( B \).
Now \
$$3 \in A $$
, and since \( B \) consists of even numbers,
$$ 3 \notin B $$;hence \( A \) is not a subset of \( B \).

(b) $$ A \subseteq C $$, but since \( C \) has elements not in \( A \), such as \( 1 \) and \( 9 \), \( A \) is a proper subset of \( C \).



## Cartesian Product
- Order matters
$$A \times B= \forall (x,y) / x\in A,y\in B$$
$$A\times B \times C = \forall(x,y)/x\in A, y \in B, z \in C$$

$$[0\ 1] \times [-1 \ 1]$$
![[Screenshot 2024-09-17 at 3.51.46 PM.png]]


$$|A^2|=|A| \times|A|=|A\times A|$$


## Relations
Is a subset of cartesian product 
$$R \subseteq A\times B$$


### Write 5 relations that satisfy:
$$\Bbb R\times \Bbb R$$

### Types of Relations:
 Assume true for all cases:$$A\neq \phi , \forall \Bbb R\times \Bbb R $$
- Reflexive
$$\forall a\in A  \rightarrow (a,a)\in R$$
- Symmetric
$$\forall (a,b) \in R \rightarrow(b,a) \in R$$
- Anti-Symmetric

## Functions 

# Unit 2 :
## Partial order set
## Lattice Theory

# Unit 3:
## Group theory
## Graph Theory

## Prop logic
## Counting Theory
