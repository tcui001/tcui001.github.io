---
layout: page
title: transport maps
description: 
img: assets/img/transport-2d.png
importance: 2
category: transport
---

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