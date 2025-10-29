---
title: "Microfluidic Device Project"
excerpt: "3D printed & casted pinch flow fractionation microfluidic device for particle sorting."
header:
  image: /assets/img/MicroFluidic Device and Mold.jpg
  teaser: /assets/img/microfluidic device.jpg
gallery:
  - image_path: assets/img/microfluidic device.jpg
  - image_path: assets/img/MicroFluidic Device and Mold.jpg
  - image_path: assets/img/microfluidic sketch.png
  - image_path: assets/img/MicroFluidic Testing Setup.jpg
  - image_path: assets/img/MicroFluidic Outlet Tubes.jpg
   
---
## Introduction
Pinched flow fractionation (PFF) is a microfluidic technique that continuously separates particles by size. A PFF device first channels a mixture of particles suspended in liquid into a pinched channel section. As the pinched channel opens to a wider section, the particles separate based on size due to buoyancy forces and are collected through different outlet channels placed at their calculated heights [1].

PFF microfluidic devices are increasingly used for precise particle sorting in biomedical and analytical applications where gentle and continuous separation is required. They are especially valuable for separating specific blood cell types, such as separating circulating tumor cells from white blood cells for cancer diagnosis and monitoring [2]. Unlike traditional methods like filtration or centrifugation, PFF separates particles purely through controlled laminar flow, avoiding clogging and minimizing mechanical stress on delicate cells. This hydrodynamic, label-free approach allows high-throughput, continuous sorting with high viability and precision, making it superior for biological samples.

[1] https://doi.org/10.1021/ac049863r
[2] https://doi.org/10.1039/c5lc01014d

## Design
* Symmetric: 
  The broad channel widens evenly on both sides after the pinched channel
* Outlet boundaries: 
  Channel heights were mathematically determined based on the width of the sections and particle diameter. Outlet channels were given wide sources to account for error in flow sorting.
* Flow Balancing: 
  Buffer liquid had two outlet ports to compensate for the greater volume of buffer liquid than particle-carrying liquid. Particle outlet channels were long and serpentine to increase resistance and balance the flow rate between all four outlet paths. 
  - image_path: assets/img/microfluidic sketch.png

## Future Iterating
Give him hope.

## Important Instructions for Designing a PFF Device
 1. Establish particle size range
 2. Establish widths of the pinched section, broad section, and outlet channels. 
  * Ensure all channel widths are at minimum 1.2x the diameter of the largest particles in use to prevent clogging. 
  * Do not exceed 1.5x the largest particle diameter in the pinched section to prevent particle stacking.
 3. Calculate particle heights based on particle size range and section widths
 4. Determine particle outlet source size based on particle heights to facilitate proper sorting within a margin of error
 5. Balance flow resistance by adjusting outlet channel length and using multiple outlets if necessary.

## Discussion
* Resin Printing:
  Resin printing is capable of printing the fine features required for microfluidic devices. 
* Scale: 
  The PFF device can be modified to accomodate a wider range of particle sized by increasing length and width of the broad section to get clearer particle separation and increasing the width of the particle channel sources.
* Particle Size limit:
  The lower limit on particle size that can be sorted with PFF is determined by channel width and flow stability.

{% include gallery caption="MicroFluidic Device Gallery" %}
