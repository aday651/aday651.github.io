---
permalink: /research/
title: "Research"
author_profile: true
redirect_from: 
  - /research.html
---

My research interests are mainly centered around statistical and computational aspects (and the interplay of the two) of modern-day machine learning techniques, motivated through considerations of how statistical methods are implemented (usually through some type of stochastic optimization procedure). In particular, here are a few topics which I’m currently thinking about:

* **(Spurious) local minima of empirical risk landscapes** – Modern machine learning methods usually consist of minimizing an empirical risk in order to find an estimate of some desired quantity of interest. However, these problems usually end up being non-convex. This is problematic as it allows for the possibility that, when trying to find a minima in practice, we instead find only a local minima which fails to be a desirable estimator – for example, we may end up returning a classification rule which fails to work well when we use it on yet unseen data. This gives rise to two questions: can we show that such `bad local minima’ do not exist, or can we design an algorithm which avoids them altogether?

* **Learned embeddings of complex structured data** – A usual statistical approach to modeling data is to specify a probabilistic model for data we observe, and then use the learned parameters of our model to perform a task we care about. However, for some types of complex structured data (such as networks, or collections of images), a surprisingly successful approach is to learn a 'embedding' of our data into a Euclidean space which is somewhat representative of the structure we hope to uncover within it. For example, if we had a social network, we would want to assign each user a point in some (possibly high dimensional) Euclidean space, where the distances between the points we assign to users are reflective of their similarity to each other in terms of interests, friendships and et cetera. We would then use the embedding data points in a typical ML algorithm (likely whatever is currently 'all the rage', or random forests) to perform our downstream task. Whether this works is contingent on whether our learned embedding carries meaningful information about the latent structure of our data, and as such natural questions arise to if and when this will be the case.

In terms of directly applied problems, I am particularly interested in applications of statistical and machine learning methods within epidemiology and the medical sciences, and I am currently exploring some projects involving tracking and predicting the spread of epidemics for infectious diseases. This is somewhat contingent on getting some interesting, usable data first, so if you have some, please get in contact with me!

Although my focus currently is theoretical, I try and take the stance that theoretical investigations should be driven by considerations which arise from actually attempting to analyze data in practice.  Due to this, I’m generally interested in hearing about how these techniques are used in any area (with exception to [advertising](https://google.com/)). Please get in contact if you think we’d have some shared interests!

## Papers ##

### Pre-prints and other manuscripts ###

* Davison, A. (2016) New advances in causal inference. _Part III Essay_. ([pdf](../files/partiiiessay.pdf))