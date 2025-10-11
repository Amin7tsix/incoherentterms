---
layout: post
title: "Compact double-pass AOM setup"
description: "I present a compact double-pass AOM setup which I recently built in the lab."
date: 2025-10-11
lang: en
tags: [physics, experiments]
---

<div style="text-align: center;">
<figure>
    <img src="{{ site.baseurl }}/images/2025-10-11/20251011_AOM_diffraction_from_Saleh_and_Teich_book
.png" 
    width="400"
    alt="Bragg diffraction schematic from Fundamentals of Photonics textbook by Saleh and Teich"
    class="center">
    <figcaption>Bragg diffraction</figcaption>
</figure>
</div>

Double-pass your AOM!\\
It’s actually pretty cool. When you retro-reflect the diffracted light back into the AOM and diffract it in the same order again (like +1 and +1, or -1 and -1), a few nice things happen:

<!--more-->

1. Tuning range: \\
There will be an effectively larger tuning range of the radio frequency drive. Because a df change of the drive frequency translates to a 2.df frequency change on the light.

2. Pointing: \\
If the AOM is placed in the focal plane of a lens followed by the retro-reflector, the pointing of the twice-diffracted light stays fixed when the drive frequency is changed.

3. Thermal sensitivity: \\
Because of feature number 2, the typical temperature sensitivity in AOMs that leads to beam pointing instability can be largely mitigated. 

I recently wanted to divide my laser beam into 5 branches and set up a double-pass AOM for each branch. They are then used for Raman sideband cooling in a Yb-171 tweezer experiment. Because I wanted to push the setup for compactness, I ended up using a polarizing beamsplitter cube glued on a mirror mount together with the AOM on a mirror mount. Combined, they provide 4 degrees of freedom to align the beam position into the AOM crystal and hit the Bragg angle of the AOM crystal. Here's the schematic of this arrangement:

<div style="text-align: center;">
<figure>
    <img src="{{ site.baseurl }}/images/2025-10-11/20251011_double_pass_AOMs.png" 
    width="500"
    alt="Schematic of the optical setup"
    class="center">
    <figcaption>Schematic of the optical setup</figcaption>
</figure>
</div>

And a top view of the experimental setup:

<div style="text-align: center;">
<figure>
    <img src="{{ site.baseurl }}/images/2025-10-11/20251011_double_pass_AOM_setup_from_the_lab
.jpeg" 
    width="500"
    alt="The experimental setup"
    class="center">
    <figcaption>The experimental setup of the double-pass AOMs</figcaption>
</figure>
</div>

It gives me satisfaction to see all 4 ports of each cube being used!

Bonus \(!): \\
If the retro-reflector is exactly f away from the lens, i.e. a cat's eye arrangement, a collimated beam entering the AOM leaves collimated after twice diffraction. Now, if the retro-reflector is moved back and forth, the beam's divergence can be tuned. This means that if we are focusing the double-diffracted light using a single lens, the focal point can be moved along the optical axis. In a [recent work](https://arxiv.org/pdf/2510.07633) from Manuel Endres team, authors propose using a grating as the retro-reflector which enables using the acoustic diffraction frequency to move the beam's focus position along the optical axis.