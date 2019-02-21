---
layout: post
title:  "CVML Literature Review"
date:   2019-01-30 13:52:42 -0500
categories: jekyll update
---

# Reparameterization Trick for Variational Autoencoders
Stumbled across variational autoencoders and was fascinated by the idea of 'reparameterization'. It seems like magic.

We all know what traditional autoencoders look like. We try to reproduce each trianing point, try to preserve structure, figure out what is important in our data. 

Variational autoencoders replace the middle step with a *distribution*. This means we can *sample?* points (lets say images, since they're really the most intersting high-dimensional data to view). We can produce cool images. Cool.

The problem with sampling is it decouples our computation graph. *This means we can't backpropagate our gradient*. Ah, disaster! We're done for.

How the heck are you supposed to backprop through a *sampling*?!

Answer: reparameterization trick. Yeah, I know. Watch this.

Say we have a computation graph. [insert drawing]
We rewrite this equation in terms of a new random variable, X ~ N(0,1).
We can backprop this a w bar and epsilon are constant.

The result is some pretty cool animations:

[show transition animations]
*transition animations inspired by Lucas Hu.

# The Magic of Random Sketching
