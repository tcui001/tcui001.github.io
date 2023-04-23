---
layout: page
title: code
permalink: /code/
description:
nav: true
---

[DIRT](#dirt), [FastFIns](#fins), ...

---

##### **DIRT: a deep inverse Rosenblatt transport method** {#dirt}

> ###### DIRT is a MATLAB package that uses functional tensor trains and sparse polynomials to construct order-preserving, self-reinforced transport maps. The map has a composite form of $$T = T_0 \circ T_1 \circ \cdots \circ T_n$$, in which each layer is a [KR map](/projects/#transport) constructed from a function approximation. Download MATLAB code from [deep-tensor](https://github.com/DeepTransport/deep-tensor). Help files will be updated in May. Examples will be released under [deep-tensor-examples](https://github.com/DeepTransport/deep-tensor-examples) in May.

<img src="/assets/img/dirt.png"  width="600" height="auto">

Suppose the log target density is $$\phi(x) := -\log \pi(x) = - 5(\log((1-x_1^2 + 100(x_2-x_1^2)^2) - 3)^2 + \cdots$$

    >> phi= @(x) ...; % define potential function
    >> base = ApproxBases(Legendre(30), BoundedDomain([-4,4]), d); % d = 2, define approximation space
    >> kr = TTDIRT(phi,base,Tempering1()); % build DIRT using TT
    >> X = random(kr, 200); % random variable generation (left below)
    >> X = sobol(kr, 200);  % quasi Monte Carlo sample generation (right below) using Sobol sequence

<img src="/assets/img/rf1.png"  width="200" height="auto">|<img src="/assets/img/rf2.png"  width="200" height="auto">



**References:**

{% reference cui2022deep %}

{% reference cui2023scalable %}

{% reference cui2023deep %}

{% reference cui2023self %}

{% reference zhao2023tensor %}
 
---

##### **FastFIns** {#fins}

> ###### Fast Forward and Inverse problems solver (FastFIns) is a set of MATLAB code for accelerate the solution of inverse problems using likelihood-informed subspaces and data-driven model reduction. This package also contains a set of routines for defining high-order finite element discretization of PDEs.
>  
> ###### A newer version of the code using fully object-oriented programming is under development. Download MATLAB code from [fastfins.m](https://github.com/fastfins/fastfins.m).

**References:**

{% reference cui2014likelihood %}

{% reference spantini2015optimal %}

{% reference cui2015data %}

{% reference cui2016scalable %}

{% reference bardsley2020scalable %}

{% reference bardsley2021optimization %}

{% reference cui2022unified %}

{% reference zahm2022certified %}

[comment]: <> <img src="/assets/img/1.jpg"  width="400" height="auto">
[comment]: <> <img src="/assets/img/1.jpg"  width="600" height="300">