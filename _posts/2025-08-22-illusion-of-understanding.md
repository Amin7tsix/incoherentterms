---
layout: post
title: "The Illusion of Understanding"
description: "An analogy between Daniel Kahneman’s book section *The Illusion of Understanding* and my experience in the lab"
date: 2025-08-22
tags: [conceptual metaphor, books]
---

Here’s a metaphor that came to mind while reading *The Illusion of Understanding* by Daniel Kahneman.  
<!--more-->

In our cold atom experiments, learning something about the atoms usually requires repeating the experiment many times. For example, suppose we want to study how the population of atoms in a certain state changes as we vary a parameter A over the range from A0 to A1. We begin by setting A = A0, let the particles evolve, then measure their state. This produces a single *shot*—essentially a snapshot of the atoms. We then increment the parameter to A = A0 + dA, repeat the process, and continue until we reach A = A1. This gives us one scan through the parameter range. To obtain meaningful results, we repeat this scan many times, each time preparing the cold atom sample from scratch, which allows us to build up a *probability distribution*.

The number of repetitions depends on the question at hand. For a typical spectroscopy experiment, where we aim to determine the energy of an atomic transition, we might repeat the experiment about 500 times. With the collected data, we fit a theoretical model to extract the relevant parameters.

Now suppose we’ve determined the transition energy and want to observe *Rabi oscillations*—coherent oscillations of an atom between two energy levels. In this case, the scan parameter is the duration of the laser pulse driving the transition, and the observable is the population of atoms in one of the states. A single scan through the range might look like this:

<figure>
    <img src="/images/2025-08-22/20250822_single_shot_data.png" 
    width="800" 
    height="450" 
    alt="Single run data">
    <figcaption>Experimental data from a single run of the experiment.</figcaption>
</figure>

The large error bars show that we are not very confident about this data yet. If we repeat the entire scan 100 times and average the results, the data might instead look like this:

<figure>
    <img src="/images/2025-08-22/20250822_many_shots_data.png" 
    width="800" 
    height="450" 
    alt="Single run data">
    <figcaption>Experimental data from a single run of the experiment.</figcaption>
</figure>

Now the error bars are smaller, which is expected, since we repeated the experiment many times and are now more confident about each data point. If we fit a model to the first (single-run) dataset, we might obtain something like this:

<figure>
    <img src="/images/2025-08-22/20250822_single_shot_data_and_fit.png" 
    width="800" 
    height="450" 
    alt="Single run data">
    <figcaption>Experimental data from a single run of the experiment.</figcaption>
</figure>

Whereas fitting the averaged dataset gives us something more like this:

<figure>
    <img src="/images/2025-08-22/20250822_many_shots_data_and_fit.png" 
    width="800" 
    height="450" 
    alt="Single run data">
    <figcaption>Experimental data from a single run of the experiment.</figcaption>
</figure>

The first fit is misleading. It suggests persistent, coherent oscillations lasting for several cycles. In quantum computing terms, this would imply an exceptionally high-fidelity NOT gate (which flips one atomic state to another). However, the averaged data tells a different story: on average, our NOT gate is not nearly as good as the single run suggested. It achieves a fidelity of about 90%.

---

*The Illusion of Understanding* is a section in Daniel Kahneman’s *Thinking, Fast and Slow*. He describes a fallacy in human reasoning: our tendency to weave coherent stories from very limited information. To quote him: *“Paradoxically, it is easier to construct a coherent story when you know little.”*  

This insight is what reminded me of the analogy above. I highly recommend this section of the book—and, in fact, the entire book.
