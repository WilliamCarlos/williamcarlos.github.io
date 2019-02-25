---
layout: post
title:  "Wait Are You Sure? Weight Uncertainty in Neural Networks"
date:   2019-02-24 15:52:15 -0500
categories: jekyll update
---

<script type="text/x-mathjax-config">
  MathJax.Hub.Config({
    tex2jax: {
      inlineMath: [ ['$','$'], ["\\(","\\)"] ],
      processEscapes: true
    }
  });
</script>

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

Diving into _<a href="http://proceedings.mlr.press/v37/blundell15.pdf">Weight Uncertainty in Neural Networks (Blundell et al.)</a>_.

#### The Big Idea
* Instead of some scalar $c \in \mathbb{R}$ for each weight of the neural network, we build a distribution over each weight and (and hidden unit).
* This is really hard! And computationally intractable for neural networks of any useful size. **Variational Inference** let's estimate the distributions in a cheap(er) (i.e. tractable) way.

#### Abstract
* **Bayes by Backprop**: Proposed algorithm to learn distribution of on weights.
* **Variational Free Energy**: AKA compression cost, expected lower bound on marginal likelihood. 
* **Unbiased Monte Carlo estimate of the gradients**
