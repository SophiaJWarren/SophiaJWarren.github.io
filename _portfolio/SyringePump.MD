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
 6. For Automated Use:
    a. Adjust desired flow rate
    b. Hit Red Button with silver Casing

 7. For Manual use:
    a. Hit third button for forward movement
    b. Hit fourth button for backwards movement

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

## Code
[View Arduino Code (.ino)] (https://github.com/SophiaJWarren/SyringePumpProject/blob/main/Syringe_Pump_Code.ino)

{% include gallery caption="Syringe Pump Gallery" %}
