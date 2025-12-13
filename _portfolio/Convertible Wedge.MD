---
title: "Convertible Wedge Generative Design Project"
excerpt: "Platform wedge attachment for Pashion Footwear sandal using generative design."
header:
  image: /assets/img/Fillament Wedge on Shoe.png
  teaser: /assets/img/Fillament Wedge on Shoe.png
gallery:
  - image_path: assets/img/Fillament Wedge on Shoe.png
  - image_path: assets/img/Wedge Mechanism GIF.gif 
  - image_path: assets/img/Foot Load Cell Diagram.png
  - image_path: assets/img/Weight Distribution Graphs.png
  - image_path: assets/img/Preserve Bodies.png
  - image_path: assets/img/Obstacle Bodies.png
  - image_path: assets/img/Starting Shape.png
---
## Generative Design & Powder Printing
Generative design is a computational design methodology that uses structural optimization to determine how material should be placed within a defined volume to meet performance requirements. Rather than modeling a final shape directly, the designer specifies loading conditions, boundary constraints, material behavior, and manufacturing limitations. The algorithm then evaluates a large solution space and produces geometries that efficiently carry applied loads while minimizing mass. These geometries often follow natural stress paths and result in organic, highly optimized structures that differ significantly from conventional prismatic designs.
In automotive engineering, generative design has been adopted primarily to reduce mass, consolidate assemblies, and improve structural efficiency without sacrificing strength. A notable commercial example is General Motors’ generatively designed seat belt bracket, developed using Autodesk’s generative design tools and produced via metal additive manufacturing. The redesigned bracket replaced an eight-part welded assembly with a single printed component, achieving approximately 40 percent mass reduction while maintaining required safety performance. By consolidating multiple stamped and welded parts into one optimized structure, GM reduced material usage, simplified assembly, and eliminated several failure points associated with joints and fasteners. This application demonstrates how generative design can directly improve both performance and manufacturability in a real automotive production environment.
Generative design is especially effective when paired with powder-based additive manufacturing processes, such as polymer selective laser sintering or metal powder bed fusion. These manufacturing methods can produce the complex internal geometries and curved load-bearing members that generative algorithms naturally create. When combined, generative design and powder bed manufacturing enable lightweight, structurally efficient parts that would be impractical or impossible to fabricate using traditional subtractive or forming techniques. This makes the approach well-suited for automotive components where weight, strength, and part consolidation are critical, including structural brackets, mounts, and load-bearing housings.

## Project Description
The assignment was to use generative design to optimize a part of your choosing. This project creates a platform wedge heel attachment for a pair of Pashion Footwear sandals. Pashion Footwear is a female-founded company that created fully convertible women’s shoes that can be worn as either flats or various types of heels. Pashion currently offers 3” and 4” stiletto and block heels for their shoes. This project creates a 5” heel attachment by utilizing a platform wedge to add an inch to the bottom without compromising the arc of the shoe. (attach links to Pashion)
<p align="center">
  <img src="/assets/img/Fillament Wedge on Shoe.png" alt="Fillament Printed Final Prototype" width="300">
</p>

## Design 
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811263ba9068cb14193?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
### Preserve Bodies
Preserve bodies are objects with important geometry that the generative design software is told not to alter in any way. 
<p align="center">
  <img src="/assets/img/Preserve Bodies.png" alt="CAD Preserve Bodies" width="400">
