---
layout: post
title: Why the normal distribution?
tags: [probability, information theory, expository]
---

When I was first studying probability theory as an undergrad, I had a bit of a conceptual hang-up with the Central Limit Theorem. [Simulating it in R](http://www.rpubs.com/christopher_castle/137490) gave a nice visual of how each additional random variable smoothed out some of the original distribution's individuality, and asymptotically we were left with a more generic shape. The proofs were relatively straightforward. One part, however, didn't really make sense to me. My problem was this: **Of all the many possible distributions, why is the normal distribution in particular that our i.i.d random variables converge to in distribution?**

The normal distribution has lots of interesting properties that I looked at to gain some intuition, but many of the them seem to follow from the CLT, rather than explaining it. In fact, it wasn't until a later course in machine learning that integrated some [information theory](https://en.wikipedia.org/wiki/Information_theory) that I found a satisfactory answer to my question.

In this post, I'll explain an insight from the principle of maximum entropy that justifies conceptually the normal distribution's role in the CLT. To do so, we'll first build up a basic introduction to entropy, how probability and entropy interact, and then explain the entropy property of the normal distribution that helped me understand the question above.

Entropy
------
Information theory makes rigorous many of our informal ideas about how much uncertainty is resolved . Instead of rigorously defining information though, let's talk about entropy, or lack of information.

This principle, then, is about epistemic modesty. We can want to choose the distribution that meets our constraints, and assumes as little additional information as possible.

The Normal Distribution
---



In one sense, this result is counter intuitive. As statisticians, when we find out that a distribution we're working with is roughly normal, we tend to feel like we have . Assumptions of normality make choosing tools to work with relatively straightforward.
