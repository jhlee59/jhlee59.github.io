---
title: Individual Block Diagram
tags:
- tag1
- tag2
---

## Overview
  This new block diagram now supports two IR Reflective Optical Sensors, still powered by a 5V, 1.5A voltage regulator, which powers all the components. One of the sensors is constantly detecting for motion while the other sensor is measuring how much depth there is in the trashcan. These sensors directly support our product requirements by allowing the can to open only when the user wants to throw garbage away and by detecting when the trash is nearing maximum capacity. These signals are filtered by the Op Amp and then sent to the microcontroller, where they are translated into a digital signal. 
  That signal is then sent to two other microcontrollers to open the can or impact an LED scale—one to Riley's board and one to Gael’s. This satisfies our requirements for automatic lid opening, fullness detection, and notifying the user when the can is full. The updated block diagram represents our current design and hardware layout, reflects our team composition, and incorporates feedback by clearly separating motion sensing and depth sensing into two different sensor paths with two different outputs.


OLD: 
<img width="460" height="324" alt="Screenshot 2025-10-27 at 10 54 55 AM" src="https://github.com/user-attachments/assets/7afa1fee-9589-4730-bd32-1db610e3148d" />

NEW:
<img width="1025" height="839" alt="Screenshot 2025-12-06 at 4 25 53 PM" src="https://github.com/user-attachments/assets/51301842-99ce-4d27-a5ff-eab36bee9b09" />


New Block diagram PDF available [here](https://github.com/user-attachments/files/24003773/Lee_IND_BLOCK.drawio.pdf)

Zipped File of Block Diagram Temple: [here](https://github.com/user-attachments/files/24026617/In_temple.drawio.png.zip)



## Connection Table

| Pin | From                 | To                    | Type            | Description |
|-----|-----------------------|------------------------|------------------|-------------|
| 1   | -                     | -                      | -                | not used    |
| 2   | Hattie (Me) (RB2)     | Riley (RA2)            | 0V / 5V Digital  | Motion            |
| 3   | Hattie (Me) (RD3)     | Gael (RE0)             | 0V / 5V Digital  | Distance            |
| 4   | Gael (RF1)            | Alessandro (RA2)       | 0V / 5V Digital  | Speaker            |
| 5   | -                     | -                      | -                | not used    |
| 6   | -                     | -                      | -                | not used    |
| 7   | -                     | -                      | -                | not used    |
| 8   | Ground                | Ground                 | Ground           | Ground      |




