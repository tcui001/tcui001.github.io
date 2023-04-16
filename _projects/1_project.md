---
layout: page
title: likelihood-informed dimension reduction
description: 
img: assets/img/changeFromThePrior_x.png"
importance: 1
category: lis
---

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