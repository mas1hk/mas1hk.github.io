---
title: "Generative Design of an Electric Skateboard Truck"
excerpt: "A project testing the capabilities of generative design for performance parts."
header:
  image: /assets/img/Testing Image.jpg
  teaser: /assets/img/Device.jpg
gallery:
  - image_path: /assets/img/Baked Bad Mould.jpg
  - image_path: /assets/img/Clear Mould.jpg
  - image_path: /assets/img/Device.jpg
   
---
# Background

*  The goal of this project is to explore the capabilties of generative desing to design parts for performance. The usual process for designing performance parts requires many iterations followed by FEA to create a part that is structurally fit for an application. Generative design is a potentially more efficient way to allow a computer to automate these iterations to produce a part that fits the requirments needed. 

# Why Generative Design? 

* **What is it?** 
  - Generative Design is the process of generating a design from design criteria, loads and constraints using AI to drive exploratory iterations of a design that eventually converge to a final solution. 

* **Load Cases** 
  - Being able to apply load cases to constrain the creation of a design ensures that the part created is strong enough for a paticular application without the need of FEA (fininte element analysis) for the user. Instead, the simulation and analysis is all automated by the generative design software and used to inform further computer generated iterations. 

* **Constrain Elements** 
  - By constraining existing elements in an assembly, generative design software is then able to create a part as needed that couples to exisiting geometries and elements as defined by the user. This is the key element of generative design that the user controls and uses to define a design. A key benifit to this is that by using generative design a single part that couples many constrained objects in an assembly can be created reducing the need for complex sub-assembelies or complicated joints. 

* **Minimise material** 
  - Another key benifit of computational generative design is that further constraints like minimising material can be applied and explored by the software. Constraints like this that are in direct relation to load cases and other design elements are much harder to implement by a user as it hard to keep track of how changes in material affect other design elements. This process is perfect for computational design where the software can iterate and explore multiple designs whilst keeping track of complex relationshops between the material, constrained element and load cases. This can result in a final part that uses less material than traditional parts thus reducing material costs and manufactuing efficency.  

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6eea03d13de859ed90?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Design Features

* **Mixing channel** 
  - A literature survey reviewing microfluidic mixing methods and geometries was used to inform the design used and is linked in the appendix. It was found that out of all passive mixing methods zig-zag channels had one of the highest mixing indexes at 0.96. Based on this knowledge a zig-zag mixing geometry was created with small horizontal channels in between to encourage flow.  
* **3D mixing feature** 
  - Utilizing the SLA printer allowed for easy fabrication of 3D features to further enhance mixing. A twisting channel was created on the final straight away for the fluid to encourage some final mixing based on geometries also found in the literature survey. 

# Fabrication technique

1) **3D printed master mould** 
  - Using the SLA printer a master mold of the microfluidic channels can be printed. The print is made of clear resin and is then cured for 25 minutes at 100°C. In the mold negative spaces are extruded such that the extruded spaces are empty when a PDMS mold is created from the 3D print. 


<img src="/assets/img/Clear Mould.jpg" alt="drawing" width="200" height ="200"/> 
<figcaption>Clear 3D printed mould.</figcaption>

  
2) **Paralene Deposition and PDMS** 
  - The master mould can then be used to create microfluidic devices with the exact geometries required. Originally, the PDMS was added in a 10:1 ratio with a curing agent directly into the master mould. However, it was found that the PDMS did not cure this way. Instead, Parleyene was deposited onto the surface of the master mould using the Labcoter PDS 2010 parylene deposition machine. An explanation of these issues is provided in the improvements section. After this PDMS could be added in 10:1 ratio with a curing solution to produce plastic microfluidic devices that are compatible with cell cultures. 


<img src="/assets/img/Baked Bad Mould.jpg" alt="drawing" width="200" height ="200"/>  
<figcaption>Over sintered mould.</figcaption>


3) **Bonding to Glass Plate** 
  - Finally, the bottom layer of the PDMS plastic is bonded to a glass plate to close the channels. This was done using the PlasmaFlo PDC-FMG plasma cleaner. 


<img src="/assets/img/Device.jpg" alt="drawing" width="200" height ="200"/>  
<figcaption>Final PDMS device bonded to glass plate.</figcaption>
 

# Testing
* **Good News or Bad News**  
  - It was found that the microfluidic device initially mixed a solution of blue and pink solution producing a purple solution. However, the small channel lengths meant the pressure within the channels was large resulting in the glass and PDMS splitting. 

 <iframe width="560" height="315" src="https://www.youtube.com/embed/d6joNObLwHE?si=FpuUn_DfC15Lp6tX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


# Improvements

* **SLA Fabrication isn’t perfect** 
  - SLA printing uses resins that contain photoinitiators that form free radicals which are very chemically reactive. As such there have been issues with creating mixing devices from the 3D mold due to PDMS not curing and adhesion to the 3D printed master mold. Two solutions were attempted in this project. 
* **Curing 3D printed parts**
  - The first solution attempted was based on the literature linked below. The theory is that after curing at 120°C for one hour the uncured monomers containing photoinitiators should have cured. Thus rendering the resin-printed master mold unreactive with the PDMS allowing it to cure. Unfortunately, this technique resulted in large warping due to cross-linking and the PDMS still did not cure.
* **Curing 3D printed parts** 
  - The second approach was from a different research paper where a thin (nm) layer of paralene is used to coat the mold rendering it unreactive and biocompatible. This technique produced a PDMS microfluidic device from the master mould. 
* **Glass Bonding** 
  - In further testing, the bond between the glass and PDMS must be improved to allow the glass to withstand the pressure produced to liquid flow within the microfluidic channels. 



# Appendix 
**Relevant papers:**  
*[Microfluidic Mixing: A Review. Int J Mol Sci.12(5): 3263–3287](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3116190/)

*[Rapid prototyping of cell culture microdevices using parylene-coated 3D prints Lab Chip, 2021, 21, 4814-4822](https://pubs.rsc.org/en/content/articlelanding/2021/lc/d1lc00744k)

*[PDMS Curing Inhibition on 3D-Printed Molds: Why? Also, How to Avoid It? Bastien Venzac, Shanliang Deng, Ziad Mahmoud, Aufried Lenferink, Aurélie Costa, Fabrice Bray, Cees Otto, Christian Rolando, and Séverine Le Gac, Analytical Chemistry 2021](https://pubs.acs.org/doi/10.1021/acs.analchem.0c04944)







{% include gallery caption="MicroFluidic Gallery" %}



