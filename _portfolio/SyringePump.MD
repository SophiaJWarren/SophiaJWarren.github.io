---
title: "Syringe Pump"
excerpt: "DIY syringe pump capable of 1 uL per minute flow rate up to 10 mL per minute."
header:
  image: /assets/img/SyringePump2.jpg
  teaser: /assets/img/SyringePump2.jpg
gallery:
  - image_path: assets/img/SyringePumpSupport.png
  - image_path: assets/img/SyringePumpcarriage.png
  - image_path: assets/img/SyringePumpTip.png
   
---
## Features
* Automated: Controlled by Arduino with adjustable flow rate
* Versatile: Supports multiple syringe sizes (5 mL and 20 mL).
* Motor Driven: Stepper motor + lead screw drive for precise dispensing.
* LED Indication: Green = running, ellow = paused, red = empty.
* Compact: All wiring is included in a small housing below the linear actuator. 
* Safety features: spill-resistant enclosure, finger intrusion prevention, & limit switch to prevent motor damage.
* Easy to disassemble and maintain.

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4bd6edd15c0531c07?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Operating Instructions
 1. Extend the carriage
 2. Simultaneously, lower the full syringe while adjusting the distance of the Flange Holder
 (carriage) to fit
 3. Slowly lower the syringe to fit into the Flange Holder, make sure plunger is inserted into
 the Plunger Holder
 4. Double check tip is resting in the Tip Support Groove
 5. Adjust desired flow rate suing dial or enter value in Program
 6. Automated Use
   a. Adjust desired flow rate
   b. Hit Red Button with silver Casing
 7. Manual use
   a. Hit third button for forward movement
   b. Hit fourth button for backwards movement

## Off-the-Shelf Parts
| Part Name              | Quantity | Source/Notes                         |
|-------------------------|----------|--------------------------------------|
| Arduino Uno (or Nano)   | 1        | Arduino.cc / Amazon                  |
| NEMA 17 Stepper Motor   | 1        | Common 3D printer motor              |
| A4988 Stepper Driver    | 1        | Amazon / Pololu                      |
| Lead Screw + Nut (4 mm) | 1        | Matches your calculations            |
| Linear Rod (support)    | 1        | Hardware store or 3D printer parts   |
| Limit Switch            | 1        | Generic mechanical switch            |
| Push Buttons            | 3        | Forward, Reverse, Start/Stop         |
| Potentiometer           | 1        | For flow rate control                |
| RGB LED                 | 1        | Status indication (R/Y/G)            |
| Power Supply (12 V DC)  | 1        | For motor                            |
| Syringe (5 mL, 20 mL)   | 2        | Lab supply or pharmacy               |
| Screws & Nuts (M3/M4)   | Many     | Hardware store                       |

## Off-the-Shelf Parts
| Part Name             | Quantity | Material | Notes                            |
|------------------------|----------|----------|----------------------------------|
| Base Frame             | 1        | PLA/ABS  | Holds entire assembly            |
| Syringe Support        | 1        | PLA/ABS  | Holds syringe barrel flange      |
| Tip Support            | 1        | PLA/ABS  | Keeps syringe tip aligned        |
| Motor Mount            | 1        | PLA/ABS  | Holds stepper motor              |
| Carriage / Plunger Holder | 1     | PLA/ABS  | Moves along lead screw           |
| Enclosure w/ Sliding Lid | 1      | PLA/ABS  | Protects electronics from spills |

## Code
 https://github.com/SophiaJWarren/SyringePumpProject/blob/main/Syringe_Pump_Code.ino

{% include gallery caption="Syringe Pump Gallery" %}
