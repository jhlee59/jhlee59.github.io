---
title: Component Selection 
---

## Motion Sensor 
                                                                  
| 1. HC-SR04 Ultrasonic Sonar Distance Sensor + 2 x 10K resistors|

  <img width="211" height="150" alt="Screenshot 2025-10-18 at 10 27 26 PM" src="https://github.com/user-attachments/assets/7abf2537-c9ea-4a8d-bb97-12026be9bb76" />

* $3.95/each
* [Link to product](https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069)

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 10cm-250cm range                               | 15 degree Beam angle  |
| Compatible with microcontrollers                      |                                         |
| Somewhat Inexpensive |

| 2. Ultrasonic Distance Sensor - 3V or 5V - HC-SR04 compatible - RCWL-1601 |

 <img width="197" height="176" alt="Screenshot 2025-10-18 at 10 45 22 PM" src="https://github.com/user-attachments/assets/10d83e69-833f-41a3-bd82-b04388937ca3" />

* $3.95/each
* [Link to product]([https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020))

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 10cm-250cm range                               | Low current  |
| Compatible with microcontrollers                      |                           |
| Smaller dimesions than Option 1 |

**Choice:** Option 2: CTX936TR-ND surface mount oscillator

**Rationale:** A clock oscillator is easier to work with because it requires no external circuitry in order to interface with the PSoC. This is particularly important because we are not sure of the electrical characteristics of the PCB, which could affect the oscillation of a crystal. While the shipping speed is slow, according to the website if we order this week it will arrive within 3 weeks.

### Style 2

> Also acceptable, more markdown friendly

**External Clock Module**

1. XC1259TR-ND surface mount crystal

    ![](image1.png)

    * $1/each
    * [link to product](http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366)

    | Pros                                      | Cons                                                             |
    | ----------------------------------------- | ---------------------------------------------------------------- |
    | Inexpensive                               | Requires external components and support circuitry for interface |
    | Compatible with PSoC                      | Needs special PCB layout.                                        |
    | Meets surface mount constraint of project |

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
