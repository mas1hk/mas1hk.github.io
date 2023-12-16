---
title: "Generative Design of an Electric Skateboard Truck"
excerpt: "A project testing the capabilities of generative design for performance parts."
header:
  image: /assets/img/Truck/Truck_render.jpg
  teaser: /assets/img/Truck/Truck_render.jpg
gallery:
  - image_path: /assets/img/Truck/Skateboard_render.jpg
  - image_path: /assets/img/Truck/Truck_render.jpg
  - image_path: /assets/img/Truck_print.jpg
   
---
# Background

*  As a final capstone project for the additive manufacturing minor the digital fabrication lab aims to create an electric longboard to encourage the use of electric vehicles as modes of transportation. The lab aims to create a longboard that is more customizable, faster and lightweight compared to a traditional longboard by adding a digital fabrication twist to the manufacturing process. A key component of a skateboard is the skateboard truck. Traditional trucks are made from metal and pair to the skateboard through a ball joint and a flexible insert.
*  The goal of this project is to explore the capabilities of generative design to design parts a  performance longboard truck that can mount a motor and has a lightweight geometry. The usual process for designing performance parts requires many iterations followed by FEA to create a part that is structurally fit for an application. Generative design is a potentially more efficient way to allow a computer to automate these iterations to produce a part that fits the requirements needed. 

# Why Generative Design? 

* **What is it?** 
  - Generative Design is the process of generating a design from design criteria, loads and constraints using AI to drive exploratory iterations of a design that eventually converge to a final solution. 

* **Load Cases** 
  - Being able to apply load cases to constrain the creation of a design ensures that the part created is strong enough for a particular application without the need for FEA (finite element analysis) for the user. Instead, the simulation and analysis are all automated by the generative design software and used to inform further computer-generated iterations. 

* **Constrain Elements** 
  - By constraining existing elements in an assembly, generative design software is then able to create a part as needed that couples to existing geometries and elements as defined by the user. This is the key element of generative design that the user controls and uses to define a design. A key benefit to this is that by using generative design a single part that couples many constrained objects in an assembly can be created reducing the need for complex sub-assemblies or complicated joints. 

* **Minimise material** 
  - Another key benefit of computational generative design is that further constraints like minimising material can be applied and explored by the software. Constraints like this that are in direct relation to load cases and other design elements are much harder to implement by a user as it is hard to keep track of how changes in material affect other design elements. This process is perfect for a computational design where the software can iterate and explore multiple designs whilst keeping track of complex relationships between the material, constrained element and load cases. This can result in a final part that uses less material than traditional parts thus reducing material costs and manufacturing efficiency. 

# Skateboard Truck Design Choices 

* **Load Cases** 
  - There are 3 main load cases to consider with the design of the skateboard truck. First is the weight of the board and the user on top of the skateboard. This force would most likely be disturbed down across the centre rod that connects the truck to the two wheels. Given a rider weight of 200lbs with a safety factor of 2 the total load used to model was 400lbs . The second load case to consider is the horizontal force transferred through the truck from the wheels when a rider hits a curb or something else in the horizontal plane. The impulse of this force was estimated to be around 100 lbs on each side.  Finally, there is the load case due to the torque of the motor acting as it drives the wheel. This is modelled as a moment arm about the motor axis. The maximum moment was estimated to be around 200 N*m given the torque rating of the motor. 

* **Constrain Elements** 
  - The truck is designed to join the wheels to the board through a few components. First, there is the part of the truck that mounts to the board. This is a preexisting part that has a circular ball and  socket joint that allows the board to rotate left and right for turning. There is a second point of joining between this skateboard mount and the truck where the truck is sandwiched between two flexible joints to provide stability by restricting motion. Furthermore, there are wheels which connect via a metal rod such that they remain in line with one another. Finally, there is the motor which drives a single wheel as is standard with electric skateboards. Driving the single wheel actuates motion in the remaining 3 wheels when the board is on the ground. 

<img src="/assets/img/Truck/Annoated assmebly without truck.jpg" alt="Annotated Assembly" width="400" height ="300"/>

