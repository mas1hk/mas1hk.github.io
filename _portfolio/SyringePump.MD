---
title: "Automated Syringe Pump Project"
excerpt: "A syringe pump that automatically pushes liquid at a user-specified flow rate."
header:
  image: /assets/img/image10.png
  teaser: /assets/img/image11.png
gallery:
  - image_path: assets/img/image10.png
  - image_path: assets/img/image11.png
  - image_path: assets/img/image8.png
  - image_path: assets/img/image9.png
   
---

# Features

* **20 mL and and 5 mL syringe holder** The device is able to hold two types of syringes- either a 20 mL syringe or 5 mL syringe.
* **3D printed enclosure** The device has a 3D printed enclosure to protect against water damage and exposure to electrical equipment. All the electronics are housed in this enclosure and can be accessed by unscrewing two bolts. 
* **Automated flow rate** The flow rate of the device can be changed by changing the variable "flowrate". A single button is then used to control the device and the state of the device is indicated by an LED. When the device is running the LED is green, and the button can be pressed again to pause the device which is indicated by the LED turning amber. Finally, if all liquid is expelled a switch is hit stopping the motor from driving further and turning the LED red. 

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

{% include gallery caption="Automated Syringe Pump Gallery" %}

