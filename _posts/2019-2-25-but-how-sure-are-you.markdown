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
* **Bayesian Inference**: Intractable. There's a whole field on *approximate bayesian learning*
* **Variational Inference (ELBO)**: what is elbo
* **Variational Free Energy**: AKA compression cost, expected lower bound on marginal likelihood. 
* **Unbiased Monte Carlo estimate of the gradients**

#### Variational Free Energy
You know the kid you never thought you'd see again? Okay gang, let's see what variational free energy really is... Chemistry??! (This looks insane you should <a href="https://slideplayer.com/slide/6553758/">check it out later</a> @self).

First, let's understand <a href="https://physics.stackexchange.com/questions/149493/gibbs-free-energy-intuition">Gibb's free energy</a>. "I want a math-free explanation. Can anyone simply explain?"??? (big mood).

water my seeds til the flower just grow

We learned about martingales but I still don't really understand them. Here are two famous ones to look into. Moving right along...

#### Implementation Notes
* NCHW = batch size, channels, height, width. Contiguous storage.
* **ReLU**: Looked <a href="https://datascience.stackexchange.com/questions/26475/why-is-relu-used-as-an-activation-function">suspiciously linear</a>.



#### Cool Topics / Articles / Refreshers
* <a href="https://www.statisticshowto.datasciencecentral.com/em-algorithm-expectation-maximization/">MLE vs. EM</a>
* <a href="https://www.theanalysisfactor.com/what-is-a-latent-variable/">Latent Variables</a>
* <a href="http://mlg.eng.cam.ac.uk/teaching/4f13/1819/">Cambridge Probabilistic Machine Learning</a>
* <a href="">Gibb's Sampling (& other MCMC methods</a>
* <a href="http://www.cs.toronto.edu/~fritz/absps/emk.pdf">Variational Free Energy (Neal, Hinton (1998))</a>
* <a href="https://en.wikipedia.org/wiki/Markov_chain_Monte_Carlo">Markov Chain Monte Carlo</a>
* <a href="https://www.cs.toronto.edu/~radford/research.html">Neal's Research Interests (are lit)</a>
* <a href=""></a>

