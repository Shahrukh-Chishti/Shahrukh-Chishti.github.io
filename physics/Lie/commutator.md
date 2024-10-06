---
layout: page
title: Lie Bracket == Commutator
description: ubiquity of commutators
permalink: "/physics/Lie-commutator/"
---

<script src="mathjax-config.js"></script>

<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/KaTeX/0.11.1/katex.min.css">
<script src="//cdnjs.cloudflare.com/ajax/libs/KaTeX/0.11.1/katex.min.js"></script>


$$
\renewcommand{\so}{\Rightarrow}
\newcommand{\im}{\iota}
\newcommand{\g}{\mathfrak{g}}
$$

# Commutators $$[A,B]$$
Commutator appears universally in physical description of dyanmics 
The commutator carries information of the underlying manifold geometry.

## First Encounter
<figure align="center"> 
<img src="/physics/Lie/parallelogram.png" width="500"> 
<figcaption>Closing of parallelogram on Euclidean geometry</figcaption>
</figure>
the nature is smooth and phenomenon are variations
The procedure to describe geometry of physics relies on differentials over a manifold surface.
Generally, the manifold is a non-Euclidean geometry embedded inside a higher dimensional space.


## Lie Bracket - Vector Fields
<figure align="center"> 
<img src="/physics/Lie/LieBracket.png" width="1000"> 
<figcaption>Flow fields generate the movement, $x_0 to x$ over $\epsilon$ time .$\tilde{X} \neq X(x)$</figcaption>
</figure>

$$
\mathcal{L}_Y X(x_0) = \lim_{\epsilon \to 0} \frac{\tilde{X}-X(x_0)}{\epsilon}  = [X,Y]
$$

Commutator describes the geometry of the flow, with respect to another flow.

### Pushforward


### Parallel transport
The Lie derivative builds on more information than a simple parallel transport.
While the latter requires only a path on the manifold, the former takes in the speed of moving over the path, as well.
Mathematically, $\phi_\epsilon(x_0)=x$ undergoes expansion.
$$\so X(x) \neq \tilde(X)$$

Flow vector fields $Y(x) = \dot{\phi}(x)$ guide the direction and the distance(mistakenly ignored in diagram)
Obviously, metric tensor is a prerequisite to define a path. The geometry of the manifold is manifest via parallel transport derivative, as well. 

$$
\lim_{\epsilon \to 0} \frac{X(x)-X(x_0)}{\epsilon} \qquad \lim_{epsilon \to 0} \frac{\tilde{X}-X(x_0)}{\epsilon} \ \tilde{X} = \phi_{-\epsilon}^{*} X(x)
$$

## Lie Derivative
Lie algebra builds a vector space, termed as [Fundamental vector field](https://en.wikipedia.org/wiki/Fundamental_vector_field).

<figure align="center"> 
<img src="/physics/Lie/TeM.png" width="1000"> 
<figcaption>Tangent space of a Lie group G at its identity 1</figcaption>
</figure> 

Lie derivative avoids explicit coordinate or basis marking.
In a way, its generalizing the point of view of reference.
Since, the laws of physics are indifferent to observers, the Lie derivative provide a better description of variation. Particularly, with locally & smoothly varying basis/coordinate system. 

Choosing a basis representation for an operator is a process equivalent to choosing a coordinate-system/basis-span/projectors for vector fields.
This fact is reflected in the appearance of commutators in both the scenario.

## Physics via Lie Groups
The Heisenberg picture of quantum dynamics makes usage of Lie groups clearer.
All of the dynamics is expressed as evolution of operators.
The generator of temporal evolution is the Hamiltonian operator. So in order to evolve the state of the quantum system, the 
More generally, the operators could be propagated under any other generator.
For example, under spatial translation, its generator being the momentum operator.

In this picture, temporal dynamics is an instance of a more general evolution.

To summarise, all unitary evolution is a smooth progression on a single-parameter path.
So, there is a direct mapping between parameter and the element on the Lie group.
The direction taken by the path is defined by vectors belonging to the lie algebra.
These vectors need not be column-like, and vary locally.

In the formulation of quantum mechanics, these *direction vectors* could be momentum, position, Hamiltonian etc. operators.

$$
\begin{gather}
A(s),U(t) \in G \qquad \dv{A}{s}(s=0) = a,\dv{U}{t}(t=0) = O \qquad a,O \in \g // 
\so A(s) = \exp{\im s a} \qquad U(t) = \exp{\im t O} //
\dv{\dv{A_{s=0}(t=0)}{t}}{s} = [a,O] \in \g
\end{gather}
$$

As a sidenote, the eigenspectrum of any observable is required to be a real quantity.
This axiom constraints the generators to be Hermitian.


### Family of Operators & Evolution

Does the Lie derivatve completely describe the dynamics of the operator ?
$$
A_s(t) = U_t^{-1} A(s) U_t
$$
The 2-parameter evolution describe an operator-valued map over suitable coordinates-t,s.





<figure align="center"> 
<img src="/physics/Lie/Lie-2D-Representation.png" width="1000"> 
<figcaption>Evolution of parametric family of operators $A_s$. For SU group, $U^{-1} \equiv U^{\dagger}$.</figcaption>
</figure>

Progression along parameter-t, $A \to B$, preserves the eigenspectrum. 
It is a smooth similarity transformation or coordinate transformation.

Traversing on the family of operators $A_s$, along the parameter-s, assign a phase evolution.
Consider an example of spatial translation, $A_s = \exp{\im \hat{p}s}$, s is the shift. 
Further, $s=0$ Y-axis is identity, $A_0(t) = 1$.

$$
A_s \ket{x} = \ket{x-s} \qquad A_s \ket{p} = \exp{\im ps} \ket{p} \\
\exp{\im t \hat{O}} = (\exp{\im \hat{O}})^t \\
H \ket{\psi} = \lambda \ket{\psi} \quad H^n \ket{psi} = \lambda^n \ket{\psi}
$$ 

### Continuous diagonalization
The 2-coordinate map $A_s(t)$ describe operator family $A_s$ under smooth basis transformation.
Consider, $A_s$ s-slice operator t-evolution:
* Is it possbile to find a diagonalized representation of $A_s$ for some t. What conditions are required on $U,A$ ?
* Since, the two operators are smoothly evolving, their diagonalization must be smoothly connected !
* If so, then, what are the contours of diagonalized representation ?
