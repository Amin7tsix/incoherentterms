---
layout: post
title: "What is an accelerometer?"
description: "Spring-mass accelerometer working principle"
date: 2025-08-24
# feature_image: images/2025-08-24/20250824-Acelerometro_wikipedia.JPG
tags: [physics, navigation]
---

<div style="text-align: center;">
<figure>
    <img src="{{ site.baseurl }}/images/2025-08-24/20250824-Acelerometro_wikipedia.JPG" 
    width="300" 
    height="150"
    alt="From wikipedia"
    class="center">
    <figcaption>Accelerometer from wikipedia</figcaption>
</figure>
</div>


An accelerometer is a device that measures linear acceleration. One of the simplest ways to build one is with a **spring–mass system**.  

Imagine a car with a spring and a small test mass mounted inside. One end of the spring is fixed to the car’s body, and the other end is attached to the mass. If we orient the spring along the direction of the car’s motion, the system will respond whenever the car accelerates.  
<!--more-->
When the engine runs, the wheels push on the ground with a force $-F$, and the ground pushes back on the car with an equal and opposite force $F$. This force accelerates the entire car—including the spring–mass system.  

But here’s the key: the fixed end of the spring accelerates exactly with the car, while the test mass resists the change in motion, as it is not connected to the car rigidly. The spring stretches or compresses, exerting a restoring force according to Hooke’s law. The displacement of the spring, $\Delta L$, becomes the observable to measure the car's acceleration. The Hooke's law applied here is

$$F - F' = k \, \Delta L,$$

where $k$ is the spring constant, $F$ the total force on the system, and $F'$ the force transmitted to the test mass. By calibrating $\Delta L$ against known accelerations $a$, we can turn spring displacement into a measurement of car's acceleration.


### Accelerometers in free fall

Here’s an interesting twist: a spring–mass accelerometer in free fall does **not** measure Earth’s gravitational acceleration ($g = 9.8 \,\text{m/s^2}$). Instead, it reads **zero**.  

Why? Gravitational force on an object is proportional to its mass. The gravitational force is  

$$F = G \frac{m M}{r^2},$$  

with $m$ the mass of the object, $M$ Earth’s mass, $r$ the distance to Earth’s center, and $G$ the gravitational constant. Because this force is proportional to $m$, the acceleration $a = F/m$ is the same for all mass elements of the system. In other words, every part of the spring and the test mass accelerate downward together.

Since there’s no relative acceleration between the parts, the spring does not stretch or compress—it stays in its rest length. That’s why an accelerometer in free fall measures zero: it can only detect *proper acceleration* (caused by forces other than gravity), not the pull of gravity itself.  

---

### Why this matters?

An accelerometer is essentially a tiny spring–mass system that compares how much a test mass lags behind its support. It’s a beautiful example of how a simple physical principle underlies much of our modern technology, from navigation systems in phones to guidance in spacecraft.