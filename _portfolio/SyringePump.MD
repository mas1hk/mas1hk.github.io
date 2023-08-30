---
title: "Automated Syringe Pump Project"
excerpt: "A syringe pump that automatically pushes liquid at a user-specified flow rate."
header:
  image: /assets/img/image12.jpg
  teaser: /assets/img/image11.png
gallery:
  - image_path: assets/img/image11.png
  - image_path: assets/img/image8.png
  - image_path: assets/img/image9.jpg
   
---

# Features

* **20 mL and and 5 mL syringe holder** The device is able to hold two types of syringes- either a 20 mL syringe or a 5 mL syringe.
* **3D printed enclosure** The device has a 3D printed enclosure to protect against water damage and exposure to electrical equipment. All the electronics are housed in this enclosure and can be accessed by unscrewing two bolts. 
* **Automated flow rate** The device's flow rate can be changed by changing the variable "flowrate" in the [Arduino code](https://github.com/mas1hk/mas1hk.github.io/blob/main/arduinocode)

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH35dfcQT936092f0e4320bbce97815dc8f2?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Part List

| Off-the-shelf    | 3D Printed              |
| ---------------- | ----------------------- |
| LED              | Enclosure Base          |
| Switch           | Enclosure Top           |
| Adruino board    | Syringe Barrel support  |
| DC motor         | Syringe plunger support |
| 8mm lead screw   | Motor Mount             |
| Flexible Coupler |                         |
| Linear Bearing   |                         |
| 3mm Screws       |                         |
| 5mm Screws       |                         |

# How to Operate 

* Fill the syringe with the desired amount of fluid. 
* Place the syringe in the device with the plunger wound so it is as close to the motor as possible.
* A single button is then used to control the device and the state of the device is indicated by an LED. When the button is pressed the device will run and the LED will turn green, and the button can be pressed again to pause the device which is indicated by the LED turning amber. Finally, if all liquid is expelled a switch is hit stopping the motor from driving further and turning the LED red.



{% include gallery caption="Automated Syringe Pump Gallery" %}

