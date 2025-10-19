---
title: Component Selection 
---

## Motion Sensor 

*Sensor component selection*
                                                                                                      | 1. HC-SR04 Ultrasonic Sonar Distance Sensor + 2 x 10K resistors|
|  <img width="211" height="150" alt="Screenshot 2025-10-18 at 10 27 26 PM" src="https://github.com/user-attachments/assets/7abf2537-c9ea-4a8d-bb97-12026be9bb76" />
|* $3.95/each|
|* [link to product](https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069)|

| Pros                                      | Cons                                                             |
| ----------------------------------------- | ---------------------------------------------------------------- |
|                                | Expensive  |
| Compatible with microcontrollers                      |                                         |
|  |

| <img width="227" height="165" alt="Screenshot 2025-10-18 at 10 14 58 PM" src="https://github.com/user-attachments/assets/998a6734-bea9-4854-819e-57fa030f43fc" /> 
Option 1.<br> HC-SR04 Ultrasonic Sonar Distance Sensor + 2 x 10K resistors <br>$3.95/each<br>[Link to product]([http://www.digikey.com/product-detail/en/ECS-40.3-S-5PX-TR/XC1259TR-ND/827366](https://www.digikey.com/en/products/detail/adafruit-industries-llc/3942/9658069))                 | \* Somewhat expensive <br>\* Compatible with microcontrollers<br>\*                                               | \* <br>\*  |
| ![](image3.png)<br>\* Option 2. <br>\* CTX936TR-ND surface mount oscillator <br>\* $1/each <br>\* [Link to product](http://www.digikey.com/product-detail/en/636L3I001M84320/CTX936TR-ND/2292940) | \* Outputs a square wave <br>\* Stable over operating temperature <br> \* Direct interface with PSoC (no external circuitry required) range | * More expensive <br>\* Slow shipping speed                                                         |

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
