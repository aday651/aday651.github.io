---
permalink: /research/
title: "Research"
author_profile: true
redirect_from: 
  - /research.html
---

My research interests in a very broad sense are centered around statistical and computational aspects (and the interplay of the two) of modern-day machine learning techniques, motivated through considerations of how statistical methods are implemented (usually through some type of stochastic optimization procedure). In particular, my current focus is with regards to the study of embedding methods used for the analysis of complex structured data, and the corresponding use of these embeddings for downstream tasks. 

To motivate why this is a problem of interest, note that a traditional statistical approach to the analysis of data is to begin by specifying a probabilistic model for data we observe, and then use the learned parameters of our model in order to perform a task we care about. When considering some types of complex structured data (such as network or relational data), while we can perform the first step of specifying a model (for instance we could try and fit an ERGM), it becomes more difficult to try and use this for a task of interest, for instance node classification or link prediction tasks. 

One approach which has turned out to be very successful is to learn a 'embedding' of our data into a Euclidean space which is somewhat representative of the structure we hope to uncover within it. For example, if we had a social network, we would want to assign each user a point in some (possibly high dimensional) Euclidean space, where the distances (or some other metric) between the points we assign to users are reflective of their similarity to each other in terms of interests, friendships and et cetera. If we were then interested in performing a classification task downstream, we would then use the embedding data points in a typical ML algorithm - be this a simple LDA, random forest or a neural network. 

Whether this works is contingent on whether our learned embedding carries meaningful information about the latent structure of our data, and as such natural questions arise to if and when this will be the case. One particular point of interest is that these embeddings are learned using SGD, where in the network setting there are several ways of specifying a subsampling scheme - what are the effects (if any) on the embedding vectors we learn? Can we describe the information encoded within learned embedding vectors?

Although I have a focus on mostly theoretical work, I take the stance that theoretical investigations should be driven by considerations which arise from actually attempting to analyze data in practice.

## Papers ##

* **Davison, A.** [Asymptotics of $\ell_2$ Regularized Network Embeddings](https://arxiv.org/abs/2201.01689). Submitted.
* **Davison, A.**, Austern, M. [Asymptotics of Network Embeddings Learned via Subsampling](https://arxiv.org/abs/2107.02363). [(GitHub repo with experiment code.)](https://github.com/aday651/embed-asym-exeriments). Submitted.
* Ward, O.G., Huang, Z., **Davison, A.**, Zheng, T. [Next waves in veridical network embedding](https://doi.org/10.1002/sam.11486). Statistical Analysis and Data Mining. 2020; 1– 13.

### Other manuscripts ###

* **Davison, A.** New advances in causal inference. _Part III Essay_. ([pdf](../files/partiiiessay.pdf))