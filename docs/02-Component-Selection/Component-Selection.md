---
title: Component Selection 
---

I chose the OPB732 Reflector Emitter and Detector, the MCP6241-E/P operational amplifier, and the L7805ABV voltage regulator because they work together to create a reliable and efficient automatic trash can that enhances convenience and durability. The OPB732 provides accurate distance detection, allowing the lid to open smoothly and quickly when a user approaches. Additionally, alert the user when the trash is full. The MCP6241-E/P op amp improves signal accuracy between the sensor and the microcontroller, ensuring the lid operates consistently without unexpected movement. The L7805ABV voltage regulator supplies a steady 5V output and includes built-in protection against overheating and short circuits, helping the electronics last longer and stay safe. Together, these components make the trash can quiet, dependable, and easy to use while keeping the overall design affordable and practical for everyday households.


## Motion Sensor 
                                                                  
 1. OPB732 Emitter and Detector Reflective Optical Sensor 3"

 <img width="234" height="212" alt="Screenshot 2025-12-06 at 3 20 42 PM" src="https://github.com/user-attachments/assets/9d9367ee-7e05-4ded-8231-4e884adb5bab" />


* $4.61/each
* [Link to product](https://www.digikey.com/en/products/detail/tt-electronics-optek-technology/OPB732/1637069)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Doesn't have a daughter board                      | Single Beam range  |
| Compatible with microcontrollers                 |                       |
| Inexpensive |

2. Ultrasonic Distance Sensor - 3V or 5V - HC-SR04 compatible - RCWL-1601 

 <img width="197" height="176" alt="Screenshot 2025-10-18 at 10 45 22 PM" src="https://github.com/user-attachments/assets/10d83e69-833f-41a3-bd82-b04388937ca3" />

* $3.95/each
* [Link to product](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 10cm-250cm range                               | Low current  |
| Compatible with microcontrollers          |  Has a daughter board              |
| Smaller dimensions than Option 1 |

3. US-100 Ultrasonic Distance Sensor - 3V or 5V Logic
    
<img width="215" height="171" alt="Screenshot 2025-10-18 at 10 58 40 PM" src="https://github.com/user-attachments/assets/fea70a56-564e-4f23-9a41-6030e1f67c79" />

* $6.95/each
* [Link to product](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4019/9808308)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 10cm-250cm range                               | has a daughter board  |
| Removable back                     | Only Compatible with Arduino or CircuitPython       |
| | Low current |


**Choice:** Option 1: OPB732

**Rationale:** The OPB732 is the best choice because it is the simplest Emitter and detector with which I have experience, and it doesn't have a daughter board connected. 

## Op Amp
                                                                  
1. MCP6004-I/P

  <img width="224" height="206" alt="Screenshot 2025-10-18 at 11 18 25 PM" src="https://github.com/user-attachments/assets/411ccfcd-c1d0-4ebd-9f79-dc29c23425f6" />

* $0.59/each
* [Link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004-I-P/523060)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Inexpensive                      | 3 Op Amp will go unused  |
| Through Hole Mount            | Larger footprint                    |

2. MCP6241-E/P

<img width="223" height="210" alt="Screenshot 2025-10-18 at 11 40 01 PM" src="https://github.com/user-attachments/assets/f24bf6f4-cdec-4f86-9a83-eaa9231f7d30" />

* $0.43/each
* [Link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP6241-E-P/683249)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Small                               | Limited to one Op Amp  |
| Through hole mount                      | Low current                      |
| Voltage Flexible |

3. IC INVERTER 1CH 1-INP SOT23-5

<img width="227" height="197" alt="Screenshot 2025-10-18 at 11 54 52 PM" src="https://github.com/user-attachments/assets/cd62fe10-ee8d-4051-99b4-483da2ef4aa9" />

* $0.12/each
* [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/SN74LVC1G04DBVR/385716)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Small                               | Doesn't read continuous signals |
| Cleans up signals                 | Surface mount                     |
  


**Choice:** Option 1: MCP6004-I/P

**Rationale:** The MCP6241 features only one op amp in the package, eliminating unnecessary components and minimizing PCB space. However, I need two op-amps, so the MCP6004 is the better choice. Additionally, I have prior experience and knowledge with the MCP6004. 

## Voltage Regulator
All are fixed at 5 V and ~1.5A

1. L7805ABV

<img width="237" height="194" alt="Screenshot 2025-10-19 at 12 36 13 AM" src="https://github.com/user-attachments/assets/2db6bca7-ed57-4424-b685-bc4153c44478" />


* $0.59/each
* [Link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV/634711)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Internal thermal shutdown and short circuit protection  | Inefficient for battery powered designs |
| Common and Inexpensive     | Dropout voltage (~2V) limitation                   |
| Through hole mount             |           |

2. L7805CV
   
<img width="260" height="177" alt="Screenshot 2025-10-19 at 12 37 54 AM" src="https://github.com/user-attachments/assets/652b4838-14f0-4f39-b6db-0202e11fb72b" />


* $0.50/each
* [Link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805CV/585964)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Smaller than Option 1 with same specs     | Poor efficiency at high voltage |
| Reliable                 | Dropout voltage (~2V) limitation   |
| Through hole mount             | Through hole mount             |

3. UA7805CKCS

<img width="246" height="189" alt="Screenshot 2025-10-19 at 12 38 48 AM" src="https://github.com/user-attachments/assets/f3994d4c-926e-4e62-a82e-a8942eeac753" />


* $1.34/each
* [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/UA7805CKCS/521612)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Through hole mount              | Linear regulator |
| Built‑in protection features    | Dropout voltage around ~2 V |


**Choice:** Option 1: L7805ABV

**Rationale:** It's the simplest and most reliable. Its thermal performance and protections make it the most balanced and robust option.
