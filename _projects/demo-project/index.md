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

## Motor 1
The first engine was an opportunity for me to learn, starting from almost zero experience.

- Machined from aluminum with a graphite nozzle
- Used 3D printed PLA fuel grain with gaseous oxygen oxidizer  
- Proved that I could build something that ignited

{% include image-gallery.html images="FirstInternals.PNG" height="400" %}
<span style="font-size: 16px">Motor components</span>

{% include image-gallery.html images="FirstTest.PNG" height="400" %}
<span style="font-size: 16px">First hot-fire test</span>

---

## Motor 2
The second engine was made to be compact, self-contained, and usable on a model rocket.

- Machined from aluminum with a low carbon steel nozzle
- Used 3D printed ABS fuel grain with nitrous oxide oxidizer
- Custom pyrotechnic valve that used solid propellant and a plastic burst disk

{% include image-gallery.html images="SecondInternals.png" height="400" %}
<span style="font-size: 16px">Motor components</span>
{% include image-gallery.html images="ShockDiamonds.PNG" height="400" %}
<span style="font-size: 16px">First successful hot-fire test, showing mach diamonds in the exhaust</span> 

---

## Custom Simulation Program
After building lots of hardware, I wrote a simulation tool to model hybrid motor performance. It used regression rate models and thermodynamic calculations to predict chamber pressure, thrust, and total impulse among other things.

{% include youtube-video.html id="nEWOL1fKOFY&t" autoplay= "false"%}
<span style="font-size: 16px">Video going through models used and program architecture</span> 
{% include image-gallery.html images="SimGraphs.png" height="400" %}
<span style="font-size: 16px">Graphs of various properties from a simulation</span> 


