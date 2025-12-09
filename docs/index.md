---
title: Welcome
tags:
- tag1
- tag2
---
<center>
<font size= "6">Hattie Lee Datasheet</font><br>
as part of<br>
<font size= "8"> Trash Canner</font><br>
for<br>
<font size= "5"> Team 207 </font><br>

**Submission: 12, 8, 2025**
</center>

![IMG_4947](https://github.com/user-attachments/assets/bf518089-10ca-4c1e-86f3-14db712dc9c5)

## Introduction

This datasheet documents my individual contribution to the Trash Canner Project. It includes the following: my Block Diagram, Component Selection, Bill of Materials, Schematic, Power Budget, PCB Design, Microcontroller Code, Hardware V2.0, Resources and Appendix.

### Project Summary

The Trash Canner Project is an automatic trash can design featuring weight, distance, and motion sensors. Through the process of benchmarking and drafting, our team identified these features as the most effective and feasible. For a more in depth look into Trash Canner, the team's documentation is available [here](https://asu-egr304-2025-f-207.github.io/). The weight sensors are linked to LEDs, providing a clear visual alert to the user when the trash needs to be taken out. The primary objective is to assist the buyer in their daily lives by simplifying a chore. 

### My Contribution

My contribution was to design the motion and distance sensor system that triggers the trash can lid to open without using a pedal or any other manual way. This system utilizes two OPB732 emitter and detector sensors to detect the user and determine the level of trash in the can. Once the user is detected, my system sends a signal to another system’s microcontroller, which then sends information to a motor. This causes the lid to open and then close after a short time. The distance sensor sends a signal to a different microcontroller, informing the buyer when the trash can is full. You can see the full system in the [Block Diagram](https://jhlee59.github.io/01-Block-Diagram/Block-Diagram/) and the [Schematic](https://jhlee59.github.io/04-Schematic/schematic/) for details.
I had to select all the necessary parts for this sensor system, which are detailed in the [Component Selection](https://jhlee59.github.io/02-Component-Selection/Component-Selection/) list and [BOM](https://jhlee59.github.io/03-BOM/BOM/). The [Power Budget](https://jhlee59.github.io/05-Power-Budget/Power-Budget/) ensures that all components, including the sensors, op-amp, and microcontroller, operate safely on the 5V rail from the L7805ABV voltage regulator.
Currently, both sensors are mounted on a single [PCB](https://jhlee59.github.io/06-PCB%20Design/PCB%20Design/). The [Microcontroller Code](https://jhlee59.github.io/07-Microcontroller%20Code/Microcontroller%20Code/) reads the signals from the sensors, triggers the motor, and updates the fullness notification for the user. While the current design works well, in the [future](https://jhlee59.github.io/08-Hardware%20V2.0/Hardware%20V2.0/) I would consider separating the sensors onto two PCBs to make wiring simpler and signals cleaner. Additional details about my design process, testing, and references are available in the [Resources](https://jhlee59.github.io/09-Resources/Resources/) section, and supporting documents can be found in the [Appendix](https://jhlee59.github.io/Appendix/Appendix/).

