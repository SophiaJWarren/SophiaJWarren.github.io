---
title: "Top-Down Modelling Phone Mount Project"
excerpt: "Print-in-place needle-nose pliers for grabbing small objects."
header:
  image: /assets/img/Phone Mount Final CAD Views.png
  teaser: /assets/img/Phone Mount CAD.png
gallery:
  - image_path: assets/img/Phone Mount Final CAD Views.png
  - image_path: assets/img/Phone Mount CAD Iterations.png

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
Rather than a traditional squeeze mechanism, the pliers employ a trigger-pull mechanism to close the jaws of the pliers because a single finger motion can be easier to repeat continuously than a full hand-squeeze. A rigid handle supports the pliers with a rigid trigger suspended in the center. Flexible jaws attach the handle and trigger such that when the trigger is pulled, the nose of the jaws bend inward and grip the item. Specific part designs are outlined in the Part Details section.
<p align="center">
  <img src="/assets/img/Pliers GIF.GIF" alt="Working Pliers" width="400">
</p>
### CAD Modelling
The pliers were designed in Fusion 360 using parameterized dimensions for efficient iteration. The pliers are symmetrical, making mirroring an effective modeling tool. Half of the design was sketched, and then the 3 parts were extruded as independent bodies so they could be printed individually in the correct material. The Fusion 360 mirror function does not recognize parameters when used in sketches (2D), so the parts were mirrored in 3D to complete the pliers. There is a total of 3 part types (handle, trigger, & jaw), creating a total of 4 bodies (handle, trigger, & 2 jaws). The pliers were 10 mm thick in each part. 

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811ac51f917b821705a?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Printing Settings
The pliers used two materials: PLA for the handle and trigger, and TPU 95A for the jaws. The PLA parts were printed with a 0.4 mm nozzle and the TPU parts were printed with a 0.6 mm nozzle. This design did contain a spring grid component, so all other settings were left to default.
### Part Details
###### Handle:
The handle is rigid (PLA) and designed to be compact, fitting comfortably in hand. The size of the handle was initially estimated from holding a computer mouse in the position the pliers would be held to assess how comfortably it fit in a hand without overextending or clenching. The result was a width of ~45 mm and a length of ~63 mm. The handle is U-shaped, with a round bottom to avoid sharp corners poking the user. The tips of the handles have the dovetails to interlock with the jaws.
###### Trigger:
The trigger is rigid (PLA) and designed to comfortably fit the index finger (~20 mm diameter). The trigger is circular with a thickness of ~4 mm. The top of the trigger has two dovetails, one for each jaw. There is a ~10 mm gap between where the two jaws attach to allow the jaws to pinch at the nose without colliding elsewhere. 
###### Jaws:
The jaws are flexible (TPU 95 A) and attached to the tips of the handle and the center of the trigger. They are at a 15-degree angle from the center axis of the handles and are ~10 mm apart at the base (where they attach to the trigger) so the nose closes with only ~10 mm of motion at the trigger. They are V-shaped with each side ~3.5 mm thick. There are three small stripes of material spaced out (~0.08 mm thick, ~10 mm apart) to prevent deformation, giving the jaws an A-shape. 

<p align="center">
  <img src="/assets/img/Pliers drawing.png" alt="Plier Dimensions" width="400">
</p>

## Iterating
<p align="center">
  <img src="/assets/img/Plier Iterations.jpg" alt="Plier Iterations" width="400">
</p>
The first iteration (left) of the pliers was largely successful, but the dovetail joints were not functional and required glue. The dovetails were too small very fine details and a tolerance of 0.2 mm was used. This resulted in very small and loose joints that did not hold the pliers together without glue. When fully glued together, Iteration 1 worked perfectly, indicating the overall design was promising.

The second iteration (center) aimed to fix the interlocking problem. The dovetails were made larger by extending the jaws along the side of the handle so the joints could be larger and more could be used in multiple locations and directions. The dovetails on the triggers were only changed slightly due to the trigger's small size. A tolerance of only 0.05 mm was used. After printing, Iteration 2 had strong joints to the handle that held the jaws firmly as desired. The trigger joints were improved from Iteration 1, but were still not perfectly stable. During use, one of the jaws would pop out of the trigger after a few pulls when not handled carefully. 

The third iteration (right) was the final version of the pliers. The dovetails on the trigger were made as large as possible without sacrificing the integrity of the trigger. The handle dovetails on Iteration 2 were ideal, so the same tolerance of 0.05 mm was used in printing. Iteration 3 worked perfectly, with stable joints holding all parts together. It was able to pick up resistors and other small items easily and repeatedly without fail. 

## Off-the-Shelf Parts

| Part Name            | Quantity | Function                                           | Source          |
|----------------------|----------|----------------------------------------------------|-----------------|
| Arduino Uno          | 1        | Microcontroller to run pump logic and interface    | Arduino.cc / Amazon |
| A4988 Stepper Driver | 1        | Drives stepper motor with microstepping control    | Pololu / Amazon |
| NEMA 17 Stepper Motor| 1        | Rotates lead screw to move syringe plunger         | Amazon / Adafruit |
| 12V Power Supply     | 1        | Provides motor and electronics power               | Amazon |
| Lead Screw (8mm) + Nut | 1     | Converts motor rotation to linear motion           | McMaster-Carr / Amazon |
| Linear Rod (smooth)  | 1        | Prevents carriage rotation, stabilizes motion      | McMaster-Carr |
| 608ZZ Bearings       | 2        | Supports rotation of the lead screw                | Amazon |
| Limit Switch         | 1        | Detects empty syringe, stops motor                 | Amazon |
| Potentiometer (dial) | 1        | Adjusts flow rate manually                         | Amazon |
| Push Buttons         | 3        | Start/stop and manual forward/reverse control      | Amazon |
| LED (RGB or 3-color) | 1        | Status indicator (green, yellow, red)              | Amazon |
| Heat Shrink Tubing   | Assorted | Protects soldered joints from fluid exposure       | Amazon |
| Jumper Wires         | Assorted | Connects Arduino to breadboard and components      | Amazon |
| Breadboard           | 1        | Prototyping circuit connections                    | Amazon |
| Syringes (20 mL & 5 mL) | 2    | Holds and dispenses fluid at controlled rate       | Local supplier |
| Fasteners (M3 screws + nuts) | Assorted | Secures assembly parts together            | McMaster-Carr |

## Custom 3D Printed Parts

| Part Name             | Quantity | Material | Notes                            |
|------------------------|----------|----------|----------------------------------|
| Base Frame             | 1        | PLA/ABS  | Holds entire assembly            |
| Syringe Support        | 1        | PLA/ABS  | Holds syringe barrel flange      |
| Tip Support            | 1        | PLA/ABS  | Keeps syringe tip aligned        |
| Motor Mount            | 1        | PLA/ABS  | Holds stepper motor              |
| Carriage / Plunger Holder | 1     | PLA/ABS  | Moves along lead screw           |
| Enclosure w/ Sliding Lid | 1      | PLA/ABS  | Protects electronics from spills |

{% include gallery caption="PIP Pliers Gallery" %}
