---
title: "Flexible Pliers"
excerpt: "A project to test multi-material printing and adding custom G-code commands."
header:
  image: /assets/img/IMG_4090.jpeg
  teaser: /assets/img/IMG_4090.jpeg
gallery:
  - image_path: /assets/img/IMG_4090.jpeg
  - image_path: /assets/img/IMG_4089.jpeg
  - image_path: /assets/img/IMG_4088.jpeg
   
---
# Background

*  The goal of this project was to explore multi-material 3D printing to improve the functionality of 3D printed prototypes. To do this I created a pair of flexible pliers where the spring component that allows a plier to close was created from a flexible plastic embedded within the pliers. The function of these pliers is to make it easier to hold a resistor when placing components or soldering in places where a soldering mount can't be placed.  

*  Dual extrusion multi-material printing is the most trivial method to achieve this, however, it has its drawbacks due to material or extruder swapping. Dual extrusion increases print times, increases the likelihood of a jam occurring and increases the amount of waste material. Furthermore, there is a large restriction on the materials that can be dual extruded as they must have similar chemical composition (specifically in terms of their intermolecular forces) and similar shrinking/cooling rates. For example, PLA and ABS can't be printed via dual extrusion.  

*  Due to these drawbacks, I decided it was better to create the multi-material flexible pliers by editing the G-code of my print to allow me to stop the print halfway through and embed the flexible component made of TPU. Pictures of the paused print and placement on the embedded TPU piece are shown below. The body of the pliers (handle and pincers) was made of PLA as it is cheap and strong enough to hold a resistor.  


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e1fe92f7086d7a4e4?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Design Features

* **Flexible TPU joint** TPU was used to create the flexible piece that allows the pincers to close. The TPU joint was created in a diagonal, cross-hatched shape to maximise tension. TPU has a higher elasticity under tension than compression hence a diagonal shape was chosen. This way when the handles are squeezed the handles stretch the TPU causing the pincers to close.  
* **Plier Body** The plier body was composed of 4 separate parts: 2 pincers and 2 legs. The legs have an ergonomic design for comfortable gripping and the pincers have a separation of 10mm to allow enough clearance to grab a resistor.
* **Improvements** The plier performed well when a load was applied to the legs to close them. The plier was able to hold weights of around 250g when the weight was held parallel to the pliers. However, although the clearance of 10mm is enough to pick up a resistor it is a little small to comfortably grab without worrying about accuracy.  Furthermore, if a load is applied perpendicularly to the face of the pliers, the flexible centre folds in on it's self causing the pincers to shear. This lack of rigidness and pincer opening could be improved in a further iteration. 




{% include gallery caption="Flexible Pliers Gallery" %}

