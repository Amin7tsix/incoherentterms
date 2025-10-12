---
layout: post
title: "A Glimpse Into My Nonlinear Optics Experiment"
description: "Exploring second-harmonic generation (SHG) in a Lithium Niobate thin film using light from a parametric down-conversion process."
date: 2025-10-12
lang: en
tags: [physics, experiments, nonlinear optics, second harmonic generation, lithium niobate]
---

While going through some old lab photos, I found a short video from my master’s thesis experiment — just 15 seconds long, but it brought back so many memories from the lab. 

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <iframe
    src="https://youtube.com/embed/e6lqZKQJmj4?feature=share"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
    frameborder="0"
    allowfullscreen>
  </iframe>
</div>

<!--more-->

\\
It shows a Lithium Niobate thin film mounted on an XYZ translation stage, sitting neatly between two miniature lenses (each with a 4.5 mm focal length):

<div style="text-align: center;">
<figure>
    <img src="{{ site.baseurl }}/images/2025-10-12/2025-10-12-Samples-in-focus-collimation-setup.jpeg" 
    width="400"
    alt="Part of the optical setup"
    class="center">
    <figcaption>Part of the optical setup</figcaption>
</figure>
</div>

\\
During the recording, the sample is illuminated by infrared light generated through a parametric down-conversion (PDC) process in a BIBO crystal. The motivation for generating the pump light via PDC was to have an easy way to tune the wavelength over a large range. We needed this to study the wavelength dependence of the SHG process, i.e., $\chi_2(2\omega_p; \omega_p, \omega_p)$. The BIBO crystal was pumped with a pulsed 532 nm laser, and by tuning the crystal angle — mounted on a rotation stage — we could achieve signal/idler wavelengths ranging from about 1100 nm up to around 1700 nm.

In the video, as the wavelength of the pump light changes, the Lithium Niobate glows in different colors — in the visible range. That glow comes from second-harmonic generation (SHG), where the material converts light into new colors by doubling its frequency. In this experiment, the main goal was actually to study another nonlinear crystal: Gallium Selenide (GaSe). It is possible to make very thin layers of GaSe and use them to generate entangled photon pairs via SPDC. The Gallium Selenide sample was installed side by side with the Lithium Niobate on the translation stage. Having them both on the same stage allowed for easy switching between the two samples. Because Lithium Niobate produced a stronger signal, it served as a convenient reference for calibration and verification. Here’s another picture showing both samples:

<div style="text-align: center;">
<figure>
    <img src="{{ site.baseurl }}/images/2025-10-12/2025-10-12-LiN-and-GaSe-on-translation-stage.jpeg" 
    width="400"
    alt="Lithium Niobate and Gallium Selenide crystals in the focal plane of two lenses"
    class="center">
    <figcaption>Lithium Niobate and Gallium Selenide crystals in the focal plane of two lenses</figcaption>
</figure>
</div>

\\
Looking back, I love how this short clip captures the magic of experimental optics — when something invisible suddenly becomes visible in a burst of color.