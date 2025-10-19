---
title: Component Selection 
---

## Motion Sensor 
                                                                  
 1. HC-SR04 Ultrasonic Sonar Distance Sensor + 2 x 10K resistors

  <img width="211" height="150" alt="Screenshot 2025-10-18 at 10 27 26 PM" src="https://github.com/user-attachments/assets/7abf2537-c9ea-4a8d-bb97-12026be9bb76" />

* $3.95/each
* [Link to product](https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 10cm-250cm range                               | 15 degree Beam angle  |
| Compatible with microcontrollers                      | Weights 8.7g                      |
| Somewhat Inexpensive |

 2. Ultrasonic Distance Sensor - 3V or 5V - HC-SR04 compatible - RCWL-1601 

 <img width="197" height="176" alt="Screenshot 2025-10-18 at 10 45 22 PM" src="https://github.com/user-attachments/assets/10d83e69-833f-41a3-bd82-b04388937ca3" />

* $3.95/each
* [Link to product]([https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020))

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 10cm-250cm range                               | Low current  |
| Compatible with microcontrollers                      |                           |
| Smaller dimesions than Option 1 |

 3. US-100 Ultrasonic Distance Sensor - 3V or 5V Logic
    
<img width="215" height="171" alt="Screenshot 2025-10-18 at 10 58 40 PM" src="https://github.com/user-attachments/assets/fea70a56-564e-4f23-9a41-6030e1f67c79" />

* $6.95/each
* [Link to product]([https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020))

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 10cm-250cm range                               | Lightly more expensive  |
| Removable back                     | Only Compatible with Arduino or CircuitPython       |
| | Low current |

## Op Amp
                                                                  
 1. MCP6004-I/P

  <img width="224" height="206" alt="Screenshot 2025-10-18 at 11 18 25 PM" src="https://github.com/user-attachments/assets/411ccfcd-c1d0-4ebd-9f79-dc29c23425f6" />

* $0.59/each
* [Link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004-I-P/523060)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| Inexpensive                      |   |
|             |                     |
| Through Hole Mount |

 2. MCP6001T-I/OT

<img width="217" height="173" alt="Screenshot 2025-10-18 at 11 22 37 PM" src="https://github.com/user-attachments/assets/1e0549c7-367d-439d-8909-d9095a1af41a" />

* $0.30/each
* [Link to product](https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020))

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
|                                |   |
|                       |   Surface Mount                        |
|  |

 3. IC INVERTER 1CH 1-INP SOT23-5
    
    <img width="238" height="193" alt="Screenshot 2025-10-18 at 11 26 40 PM" src="https://github.com/user-attachments/assets/2f2eeb1e-c7ec-4290-98c9-c1547fd14b60" />

* $0.12/each
* [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/SN74LVC1G04DBVR/385716)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
|                              |  |
|                      | Surface Mount       |
| |  |

**Choice:** Option 2: CTX936TR-ND surface mount oscillator

**Rationale:** A clock oscillator is easier to work with because it requires no external circuitry in order to interface with the PSoC. This is particularly important because we are not sure of the electrical characteristics of the PCB, which could affect the oscillation of a crystal. While the shipping speed is slow, according to the website if we order this week it will arrive within 3 weeks.


1. CTX936TR-ND surface mount oscillator

    ![](image3.png)

    * $1/each
    * [Link to product](http://www.digikey.com/product-detail/en/636L3I001M84320/CTX936TR-ND/2292940)

    | Pros                                                              | Cons                |
    | ----------------------------------------------------------------- | ------------------- |
    | Outputs a square wave                                             | More expensive      |
    | Stable over operating temperature                                 | Slow shipping speed |
    | Direct interface with PSoC (no external circuitry required) range |

**Choice:** Option 2: CTX936TR-ND surface mount oscillator

**Rationale:** A clock oscillator is easier to work with because it requires no external circuitry in order to interface with the PSoC. This is particularly important because we are not sure of the electrical characteristics of the PCB, which could affect the oscillation of a crystal. While the shipping speed is slow, according to the website if we order this week it will arrive within 3 weeks.
