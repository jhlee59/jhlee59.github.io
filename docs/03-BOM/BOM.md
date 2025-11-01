---
title: Bill of Materials
tags:
- tag1
- tag2
---


## Overview
This Bill of Materials (BOM) supports a custom microcontroller-based ultrasonic sensing system designed around the PIC18F57Q43. The circuit measures distance using an HC-SR04 ultrasonic sensor, amplifies and conditions signals with a Microchip MCP6241 op amp, and regulates power through an STMicroelectronics L7805ABV 5 V linear regulator. A 74HC595 shift register manages serial-to-parallel data control, while standard resistors and capacitors provide biasing, filtering, and power stability. All components are readily available through Digi-Key and are suitable for prototyping or small-scale production.


## Bill of Materials 


| **Part Name/Description** | **Qty** | **Unit Cost** | **Total Cost** | **Manufacture** | **Manufacturer #** | **Vendor Link** |**Datasheet Link** | **Schematic Reference Designators** |
|:--------------------|:----|:---------------|:-----|:--------|:-----|:-----|:----|:-----|
8-bit SIPO/SISO Shift Register, SOIC-16 package | 1 | $0.49 | $ 0.49 | NXP | 74HC595D,112 | [DigiKey](https://www.digikey.com/en/products/detail/nexperia-usa-inc/74HC595D-112/763550) | [datasheet link](https://assets.nexperia.com/documents/data-sheet/74HC_HCT595.pdf) | U1 |
0.1 µF Ceramic Capacitor, +/-10%, X7R, 50V, 0805 package |10 | 0.2750 | $2.75 | KEMET | C0805F104K5RACTU | PRLTA 109 |n/a | C2, C4, C6, C7, C8, C9, C10, C11, C12, C16

| **Part Name/Description** | **Qty** | **Unit Cost** | **Total Cost** | **Manufacture** | **Manufacturer #** | **Vendor Link** |**Datasheet Link** | **Schematic Reference Designators** |
|:--------------------|:----|:---------------|:-----|:--------|:-----|:-----|:----|:-----|
| Ultrasonic Sensor Module (HC-SR04) | 1 | $3.95 | $3.95 | Adafruit Industries LLC | 4007 | [DigiKey](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020) | [Datasheet](https://cdn-learn.adafruit.com/downloads/pdf/ultrasonic-sonar-distance-sensors.pdf) | U10 | 5 V ultrasonic distance sensor |
| Op Amp, Single, Rail-to-Rail, 5 V, DIP-8 | 1 | $0.43 | $0.43 | Microchip Technology | MCP6241-E/P | [DigiKey](https://www.digikey.com/en/products/detail/microchip-technology/MCP6241-E-P/683249) | [Datasheet](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/21969b.pdf) | U3 | Low-power signal-conditioning op amp |
| Linear Voltage Regulator, 5 V, 1.5 A, TO-220 | 1 | $0.59 | $0.59 | STMicroelectronics | L7805ABV | [DigiKey](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV/634711) | [Datasheet](https://www.st.com/resource/en/datasheet/l7805.pdf) | U5 | 5 V regulator for system power |
| 100 Ω Resistor, ¼ W | 1 | $0.10 | $0.10 | Yageo | MFR-25FBF52-100R | [DigiKey](https://www.digikey.com/en/products/detail/yageo/MFR-25FBF52-100R/398308) | [Datasheet](https://www.yageo.com/upload/media/product/productsearch/datasheet/rchip/MFR.pdf) | R1 | Current limiting resistor |
| 10 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-10K | [DigiKey](https://www.digikey.com/en/products/detail/yageo/MFR-25FBF52-10K/398336) | [Datasheet](https://www.yageo.com/upload/media/product/productsearch/datasheet/rchip/MFR.pdf) | R2, R3, R4, R5 | Biasing and pull-up resistors |


Note: Setting it up as a table is nice because it is completely viewable without scaling issues. <ins>Downside</ins> is that you have to do the math.

* You could also import your BOM via a screenshot of the spreadsheet created BOM
