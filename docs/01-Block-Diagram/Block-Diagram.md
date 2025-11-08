---
title: Individual Block Diagram
tags:
- tag1
- tag2
---

## Overview
This block diagram shows a motion sensor powered by a 5V, 1.5A voltage regulator, which powers all the components. The motion sensor sends a signal that is filtered by the Op Amp to the microcontroller. The microcontroller reads the sensor through an analog input, and if motion is detected, it sends a digital signal to Riley’s board through pin 2. The board then activates a motor to open the trash can lid. This has changed.

This new block diagram now supports two IR Reflective Optical Sensors, still powered by a 5V, 1.5A voltage regulator, which powers all the components. One of the sensors is constantly detecting for motion while the other sensor is measuring how much depth there is in the trashcan. These signals are filtered by the Op Amp and then sent to the microcontroller to be translated into a digital signal. That signal is then sent to two other microcontrollers to open the can or impact an LED scale. 


OLD: 
<img width="460" height="324" alt="Screenshot 2025-10-27 at 10 54 55 AM" src="https://github.com/user-attachments/assets/7afa1fee-9589-4730-bd32-1db610e3148d" />

NEW:
<img width="463" height="487" alt="Screenshot 2025-11-08 at 4 48 38 PM" src="https://github.com/user-attachments/assets/12691c81-5f2d-4104-8c8d-2a8738e4e682" />


NEW PDF available [here](https://github.com/user-attachments/files/23435107/IND_Block_Diagram_FINAL.drawio.pdf)

