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
<p float="left">
  <img src="/assets/img/Phone Mount CAD.png" width="45%" />
  <img src="/assets/img/Phone Mount Back CAD.png" width="45%" />
</p>
## Project Description
The assignment was to use top-down modeling to design and 3D print a phone mount for a bike handle. The mount must grip the handlebar tightly to remain secure during travel. Tools and screws can be used to mount the device to the bike, but the phone must come in and out of the holder without the need for tools. The phone must be able to rotate and snap into place in at least portrait and landscape positions without the use of tools. 
<p align="center">
  <img src="/assets/img/Phone Mount Use.gif" alt="Detent Mechanism" width="300">
</p>

## Design 
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281129ad2b80fb82f453?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Rotation Mechanism
The phone mount was required to rotate and lock into at least an upright portrait and landscape position. A detent mechanism (shown below) was used to achieve this function. A detent mechanism is composed of a compression spring, a ball bearing, and a cylindrical post with semi-circular holes around the perimeter. The compression spring holds the ball bearing up to the cylinder such that it fits into the slot in a locked position. When the cylinder is rotated, the ball bearing is pushed outward until it can fit back into a slot and lock again. 
<p float="left">
  <img src="/assets/img/Detent Mechanism CAD.png" width="45%" />
  <img src="/assets/img/Detent Mechanism Closeup.gif" width="45%" />
</p>


### Phone Holder
The cylindrical portion of the detent mechanism described above is part of the phone holder component of the mount. This component is essentially a large phone case designed to fit an iPhone 15 in a thin case. It has slots for the volume and power buttons and an indent for the camera on both sides so the phone can be inserted with the holder in different positions. There is a small overhang on the top, bottom, and sides to hold the phone in place. It was filament printed in a flexible material so the phone can be easily inserted. After multiple printed iterations, no tolerance on the phone slot dimensions was used as the phone was not secured in place until the dimensions of the phone slot matched those of the phone case itself. On the back of this phone section is the cylinder portion of the detent mechanism with an hole in the center for an M5 heat set insert. Information about the Phone Holder component can be found in the 3D Printed Parts table.
### Detent Arm
The ball bearing and spring portions of the detent mechanism is attached to the Detent Arm component. The detent arm is a rectangular block with a hole for the detent cylinder. A tolerance of 0.5 mm was used to ensure the components would fit together after filament printing. The detent block has a slot with a small post for the spring and ball bearing to fit into. Attached to the block is the arm that is inserted into the Bike Attachment. There is a hole for a M5 heat set insert at the bottom of this arm so the Detent Arm can be screwed tightly into the Bike Attachment. The Detent Arm is printed from a rigid material to hold the Phone Holder upright. Information about the Detent Arm component can be found in the 3D Printed Parts table.
### Bike Attachment
The Bike Attachment component is a clamp with two screw lots for tightening onto the bike handlebars with nuts.This component was modeled separately from the Detent Arm to allow for the attachment to be swapped out for a new part modeled for a different part modeled to attach to something else (ex. car air vent or tripod). The Detent Arm must be inserted into the Bike Attachment component and screwed into place. A tolerance of 0.8 mm was used do the arm slot to allow room for filament printing imprecision and room for the M5 heat set insert in the arm to fit into the slot. The Attachment part (Bike or any other future option) must be printed from a rigid but not brittle so it can be tightened around the object without cracking or snapping. Information about the Bike Attachment can be found in the 3D Printed Parts table.  
### Detent Cover
The Detent Cover is a small thin disk that attaches to the back of the mount, sandwiching the Detent Arm between itself and the Phone Holder. The Detent Cover prevents the ball bearing and spring in the detent mechanism from becoming undone. The Detent Cover was laser cut from transparent acrylic so the detent mechanism could be visible from the outside, but can be cut or printed from nearly any material. Information about the Detent Cover can be found in the 3D Printed Parts table. 

## Iterating
<p align="center">
  <img src="/assets/img/Phone Mount CAD Iterations.png" alt="Phone Mount Iterations" width="400">
</p>
Version 1 of the Phone Mount was a good proof-of-concept prototype. The detent mechanism worked perfectly, and all of the 3D printed parts fit together well. The Phone Holder tolerances were too large and there were no slots for the buttons, so the phone was not held in securely. The Phone Holder and Detent Arm were bulkier than necessary, wasting material. The first iteration of the arm and attachment slot had a circular cross-section. The arm was short, so the Bike Attachment interfered with the Phone Holder when rotating. 

Version 2 improved significantly on the first iteration and clearly displayed the issues to be addressed for the next iteration. The Phone Holder fit the phone more snugly and had some overhang to keep the phone in and slots for buttons, but the grip was still not tight enough and the button locations were off. The Phone Holder’s phone case and detent portions and the Detent Arm were all made slimmer, but the phone case section could still be less bulky. The arm was made longer to allow for free rotation. When inserting the M5 heat set insert into the arm, it became clear that the insert was too large to fit into the arm slot of the Bike Attachment. 

Version 3 was the final iteration of the Phone Mount as it resolved all of the issues in Versions 1 and 2. The Phone Holder was made slimmer and tighter, the overhang was made larger, the button slots were shifted, and indents for the camera were added. The phone and phone case were held securely in the Phone Holder. The arm cross-section was changed from circular to square, and the tolerance in the slot in the Bike Attachment was increased to fit the heat set insert. The fillets on the Bike Attachment were also removed to make the removal of support material easier. 

## Assembly
 1. Insert M5 heat set inserts into the detent cylinder on the Phone Holder and Detent Arm
 2. Insert Detent Arm into Bike Attachment and tighten with M5 screw and nut
 3. Place Detent Arm around the detent cylinder on the Phone Holder
 4. Place spring and ball bearing inside detent assembly
 5. Place Detent Cover on top of Detent ARm-Phone Holder Assembly and screw together
 6. Slide Bike Attachment onto handlebars and tighten using M5 screws and nuts
 7. Insert phone into Phone Holder


## Off-the-Shelf Parts

| Part Name              | Quantity | Function                              | Source            |
|------------------------|----------|----------------------------------------|-------------------|
| 8mm Ball Bearing       | 1        | Detent mechanism                       | McMaster-Carr     |
| 20mm Extension Spring  | 1        | Detent mechanism                       | McMaster-Carr     |
| M5 Heat Set Inserts    | 2        | For screws in detent and arm           | McMaster-Carr     |
| M5 Screws              | 4        | Detent, arm, and attachment clamp      | General / McMaster-Carr |
| M5 Nuts                | 5        | Detent arm and attachment clamp        | General / McMaster-Carr |

## Custom 3D Printed Parts

| Part             | Name | Material | Notes                            |
|------------------------|----------|----------|----------------------------------|
|  <img src="/assets/img/Phone Holder Iso.png" width="100"> | Phone Holder        | TPU  | Large phone case with detent cylinder on back            |
|  <img src="/assets/img/Mount Arm Iso.png" width="100"> | Detent Arm        | ABS/PETG  | Connects phone and modular attachment clamp      |
|  <img src="/assets/img/Bike Attachment Iso.png" width="100">  | Bike Attachment        | ABS/PETG  | Bike handlebar attachment clamp        |
|  <img src="/assets/img/Detent Cover Iso.png" width="100">  | Detent Cover        | Acrylic  | Keeps spring and ball bearing in place              |


{% include gallery caption="PIP Pliers Gallery" %}
