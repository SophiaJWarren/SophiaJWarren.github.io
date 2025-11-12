---
title: "PIP Plier Project"
excerpt: "Print-in-place needle-nose pliers for grabbing small objects."
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
## Print-in-Place 
Print-in-place (PIP) parts are 3D-printed as fully assembled, functional mechanisms where joints, hinges, and links come straight off the printer ready to move. No screws, glue, or tools required. Clever clearances between layers create motion where you’d normally expect an assembly.

PIP success depends on pairing materials that stick together just enough to survive printing but still move freely afterward. Common pairings include:
* PLA + TPU (95A) – strong handles with flexible hinges or springs.
* PETG + TPU – higher temperature resistance, good for functional parts.
* Nylon + TPU – very durable but can be tricky to bond cleanly.

Some examples of PIP include 
* Mechanical toys and fidget mechanisms that print in one piece and articulate immediately.
* Prosthetic hands and grippers where fully printed hinges reduce cost and assembly time.
* Robotic linkages and valves that use printed flexures for repeatable motion.

## Project Description
This project explores this idea by designing needle-nose pliers that can grip and lift tiny through-hole resistors. Two materials are used, TPU and PLA, to form a pair of grippers that flex and return to position when released. Each pair of pliers must be able to pick up a through-hole resistor and move it in testing.

## CAD Design
* Trigger: 
  Rather than a traditional squeeze mechanism, the a trigger-pull mechnaism was used to close the jaws of the pliers.
* Handle:
  The handle was rigid and designed to be compact, fitting comfortably in hand. It was printed from PLA.
* Trigger:
  The trigger was rigid and designed to comfortably fit the index finger. It was printed from PLA. 
* Jaws:
  The jaws were flexible and attached to the tips of the handle and the center of the trigger. They were printed from TPU95.

## Iterating
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