* **Motor mounting and minimising material** 
  - A key element in designing the truck was correctly positioning the motor such that the pulley is taught between the motor and wheels. Furthermore, the motor must be positioned such that when the board bends to turn it will not collide with the motor. As such a pulley calculator was used to find the exact horizontal distance between the two wheels since the motor belt length was known to be 285mm and both pulleys have a 5mm pitch and known number of teeth so the wheel diameter can be calculated. To ensure that the board doesn’t collide with the motor the motor is positioned such that it’s center is halfway between the underside of the deck and the bottom of the wheels. 
  - Based on the positioning of the key elements of the sub-assmebly. Objects were created such that when the design of the truck was created geometries like the rod,  ball and socket joint and motor face are preserved whilst other objects like the motor body, wheels and flexible truck inserts were classified as objects to ensure the design did not interfere with these parts. Then with these geomerties outlined generative design software was used to create a design that joined the components given the load cases using the minimum amount of mass. 


# Results 

* **Two designs produceded** 
  - Using generative design two designs were produced. One out of Nylon-12 and the other out of aluminium. Both of these designs are shown below. Due to the material properties of Nylon 12 the mass of material required was much larger given the load cases applied and the design created would not be a suitable truck due to the size and material requirments required to deal with the load cases. As such the Nylon-12 design was not used in the creation of the skateboard and based on the generative design it is assumed that Nylon-12 is not a suitable material to create a skateboard truck out of. 

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e473f5ee3060bc62e?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6eb0e6e979ebeb3e13?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

* **Manufacturing (how do you make a part that looks like this?)** 
  -  As shown in the CAD Models above both designs are very unique and organic. As such it is very hard to create parts like this using traditional manufacturing methods. This is where digital fabrication comes into play. Utilsing SLS (selective laser sintering) powder bed fusion complex, organic parts can be manufactured with istropic material properties. Nylon-12 is the polymer used in this process and there is the drawback that this material is not as strong as traditional aluminium however it allows for the manufacturing of much more complex parts. 
  -  For the final creation of the truck alumiium will be used as it requires less material and is thus more lightweight. However, due to the organic nature of the design the part will be sent to a manufacturer to either metal print or create through an extensive machining process. 

<img src="assets/img/Truck/Truck_render.jpg" width="350" height ="350"/>

* **Load Cycles** 
  - The SLS printed version of the alumiium truck was tested as a proof of concept. All geometries fit as required thus the truck worked functionality to join all components of the board. However, after 5 repeated  test cycles of inserting and removing the truck the ball joint eventually snapped. This is due to the rigidity of the part and the fact that the truck requires some flexibility to fit into the socket and elastic joint. This was unknown at the time of the design so further iterations would need to be to allow for some flexibility. 

<img src="assets/img/Truck/truck_print.jpg" width="350" height ="350"/>

# Generative Design in the automotive industry

* **Hamilton an 8-time F1 champ** 
  - Since computational design can be used to minimise the mass of parts with extreme efficiency it is something that is becoming increasingly to use in industry. When performance parts are needed weight is often a big consideration espceicallyt in the automotive and aerospace industries where vehicle weight makes a big difference to it’s efficiency. In formula 1, as teams compete to create the most lightweight Mercedes have started to work with autodesk to use generative design to create parts that are more lightweight. 
* **Toyota on top** 
  - Creating parts that are more lightweight isnt the only use case for this sort of technology and companies like Toyota have used autodesks generative design to create thinner car seat frames to create more space within the vehicle to improve comfortabltiltiy. As AI continues to evolve the number of potential applications of this technology and it’s efficiency will continue to improve. As such it is important that manufacturing methods also evolve so that complex parts can be created.  




# Appendix 
**Relevant papers:**  
*[Generative Design for Formula 1 Car Design](https://www.autodesk.com/autodesk-university/content/generative-design-for-formula-1-car-design)

*[Toyota Generative Design - Generative design in manufacturing is transforming the industry](https://www.autodesk.com/design-make/articles/generative-design-in-manufacturing)








{% include gallery caption="MicroFluidic Gallery" %}



