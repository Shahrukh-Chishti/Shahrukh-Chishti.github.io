---
layout: page
title: Lie Bracket == Commutator
description: ubiquity of commutators
permalink: "/physics/Lie-commutator/"
---
window.MathJax = {
  loader: {load: ['[tex]/physics']},
  tex: {packages: {'[+]': ['physics']}}
};

$$
\renewcommand{\so}{\rightarrow}
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
<figcaption>Closing of parallelogram on Euclidean geometry</figcaption>
</figure>

### Pushforward

### Parallel transport
The Lie derivative builds on more information than a simple parallel transport.
While the latter requires only a path on the manifold, the former takes in the speed of moving over the path, as well.
Obviously, metric tensor is a prerequisite to define a path. The geometry of the manifold is manifest via parallel transport derivative, as well. 

## Lie Derivative
Lie algebra builds a vector space, termed as [Fundamental vector field](https://en.wikipedia.org/wiki/Fundamental_vector_field).

<figure align="center"> 
<img src="/physics/Lie/TeM.png" width="1000"> 
<figcaption>Tangent space of a Lie group G at its identity 1</figcaption>
</figure>

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

