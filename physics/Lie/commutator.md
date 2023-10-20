---
layout: page
title: Lie Bracket == Commutator
description: ubiquity of commutators
permalink: "/physics/Lie-commutator/"
---

$$
\renewcommand{\so}{\Rightarrow}
\newcommand{\im}{\iota}
$$

# Commutators $$[A,B]$$
Commutator appears universally in physical description of dyanmics 
The commutator carries information of the underlying manifold geometry.

## First Encounter
<figure align="center"> 
<img src="/physics/Lie/parallelogram.png" width="500"> 
<figcaption>Closing of parallelogram on Euclidean geometry</figcaption>
</figure>

## Lie Bracket - Vector Fields
<figure align="center"> 
<img src="/physics/Lie/LieBracket.png" width="1000"> 
<figcaption>Flow fields generate the movement, $x_0 to x$ over $\epsilon$ time .$\tilde{X} \neq X(x)$</figcaption>
</figure>

### Pushforward

### Parallel transport
The Lie derivative builds on more information than a simple parallel transport.
While the latter requires only a path on the manifold, the former takes in the speed of moving over the path, as well.
Mathematically, $\phi_\epsilon(x_0)=x$ undergoes expansion.
Flow vector fields $Y(x) = \dot{\phi}(x)$ guide the direction and the distance(mistakenly ignored in diagram)
Obviously, metric tensor is a prerequisite to define a path. The geometry of the manifold is manifest via parallel transport derivative, as well. 

## Lie Derivative
Lie algebra builds a vector space, termed as [Fundamental vector field](https://en.wikipedia.org/wiki/Fundamental_vector_field).

<figure align="center"> 
<img src="/physics/Lie/TeM.png" width="1000"> 
<figcaption>Tangent space of a Lie group G at its identity 1</figcaption>
</figure>

Lie derivative avoids explicit coordinate or basis marking.
In a way, its generalizing the point of view of reference.
Since, the laws of physics are indifferent to observers, the Lie derivative provide a better description. 

## Physics via Lie Groups
The Heisenberg picture of quantum dynamics makes usage of Lie groups clearer.
All of the dynamics is expressed as evolution of operators.
The generator of temporal evolution is the Hamiltonian operator. So in order to evolve the state of the quantum system, the 
More generally, the operators could be propagated under any other generator.
For example, under spatial translation, its generator being the momentum operator.


$$
A(s),U(t) \in G \qquad \dv{A}{s}(s=0) = a,\dv{U}{t}(t=0) = O \qquad a,O \in \mathfrak{g} 
\so A(s) = \exp{\im s a} \qquad U(t) = \exp{\im t O} 
$$

As a sidenote, the eigenspectrum of any observable is required to be a real quantity.
This axiom constraints the generators to be Hermitian.

### Family of Operators & Evolution

<figure align="center"> 
<img src="/physics/Lie/Lie-2D-Representation.png" width="1000"> 
<figcaption>Evolution of parametric family of operators $$A_s$$</figcaption>
</figure>
Progression along parameter-t, $A \to B$, preserves the eigenspectrum. 
It is a smooth similarity transformation or coordinate transformation.

Traversing on the family of operators $A_s$, along the parameter-s, assign a phase evolution.
Consider an example of spatial translation, $A_s = \exp{\im \hat{p}s}$, s is the shift. 
$$
A_s \ket{x} = \ket{x-s} \qquad A_s \ket{p} = \exp{\im ps} \ket{p} \\
\exp{\im t \hat{O}} = (\exp{\im \hat{O}})^t \\
H \ket{\psi} = \lambda \ket{\psi} \quad H^n \ket{psi} = \lambda^n \ket{\psi}
$$ 

