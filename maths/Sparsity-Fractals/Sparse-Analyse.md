---
layout: page
title: Sparsity Fractals
description: mathematical description of sparsity function responsible for emergence fractal structure
permalink: "/maths/sparse-analyse/"
---
$$

\newcommand{\Enc}{\mathcal{E}}
\newcommand{\R}{R_r}
\newcommand{\Dec}{\mathcal{D}}
\newcommand{\s}{\mathbb{s}}
\newcommand{\Operator}{\mathcal{O}}
\newcommand{\x}[1]{x^{[#1]}}
\newcommand{\seed}{ \theta }
\newcommand{\Invariance}{ \mathcal{I} }
\newcommand{\whole}{\mathbb{W}}
$$


# Abstract
In the previous article, we have observed fractal symmetries in place-value encoding of various integer series.
In this section, mathematical statements are presented to describe the behaviour algebraically. The nature of recursion is probed through fractal patterns appearing in the sparsity of fundamental representation of number systems.

Here, we try to characterise the observations, and answer three questions:
* why we get fractal patterns ?
* how is this changing ?
* what is it suggesting ?

# Numeral Systems
Numbers are mathematical object that are used for counting, measuring and representation. In writing a number under a script requires rules of representation, known as numeral system.
Representing a numerical value in symbolic notation is next only to counting in the development of mathematics. And it is necessary for communication to assign language & script to a value.

<figure align="center"> 
<img src="/maths/Sparsity-Fractals/ChineseNumeral.jpg" width="800" > 
<figcaption>Chinese numeral system in Abacus</figcaption>
</figure>

Physical representation of number directly affects computation & calculations and simulations and so on. Based on diverse cultural expression and computational utility many number systems have evolved:
* [Positional Number system](https://en.wikipedia.org/wiki/Positional_notation)
	* Fixed radix, [Mixed radix](https://en.wikipedia.org/wiki/Mixed_radix), [Factorial radix](https://en.wikipedia.org/wiki/Factorial_number_system)
	* [Babylonian](https://en.wikipedia.org/wiki/Babylonian_cuneiform_numerals)
* [Roman numerals](https://en.wikipedia.org/wiki/Roman_numerals)
* [Asymmetric number system](https://en.wikipedia.org/wiki/Asymmetric_numeral_systems)

# Recursion
A rule that repeats is recursion, not the rule, but the repitition.
It build fractals are also related to evolution of dynamical systems.
Number series generation and place-value encoding could also be represented as repeated progression. 
_<center>Through many examples we find, recursion is necessary extension to reach infinity</center>_
## Fractals
Fractals are self-similar structures that appear in diverse natural contexts. From biology to ion-propulsion technology to non-linear dynamics they have been diversely used to represent, explain & optimise various phenomenons.

Generally(_disputed definition_), fractals consist of a intial starting structure and a recursive rule that grows a fractal structure out of seed pattern. 
Recursive growth keep their algorithmic complexity ridiculously low.
And also, make them scale invariant.
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Irrawaddy-River-Myanmar-Burma-2005.jpg" width="800" > 
<figcaption>Fractal river basin of Irrawaddy</figcaption>
</figure>

## Dynamical Systems
Dynamical system $f$ demonstrate recursive evolution of state $x_n$ given a starting point $x_0$ and parameters of evolution $\theta$.

$$x_{n+1} = f_{\theta}(x_n \cdots)$$

### Series Generation
Generation of number series can be represented as recursive process with seed parameters $\theta$, that defines initial position and parameters of the recursive rule $G$.
Algorithm generates $L$ number in the series: 

$$
    \Rightarrow x_0 \cdots x_n \cdots x_{L-1} 
$$

Three fundamental series are considered :
* Arithmetic Progression : $ A := G ( x_n ) \rightarrow x_n + a$. $x_{n+1} = x_0 + na \ \Rightarrow A^n(x_0)$ 
    
    $0,1,2,3,4 \cdots $. $x_0=0,a=1$ .
* Geometric Progression : $ B := G ( x_n ) \rightarrow x_n * g$. $x_{n+1} = x_0 g^n \ \Rightarrow B^n(x_0)$
    
    $1,2,4,8 \cdots $. $x_0=1,g=2$ .
* Fibonacci progression : $ F:= G ( x_n , x_{n-1} ) \rightarrow x_n + x_{n-1} $. $ ?? $ nothing here, doesnt belong to the class of $F^n(x_0)$
    
    $1,1,2,3,5 \cdots $ . $x_0=1,x_1=1$ . 

_Fibonacci series cannot be analytically represented because of its non-linear progression rule.  It should be noted that geometric is multiplicative in progression, but under logarithm transform it is equivalent to linear series._

### Place Value Notation
Almost all of modern world uses place-value notation to write down numbers $x$, which is composed of symbols $S$, called digits $d$.
The cardinality of symbol set $S$ is called radix or base $r$.

A good way to express this encoding $\Enc$ is through set of digits $S^{N}$, where $N$ is the representation capacity.
Many physical manifestation of these numbers require closure of space. It is a bound because of physical limits of computation that is needed to represent the complete space, irrespective of what the real value is. 

$$ x \in \whole \qquad \Enc(x) \rightarrow S^{N} \qquad \Rightarrow d_{N-1} \cdots d_0 \qquad d_i \in S $$

An insignificant symbol which is usually zero $0$, that doesn't hold any value, is appended to the remaining left.

<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Positional.svg" width="800" > 
<figcaption>Place value system</figcaption>
</figure>

### Recursive Encoding
Beginning with $\x{0}=x$ and radix $r$ and capacity $N$ positional-notation encoding can be carried as follows:

$$
    d_i = \x{i} \mod{r} \qquad \x{i} = \lfloor{\frac{\x{i-1}}{r}}\rfloor = \R(\x{i-1}) = \R^{i}(x) 
$$

<figure align="center"> 
<img src="/maths/Sparsity-Fractals/FloorFunction.svg" width="400" > 
<figcaption> Floor function $y=R(x)$ . Attractor at origin </figcaption>
</figure>

while computationally equivalent decoding process $\Dec$ is better understood and expressed as iterative sum

$$
    \Dec : S^N \rightarrow \whole \qquad x = \sum_{i}^{N} r^i d_i
$$

, given $N$ is sufficient capacity $N \geq \log_r x_{L-1}$.


<figure align="center"> 
<img src="/maths/Sparsity-Fractals/DynamicalMap.svg" width="600" > 
<figcaption> Dynamical System of $\R^i(x) \mod{r}$, is roughly shown by linear maps, ignoring the non-linear flooring.
 The uncertainty in $\frac{x_0}{r^{n}} \sim  R^n(x_0)$ and inaccuracy in the diagram increases with every step $i$.</figcaption>
</figure>

# Sparsity Function

Sparsity is the count of zeros in a given tuple and it can be generalised as appearance of any digit $d \in S$.
Series generation is the time evolution of $G$ indexed by $i$. 

$$
\begin{gather*}
	\s : \whole \rightarrow S^N \rightarrow \{0,1,2,..N \} \\
	\s : x \xrightarrow{encode} d_{N-1} \cdots d_0 \xrightarrow{count} \sum |\{d_i | d_i==0\}| \\
	\Rightarrow \s(x_i) = \sum_j 1(\R^{j} (x_i) \mod r == 0) \qquad x_i = G^i(x_0)
\end{gather*}
$$

This defines the sparsity function $\s$, that describe all mathematical properties of the emergent fractals.
For $N \geq \lfloor{\log_r l}\rfloor $, the place-value notation just sufficiently represents all the numbers from $0$ to $l-1$.

Appearance of $d_{i+1}=0$ in this representation is attributed to following condition

$$
\begin{gather*}
    \lfloor{\frac{R^i(x)}{r}}\rfloor \mod{r} = 0 \ \Rightarrow \ \text{if} \lfloor{\frac{R^i(x)}{r}}\rfloor = zr \ \text{, for some integer }z \\
    \Rightarrow R^i(x) \in \left[ zr^2, (zr+1)r \right)
\end{gather*}
$$

<figure align="center"> 
<img src="/maths/Sparsity-Fractals/NumberLine.png" width="600" > 
<figcaption>Regions on $x$ number line leading to $0$ in representation, as dynamical encoding gets attracted towards $0$ origin </figcaption>
</figure>

## Two-way recursion

<figure align="center"> 
<img src="/maths/Sparsity-Fractals/BiRecursive.svg" width="600" > 
<figcaption>Two-way recursion is enabling fractal emergence</figcaption>
</figure>

### Annihilation
For the case of geometric progression $2,4,8...$ that fractal patterns disappear for binary, octal & hexadecimal bases. Instead, linear & stepped structures appear.
This behaviour is demonstrate annihilation of generation process & encoding process, when both match each other at certain parameters.

# Seed structure
If we just consider fractals of arithmetic progression, across various bases, a characteristic seed structure is notable.
By changing basis, it could be modified. But the recursion pattern is unchanging.
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/SparsityFractal.svg" width="1000" > 
<figcaption>Seed structure of Arithmetic fractals. Parameterized by basis $r$</figcaption>
</figure>

## Appearance of other digits
<iframe align="center" src="/maths/Sparsity-Fractals/oct.4.10000.html" width="800" height="600" frameBorder="0"></iframe>
In this plot, arithmetic series is encoded with octal radix. And instead of observing $0$, we have plotted count of $4$.
The seed structure slightly different to _sparsity fractals_ of $0$, suggesting higher generalisation in parametric seed structure. 

## Sampling Fibonacci from Arithmetic
Fractal patterns show that fibonacci sequence has virtually no patterns; while, arithmetic fractals are most ordered.
However, fibonacci sequence, or any other, could be sampled from arithmetic progression.
It could be suggesting that all other integer series might have complex multi-fractal nature.
And the arithmetic fractal seed could serve as basis to them.

## Invariance
The algebraic equation for auto-encoding,
$$ 
    \sum_i^N \big( \R^i (x) \mod{r} \big) r^i = x
$$ is invariant over radix $r$, 

In this way, the summation aggregation $\sum$ is counter-acting recursive flooring $\R$.