</p>
#### Mechanism
The geometry of the mechanism that connects different heel attachments to a shoe is very particular and must be kept completely faithful to the geometry of that of the commercial heels. The heel is inserted at a 90° angle and is turned towards its functional position until it clicks into place. Current Pashion heels include a release button to more securely lock the heel into place, but this was omitted in this design to comply with the assignment requirements. 
#### Base
To adhere to the assignment guidelines, only one part could be created. Because of this constraint, while indiviso heel and platform parts would likely be sufficient (and more aesthetically pleasing), a full wedge heel had to be created. The Base is a thin outline of the shape of the shoe from a top/bottom view at 5” from the heel-shoe interface, creating the bottom of a 5” wedge heel. Measurements were taken to try to match the curved outline of the shoe. 
#### Arch
As this design is a wedge heel that spans the length of the shoe, the arch of the shoe must be matched to ensure the wedge lines up with the shoe properly. The arch is the same x-y shape as the base, projected up 1” at the toe to form the platform, and curved to match the arch of the shoe in its 4” position. Measurements were also taken to match this curve.
### Obstacle Bodies
Obstacle bodies represent areas that the generative design tool cannot add material. These are represented in transparent material below so the design would still be visible. 
<p align="center">
  <img src="/assets/img/Obstacle Bodies.png" alt="CAD Obstacle Bodies" width="400">
</p>
#### Ground
The generative design tool was told not to generate any material below the Base to ensure the wedge would lie flat on the ground beneath it.
#### Foot/Shoe
The space above the Arch and surrounding the Mechanism needed to be reserved for the sandal and the user’s foot, so it was established as an obstacle geometry.  
### Starting Shape
Starting shapes are bodies that the generative design tool is free to alter. 
<p align="center">
  <img src="/assets/img/Starting Shapes.png" alt="CAD Starting Shapes" width="400">
</p>
#### Wedge
The lofted volume between the Base and Arch created the shape of the Wedge itself, which the generative design tool was free to add or remove material from to create a part that could withstand the applied load using minimal mass. 

## Forces
Generative design is only as realistic as the load cases it’s given. If insufficient loads are applied in the generative design space, the resultant part will not be able to withstand its function. For this mechanism, the goal was to represent how a real human foot loads a high-heeled shoe under regular walking conditions.
<p align="center">
  <img src="/assets/img/Applied Shoe Forces.png" alt="Applied Forces" width="300">
</p>
For a previous project, I used an array of load cells to measure my own weight distribution barefoot versus in multiple pairs of heels. The load cell setup, as well as the results of this study are below,
<p align="center">
  <img src="/assets/img/Foot Load Cell Diagram.png" alt="Load Cell Diagram" width="300">
</p>
<p align="center">
  <img src="/assets/img/Weight Distribution Graphs.png" alt="Weight Distribution Graphs" width="300">
</p>
Barefoot, the majority of my weight is on my heel, but in heels, the majority of my weight is on the ball/toe of my foot. To account for the impact from walking, the conservative estimate used was twice the body weight. The distribution applied was 60% on the toe, 15% on the arch, and 25% on the heel. There is still substantial weight on the heel in the standing study, which was accounted for using moments. 

## Generated Designs
### Aluminum ALSi10Mg Outcome
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281114564efc64ca87ca?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
The aluminum outcome produces a structure that closely matches how the wedge heel is expected to carry load during walking. Material is concentrated through the arch and heel region, where bending and torsional effects dominate, while the toe region remains relatively open. Rather than relying on solid volume, the solver forms rib-like members that follow clear load paths between the ground contact surface and the shoe interface. This creates a design that feels structurally intentional and easy to interpret.
The resulting geometry also remains manufacturable and visually coherent despite its complexity. Because of aluminum’s high stiffness, the solver is able to remove material aggressively without sacrificing structural performance, leading to a favorable stiffness-to-weight ratio. For this reason, the ALSi10Mg design was selected for printing. Its behavior under load is predictable, and the final form aligns well with both the mechanical demands of the application and the constraints imposed by the heel mechanism and shoe geometry.
### Nylon 12 Outcome 
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028117a698f46e7f35c69?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></>
The Nylon 12 outcome behaves very differently under the same constraints and loading conditions. Due to the significantly lower elastic modulus of the material, the generative solver compensates by adding substantial volume in an attempt to meet stiffness requirements. Instead of forming distinct internal load-bearing members, the geometry grows outward and around nearby obstacle bodies, resulting in a bulky and less intuitive structure.
This behavior required increasingly large obstacle volumes to prevent material from forming in unusable regions, which further restricted the solver and reduced the quality of the result. The final geometry lacks the structural clarity seen in the aluminum outcome and appears overbuilt relative to the actual loads applied. For a component that must fit tightly within a shoe and maintain a refined external form, this result is impractical both mechanically and aesthetically. While Nylon 12 is well suited for many powder-printed parts, this application highlights its limitations when stiffness, compact geometry, and controlled load paths are critical.


