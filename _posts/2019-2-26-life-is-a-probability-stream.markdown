---
layout: post
title:  "Life is a Probability Stream: Probability & Computing"
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

A cheat sheet/study guide for Oxford's <a href="https://www.cs.ox.ac.uk/people/elias.koutsoupias/pc2018-19/">Probability & Computing</a> course. Probably the most engaging (and frustrating) course I've taken so far. Disgustingly yet beautifully theoretical. Hopefully I'll get some practical examples up soon...

#### Motivations
There are a lot of difficult problems in computer science. Many of them we can only solve probabilistically. Others we can solve faster using a probabilistic algorithm, with either no hit to accuracy or a controlled hit bound by some error $\epsilon$ and probability of being within that bound $\delta$.

#### Table of Contents
* THIS IS JUST 8 WEEKS!!!!!!!!!
* <a href="">Secretary Problem</a>
* <a href="">Indicator Variables and Linearity of Expectation</a>
* <a href="">Concentration Bounds</a>
	* <a href="">Chernoff Bounds</a>
* <a href="">Sampling and Counting</a>

#### Secretary Problem
Listen up chaps. This will help you get married.

#### Indicator Variables and Linearity of Expectation
One of our most powerful tools.

#### Concentration Bounds
With indicator variables and linearity of expectation it's usually pretty easy to figure out the mean. However, because the mean of a distribution is a summary statistic, it's usually not as descriptive as we need it to be. For example (insert 2 distributions with the same mean, shifted distributions, concentrated ones). To address this, we introduce the idea of **concentration bounds**, which describe how tightly we are distributed about the mean. We have four bounds for this -- **Markov's Inequality**, **Chebyshev Bounds**, **Chernoff Bounds**, and the **Azuma-Kiszuki** bound.

#### Chernoff Bound
We're going to take a quick detour into the land of sampling and counting. Calculating the area of a body. Columbia dude sampling animation.

We'll dive deeper into sampling and counting methods later.

#### $\epsilon$-uniform Sampling
I like this topic a lot because it starts very intuitively and by adding just a little bit of machinery, we can build the tools to solve some NP-hard problems. Very elegant. You'd think Monte Carlo algorithms would tend to be quite brute-forcey but oftentimes they're actually quite pretty. **$\epsilon$-uniform sampling**, in particular, seems to be a very useful tool.

relevent excerpt from Oxford's probability class (please don't sue me Oxford)

In general, we call these algorithms **Fully Polytime Approximation Scheme** and **Fully Polytime Uniform Sampling Scheme**. Really the *fully polytime* is redundant within the context of these notes. *All* algorithms here are going to be polytime. Once we open up complexity classes to exponential, deterministic algorithms probably exist. I do
n't even want to meet a problem that results in an exponential-time randomized algorithm. Wew lad. So let's shorten the names. We have a randomized **Approximation Scheme** and a randomized **Uniform Sampling Scheme**. We also have a theorem that states you can create any approximation scheme if you are given a uniform sampling scheme. Which makes sense. A quote from class was, "if you can sample it, you can count it". [insert elias photo + quote]

And it looks like it telescopes away. Coolio. Moving right along.

#### DNF Counting and an Exponentially Small Target
mit ocw

#### Topics to Cover
Set balancing, martingales, Markov Chains and Stationary Distributions, mixing times, sampling and counting, balls and bins, permutations, secretary problem, MCMC, resevoir sampling, abacadabra & [] martingales, random walks/gambler's ruin

#### Life is a Probability Stream
Feat. elon boi: https://www.youtube.com/watch?v=GPaYrhUZSYQ
I had this idea independently (in the face of the outcome of undergraduate college admissions, 'meritocracy', what I'd been working towards for pretty much my whole life) and it's cool to see Elon reach this conclusion too. Don't pretend like your actions are deterministic kids -- the best you can do is change your probability stream to your liking and roll with the punches (or dice rolls).

Brief paraphrase: Technology DEGRADES without high effort from key people. It actually degrades.

I'm suspicious of the set-balancing regime. Let's test it out.
