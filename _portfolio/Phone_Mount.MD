---
title: "Top-Down Modelling Phone Mount Project"
excerpt: "Rotating phone mount with modular attachment created using top-down modeling"
header:
  image: /assets/img/Phone Mount Final CAD Views.png
  teaser: /assets/img/Phone Mount Final CAD Views.png
gallery:
  - image_path: assets/img/Phone Mount Final CAD Views.png
  - image_path: assets/img/Phone Mount CAD Iterations.png 
  - image_path: assets/img/Phone Mount Use.gif
---
## Top-Down Modeling
Top-down modeling is a CAD approach where the overall geometry and key relationships of the design are defined first, then each component is built from that shared framework. Instead of making parts separately, every piece references the same master sketches, planes, and dimensions, so the whole assembly stays aligned and updates automatically with changes.
For this project, this method let all components be modelled inside one controlled layout. The clamp diameter, phone thickness, and mounting geometry all came from the same parameters and referenced each other, which made iteration easier and guaranteed that every part fit together correctly once printed.

## Project Description
The assignment was to use top-down modeling to design and 3D print a phone mount for a bike handle. The mount must grip the handlebar tightly to remain secure during travel. Tools and screws can be used to mount the device to the bike, but the phone must come in and out of the holder without the need for tools. The phone must be able to rotate and snap into place in at least portrait and landscape positions without the use of tools. 

## Design 
### Rotation Mechanism
The phone mount was required to rotate and lock into at least an upright portrait and landscape position. A detent mechanism (shown below) was used to achieve this function. A detent mechanism is composed of a compression spring, a ball bearing, and a cylindrical post with semi-circular holes around the perimeter. The compression spring holds the ball bearing up to the cylinder such that it fits into the slot in a locked position. When the cylinder is rotated, the ball bearing is pushed outward until it can fit back into a slot and lock again. 
<p align="center">
  <img src="/assets/img/Detent Mechanism CAD.png" alt="Detent Mechanism" width="400">
</p>

### Phone Holder
The cylindrical portion of the detent mechanism described above is part of the phone holder component of the mount. This component is essentially a large phone case designed to fit an iPhone 15 in a thin case. It has slots for the volume and power buttons and an indent for the camera on both sides so the phone can be inserted with the holder in different positions. There is a small overhang on the top, bottom, and sides to hold the phone in place. It was filament printed in a flexible material so the phone can be easily inserted. After multiple printed iterations, no tolerance on the phone slot dimensions was used as the phone was not secured in place until the dimensions of the phone slot matched those of the phone case itself. On the back of this phone section is the cylinder portion of the detent mechanism with an hole in the center for an M5 heat sink insert. Information about the Phone Holder component can be found in the 3D Printed Parts table.
### Detent Arm
The ball bearing and spring portions of the detent mechanism is attached to the Detent Arm component. The detent arm is a rectangular block with a hole for the detent cylinder. A tolerance of 0.5 mm was used to ensure the components would fit together after filament printing. The detent block has a slot with a small post for the spring and ball bearing to fit into. Attached to the block is the arm that is inserted into the Bike Attachment. There is a hole for a M5 heat sink insert at the bottom of this arm so the Detent Arm can be screwed tightly into the Bike Attachment. The Detent Arm is printed from a rigid material to hold the Phone Holder upright. Information about the Detent Arm component can be found in the 3D Printed Parts table.
### Bike Attachment
The Bike Attachment component is a clamp with two screw lots for tightening onto the bike handlebars with nuts.This component was modeled separately from the Detent Arm to allow for the attachment to be swapped out for a new part modeled for a different part modeled to attach to something else (ex. car air vent or tripod). The Detent Arm must be inserted into the Bike Attachment component and screwed into place. A tolerance of 0.8 mm was used do the arm slot to allow room for filament printing imprecision and room for the M5 heat sink insert in the arm to fit into the slot. The Attachment part (Bike or any other future option) must be printed from a rigid but not brittle so it can be tightened around the object without cracking or snapping. Information about the Bike Attachment can be found in the 3D Printed Parts table. 
### Detent Cover
The Detent Cover is a small thin disk that attaches to the back of the mount, sandwiching the Detent Arm between itself and the Phone Holder. The Detent Cover prevents the ball bearing and spring in the detent mechanism from becoming undone. The Detent Cover was laser cut from transparent acrylic so the detent mechanism could be visible from the outside, but can be cut or printed from nearly any material. Information about the Detent Cover can be found in the 3D Printed Parts table. 

## Iterating
<p align="center">
  <img src="/assets/img/Phone Mount CAD Iterations.png" alt="Phone Mount Iterations" width="400">
</p>
The first iteration (left) of the pliers was largely successful, but the dovetail joints were not functional and required glue. The dovetails were too small very fine details and a tolerance of 0.2 mm was used. This resulted in very small and loose joints that did not hold the pliers together without glue. When fully glued together, Iteration 1 worked perfectly, indicating the overall design was promising.

The second iteration (center) aimed to fix the interlocking problem. The dovetails were made larger by extending the jaws along the side of the handle so the joints could be larger and more could be used in multiple locations and directions. The dovetails on the triggers were only changed slightly due to the trigger's small size. A tolerance of only 0.05 mm was used. After printing, Iteration 2 had strong joints to the handle that held the jaws firmly as desired. The trigger joints were improved from Iteration 1, but were still not perfectly stable. During use, one of the jaws would pop out of the trigger after a few pulls when not handled carefully. 

The third iteration (right) was the final version of the pliers. The dovetails on the trigger were made as large as possible without sacrificing the integrity of the trigger. The handle dovetails on Iteration 2 were ideal, so the same tolerance of 0.05 mm was used in printing. Iteration 3 worked perfectly, with stable joints holding all parts together. It was able to pick up resistors and other small items easily and repeatedly without fail. 

## Off-the-Shelf Parts

| Part Name              | Quantity | Function                              | Source            |
|------------------------|----------|----------------------------------------|-------------------|
| 8mm Ball Bearing       | 1        | Detent mechanism                       | McMaster-Carr     |
| 20mm Extension Spring  | 1        | Detent mechanism                       | McMaster-Carr     |
| M5 Heat Set Inserts    | 2        | For screws in detent and arm           | McMaster-Carr     |
| M5 Screws              | 4        | Detent, arm, and attachment clamp      | General / McMaster-Carr |
| M5 Nuts                | 5        | Detent arm and attachment clamp        | General / McMaster-Carr |

## Custom 3D Printed Parts

| Part Name             | Quantity | Material | Notes                            |
|------------------------|----------|----------|----------------------------------|
| Phone Holder             | 1        | TPU  | Large phone case with detent cylinder on back            |
| Detent Arm        | 1        | ABS/PETG  | Connects phone and modular attachment clamp      |
| Bike Attachment            | 1        | ABS/PETG  | Bike handlebar attachment clamp        |
| Detent Cover            | 1        | Acrylic  | Keeps spring and ball bearing in place              |


{% include gallery caption="PIP Pliers Gallery" %}