## Iterating
### Filament Printed Prototype
<p align="center">
  <img src="/assets/img/Fillament Wedge on Shoe.png" alt="Filament Printed Final Prototype" width="300">
The wedge prototype was filament printed from PLA. The part was largely a success, with the exception of the curves at the front of the foot. Roughly at the midpoint of the Arch, the wedge diverges from the sole, indicating that the arc and curve measurements were off. This was to be expected considering the complexity of the anatomical curves. The back of the wedge was fitted perfectly. The arch and outline of the wedge lined up closely with the sole. The mechanism also worked perfectly despite the lack of release button. As shown below, the heel twisted and locked in position just like the commercially available heels. The first prototype of the heel was filament printed using PLA. The curve on the front half of the shoe (arch and curve in the toe) was not well matched to the shoe as the wedge and sandal diverge roughly at the arch’s midpoint. The back half of the wedge fit the shoe very closely, with the arch against the sandal and the outline of the curve in the back of the foot lining up very well. The mechanism worked perfectly, smoothly locking the wedge into the sandal as shown below.
<p align="center">
  <img src="/assets/img/Wedge Mechanism GIF.gif " alt="Working Mechanism" width="300">
### Next Steps
The first prototype successfully met the assignment requirements, so future iterations will be pursued for personal use rather than academic constraints. Rather than a single continuous wedge connected at the heel mechanism, the next design will separate the system into an individual 5 inch block heel and a 1 inch toe platform. The block heel will include a flared base for stability and will be powder printed from Nylon 12.
To improve fit and comfort, a 3D scanner will be used to capture the exact curvature and contact geometry of the shoe sole. This data will allow the platform and heel interfaces to match the shoe more accurately than manual measurements. Given the relatively uniform loading and aesthetic priorities of the design, a lattice-based approach may be more appropriate than full generative design for future iterations. Lattices would allow controlled weight reduction, tunable stiffness, and a cleaner external form while simplifying the design process.
The toe platform will likely be filament printed from TPU to provide cushioning in the most heavily loaded and uncomfortable region of the shoe. A thin layer of TPU will also be attached to the bottom of the block heel to absorb impact from walking and improve durability. These changes aim to achieve the same structural performance with less material while improving comfort and wearability.
## Critique of Generative Design
Generative design is a powerful tool, but its usefulness depends heavily on the scale, function, and intent of the part. It excels in applications where loads are complex, weight reduction is critical, and the design space is large enough to allow meaningful optimization. Automotive and aerospace brackets, mounts, and structural connectors are strong examples, where part consolidation and mass savings outweigh concerns about visual complexity.
For this project, however, generative design often complicated the process more than it helped. The wedge heel is a relatively small part with a tightly constrained envelope, and much of its success depends on aesthetics and fit rather than extreme structural optimization. Defining preserve bodies, obstacle volumes, and load cases required significant iteration, and small changes in assumptions led to large shifts in the generated geometry. In this context, a traditionally designed part informed by basic structural analysis may have achieved a similar or better result with less effort and greater control over form.
Another limitation is appearance. Generative outcomes tend to prioritize structural efficiency over visual refinement, which is not always desirable for consumer-facing products like footwear. While the aluminum result was acceptable, the organic geometry produced by the solver was not inherently aligned with the design language of the shoe. This reinforces the idea that generative design is most effective when performance clearly outweighs aesthetic concerns, and less effective when visual intent plays a dominant role.

{% include gallery caption="Generative Design Wedge Prototype Gallery" %}
