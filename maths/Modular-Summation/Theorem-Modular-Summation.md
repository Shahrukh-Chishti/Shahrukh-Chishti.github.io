---
layout: page
title: Modular Sum Invariance - Theorem 
description: modular summation theorem & extension to multiple participant sets 
permalink: "/maths/theorem-mod-summa/"
---
$$
\newcommand\Perm[2][n]{\prescript{#1\mkern-2.5mu}{}P_{#2}}
\newcommand\Comb[2][n]{\prescript{#1\mkern-0.5mu}{}C_{#2}}
\newcommand{\reg}[4]{\{ #1|0\rangle #2|1\rangle #3|2\rangle #4|3\rangle \}}
\newcommand{\wave}[4]{\begin{bmatrix}#1\\#2\\#3\\#4 \end{bmatrix}}
\newcommand{\diag}[4]{\begin{bmatrix}#1&0&0&0\\0&#2&0&0\\0&0&#3&0\\0&0&0&#4 \end{bmatrix}}
\newcommand{\U}{\Omega}
\newcommand{\Z}{\mathbb{Z}}
$$

## Abstract
Action of modulo sum operator on cyclic groups is expressed with set operations. 
Invariant properties of the distribution of modular integers is illustrated with basic examples.
A further discussion is expressed for scope of fundamental set operations for more general class of groups.

It is further related to classification problem, as in hidden subgroup problem

## Cyclic groups
Consider group of positive integers $$\U = \{ 0,1 \cdots (N-1) \} $$ upto $N$, under modulo sum operation $\oplus$ . Further consider subgroups $A,B \leq \U $ , with their group structure $\Z_a,\Z_b$ respectively.

The cartesian product, 
$$
\begin{gather}
 A \times B \rightarrow \{ (a,b) \ | \ a \in A , b \in B\ \} 
 \end{gather}$$ is group under direct sum of modular addition $$\begin{gather}
 (a,b) \bullet (x,y) = (a \oplus x , b \oplus y ) \in A \times B \\
 A \times B \sim \Z_a \times \Z_b
 \end{gather}
$$

## Modular Invariance
 Define invariant function acting on $A \times B$ 
$$
\begin{gather}
I(a,b) = a + b \ mod \ N  \\
S \subset A \times B \ | \ I:S \rightarrow 0
\end{gather}$$
 as its normal subgroup $S$ (kernel of the isomorphism) and corresponding coset $C$.

<figure align="center"> 
<img src="/maths/Modular-Summation/invariant-homomorphism.png" > 
<figcaption>Invariant Homomorphism. Invariance over coset.</figcaption>
</figure>

## Binary summation
_<center> The subgroup and coset-group of $A \times B$, defined by $I$ are isomorphic to - $S \sim A \cap B$ and $C \sim A \times ( B \setminus A ) $.
The modularity of $I$ is defined as $ |I| = LCM(|A|,|B|)$
</center>_


## Extension
This theorem has extension on multiple subgroups $A,B,C \cdots $ defined on $\U$, with appropriate invariant operation, $I = a + b + c  \cdots \ mod \ N$ 

_<center>
Kernel of the isomorphism $I$ on $A \times B \times C \cdots $ is isomorphic to $A \cap B \cap C \cap \cdots $
</center>_

It applies to all cyclic groups with equivalent modular summation $I$ function.
Definition of invariant is evident from its utility to classify cosets based on the value of function $I$. 

## Examples
In following examples, $A \rightarrow I_0$ and $B \rightarrow I_1$

### $I_0 = \Z_4$ and $I_1 = \Z_6$
$$
S \sim (6,6)^{\Z_2}
$$
<figure align="center"> 
<img src="/maths/Modular-Summation/3,2.png" width="1000"> 
<figcaption>Modular Summation table. Invariant set overlap</figcaption>
</figure>
<figure align="center"> 
<img src="/maths/Modular-Summation/3,2-overlap.png" width="600"> 
<figcaption>Overlapping Rings</figcaption>
</figure>
### $I_0 = \Z_2$ and $I_1 = \Z_3$
$$
S \sim (0,0)
$$
<figure align="center"> 
<img src="/maths/Modular-Summation/4,6.png" width="1000"> 
<figcaption>Modular Summation table. Invariant set overlap</figcaption>
</figure>
### $I_0 = \Z_4$ and $I_1 = \Z_8$
$$
S \sim (6,2)^{\Z_4}
$$
<figure align="center"> 
<img src="/maths/Modular-Summation/6,7.png" width="1000"> 
<figcaption>Modular Summation table. Invariant set overlap</figcaption>
</figure>
