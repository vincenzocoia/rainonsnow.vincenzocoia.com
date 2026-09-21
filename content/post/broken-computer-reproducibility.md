---
title: "My computer died and took the analysis with it"
date: "2026-07-15"
---

Earlier this year my computer broke, and every output of the project's data analysis went with it. Fitted models, diagnostic plots, the probability contours, the figures I had been building slides around — all of it.

There is a particular feeling that arrives in the first few seconds after you understand what has happened. I do not recommend it.

## Then the feeling passed

Because none of it had been made by hand.

Every one of those outputs was produced by a pipeline: download the ERA5-Land data, extract peak events over a threshold, fit the distributional learning model, graft the tails, generate the diagnostics, draw the figures. Nothing important had been typed into a console once, admired, and then forgotten. Nothing existed only as an object sitting in a workspace that I could not reconstruct.

So the recovery plan was embarrassingly short: run it again.

That is not the same as getting the work back for free. It cost time, and it surfaced a few places where the pipeline turned out to be less automatic than I had believed — steps I had assumed were captured and were in fact living in my head, or in my old file system. Those got fixed on the way through, which is the one genuinely good thing to come out of a broken computer.

## An experiment nobody would volunteer for

Reproducibility is usually argued for on someone else's behalf. Reviewers should be able to check your work. Other researchers should be able to build on it. Future readers should be able to see what you actually did. All true, all slightly abstract, and all easy to defer when a deadline is closer than the principle.

What I had not appreciated is how much of it is insurance for *you*. A pipeline is a promise that the work is recoverable from its inputs, and that promise is worth exactly nothing until the day it is worth everything. I got an unannounced audit of mine, of a kind I would never have scheduled deliberately, and it passed.

If you want to know whether your own analysis is reproducible, there is a cheap version of this test: on a clean machine, from the raw data, can you regenerate the figure you are proudest of? If the honest answer is "probably, given a week", that is a different answer from yes.

## Since then

The work carried on, with two changes. The study area was temporarily cut down to a small grid over the Alps, so that experiments run in minutes rather than hours while the methodology is still moving. And the project is now set up on the [CINECA](https://www.cineca.it/en) supercomputer, ready for the full-scale runs in year two.

The new computer is fine, thank you for asking. It has not been tested.
