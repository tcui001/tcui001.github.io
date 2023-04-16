---
layout: page
title: research
permalink: /projects/
nav: true
description: 
---

My research interests are broadly in computational mathematics for scientific machine learning and data science. I develop mathematically rigorous computational methods for statistical inverse problems, data assimilation and uncertainty quantification. These methods aim to optimally learn hidden structures and driven factors of complex mathematical models from data for issuing certified model predictions and making risk-averse decisions.
 
> ###### Selected research topics: [likelihood-informed space](#lis), [transport maps](#transport), [model reduction](#mor), ...

##### **Likelihood-informed subspace** {#lis}

<img src="/assets/img/changeFromThePrior_x.png"  width="600" height="auto">

As a combined result of the smoothness of forward models, the regularity imposed by prior assumptions and the noise in incomplete data, the information update from the prior distribution (left figure) to the posterior distribution (right figure) may be confined to a relatively low-dimensional parameter subspace (indicated by red arrows).

We work on *likelihood-informed subspace* (LIS) to identify this subspace for breaking the curse of dimensionality. See [my recent presentation](/assets/pdf/lis-dtu.pdf) for details. For more information, see the work on building dimension-robust MCMC samplers using LIS [1,2], its optimality in linear problems [3,4], and error analysis for general problems [5-8].


<sub>[1] {% reference cui2014likelihood %}</sub>

<sub>[2] {% reference cui2016dimension %}</sub>

<sub>[3] {% reference spantini2015optimal %}</sub>

<sub>[4] {% reference spantini2017goal %}</sub>

<sub>[5] {% reference cui2021data %}</sub>

<sub>[6] {% reference cui2022unified %}</sub>

<sub>[7] {% reference zahm2022certified %}</sub>

<sub>[8] {% reference cui2022prior %}</sub>

---

##### **Transport maps** {#transport}

<img src="/assets/img/transport-2d.png"  width="600" height="auto">

Characterising intractable high-dimensional probability distributions is one of the central tasks in data-science, computational physics, machine learning, and many other disciplines. The start of this dates back to the first general-purpose digital computer ENIAC, on which Metropolis, von Neumann, Ulam and other pioneers invented MCMC to simulate neutron diffusion. MCMC and its variants have become the workhorse for this task since then. The Markov construction makes MCMC methods challenging to parallelise and optimise. Transport maps offer a promising way to overcome MCMC’s limitations using order-preserving transforms that couple complicated target variables with analytically tractable reference variables.

We work on deep tensor-train and polynomial methods for building Knothe-Rosenblatt (KR) rearrangement [1,2]. This has been applied to build generative models with high-dimensional parameters and data [3], importance sampling for simulation data-driven rare events [4], and sequential learning in state-space models [5]. See [my presentation at the HDA workshop](/assets/pdf/dirt-hda.pdf) for some of these works. 

We also extended the [Stein variational transport maps](https://proceedings.neurips.cc/paper/2016/hash/b3ba8f1bee1238a2f37603d90b58898d-Abstract.html) of Liu and Wang by introducing [Newton-type training algorithms](https://arxiv.org/abs/1806.03085) and using LIS methods to design the reproducing kernels [6]. We developed optimisation-based transport maps for infinite-dimensional hierarchical inverse problems [7,8].

[slides](/assets/pdf/dirt-hda.pdf)


<sub>[1] {% reference cui2022deep %}</sub>

<sub>[2] {% reference cui2023self %}</sub>

<sub>[3] {% reference cui2023deep %}</sub>

<sub>[4] {% reference cui2023scalable %}</sub>

<sub>[5] {% reference zhao2023tensor %}</sub>

<sub>[6] {% reference detommaso2018stein %}</sub>

<sub>[7] {% reference bardsley2020scalable %}</sub>

<sub>[8] {% reference bardsley2021optimization %}</sub>

---

##### **Model reduction and multilevel methods** {#mor}

[slides](/assets/pdf/adaptive_rom.pdf)

<sub>[1] {% reference cui2015data %}</sub>

<sub>[2] {% reference cui2016scalable %}</sub>

<sub>[3] {% reference peherstorfer2016multifidelity %}</sub>

<sub>[4] {% reference cui2011bayesian %}</sub>

<sub>[5] {% reference cui2019posteriori %}</sub>

<sub>[6] {% reference cui2019multilevel %}</sub>

<sub>[7] {% reference cui2023multilevel %}</sub>