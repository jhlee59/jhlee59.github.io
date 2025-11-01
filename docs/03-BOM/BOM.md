---
title: Bill of Materials
tags:
- tag1
- tag2
---


## Overview
This Bill of Materials (BOM) supports a custom microcontroller-based ultrasonic sensing system designed around the PIC18F57Q43. The circuit measures distance using an HC-SR04 ultrasonic sensor, amplifies and conditions signals with a Microchip MCP6241 op amp, and regulates power through an L7805ABV 5 V linear regulator. A 74HC595 shift register manages serial-to-parallel data control, while standard resistors and capacitors provide biasing, filtering, and power stability. All components are readily available through Digi-Key and are suitable for prototyping or small-scale production.


## Bill of Materials 

| **Part Name/Description** | **Qty** | **Unit Cost** | **Total Cost** | **Manufacture** | **Manufacturer #** | **Vendor Link** |**Datasheet Link** | **Schematic Reference Designators** |
|:--------------------|:----|:---------------|:-----|:--------|:-----|:-----|:----|:-----|
| Ultrasonic Sensor Module (HC-SR04) | 1 | $3.95 | $3.95 | Adafruit Industries LLC | 4007 | [DigiKey](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020) | [Datasheet](https://cdn-learn.adafruit.com/downloads/pdf/ultrasonic-sonar-distance-sensors.pdf) | U10 | 5 V ultrasonic distance sensor |
| Op Amp, Single, Rail-to-Rail, 5 V, DIP-8 | 1 | $0.43 | $0.43 | Microchip Technology | MCP6241-E/P | [DigiKey](https://www.digikey.com/en/products/detail/microchip-technology/MCP6241-E-P/683249) | [Datasheet](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/21969b.pdf) | U3 | Low-power signal-conditioning op amp |
| Linear Voltage Regulator, 5 V, 1.5 A, TO-220 | 1 | $0.59 | $0.59 | STMicroelectronics | L7805ABV | [DigiKey](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV/634711) | [Datasheet](https://www.st.com/resource/en/datasheet/l7805.pdf) | U5 | 5 V regulator for system power |
| 100 Ω Resistor, ¼ W | 1 | $0.10 | $0.10 | Yageo | MFR-25FBF52-100R |  PRLTA 109 | n/a | R1 | Current limiting resistor |
| 10 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-10K | PRLTA 109 | n/a | R2, R3, R4, R5 | Biasing and pull-up resistors |
| 0.1 µF Ceramic Capacitor, ±10%, X7R, 50 V, 0805 package | 3 | $0.28 | $0.84 | KEMET | C0805F104K5RACTU | PRLTA 109 | n/a | C1, C2, C3 | Decoupling capacitors for power and op amp stability |

