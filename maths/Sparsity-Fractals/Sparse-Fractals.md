---
layout: page
title: Sparsity Fractals
description: fractal structure emerging in numeral encoding by place-value notation
permalink: "/maths/sparse-fracs/"
---
$$

\newcommand{\Enc}{\mathcal{E}}
\newcommand{\R}{R_r}
\newcommand{\Dec}{\mathcal{D}}
\newcommand{\sparsity}{\mathbb{s}}
\newcommand{\Operator}{\mathcal{O}}
\newcommand{\x}[1]{x^{[#1]}}
\newcommand{\seed}{ \theta }
\newcommand{\Invariance}{ \mathcal{I} }
\newcommand{\whole}{\mathbb{W}}
$$

## Abstract
Place-value notation used in most of modern numeral representation is a recursive method.
Representation of an integer series in a positional notation inherits this recursive nature.
This study exposes fractal patterns emerging in the sparsity of place value notation of integer series.


# Introduction
Sparsity is the count of zeros in a vector or matrix. It this study we generalise it as appearance of digit $d$ in numerical encoding.

Running multiple experiments across various encoding \& series attempts to explain variation in fractal geometry generated as a result of change in seeds \& recursive rule. For this study we restrict the scope to whole numbers $\mathbb{W}$ representation.

# Generating Fractals
The fractals generated below is straightforward derived from place-value encoding of three series:
* Arithmetic Progression : $1,2,3,4, \cdots $
* Geometric Progression : $2,4,8,16, \cdots $
* Fibonacci Series : $ 1,1,2,3,5,8, \cdots $

Place-value encoding is done on 4 radices(bases):
* Binary
* Octal
* Decimal
* Hexadecimal

As defined, Sparsity is count of zeros appearing in representation string.
So, length of representation $N$, that is number of digits allocated, is prefixed depending upon biggest number of the series.

For example, representation string $00001010$ of number $x=10, N=8$ under radix $2$ has $6$ appearance of zero. 

### Fractal & Infinity
Usually fractal is studied by zooming in a finite patch of geometry. As in [Mandelbrot fractals](https://en.wikipedia.org/wiki/Mandelbrot_set), we keep discovering structures inside.
Or we build them using recursive structure, as in [Koch curve](https://en.wikipedia.org/wiki/Koch_snowflake)

In dealing with integer series we define an upper bound on representation size $N$.
The fractal in its infinitive glory emerges when we extend this $N \rightarrow \infty$.
Formally, then sparsity would have to be defined as $count(0) / N$, where $N \rightarrow \infty$.

# Sparsity Fractals
Each of the following plots show multiple extension of representation capacity $N$.
It present reverse infinity perspective.
The abscissa (X - axis) doesn't show number encoded $x$, but index position of that number in the series. 

*dynamic plots are heavy, so for ease, we show png*
## Arithmetic progression
### Binary
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Arith-Bin.png" width="800" > 
</figure>
if you move up-down they appear moving side ways
<!-- <iframe align="left" src="/maths/Sparsity-Fractals/bin.0.500000.html" width="1000" height="600" frameBorder="0">) -->
### Octal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Arith-Oct.png" width="800" > 
</figure>
### Decimal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Arith-Dec.png" width="800" > 
</figure>

### Geometric Progression
### Binary
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Geo-Bin.png" width="800" > 
</figure>
### Octal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Geo-Oct.png" width="800" > 
</figure>
### Decimal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Geo-Dec.png" width="800" > 
</figure>
### Hexadecimal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Geo-Hex.png" width="800" > 
</figure>

### Fibonacci Series
### Binary
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Fib-Bin.png" width="800" > 
</figure>
### Octal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Fib-Oct.png" width="800" > 
</figure>
### Decimal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Fib-Dec.png" width="800" > 
</figure>
### Hexadecimal
<figure align="center"> 
<img src="/maths/Sparsity-Fractals/Fib-Hex.png" width="800" > 
</figure>
