---
title: "Manufacturing a longboard deck"
excerpt: "Large format 3D printing using pellet extrusion"
header:
  image:  /assets/img/Truck/Skateboard_render.jpg
  teaser:  /assets/img/Truck/Skateboard_render.jpg
gallery:
  - image_path: /assets/img/Deck/my_deck.jpg
  - image_path: /assets/img/Deck/Truck/full_board.jpg
  - image_path: /assets/img/Deck/Mini_deck.jpg
   
---
# Background

*  As a final capstone project for the additive manufacturing minor the digital fabrication lab aims to create an electric longboard to encourage the use of electric vehicles as modes of transportation. The lab aims to create a longboard that is more customizable, faster and lightweight compared to a traditional longboard by adding a digital fabrication twist to the manufacturing process. A key component of this design is the longboard deck. Thanks to our professor Dr Florian we have access to a large format 3D printer that can print a full-size longboard deck.

#Large Format 3D printer 

* **What is it?** 
  - Just as the name suggests a large format 3D printer is a large version of a filament 3D printer. Dr Florian's 3D printer has a 4’ x 4’ x 4' build volume and as such has a large nozzle, large belts, a large frame and large gantries and linear actuators. To extrude such a large volume a screw extruder that has a plastic melting capacity of 1kg/hr. To feed plastic into the 3D printer a pellet extruder uses a vacuum system to blow stored pellets into the extruder when needed. 

# Skateboard Deck Design Choices 

* **Longboard dimensions** 
  - Longboard dimensions dictate its rideability based on a board's wheelbase. This is the distance between the wheel axis’ of a board. A long wheelbase results in a large turn radius but a more stable board. Whereas a shorter wheelbase results in a smaller turn radius (better manoeuvrability) but less stability. Given the average wheelbases for different longboards a distance that would enable usage for both freestyle longboarding and downhill longboarding was chosen. This was found to be around 29” with a total board length of 43”. As such this board should be able to handle the speed that comes with an electric-powered longboard due to its length which is common for downhill high-speed longboarding. Furthermore, it should also be able to be quickly manipulated by skilled users for more intricate rides similar to the way freestyle longboards are used. Finally, for added stability at high speeds, the deck is at a width of 18” as is common for downhill longboard decks. 

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e2d8d938a1c398f1b?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

* **Sleekness and flexibility** 
  - The thickness of the board was designed such that there is some flexibility when a 200lb rider stands on the board but not enough bending that the board would feel loose to stand on. As such the design was constrained such that no more than 12mm of deformation would occur with a 200lb rider. At the same time to ensure that the board is lightweight the design was made to be sleek and thin. To improve sleekness and allow for better turning the board was designed such that there is a gap for the wheels so they do not limit the bend in the board during turns. This means riders can sit deeper in the turn improving the turning radius and maneuverability of the longboard. 
  - The board was made 16mm thick to allow for two aluminium plates to be sandwiched between the gap to which the trucks would screw in. Aluminium plates sandwiched between a square geometry were used to increase the area of contact with the plastic and reduce the compressive force. Due to the nature of filament 3D printing, compressive bolts would most likely shear along neighbouring lines of plastic formed by the printer. 
  - With the force of a 200lb rider the board deflected a maximum of 3.175mm according to Fusion’s FEA simulation. This deflection is a good amount that should allow for flexibility whilst ensuring stability. 

<img src="/assets/img/Board/Deflection.jpg" alt="Deflection" width="500" height ="200"/>

* **Handle** 
  - Finally, a handle was designed on the board to allow for easy accessibility and transportation of the board when it is being carried. The handle was designed to be 0.75” wide to provide a comfortable grip. 



# Results 

* **Prototyping** 
To model the use of the deck design and get an idea of the full longboard geometries a miniature version of the full skateboard assembly was printed on the SLA printer. The SLA printer was used for its ability to print complex parts quickly. The complete longboard was printed at 1:20 scale and based on the board geometries it was then concluded that moving on to large format printing the board was possible.  


<img src="/assets/img/Board/Mini_deck.jpg" alt="Mini Longboard" width="500" height ="200"/>

* **Deck** 
  - The board was printed on the large format 3D printer and came out just as expected. When testing the board the deflection was slightly larger than expected but it still functioned. Another design was also tested and provided less deflection. That board was then used to attach the 3D printed trucks, motor and battery to produce a fully functioning, digitally fabricated electric longboard. 

<p float="left">
  <img src="/assets/img/Board/my_deck.jpg" alt="Longboard deck" width="200" height ="200"/>
  <img src="/assets/img/Board/full_board.jpg" alt="Final Longboard" width="200" height ="200"/>
</p>

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6efc949877b2c2ac26?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


# Appendix 
**Relevant material:**  
*Details on Dr Florian’s Large Format 3D printer](https://www.youtube.com/playlist?list=PLZ9ac-f1U5V-FCBdhjv56bcvn9yc6JSfY)

*[Information on longboard deck geomerties for riding](https://stokedrideshop.com/blogs/stoked-school/what-size-longboard-should-i-get)








{% include gallery caption="Longboard Deck" %}
