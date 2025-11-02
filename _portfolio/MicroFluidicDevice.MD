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
  - image_path: assets/img/pre_post_treatment.png  
---
## Introduction
Pinched flow fractionation (PFF) is a microfluidic technique that continuously separates particles by size. A PFF device first channels a mixture of particles suspended in liquid into a pinched channel section. As the pinched channel opens to a wider section, the particles separate based on size due to buoyancy forces and are collected through different outlet channels placed at their calculated heights [1](https://doi.org/10.1021/ac049863r).

PFF microfluidic devices are increasingly used for precise particle sorting in biomedical and analytical applications where gentle and continuous separation is required. They are especially valuable for separating specific blood cell types, such as separating circulating tumor cells from white blood cells for cancer diagnosis and monitoring [2](https://doi.org/10.1039/c5lc01014d). Unlike traditional methods like filtration or centrifugation, PFF separates particles purely through controlled laminar flow, avoiding clogging and minimizing mechanical stress on delicate cells. This hydrodynamic, label-free approach allows high-throughput, continuous sorting with high viability and precision, making it superior for biological samples.

[1] https://doi.org/10.1021/ac049863r [Yamada et al, 2004](https://doi.org/10.1021/ac049863r)
[2] https://doi.org/10.1039/c5lc01014d [Pødenphant et al, 2015](https://doi.org/10.1039/c5lc01014d)

## Design
* Symmetric: 
  The broad channel widens evenly on both sides after the pinched channel
* Outlet boundaries: 
  Channel heights were mathematically determined based on the width of the sections and particle diameter. Outlet channels were given wide sources to account for error in flow sorting.
* Flow Balancing: 
  Buffer liquid had two outlet ports to compensate for the greater volume of buffer liquid than particle-carrying liquid. Particle outlet channels were long and serpentine to increase resistance and balance the flow rate between all four outlet paths. 
  - image_path: assets/img/microfluidic sketch.png
<p align="center">
  <img src="SophiaJWarren.github.io/assets/img/microfluidic sketch.png" alt="PFF Device Sketch" width="400">
</p>

## Testing
The PFF devices were tested using a syringe pump to introduce the particle and buffer fluid mixture. Barbs connected to tubes were used to collect the particles and liquid from the device. In initial testing, turbulence was observed in the device, disrupting particle sorting. To combat this, a denser and more viscous fluid was added to the mixture. The particles were not perfectly neutrally buoyant in this mixture, however, causing the particles to float. The tubes connected to the outlet barbs had variations in pressure head, causing varying resistances at each outlet and disrupting flow.

![MicroFluidic Testing Setup](SophiaJWarren.github.io/assets/img/MicroFluidic Testing Setup.jpg) ![Outlet Tubes](SophiaJWarren.github.io/assets/img/MicroFluidic Outlet Tubes.jpg)
This particular PFF device was only tested briefly due to time and resource limitations. It was tested without barbs and with few particles in the mixture. Sorting was moderately successful given these restrictions, outperforming many of the other designs tested.
*  Wide outlet channel sources provided appropriate tolerance, allowing for better sorting given imperfect particle flow paths.
*  The large width of the broad section created greater space between the paths of the particles, providing better sorting. 

## Future Iterating
This PFF design was promising, providing moderately successful sorting despite imperfect testing conditions. Some potential improvements for future testing are listed below:
*  The original buffer fluid should be used at a reduced flow velocity to prevent turbulence without altering particle buoyancy.
*  A helping hand tool (a tool with multiple adjustable arms with gripping mechanisms) could be used to provide stable support to the outlet tubes so their heights can be precisely adjusted to remove the pressure head resistance obstacle.
*  Programmable syringe pumps could be used at the outlets to provide stable flow rates. The final project of a prerequisite class is to make such syringe pumps, so this could be a collaborative effort between DF 2100 and CHBE 4200 students. 

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
