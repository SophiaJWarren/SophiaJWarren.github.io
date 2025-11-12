---
title: "PIP Plier Project"
excerpt: "Print-in-place needle-nose pliers for grabbing small objects."
header:
  image: /assets/img/Plier Iterations.jpg
  teaser: /assets/img/Plier Iterations.jpg
gallery:
  - image_path: assets/img/Plier Iterations.jpg
  - image_path: assets/img/Pliers GIF.GIF
  - image_path: assets/img/Pliers drawing.png 
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
This project explores this idea by designing needle-nose pliers that can grip and lift tiny through-hole resistors. Two materials are used, TPU and PLA, to form a pair of grippers that flex and return to position when released. Each pair of pliers must be usable immediately off the printer (no glue, tape, screw, etc,) and able to pick up and move a through-hole resistor in testing.

## Design 
### Concept Overview
Rather than a traditional squeeze mechanism, the pliers employ a trigger-pull mechanism to close the jaws of the pliers because a single finger motion can be easier to repeat continuously than a full hand-squeeze. A rigid handle supports the pliers with a rigid trigger suspended in the center. Flexible jaws attach the handle and trigger such that when the trigger is pulled, the nose of the jaws bend inward and grip the item. Specific part designs are outlined in the Part Specifications section.
### CAD Modelling
The pliers were designed in Fusion 360 using parameterized dimensions for efficient iteration. The pliers are symmetrical, making mirroring an effective modeling tool. Half of the design was sketched, and then the 3 parts were extruded as independent bodies so they could be printed individually in the correct material. The Fusion 360 mirror function does not recognize parameters when used in sketches (2D), so the parts were mirrored in 3D to complete the pliers. 
### Part Specifications
* Handle:
  The handle was rigid (PLA) and designed to be compact, fitting comfortably in hand. The size of the handle was initially estimated from holding a computer mouse in the position the pliers would be held to assess how comfortably it fit in a hand without overextending or clenching. The result was a width of ~45 mm and length of ~63 mm. The handle has a round bottom to avoid sharp corners poking the user.
* Trigger:
  The trigger was rigid (PLA) and designed to comfortably fit the index finger (~20 mm diameter). 
* Jaws:
  The jaws were flexible and attached to the tips of the handle and the center of the trigger. They were printed from TPU 95A.

## Iterating
The first iteration of the pliers was largely successful, but the interlocking joints were not functional and required glue. The interlocking joints were too small very fine details and a tolerance of 0.2 mm was used. This resulted in very small and loose joints that did not hold the pliers together without glue. When fully glued together, Iteration 1 worked perfectly, indicating the overall design was promising.

The second iteration aimed to fix the interlocking problem. The interlocking joints were made larger by extending the jaws along the side of the handle so the joints could be larger and more could be used in multiple locations and directions. The joints on the triggers were only changed slightly due to the trigger's small size. A tolerance of only 0.05 mm was used. After printing, Iteration 2 had strong joints to the handle that held the jaws firmly as desired. The trigger joints were improved from Iteration 1, but were still not perfectly stable. During use, one of the jaws would pop out of the trigger after a few pulls when not handled carefully. 

The third iteration was the final version of the pliers. The joints on the trigger were made as large as possible without sacrificing the integrity of the trigger. The handle joints on Iteration 2 were ideal, so the same tolerance of 0.05 mm was used in printing. Iteration 3 worked perfectly, with stable joints holding all parts together. It was able to pick up resistors and other small items easily and repeatedly without fail. 

{% include gallery caption="PIP Pliers Gallery" %}
