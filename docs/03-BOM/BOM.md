---
title: Bill of Materials
tags:
- tag1
- tag2
---


## Overview
This Bill of Materials (BOM) supports a custom microcontroller-based emitter and detector sensing system designed around the PIC18F57Q43. The circuit measures distance using two OPB732 sensors, amplifies and conditions signals with a Microchip MCP6004 op amp, and regulates power through an L7805ABV 5 V linear regulator. A L7805ABV shift register manages serial-to-parallel data control, while standard resistors and capacitors provide biasing, filtering, and power stability. All components are readily available through Digi-Key and are suitable for prototyping or small-scale production.


## Bill of Materials 

| **Part Name/Description** | **Qty** | **Unit Cost** | **Total Cost** | **Manufacture** | **Manufacturer #** | **Vendor Link** |**Datasheet Link** | **Schematic Reference Designators** |
|:--------------------|:----|:---------------|:-----|:--------|:-----|:-----|:----|:-----|
| Reflective Emitter and Detector Sensor (OPB732) | 2 | $4.61 | $13.83 | TT Electronics/Optek Technology | 365-1691-ND | [DigiKey](https://www.digikey.com/en/products/detail/adafruit-industries-llc/4007/9857020) | [Datasheet](https://www.ttelectronics.com/TTElectronics/media/ProductFiles/Datasheet/OPB732.pdf) | U3, U4 | 5 V Emitter and Detector |
| Op Amp, Four, Rail-to-Rail, 5 V| 1 | $0.59 | $0.59 | Microchip Technology | MCP6004-I/P | [DigiKey](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004-I-P/523060) | [Datasheet](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/21969b.pdf) | MCP6004_OPAMP1 | Low-power signal-conditioning op amp |
| Linear Voltage Regulator, 5 V, 1.5 A, TO-220 | 1 | $0.59 | $0.59 | STMicroelectronics | L7805ABV | [DigiKey](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805ABV/634711) | [Datasheet](https://www.st.com/resource/en/datasheet/l7805.pdf) | U2 | 5 V regulator for system power |
| 100 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-100K | PRLTA 109 | n/a | R8, R10, R17, R18 | Current limiting resistor |
| 10 kΩ Resistor, ¼ W | 3 | $0.10 | $0.30 | Yageo | MFR-25FBF52-10K | PRLTA 109 | n/a | R5, R7, R16 | Current limiting resistor |
| 2 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-2K | PRLTA 109 | n/a | R1, R2, R13, R14 | Current limiting resistor |
| 1 kΩ Resistor, ¼ W | 3 | $0.10 | $0.30 | Yageo | MFR-25FBF52-1K | PRLTA 109 | n/a | R3, R4, R15 | Current limiting resistor |
| 220 kΩ Resistor, ¼ W | 4 | $0.10 | $0.40 | Yageo | MFR-25FBF52-220K | PRLTA 109 | n/a | R11, R12, R19, R20 | Current limiting resistor |
| 220 Ω Resistor, ¼ W | 2 | $0.10 | $0.20 | Yageo | MFR-25FBF52-220K | PRLTA 109 | n/a | R6, R9 | Current limiting resistor |
| 0.1 µF Ceramic Capacitor, ±10%, X7R, 50 V, 0805 package | 3 | $0.28 | $0.84 | KEMET | C0805F104K5RACTU | PRLTA 109 | n/a | C1, C2, C3, C4, C5 | Decoupling capacitors for power and op amp stability |

