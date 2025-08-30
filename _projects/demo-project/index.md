---
layout: post
title: Hybrid Rocket Engines
description: Designed, fabricated, and tested two hybrid rocket motors, built custom simulation software using models from available literature.
skills: 
  - CAD
  - Metal machining
  - Numerical simulation
  - Risk analysis
main-image: /ShockDiamonds.PNG
---

## Overview
I designed, fabricated, and tested two hybrid rocket engines, supported by a custom-built simulation program. This project combined machining, risk analysis, and performance modeling, creating a complete cycle of design → build → test → validate.

---

## Engine 1: Proof-of-Concept
The first engine was a small-scale prototype focused on proving ignition and combustion stability.

- Machined from aluminum
- Used 3D printed PLA fuel grain with gaseous oxygen oxidizer  
- Proved that I could build something that ignited

{% include image-gallery.html images="FirstInternals.PNG" height="400" %}
<span style="font-size: 10px">Motor components 1</span>

{% include image-gallery.html images="FirstTest.PNG" height="400" %}
<span style="font-size: 10px">First hot-fire test 1</span>

---

## Engine 2: Development Motor
The second engine scaled up thrust and burn duration, building on lessons from the first design.

- Redesigned injector using models from literature  
- Optimized fuel grain geometry for higher regression rate  
- Added chamber pressure and thrust instrumentation  

{% include image-gallery.html images="engine2.jpg" height="400" %}
<span style="font-size: 10px">Engine 2 firing with improved performance</span>

**Results**  
- Stable combustion across multiple tests  
- Experimental thrust data aligned with simulation  
- Identified thermal management as the main improvement area  

---

## Custom Simulation Program
Alongside hardware, I wrote a simulation tool to model hybrid motor performance. It used regression rate models and thermodynamic calculations to predict chamber pressure, thrust, and total impulse.
