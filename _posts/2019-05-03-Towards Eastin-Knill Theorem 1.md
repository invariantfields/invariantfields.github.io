---
layout: post
mathjax: true
---
# Towards Eastin-Knill Theorem
I worked on a special case of (what it popularly is known as) Eastin-Knill theorem. And here is an attempt at summarising it in as simple and self-contained as possible. I will be trying my best to make this self-contained but in case I miss anything I would try to add a reference or two on the same. 
## Introduction
This theorem basically states that there can be no universal set transversal quantum gate. Yes, that sentence is loaded but I will introduce what each of those words mean as we roll through the prerequisites and the proof. 

## Prerequisites 1.0

### Groups
A group $\mathcal{G}(S,.)$ is a set equiped $S$ with a binary operation $.$ which satisfy the following axioms. 
1. Closure. $a.b \in S \forall a,b\in S$
2. Associativity. i.e. $(a.b).c=a.(b.c) \forall a,b,c \in S$
3. Existence of identity. i.e. $\exists e \in S$ such that $e.x=x.e, \forall x \in S$.
4. Existence of Inverse. i.e. $\forall x \in S \exists x^{-1} \in S$ such that $x.x^{-1} =e=x^{-1}.x$.

**Example**: Is integers under addition a group? $\mathcal{G}(\mathbb{Z},+)$.
1. True. Since, sum of 2 integers is always another integer.  
2. True. sum is associative. 
3. True. $e = 0$ for this group. 
4. True. $\forall x\in \mathbb{Z}$ we have $-x\in \mathbb{Z}$ such that $x+(-x)=0$.

#### Sub Group
A subgroup is a subset of $S$ with the same binary operation and follows the same axioms as the group.
 **Example**: Is integers divisible by 3 under addition a subgroup of $\mathcal{G}(\mathbb{Z},+)$?
It is obvious that $S\in \mathbb{Z}$
1. True. Sum of 2 numbers divisible by 3 is divisible by 3. 
2. True. This is directly inherited.
3. True. $0$ still stays the identity
 
#### Coset
Given a subgroup $\mathcal{C}$ and an element $g \in S$ we say 
1. $gC= \\{ gc:$ for every element $c \in C\\} $ is called the left coset.
2. $Cg= \\{ cg:$ for every element $c \in C\\} $ is called the right coset. 

**Example**: Consider the subset $C$. We have 3 unique cosets, $C,(1+C),(2+C)$.

#### Extra Notes
**Theorem**: 2 cosets  are either totally overlapping or don't have any intersection.( Disjointness of cosets) 

From the fact that all the cosets are disjoint and each of the cosets can be considered as an equivalence class.  These cosets can be considered as a division of group into equal and disjoint sets. This is equivalent to division with $\mathbb{R}$. Hence, the set in which one element (representative elements) from each of the coset is called a Quotient group(It isn't too difficult to show that, it indeed is a group.) also represented as $\mathcal{G}/C$ which in above example would be $\\{[0],[1],[2]\\}$  
   
### A brief, shabby and relevant introduction to Lie Groups. 
(Please dig in the only reference below to understand them better and deeper)

#### Lie groups
Basically a special case of a group where $S$ is a differentiable manifold. 

#### Path connected
If for 2 points $a,b \in S$ there exists a map $f:[0,1]\mapsto S$ such that $f(0)=a$ and $f(1)=b$ then $a$ and $b$ are path connected. 

#### Compact
A given Lie group is compact if it is closed and bounded. 



### References
[1] Brian C. Hall, [Elementary introduction to Lie groups and representation.](https://arxiv.org/abs/math-ph/0005032)

## Up next
### Prerequsites 2.0

#### Projectors
#### Logical operators
#### Codes


