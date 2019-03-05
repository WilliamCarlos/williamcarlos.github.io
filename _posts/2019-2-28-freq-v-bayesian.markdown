---
layout: post
title:  "Frequentist or Bayesian"
date:   2019-03-05 10:59:54 -0500
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

Ahh. The great crusades in computer science. Vim or Emacs (if sublime, please show yourself out).' Tabs vs Spaces (if tabs, please show yourself out)''. These crusades I understand. The next big crusade is frequentists vs bayesian views on probability.

[insert twitter screenshots of arguments]

'just kidding ily
'' like lowkey fr tho

#### Frequentist? Bayesian? What does this even mean?
Dutch book example. Seems like a weird convoluted idea to formalize an intuitive idea -- it's a measure of belief. The dutch book example specifies it as a *universal measure of belief*; there are no assymmetries to belief.

All things follow from the *Axioms of Probability*, which consist of two main parts.
	1. A definition of our probability space
	2. Inducing a *measure* (i.e. probability) to elements in our probability space.

Rigorously, we can define these as follows:
* event space omega
* unions are also events
* probability of event space is 1

Intuitively, this translates to:
* We have a set of possible events.
* Any subset of the space of possible events is also an event (e.g. if {sun, rain, cloud} is in our event space, then {sun, rain}, {rain ,cloud}, {sun, cloud}, singleton sets, are also in our event space omega. 
* The outcome of an experiment will be an event in our defined space.



