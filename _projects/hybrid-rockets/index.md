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

```python
# --- Fuel regression and mass flow update ---

# port cross-sectional area (m^2)
a_p = math.pi * (dia_p / 2) ** 2

# oxidizer mass flux (kg/m^2s)
G = m_dot_i / a_p

# regression rate (m/s) from empirical model
r_dot = a * (G ** n)

# update port diameter with regression over timestep
dia_p += 2 * r_dot * d_time

# fuel mass flow (kg/s) from port growth
m_dot_f = (math.pi * (dia_p / 2) ** 2 - a_p) * l_g * rho_f / d_time
```
<span style="font-size: 16px">Sample snippet from simulation code</span> 

{% include youtube-video.html id="nEWOL1fKOFY" autoplay= "false"%}
<span style="font-size: 16px">Video going through more complex models used and general program architecture</span> 
{% include image-gallery.html images="SimGraphs.png" height="400" %}
<span style="font-size: 16px">Graphs of various quantities from a simulation</span> 


