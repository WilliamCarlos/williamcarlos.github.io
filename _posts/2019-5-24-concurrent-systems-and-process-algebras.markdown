---
layout: post
title:  "Algorithms"
date:   2019-02-26 22:01:21 -0500
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

#### Table of Contents
* What is a concurrent system?
Life is a concurrent system. (Sounds dramatic, I know, but bear with me, it's actually not a bad example). When most people think of computers, you think of a computation machine that processes things sequentially. For example, when you run a script on your computer, it executes... sequentially. In life, the things you do are done, by and large, sequentially. Birth -> Kindergarten -> High School -> College -> #CubicleLyfe -> Retirement -> Death. Breakfast -> Classes -> Lunch -> Homework -> Dinner -> Game of Thrones -> Sleep.

Concurrent systems is the study of how multiple sequential processes interact. What kind of behavior can we expect? Will the system ever "Deadlock"? (we'll get to that term later). 

For example, imagine you want to get coffee with your friend, Alex. Here is your schedule:
Your Schedule = Wake Up -> Breakfast -> Class -> You + Alex Coffee -> Class -> Homework -> Sleep

Here is Alex's schedule:
Alex Schedule = Wake Up -> Breakfast -> You + Alex Coffee -> Class -> Nap -> Class -> Sleep

Here, we have two sequential processes that *synchronize* on an event. You can wake up at any time. Alex can wake up at any time. You can have breakfast any time after you wake up. Alex can have breakfast any time after he wakes up. However, You + Alex Coffee must occur at the same time. The sequential processes interact. Alex needs to wait for your class to end before you can both execute/synchronize on You + Alex Coffee. After this synchronization is done, your sequential processes can diverge.

This is but one example/type of synchronization (called *Alphebatized Synchronization*). In this post I'll cover 3 total types of syncrhonization.

We tackle the study of these interactions between sequential systems from a (very) theoretical standpoint. We build an algebra, called a *process algebra*, to represent these systems. From this theory we can understand how these concurrent systems will behave, whether they meet program specifications. How to solve puzzles by building concurrent models.

The most interesting part of this area of computer science, in my opinion, is how something so theoretical (we'll literally biuld an algebra fam) can be applied to model real world systems, and solve puzzles. 

* Process Algebras
* Communicating Sequential Processes
* Solving Puzzles
* Refinement and Verification
