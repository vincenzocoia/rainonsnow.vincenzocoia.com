---
title: "New {discretes} R package available"
date: "2026-03-31"
---

![discretes logo](discretes-logo.png)

Launching the [Probaverse](https://probaverse.com) packages last December has for sure streamlined my workflow around distributions. But one critical thing was missing: native support for discrete distributions more generally.

While continuous distributions get the most attention, my workflows encounter distributions with a discrete component all the time. Think: empirical distributions; zero-inflated models; poisson processes.

The difficult part of discrete distributions is keeping track of what the possible outcomes are, because sometimes there are infinitely many possibilities, as in the Poisson distribution. Start manipulating these distributions, and keeping track of these becomes much harder.

That's what the new [{discretes}](https://discretes.netlify.app) package does. I'm happy to announce that this package is now available on CRAN as of today! I talk more about this package in the [official blog post on the probaverse.com website](https://probaverse.com/post/2026-03-31-introducing-discretes-0-1-0/). While it stands alone from the Probaverse ecosystem, it will become a critical component to support discrete distributions, and the distributional learning tasks faced by this rain-on-snow research project.
