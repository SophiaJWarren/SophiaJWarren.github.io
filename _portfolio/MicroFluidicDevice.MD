---
title: "Microfluidic Device Project"
excerpt: "3D printed & casted pinch flow fractionation microfluidic device for particle sorting."
header:
  image: /assets/img/SyringePump2.jpg
  teaser: /assets/img/SyringePump2.jpg
gallery:
  - image_path: assets/img/SyringePumpSupport.png
  - image_path: assets/img/SyringePumpcarriage.png
  - image_path: assets/img/SyringePumpTip.png
   
---
## Introduction
Pinched flow fractionation (PFF) is a microfluidic technique that continuously separates particles by size. A PFF device first channels a mixture of particles suspended in liquid into a pinched channel section. As the pinched channel opens to a wider section, the particles separate based on size due to buoyancy force and are collected through different outlet channels placed on their calculated heights.


## Design
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4bd6edd15c0531c07?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Instructions
 1. Extend the carriage
 2. Simulnt

## Discussion
* Automated: Controlled by Arduino with adjustable flow rate
* Versatile: Su

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
